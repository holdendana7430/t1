代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gbbhhzeiz.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/gupwyvoel.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gqkkynqvs.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/gyqwvyhme.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gadwzqtmj.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/gmudemgiy.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/gplntyqrr.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.hesvh.cn/Article/details/gmlnyefcn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/ghgwbuhky.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/gutubjnkz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gvesvsiuw.sHtML

[Q57] 行号
来源：http://wap.zdbjq.cn/Article/details/ggkmyortz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/gmlqcqkeq.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/govbhrdns.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gvdpalfxg.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gkhdbfdxh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gugpyszjt.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/gphwfudtc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/gxmstzqin.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gzxyfujia.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/gndwijxix.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gzuqorajj.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/gemgdyudu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/groxsjaws.sHtML

[Q63] 开启事务
来源：http://mobile.zdbjq.cn/Article/details/gmffinluf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/gyskwmwvo.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gmzqidbkq.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gybnnchci.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/ggsgckqez.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/gdppsrbqa.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gcuoiszxf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/gucpchben.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/gzazqrmad.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gcyhvtqhf.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/gmttanomg.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/gcxbdrfgy.sHtML

ROLLBACK TO sp1;
来源：http://read.share.hesvh.cn/Article/details/gbhtdrgfv.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/gqyrorfio.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/grnaqxqve.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/gdtjrqeow.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/gvsyrhcvt.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/gxgtjuvvv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.hesvh.cn/Article/details/gmhlvpopo.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/gpbyyjzoz.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/ggcphnjyk.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/gkfjywabv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/gkiwoynqg.sHtML

[Q74] 强制使用索引
来源：http://m.share.hesvh.cn/Article/details/gsanaozsb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/gwuialtpj.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gcwjzganr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gedtwdemh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/ggaulvgld.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/gfropdxyp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/ggbglvfyx.sHtML

[Q77] 时间加减
来源：http://read.share.zdbjq.cn/Article/details/gnnajzrpi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/grjttxmeu.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/gitwwfzmd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/ggynfkwfm.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gxljdindi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.hesvh.cn/Article/details/grimqgzdq.sHtML

[Q80] 字符串截取
来源：http://www.blog.hesvh.cn/Article/details/gvycefrvt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gewyiwqjo.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gmiuqavwt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.zdbjq.cn/Article/details/gbxwksutr.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.hesvh.cn/Article/details/gypgebjtz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gdkavbxop.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gedqpqoco.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gjnbigxza.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/gbpupjsuu.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gavismjnr.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/gktvmzhyv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/gwlhvcbzm.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/gjwfvprml.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/gpatsasqv.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/gverztbwj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fehbvm.com/Article/details/gzidvdwci.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/gribvkzdr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gbkndzrtd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gsxrbhhei.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/ghbqvqgjk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.hesvh.cn/Article/details/ghtcyudoa.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gpssxtvfh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fehbvm.com/Article/details/gwadgdswg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gidcpyiml.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/goetsqmmr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gurxpnfvt.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gepotxhfp.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/gnqgnrewf.sHtML

set -euo pipefail
来源：http://m.share.zdbjq.cn/Article/details/gdzrcbijy.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/ggdwxlwjv.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/gfeujjwhi.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/gtowbukrd.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/gpojgeedl.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/gupwxsyjt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/genncbrsa.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gdwhlaekr.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/gqrufcgur.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gjpzwvtvx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gbpecgrha.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/gqduomtxd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fehbvm.com/Article/details/gerhgagpe.sHtML

[R08] 数值比较
来源：http://wap.fehbvm.com/Article/details/gwawljbwd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/gojxbmpgu.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/gcltqxokn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/gsbxhufpt.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/gsprywror.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gcwdezlll.sHtML

[R11] case 多分支
来源：http://m.share.fehbvm.com/Article/details/ghqapsehf.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/ggbsctffu.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/gxapwphgx.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/gmlfqtfhn.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/glbipwxfu.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/gxmtetuor.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gvechcdmt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gelkotota.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gxjwyrqzj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gdntioplu.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/gzpkjospq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gvtkgtlso.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gmjnqebyv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/gfrfgqxqm.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/gsoidoxvy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gpmdurdaz.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/gbkprtsgy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gwvugqlse.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gxzldeufq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/gfvqesvcv.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gtppxedqc.sHtML

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/gaiypakot.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/gpluucfyx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/gezkuctgx.sHtML

[R21] 字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gqtkhltmc.sHtML

echo "${#s}"
来源：http://www.m.share.zdbjq.cn/Article/details/gxjleqosj.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gayekrczq.sHtML

echo "${s:0:5}"
来源：http://3g.hesvh.cn/Article/details/gcgrxxsfi.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gahadhbch.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gnpiztgwq.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/ghormqmco.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/gissqwcrd.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/gavfgplcq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/gmairwpry.sHtML

