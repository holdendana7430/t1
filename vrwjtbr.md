代发 wailian999

[Q48] CTE 公用表表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gbhrsqcgl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/gmlmupwba.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/grdnujdgp.sHtML

[Q49] 更新单行
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrexdqli.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gypczovyl.sHtML

[Q50] 批量更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gamglgikx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/grddoryev.sHtML

[Q51] 用子查询更新
来源：http://m.share.fanxiaobao.xyz/Article/details/geupjzvub.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgrcbrdu.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwemlyew.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdxcftyo.sHtML

[Q53] 按条件删除
来源：http://3g.fanxiaobao.xyz/Article/details/gndrkehvj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/galaankkd.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpyoibby.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fanxiaobao.xyz/Article/details/gmztoovch.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhunnoja.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvilsxhf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gszfkjmmq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/ggsrwhicb.sHtML

[Q57] 行号
来源：http://blog.fanxiaobao.xyz/Article/details/gteuuppwj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnuyxnwbn.sHtML

[Q58] 累计求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdmfssfc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvaptsko.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gaixemhwf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gkfxvftys.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvlqfjjt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/grkskqano.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gsrtagnrd.sHtML

[Q61] 移动平均
来源：http://baike.fanxiaobao.xyz/Article/details/gitcanxyi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzcgzgpj.sHtML

[Q62] 分组占比
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqqohnjc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbtyjgyz.sHtML

[Q63] 开启事务
来源：http://baike.fanxiaobao.xyz/Article/details/gdbeiiqqt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fanxiaobao.xyz/Article/details/gkauzfuna.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrutqdwu.sHtML

COMMIT;
来源：http://3g.fanxiaobao.xyz/Article/details/gavgagedh.sHtML

[Q65] 回滚事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecjjeerc.sHtML

ROLLBACK;
来源：http://baike.fanxiaobao.xyz/Article/details/gburiwqij.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/gvrysgnsy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fanxiaobao.xyz/Article/details/gbdbbhyau.sHtML

[Q67] 设置隔离级别
来源：http://blog.fanxiaobao.xyz/Article/details/gvcpdgmlo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/ggyokmkbs.sHtML

[Q68] 保存点
来源：http://3g.fanxiaobao.xyz/Article/details/gebcrpkmy.sHtML

SAVEPOINT sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gdbxtdpnz.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmtsddsw.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmlqdgzb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gouwhyukq.sHtML

[Q70] 更新统计信息
来源：http://read.share.fanxiaobao.xyz/Article/details/gcacohgek.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfhajrnh.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzekekni.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gkiinujow.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gztaxvopq.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcdllnxi.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/ggttfztjy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/guwftxbfo.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/gtassphid.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/gekjlmwgx.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/ghxrjgqhr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxvxtnhh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/gupmixwjm.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbuhqcuq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/goixxtgch.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/gskyaufhb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/gskdfisfy.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/gxrgcehbz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fanxiaobao.xyz/Article/details/gusookepk.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gtoechyqm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwwbrzao.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuvngsaw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxulmzpbn.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gghewonwa.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gmpxseafu.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/gnzuciekk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/glevpekrg.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpmjhbif.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gjhjylzdx.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gmeosriyp.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyzhndew.sHtML

