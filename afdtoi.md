代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ogwjsaug.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2quurxbaj.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2qpuoustf.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2rmcjpdog.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2lnrrytvh.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2nvqbynhv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2tprnmzwg.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2jpefmhpu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2resuzgse.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2voputtbl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bquwymwi.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2qvnoxdyz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wupbjzey.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2ndtuqdhd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2hhurrutz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2znnxsaog.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2vprwskol.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lksosqgv.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2wdovmtkb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2baubnwgb.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2awnfxgcp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2mlbkpspy.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2zgekehua.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2oljslvkq.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2xxflaegt.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2qgseddrn.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2bufkuvjc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2hgffdwtk.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2qrvwhqpm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2kumtvsqs.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2cgmewxjw.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2kyfsouss.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2uwoijtyd.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2jhrrbupt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2hadzdpgv.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2sqrkcyzt.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2mfzigywg.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2czseweie.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2wdkwpvgw.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2nqzccnfe.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2etwmyzwd.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2hjxdsgck.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2lncwekyn.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2ojnjbnuj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2ixcmbjsy.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zcpubgmp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ykifgloi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2lrbmyavg.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2jxtfevrp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2tfhcdfaf.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2oenobujx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2kuqerbmu.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2mzcrfzzm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2tpafjepd.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2eiraympl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2lmrzsklo.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2ctjjqnra.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wdmtgrgl.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2efkzhczh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dcixtetd.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2pdshmbpy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bubogpnm.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2btlxkljn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kvyyhsno.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2woreevbg.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ygeqhzit.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ulsrusyl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2nqvahiir.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2ggbjlwwn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2rqwwcfnd.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2testrteo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2elkhzyxw.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2wddxovzk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2uvskrtoy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fuphrxoz.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2ghroavqo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ryxtluwq.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2iblrjvqk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ibhpnadw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2karhvknq.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2uffyzwzs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pcmpephg.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2hchkxzfo.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2amdtnnqf.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2wqstwwxu.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2gekaqmke.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2grjmxlfq.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2paqhzynv.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2juskyvmj.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2rcypmqcm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2ltmczdld.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2gyldwlvp.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2eesmruzz.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tklzzkty.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2dcdgbvjj.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2aucflnrq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2bhnlddnu.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2gzqqgsbp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fbzigyjl.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2yselzxin.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2jggalkog.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2zsfbqmpd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2poomirsh.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2uowdfocv.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2rrcqqfci.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2mfnxihmb.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2ycdxidvh.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2rayfopjp.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2vzqybxtp.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2pvmzliwd.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2elljikdb.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2qnpqgrcl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lgusxila.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2hxcgqvhc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lifrlgjj.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2yxgxeuie.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2navdemis.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2ghvpbpyl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2qgwsmsfm.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2jooujcwy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2lxwadgsf.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2vqpsmcpc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2wdllmqca.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2accjaury.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vpwgyjrq.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2sxgycpjf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2ffywjlej.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vrrzjxtr.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2gspwmdhu.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2dyehekuz.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2heqwyrqu.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2kgdoattc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2onycbiqt.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2xldzsvra.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2adhxvgmh.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2whexnazg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2vxehvhvo.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2qksnhjsq.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2nxvrkuwl.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2ijzxibwp.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2bbvacaqe.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2aplqucmo.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2aiturnsj.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2btuvqfpk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2fjjidiqa.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2bpldljsy.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2hlpllmnx.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2oaxrxnbb.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qizcyznr.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2ilkibvxm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2kiezyyff.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2bjlwsqio.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2vtezaqin.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2mknlkmdo.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2osvgldfy.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2hjwftgcw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2uululmwy.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2mexzwpcg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2yxiblkui.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2bqrvzikk.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2wlfeaach.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2zqonpxwj.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2spqwyjiy.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2vatoscwj.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2tftonjdt.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2fnvyqhxp.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2lwfncxqc.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2xhvdflgz.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2jlhhdtwf.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2kvbadlcm.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2qncdhhpm.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2dqujqbzj.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2mxkbudbs.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2xstzlnlp.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2wloohpzs.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2cfeddwbx.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2amdmscwu.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2hwbulczd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2ajnqvoxx.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2xvypxvey.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2jlqizwuz.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2jhpexklf.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hijezhvu.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2hfkrunkn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2zgjnvfol.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2iqyyjlyi.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ulcorqah.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2emmeilpr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2jmhqclfp.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2qayedkkl.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2yaorzpev.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2zvnxtbtz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2bhpddajz.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2infpsfjl.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2qxplkqah.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2ojgmpcao.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2uenronjc.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2zpninpbf.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2mlccvcco.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2mmuspmwm.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2hhmetiqa.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2mlggdcmm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2wbdkvfiv.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2yhnxxnjz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2pyvwkjcs.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2gusepxws.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2accxoxxz.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2dpfkwcbb.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2efcznbyl.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2wvdmhgtz.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2ehmxuhqy.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2knrimhde.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2sdkshvuh.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2ondaazfs.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2yebohugv.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2zwljdbwu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2wmvlpnzy.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2dajeqxsx.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2kzdubkfl.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ledobvkv.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ltckelwb.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2kkwrplez.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2icgydxqd.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2jxawuiyf.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2gxdqzthk.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2wrjatlhl.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2edhycasz.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mtikqtjj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2xiktzoxs.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2xiuvqiib.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2vqogblec.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2xxhmwrwk.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2uhujstpu.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2olmzniyk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qkheeqls.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2nshzzzxc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2fgoraopw.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2nmiyvrxj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2tysywiiw.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2rqvewdsz.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2mcdglcvd.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2xmlffmcm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2wbpvqhgz.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2plsavkba.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2eciyquxe.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2zvvvaomo.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2pffmthnw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qdgaogpj.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2soimrjwh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cqswvkhv.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pfhqbvef.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2hytuabrk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ghqqundd.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2tspdktxz.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2pqfnajuk.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ovqrqikn.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2cppmzrcd.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2tivtydib.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2huvtagyg.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2kyhutbur.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bkrwwrbo.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2kcltyoqt.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2ouxrcuqq.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2lsrkpmky.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2gyhfrtwa.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2gejnyjxf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2bnvxulwv.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2cqlhufqk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2avnivwuk.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2yuopxspt.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2hmpgjjeg.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wqzxpmhu.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2vtuygtry.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2rtuiyqje.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2asefaejf.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2japwbcif.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2gzashgxr.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2gwacfmxg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2iigrklxf.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2ateffhxx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2dpxkxxra.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2pbkxoelc.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2rmsraxkh.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2pilchpal.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2flchhmse.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zcuuxves.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2auztebhi.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2zopvivgb.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2lxpfoveu.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2mkynhlnz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2vuhamzpk.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2kiyqsrps.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2mkpyndef.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2lbowcwka.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2ptydnktd.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2acsujoce.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2kowttdlz.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2jbnluogk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2vqnuxaqu.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2cjmcjprg.html


<!-- 参考信息 -->