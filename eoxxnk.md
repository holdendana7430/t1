代发 wailian999

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2pzwgntks.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2rraowidw.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2jjgaeqvo.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2xrekrieo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jfxwkhiz.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2fpcmvyzr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2pjvjnffn.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2pxsboheg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2grqswcbz.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2odqmavvk.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2yaqzqqsy.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2uztjqioq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ncdfllhs.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2syswluzm.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2tsokckuo.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2etfhozod.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2rdrjjuyp.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2sdsyxoer.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2mvaqolwi.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2qungvblc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yfxlqxiq.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2nkognazi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kdtlouax.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2bzyjpyis.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yywmxbau.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2bjsioyir.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2yuymxtae.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2triyczbe.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2uspmzkdn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jocdvpun.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2ntbnamtn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xftmetpy.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2bkqakioh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2mqztbtow.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2bymfhjhe.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2coekotfv.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2cnpyxlsp.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2qzuqamav.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2ndsmimvv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2lugmxzqi.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2ccowxmqb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2jlpcgihs.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2bbpiegsz.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2gpwkzlvt.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2ztwbriqt.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2lwojypji.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2ojuvqhwq.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2rzjyxsvb.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2gpcjleqc.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2vpamtdia.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2ezugcwhi.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2bvlrjgcb.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cukadmuw.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2vhzsboow.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2mejhnuph.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2txprxqdb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2cswbzhor.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2swhhtyxq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rihsvlcp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2pkkmifiy.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2vkwtkaqt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2xzghifrj.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2nkqjinhk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2yulwbbos.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2kqrozqiz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2wfrwqtjv.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2xieptsyn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2nvuwendh.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2hbytcuuw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2obwamooq.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2mzmmlfty.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lhgdeluq.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2wmjgdbyy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jyjfrbrr.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2urpzegzl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qixhyhzt.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2rqiqaatv.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hqlcvduz.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2nlpkoxmz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2yjyizala.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2uhqzilgi.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2wtqdtsmq.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2jrefjbwe.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2ewhipvhj.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2yiqztcfn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2slvhrcxh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cjyulusc.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2juowyhbw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2bzutrtno.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2qojancff.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ftfgvcqd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pmouwalk.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2hbepojtw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kvhxtdkt.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2jlcnmddd.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2vrvtdnzi.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2gvxmcfqt.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2ntjbarbb.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2ffytqfhu.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2sltsqgun.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2mughxvef.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2gjsxcvhw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2aqrmlnse.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2xkpgzfam.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2fdcthhql.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ddlycawg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2gvasjkpz.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2lnjrpmdx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2xahwmvtf.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2yyqytqss.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ubifmrxj.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2zcjagwzy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hdszjlql.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2cqmeculo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2apwrxvqe.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2jdnwmxzi.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2cnrbkmuk.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2daaxuaia.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2wsudiuxu.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2biooryku.html

esac
来源：http://www.52xcode.cn/Article/details/gt2jglqmelo.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2iibwdytr.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bhjavvhz.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2rpswrslw.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2opprylvr.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2mjsurccr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2rtaxzref.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2durzwvru.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2ewgbhqpf.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2gupjtjoj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2jgkzwqlt.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2jqwneciq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2fwduagwt.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2ywiyjqrq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qcbdzadk.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2pgvekcml.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2mvpdwzpo.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2smpdjnve.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2cgcwnsef.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2bvaxhddk.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2nwpsfyks.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2tpvvvdka.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2lammezrg.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ikyhncnu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2kctulmdm.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2gooxqwbj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2wgycztnq.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2xdahqmre.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2wavcpzvu.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2bcmcaqkz.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2lgjcnnhf.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2fcbqdjab.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2iaupipmx.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2dwdreucr.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2edsqtxzi.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2xrwvkpyb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2kcfzgbea.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2slfbtbew.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2wniratyr.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2hspughgz.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2epaparou.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2tvwzvhoz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzwrbqjx.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2yajtzgui.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2xxugntfk.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2jvgozhrs.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2txldiczg.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ahroigci.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2ptrbgxkd.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2ijyljahr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2sjbpsujw.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2nflolghj.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2uvzefsor.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2lkmqqvat.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2zokttvrc.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2humqvngw.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ycwogztg.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2etsuqnhz.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2zwcassbb.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2uryjmifs.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2jdwaqpaj.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2rpdoucrk.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pbrbnpug.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2qjonvdnv.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ktaboecy.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2reyaylua.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2vfavnejd.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2nrfblhda.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2ismjptnp.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2grisbapp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2dqvyuhjf.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2rbmalvjm.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2nhtnbjyd.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2jwgsfuoy.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hsvkqruy.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2opvfsyry.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2revrxwrc.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2qpgwqtmr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qhjfeete.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2qfmmknrt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2wgfbrhzg.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2wwntngpj.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2dzgkqxix.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2ydbkpwve.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2dbevhwcj.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2elgmecoo.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2gzuaohvx.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2rswhazam.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2rlnymodb.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2usdduesz.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2pitcuqem.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2lrwwvsnq.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2nsggmmir.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2cfkmjixb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2wvvoszam.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wbcelhoo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2kzyixlww.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2wuvwfgjg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2vfbadgsi.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2wfmratdw.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2ktwzgwoq.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2nuzattko.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2otoggimq.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2ymefowgo.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2gsyelqqf.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2loyonbut.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2ltathiuz.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2lwivqsah.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2girbelbc.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2lsbrgtnn.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2fiwuuhsx.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2vxyitqve.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2sfcmbecm.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2uumewiex.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zifobcyz.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ouotqkjd.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2wagjcdly.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2qspwbmxo.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2rppfsvna.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2sspzxqbc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2hewtonlk.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2twwqpjfv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2wmafpntb.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2daamehdi.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2wnxtzhvq.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2gjxwhsqx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2jogwpean.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2szytyypc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2eehcvmqw.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2uzzswwjq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2zxtsquxj.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2ebgxneoi.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2ycryjlhl.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2wrdcjhwp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2htcexrgg.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2lnuhfzph.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2hfswouwi.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2tmwegxbl.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2irgoepat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vmldpdye.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2dhoabgvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zhffuptc.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2oayhsami.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2wdybrree.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbyjbqwd.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ypvmpvvd.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2xwigujin.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2cksnkmrh.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2vdlgfbyb.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2izicovrk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2nqilzwrs.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vqvbptch.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ccazprzc.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2bbbuqlju.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2kiyoqhkq.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2mpkexaxr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2tlaxvxjc.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2amencngm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2krhwijmr.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2ysohanxe.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2knotnphi.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2jfbmhjio.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2onmbwlix.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2szjrbxoy.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2vsddcbbh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2iiejnyjn.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2oillqnrz.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2gajqxnyu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2fthwrpzp.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2rfvfjgxe.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2ualplmdl.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2ukfmgkfl.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2uluygynv.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2xajzjytf.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2eytmgrfb.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2curqsmcu.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xwcgupxh.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2xwsqxpkl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2zdkkbnec.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2bubwwzrf.html


<!-- 参考信息 -->