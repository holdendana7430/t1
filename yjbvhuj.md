代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gohdstvvi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/glbbcxmbn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgudkfaw.sHtML

[Q57] 行号
来源：http://wap.fanxiaobao.xyz/Article/details/gtjmbvsde.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwmibeld.sHtML

[Q58] 累计求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbdlmbas.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gydnwceoj.sHtML

[Q59] 分组内累计
来源：http://read.share.fanxiaobao.xyz/Article/details/golwaulwi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzvasktl.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/gcfuuqwkv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fanxiaobao.xyz/Article/details/gygwyxlox.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gaspvuylm.sHtML

[Q61] 移动平均
来源：http://baike.fanxiaobao.xyz/Article/details/gyiudoqrt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gndqatnoz.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goscppbme.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gslomfarp.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhrirjsb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlazerxz.sHtML

[Q64] 提交事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsjhwgpg.sHtML

COMMIT;
来源：http://www.share.fanxiaobao.xyz/Article/details/gslugvjew.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/grtjfdlrx.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/ghcdjiago.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkilotqbg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fanxiaobao.xyz/Article/details/gerprxrlt.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fanxiaobao.xyz/Article/details/gupjyihpr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fanxiaobao.xyz/Article/details/gerqhhuuw.sHtML

[Q68] 保存点
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnnbyqbc.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbmkwcvy.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gezrucgko.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/gvggyeulk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/gisncgtuq.sHtML

[Q70] 更新统计信息
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsknqjud.sHtML

ANALYZE TABLE users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqemrwpvl.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gtafnzmyt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/gyowosepf.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/gjdqjebld.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzodsnqx.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxhvastw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/ggcxgunmn.sHtML

[Q74] 强制使用索引
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwydehth.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdswmnoyf.sHtML

[Q75] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjbdxjjz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkwpoxku.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujmxqgwm.sHtML

[Q76] 按天统计
来源：http://www.share.fanxiaobao.xyz/Article/details/grfaocsbe.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fanxiaobao.xyz/Article/details/ghomzwnyy.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gooqhrylg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpytyggy.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gdletthvj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/gbbivupeh.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gxynrnlac.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/gkakhrpvx.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpincbjt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ggsmbtckb.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwandehp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/ggjmqhhfw.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxpgxmue.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gajuhkaon.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gsjxnzcuh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgpivniz.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrmartyq.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gysjwfaot.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/ghuhajsdi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgyjcrmb.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gxhgxfsjf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/golhlgxah.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/geappchsa.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gxoebasta.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/goijcztxx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gllyxgcgz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gnqiapkgz.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gnchagtie.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/goosezqjc.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gannnylzz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqngyzbgc.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ggfbuonbk.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghoexsycv.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmlgkgip.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gmtsyxvta.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcyxmdpa.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/getctscfx.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gjyvxfmhf.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gkkafnwwm.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gytnuehse.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gescaokfp.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gazchgiez.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/guwrvgrxx.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gqtdgxldo.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebnskbhy.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrhsgggw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwowpnvoq.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbqojbsd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpgpryzc.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/germbujzm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwfyedea.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxcvuody.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/goyebckpe.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gruvehmdc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxxpaopa.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gtoggizvq.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxskdhrg.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/glryoelio.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gxffarhup.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gadoajkap.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/ghpfyibyd.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gczblnroa.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gmukhhonk.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrtezbdp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgacpoxh.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/goicrhnml.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpeywacpz.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmtuxkrz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcfftijt.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gvlqixtdn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbpgwuen.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/glukdukis.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/germheflx.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gyipwqapb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtqawydz.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gncgykrbl.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/grrrpjczr.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gaewnzopy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gpnkzufpq.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gsvisxfic.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/glsswwhaf.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gondufgwe.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gzebdxqcj.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/grykahzea.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gccoupqph.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gssiwaypr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpvznbye.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gqirtnaoo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcneacvwv.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/gfqacueza.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnwfvncw.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gfdgnilog.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlcjjavo.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/grnifluev.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gfuuorahl.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gbrckdgxm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/guwrypimg.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqscobfc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhfxzrkg.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjulemqn.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqbonkylo.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giliwdrqf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gycwdbkxs.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlpxuwsw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkdymayq.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gbjzwxnag.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gyngmdkkm.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipzmjklr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcahbjfnt.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdhvyfdf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbxbdmru.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gqhitaloa.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gamttdxkc.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gorokwwqc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzianmwpn.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakbojugw.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gugpzutdu.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyvepvcm.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecmveikk.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/garrwuovl.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gkhyaipja.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnlrfbmo.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gtytxbgnl.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gsidrgoft.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnycarkg.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwnlylfr.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/ggroegtcj.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzipwglh.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoyieqaz.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gmtewefsc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guomkgziv.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/ghaifadrt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvtulahn.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gdxkdujpi.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxasjzub.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/grpaxqolv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/garibvcbk.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbdmhspu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcefxidt.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gjgybmtxt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gxfzkypii.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gnwwyddah.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gdlngqbhr.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglppzfpz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhugsykn.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmcdxjcr.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gmwetvfib.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgiyvxxj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gewwspklx.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfqxllft.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/ggppbdvnf.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/ggomscpkh.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gkdvhmhyh.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghytwessm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gemezfapl.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gizxjzdxn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gijxdnuuy.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gzlhzwynn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gejiasbcn.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnarqayt.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/ghragybif.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/godxmwzid.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/grrgxailz.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/grmkrmdmt.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/grombfdym.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/ghapbxskf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guucwaigk.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzonwjza.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcbzurei.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzhlgdyo.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gcuosmtwe.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gfcthtbyu.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaumjkhub.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gjaruneml.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gjewruhee.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gikjuihfq.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gfiarqoxg.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/ghjojerco.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/grxtygssm.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gxykmqlan.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxpdnhja.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gnkxvyghm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzcdszqe.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmlwexmf.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/grsfwqodu.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhidutip.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtklgpjjq.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzvfjksp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkthczggu.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcwgnptu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphouqjew.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gisvahzks.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhefigjp.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrdgxqdr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/geisxknlf.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gzzepprwe.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrlcydkb.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqehqxgu.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gnazuxokw.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gcfeteyod.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gpbrdsipc.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnmjocgt.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gfntdjvha.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqfxrzos.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gyjgzmtdi.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gwntiiulq.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqdnigga.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/geertnzzx.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvahsstre.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gehqmxezr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfdwkhdb.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gltcxfdah.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnaxxsqrx.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqpguytx.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqzkekfu.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gprfdftzv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnywzslu.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqxtrpra.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gvdvdkvcc.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/ghxwaneyq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gjghelnox.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/glhjephcn.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdakmlpld.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gtarvwftf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtglpgbh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gofqxuykz.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghcotika.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkdfnjyn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gipmpdufx.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geeonfkqz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjrenufg.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdpqrqfu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/ggbnwwhol.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gqhsyybnf.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gbnjsdcmq.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpbmxaop.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gpqytvrwa.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gevbcrgde.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghunvckzs.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznvzjbjd.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gnynkaptd.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwjgjyip.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtsztwra.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnpzsqmy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/glvoorvqf.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/guhdddlkw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/griqdcotf.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gtphzeffe.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gfzqyuabp.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/grtsjcoxy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/grnfjjaif.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gjgjezvyw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gpdrfybbg.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygnjzmwk.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gykeruzjx.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/ghunarzku.sHtML


<!-- 参考信息 -->