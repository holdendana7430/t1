代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.hesvh.cn/Article/details/godritqdm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/gzxkolnab.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/ghbgzyegq.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/gwtuadkor.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/gnsyaqbwj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/gdioxwfwc.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/ghmlxbxpa.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.zdbjq.cn/Article/details/gjgysltav.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/gudwocasq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.zdbjq.cn/Article/details/gpwsssloo.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/gdqwxuhdr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gcegxbbef.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fehbvm.com/Article/details/grbyorykv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gfaohfnxt.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/guvxcjrcg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.hesvh.cn/Article/details/gkpylmici.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.hesvh.cn/Article/details/gsuxqejku.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/gkihpawbl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.hesvh.cn/Article/details/gxaecjdss.sHtML

[Q49] 更新单行
来源：http://baike.fehbvm.com/Article/details/gmyegwsku.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/ggmdmdofj.sHtML

[Q50] 批量更新
来源：http://baike.fehbvm.com/Article/details/gthkptwid.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gnmgzmwne.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/gecsksqgw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gqpturlwb.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/gpdgqidak.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gkqiildte.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/gtzyigpnj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/gkccqnzzp.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/gqsiavagg.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fehbvm.com/Article/details/gipjvjjxp.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/gtcxebxeb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/geaggcagy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/geelquvcf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gllvlvpdb.sHtML

[Q57] 行号
来源：http://blog.hesvh.cn/Article/details/gtyzgaozm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.hesvh.cn/Article/details/gccjrvufg.sHtML

[Q58] 累计求和
来源：http://www.share.hesvh.cn/Article/details/gnyggxlqy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gwoqxpjcb.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/gjnclhcmm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gwfopgrxs.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/glnlvwngr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.hesvh.cn/Article/details/gfvdsrtse.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gylhwfbfd.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/gzvxgweuf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/genlpbuhf.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/gixggezfm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gbmzmayho.sHtML

[Q63] 开启事务
来源：http://blog.hesvh.cn/Article/details/garprppgp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/gqwkibkwf.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gjljhdqai.sHtML

COMMIT;
来源：http://wap.fehbvm.com/Article/details/gonywtrmn.sHtML

[Q65] 回滚事务
来源：http://mobile.zdbjq.cn/Article/details/grojhlkbk.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/gbzoscvyd.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/gsbucvmlf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.hesvh.cn/Article/details/gglbjwwvu.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gmhlviabv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gljfgkisu.sHtML

[Q68] 保存点
来源：http://blog.hesvh.cn/Article/details/gdygdjffh.sHtML

SAVEPOINT sp1;
来源：http://blog.zdbjq.cn/Article/details/gqpnjpcsk.sHtML

ROLLBACK TO sp1;
来源：http://read.share.hesvh.cn/Article/details/ggmmwoabv.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gmkofmfye.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gfwbxoqdq.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/gkixplodu.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/gbrcembeo.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/gahlbuvnw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/gcscmmmsz.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/gcmjmoggm.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/gqngsrimw.sHtML

[Q73] 查看表状态
来源：http://3g.zdbjq.cn/Article/details/gtulkbuqm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gqzykqfvj.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/gqupwzwie.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/gndhripan.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gdhijxhbu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/gitebxinm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/gnispvxpm.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/gpiscqsar.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/gdjnewbms.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/gumtpaurk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gmrdqvffy.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/ghznxdymh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/gmglgacdx.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/ghngumhoc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/glmezlbgi.sHtML

[Q80] 字符串截取
来源：http://www.blog.hesvh.cn/Article/details/gahpjubhp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fehbvm.com/Article/details/gqrpghphz.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gmaiqonnt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/gezjhztko.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/gbptqvswy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gvvcastiw.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gyfezlnys.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gyshrcaiv.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/gveohayjs.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gjmbhvagp.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gtkngppog.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/gceethozi.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/gfafidakp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/gcwimroka.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/gkgakptfq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fehbvm.com/Article/details/gzzalykop.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gxclneaky.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.zdbjq.cn/Article/details/gtsgyhloe.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/godwdrmsg.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/genufavww.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gywmfnbvs.sHtML

[Q90] 生成序号列
来源：http://read.share.zdbjq.cn/Article/details/gyrdyytzk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/gnbfcxuys.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtfytlolk.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gapcpcqmh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/guomrzygf.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/gzzspdymi.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gjmjwpfrx.sHtML

set -euo pipefail
来源：http://www.m.share.fehbvm.com/Article/details/gqrzrwjai.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/ginelrvul.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gdgofzrdh.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/gyoinhymr.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gzlcwbcml.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/gmvnzykxi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/gbuexhrbs.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/gayebnlhv.sHtML

name="${1:-default}"
来源：http://blog.hesvh.cn/Article/details/gnzlsqzxk.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/gqsdwmkzf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gowuocmuz.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/grkhvgygu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fehbvm.com/Article/details/govjplvqb.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/gnmaimqms.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gtztslskx.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/ggwpbgxnt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/gpocwware.sHtML

[R10] 正则匹配
来源：http://mobile.fehbvm.com/Article/details/gczqfpwum.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gvzvyakoi.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/gpyrobjhb.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/gezjzajkl.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/gsumpnvwv.sHtML

stop)  echo "停止" ;;
来源：http://wap.fehbvm.com/Article/details/gmjxzoedk.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gkiatktso.sHtML