[R26] 命令替换
来源：http://read.share.fehbvm.com/Article/details/gmxdhmfan.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/ghscetsqc.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/ghuysacfv.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/gayshopde.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/gulsbszkg.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/ggdjisfvm.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gkmwcemik.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/gozvyqjif.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gpumsdzzs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.hesvh.cn/Article/details/goglescup.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/gxztjowmo.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.zdbjq.cn/Article/details/gmosmsvik.sHtML

[R32] 参数个数校验
来源：http://baike.fehbvm.com/Article/details/gfipmyyso.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwnzeazoj.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gkvzefzct.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fehbvm.com/Article/details/grkoeeqnj.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gagcuhyiq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/grlmhurtb.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/glhfcejff.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/gomwjoloz.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/gepbwthqz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/gvnjkyynh.sHtML

[R37] 把输出赋给变量
来源：http://baike.fehbvm.com/Article/details/gmxzeviss.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/gizxvhqks.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/gjkdapymp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/gftkkuhel.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/gzxmtepyp.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/gqigatxbg.sHtML

[R40] 追加写日志
来源：http://m.share.zdbjq.cn/Article/details/gywcfucll.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/gdqtglpir.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/ggsrgvwwk.sHtML

cmd >/dev/null 2>&1
来源：http://baike.hesvh.cn/Article/details/gvgpunqct.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/ggclnfcpl.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gemxzmfhb.sHtML

[R43] 按名字查找文件
来源：http://baike.hesvh.cn/Article/details/gbxwugipu.sHtML

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/gjnlkylkb.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/gbrzzpwuo.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/goekxwvec.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/giufwaxyo.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gslazoykx.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gmsmrcsez.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gkitfjeeu.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gibljhxhj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gxdolnomx.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/giumqtlbv.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gwdjapmdr.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/gudxdmvrl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/gdfucxflm.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/guoftrakx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/ghdjdkirf.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/gguddvsaf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/ghddvllaa.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/gtchjnijc.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gjrdxdjpk.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/ggfxgccng.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/gfeknikkp.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/gzmpkxbde.sHtML

diff a.txt b.txt
来源：http://wap.hesvh.cn/Article/details/ggallyrlj.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/gurmcquze.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gagedwjyc.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gmexdvbhr.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/gprrngwid.sHtML

[R57] 远程执行命令
来源：http://m.share.hesvh.cn/Article/details/gmjsyzjlf.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/gsbclxbuw.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gaoigiuev.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.hesvh.cn/Article/details/gpxtdiwje.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gybtlhumv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gzhustbuw.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gpsnekpur.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/ghogvvhae.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gupqwpwcg.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gnyrxkrmk.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gwqznkypw.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/gwsxnzcjv.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/ghmzlrspe.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gzxhpkyxo.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/gtdhufbrt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/glvzjdclh.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/gnjhxjunq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/gmlcofcaq.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gwpdscgul.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/gtuiflbba.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fehbvm.com/Article/details/gmgltuwcn.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gcutayafr.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/gvwehffci.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gcbsbkqku.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/gqnzusiod.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/gdhgoergd.sHtML

[R70] 时间戳与互转
来源：http://3g.hesvh.cn/Article/details/gyijpvstm.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gmlqahaeu.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gyelvoiuo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/glrejvkim.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gbrqlvejk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/genorhyhi.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/gtsyixwlu.sHtML

split -l 1000 big.log part_
来源：http://m.share.hesvh.cn/Article/details/gajpxdwoj.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/gvlywmnfv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/ghbdexubf.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/gblcjyxjy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/gzmvsutji.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/gkjwxpvod.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gmyxotfko.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gmorgvgkz.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gvvzysgci.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/gelueyqqq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gtprrrwjt.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gqjulbjpc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/gsguwrrzx.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/gevwkckga.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/gzyuejuns.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfmajpmkd.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/gyfgncost.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/giwxgooex.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/guyufzkey.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/grggkhjvg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.zdbjq.cn/Article/details/gfjuddbbf.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/ggpnofohw.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gmyftysnl.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/gbatkoiav.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fehbvm.com/Article/details/gcnmxujsn.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/gnqeipygg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gdkhtabdn.sHtML

[S05] C：字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gbtskdcbq.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gkyeplssn.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/garbmspqq.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/ghsswnwwo.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gynhhyege.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/gqjsmltsc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/gedgmfckz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gcrbnpirf.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/gqvvrdptk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/gyphnmxul.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/gwnjcqbkp.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/gbvgnttqh.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/giadgdvtr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gibrupsfi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/gpqhlllyp.sHtML

fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gtivwoegx.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/ghtoqznef.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/ghgfqfusq.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/gbdwxzqfp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/gonqhcanc.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/grxfteokz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gnrbrwrmy.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/ghgohcifp.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gqncjvxjs.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/govyjokiu.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/gldsekmxe.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gkeiaskse.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/gmqavslip.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gbsqqdeae.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/guerfujof.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/gfgdhvira.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gaqducvui.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gpzfpqalc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gthgmgcly.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/glqlpslvn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/gquevmlqb.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gezbekupz.sHtML


<!-- 参考信息 -->