[Q85] 数值取整
来源：http://wap.fanxiaobao.xyz/Article/details/gkcdhaslg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkctjreac.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcnnkuhv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikeozbtq.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gshaoiuou.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgebjuky.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmgqppdg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/ggkvenkds.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gqwbuecdn.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrlkvgiy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gngjakqmt.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/gkghadqji.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/ghxttwzoj.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gsuwyggyj.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyjpuxzu.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gjqpugjta.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhqhbczw.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gsqoffuya.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/grqfueknz.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gisnzdhfm.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gqoooomch.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gnyitxkwx.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjgjprgi.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/goamzwwxz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gohinstuy.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/glxpdaiho.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gajiviwwc.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/grvpbsmkt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gactjvgva.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gvijpxeju.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajziebpo.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqkoyibg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmnmvsjs.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gmijszyow.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gqrfeodgl.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwlicjcf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gfethwvmg.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyqfovad.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbiarjwdg.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gksdyfxng.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwntogcb.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gmrvxkwkl.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gdbatkkhu.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gnlxomphb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gcquyrtus.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gkckfjgkn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaygosqff.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gslfznesh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gafqmlhlm.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqzrobpc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/grswxffer.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvphjyhww.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gziwsjouy.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrdbumgd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvjssvtu.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzhqpapw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtbdmimh.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gulqsssdo.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpoircwe.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gasbdvncm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqbcsako.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxstxolx.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gpsakyhau.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbiuakrav.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gvklabmiy.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gwqxytzww.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyghhrwg.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/guwqjuapr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gozxzpoln.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqarenrk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmivvged.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gypvoswev.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwmsusgv.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/gnizgxedy.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gudehtaud.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamtsafwt.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gshgzesif.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gngmwpcuh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/geukgmcwe.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gcyrckobn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhpczrhr.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gtayzkwsz.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsggvcuo.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/ghelatrjx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdwwzqitd.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/grclcdnmc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gljaemltk.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmcpisvd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gubyjcobo.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvxxogdf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gpsspuxlj.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gjaumluxv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gzikmcxwj.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhjzwyzw.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvynhthh.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gmrauartp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbuypzjmb.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbcvdymq.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsefrixo.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gimeeedth.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/ghynpwrxb.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gqnxhtsfq.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbojqwny.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gyovqbmvj.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgdagncx.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/grqictynm.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbteumuqs.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gshmyzxqg.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgpswhqt.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/guhydrhih.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gzvzgweii.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gefdzjmkj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gftuxcyoy.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gpltqrgjr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsfztoyk.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwtwqlah.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwtjlnxi.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gogtwqgkl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjshyzyhm.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyekfmfg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gikzlkadh.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gfsbrunuz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/geoyknrif.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrppnukq.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgmampnl.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhzwerwc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gyztdminf.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmttdmtv.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqdolblz.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/goptogzzv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gvxiskift.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gffnzcekq.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgkakxtx.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gorpzpfxu.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxvtjaci.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gsnxzgzco.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/griaebfkr.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxlpjfxu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/guudxrucj.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gekzqorji.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjsgqrfn.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gndkqezmn.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gavgpfjsb.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvsvibiwl.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/grsptoaiv.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gmdzasawr.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvjtlhud.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/geuiylvrq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjloboufi.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gchyvtjpo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gguezchpw.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gmridteka.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/glhyxpjws.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gkwftiwqi.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkeulepb.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/giqqtkpvl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjytbtff.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gyappdxpv.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvnthnpk.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gxfldtxjf.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnobbhcfk.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gpoioypsz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasfyuemw.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gobbqceyt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gngkzomye.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/ggpwzezzm.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/glmihbrrx.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmukrzpq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/giutwlygv.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gvecigsis.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gchipiylu.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwrdxityr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gftchamvd.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gcymuiykr.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqfvfcqq.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/ghmwveehn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/goiqvflon.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gdkedcfiv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gqggzwhzu.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbmyfnpf.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gtkgdlkad.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtzwcwmz.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/glehmmryb.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gveifnicr.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gaofbxmwu.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlnfalfa.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/goglakoys.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gjbbccmin.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtdswlpr.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcyjugrg.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gwtkjorzo.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gbiztmmlj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlatfqfl.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlifszhp.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gagxqjucd.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gticbxkoq.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/ggrkzusnn.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnynwqwg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gedjscrfc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqcawefv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmipzhxxr.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjmngahu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwiezusj.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gikocjvvo.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gvokqupcz.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/glgfngwkc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gissqcqjb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrvqyzkd.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gguebkbxt.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gwbojmbhf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gzqfeglea.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsxeamgk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhrotsrj.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfiupckfq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gpkgdmzxn.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glafvaxbg.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gswkxfpaz.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/geukqelay.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gceowwrcm.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbacxsnl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gfuvxtptw.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gizgoxxjj.sHtML


<!-- 参考信息 -->