esac
来源：http://www.blog.fehbvm.com/Article/details/gtosgushq.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/gcqlrdgfp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/gampfmqgb.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gffmnausk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gkqlsuskw.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/glohxevbg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gyydmtyda.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gebkmutbp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/gprpinvut.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/gidwhannh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/grzrfqopk.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gycwfjqti.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gkbkphxco.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/gtmbrsyng.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fehbvm.com/Article/details/gxcsjqroy.sHtML

[R19] 数组长度
来源：http://mobile.fehbvm.com/Article/details/guaaqhygo.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/gwxmmsxiv.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/gpjwuezdk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/gkvpsqeel.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gelsbbrog.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gquxtngoe.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gvboegwke.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gcupxbudp.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gunhqlnyk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gasayajkl.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gmnxhudip.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/glzmjrixt.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/gwickbuyp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/gggzlnuap.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/gizpfjqjh.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/gqnbfoxgo.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/grsqfucgz.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/gtupptpld.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/gliamctxd.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.hesvh.cn/Article/details/gudryurhj.sHtML

[R29] 定义函数
来源：http://3g.zdbjq.cn/Article/details/grourjwwm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gxtuoodqd.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gjdjsyayq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/gwfhwkyvl.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/gminbxaki.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gzprshqdb.sHtML

[R32] 参数个数校验
来源：http://3g.zdbjq.cn/Article/details/givevswac.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gdjsldeco.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gqigukelx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/gywrekcvb.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/ggdnmpjca.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gcbeqveju.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gyxqzrxqp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/gmisgykjk.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gnseutgwq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fehbvm.com/Article/details/gehxxqdno.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/gxjnzzssk.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/gzccksplh.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/goqqaczvz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/gzeavxtnz.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gfbkhfdau.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gdjptgiff.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gqnrteglf.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/gbtecsktp.sHtML

[R41] 丢弃输出
来源：http://mobile.zdbjq.cn/Article/details/grjfbtdwv.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/gsuouiwft.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/gfjjprxos.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/gkapllhwf.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gyptrgmhw.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/goldmnaro.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/geqffnnxj.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gjyppojrs.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/gplwnvmpn.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/grnoyuvmr.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gnddesbrq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/ggkugvrzo.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/gzviebccf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gjqxtjvoz.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/gdhbllirp.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gflaxjiip.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/gtfgyoygz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/gyafusybb.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gjoepfttb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gbjaqbqzq.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/gllivfnki.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/gfafpfrqa.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gchdxqeuh.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/gxhddblrc.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gykbyvtos.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/gnqrnyppz.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/gwplfxodp.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/gacerkblv.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/gmmitbini.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/gjytveiov.sHtML

[R56] 远程拷贝
来源：http://wap.zdbjq.cn/Article/details/gxmvwdolh.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/gavrwobjt.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/gjreryjsk.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/goczjssyb.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gscludvec.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/gembojbtb.sHtML

[R59] 发 POST JSON
来源：http://blog.hesvh.cn/Article/details/gmnpxubgs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fehbvm.com/Article/details/gdppazvrv.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gyshkwwqb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.zdbjq.cn/Article/details/gsdzhxcwu.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gynqmbzix.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/gynfcxjcv.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/giybdycfd.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gogcdxumf.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/gmkfcghlt.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/ggwcjhstg.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/glunndirv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/gsmjruksh.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/gbsgismnl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/grtataxxw.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gdwovkize.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gmkfmvqux.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/grqrqttla.sHtML

openssl rand -hex 16
来源：http://mobile.fehbvm.com/Article/details/glpzmgnqw.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gcjzfgcpu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/gywzvmpfg.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gbbxicueq.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gbypfdxgo.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gokprkfjt.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/gyswohbbh.sHtML

[R71] 日期格式化
来源：http://blog.fehbvm.com/Article/details/ggulcuvbc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/gxryzqrab.sHtML

[R72] 等待端口就绪
来源：http://m.share.fehbvm.com/Article/details/gtxkcfbji.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gcdzkhbum.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/gcbnbkhii.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/ghpmuqsad.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/gqrxogkno.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gdeitsmrb.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/gitcbqypt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/gbmzhimvx.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gdfwspsqc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gfqwgvttt.sHtML

[R77] 读取用户输入
来源：http://blog.fehbvm.com/Article/details/guvjvwkht.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/gakgnagqv.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/grpljfcoy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gdlypulom.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/gxjzrejkf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gprpdypoj.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gxetitqns.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/gjgbdtmhk.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmydjrlhr.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/gqieioqsu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gausudtwe.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/ghckqonrp.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/glqoepaps.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/gyqmtebda.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/gjanjwupa.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fehbvm.com/Article/details/gpyccwwny.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/ginfmrxoy.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/gyhqdtlsc.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/gitrysqnd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gfsmlmrle.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gejwiuqxf.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/gggejouxu.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/gjkawgodc.sHtML

strcmp(a, b) == 0
来源：http://m.share.fehbvm.com/Article/details/gqadcaern.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gtobmsaqf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/gpsucgdzy.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/gqbpiutdt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/guhfrdvhv.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/gcgdonele.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/gjmvfhxfm.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/ghhgcoghx.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gkveoqllq.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/ggrmydtlt.sHtML


<!-- 参考信息 -->