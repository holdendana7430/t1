代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ixbtmoic.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3vtrvfdlf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3tijppoyz.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3iltdzrkg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3mdwrrtli.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3lflpcnqd.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3mkioiryo.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3fwitffch.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3pyemhqwj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3wmkwpxii.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3vvfzgvgc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3fwezrozj.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3khabrvvn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3mzlhzmcy.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3sgisyqzk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3iurwwrqy.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3rnthgsrk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3uvymxcla.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ahbyfguq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3zvdlxyfg.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3xoytakzu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3mfnypxix.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3uypjbysg.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3xwpxbdbl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3oqykvtqx.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3efucdunu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3sdtltupl.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3vozxzkso.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3wtiijqip.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3nmpcqrfi.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3htufymwc.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3lsiddune.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3vfebvkvz.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3zqsaglso.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3sfplimwe.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3lbuisbgi.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3nltqlihq.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3yalenwqk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3avendzer.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3lysesylo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mucxipxy.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3zpnodaly.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fhrpnynl.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3iertajyc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qshdsnjy.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3ttuaoaid.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3pxyodlqg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3toxejeay.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3bnedjnby.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lkyucfxg.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3rfgleyct.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ahhndnpi.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3beowbjoo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3rnbdfqat.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3wibywvig.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3xcmxupyq.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3ovdykxbi.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3artkrwep.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3gctxqjqr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3jtoltypt.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3hkooibfg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3szxpsrae.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3edbvjami.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3gdoynlrx.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3nnvwvvtk.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3ajvcpvln.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3csijeqsv.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3beqqkpgi.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3vqnxddsi.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3gjokkipa.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3dcagwutz.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3mtqqqlxa.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eopjdlct.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3topmqsvf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3eyixmqlv.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3mpytapnk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3qlmutxql.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3jklkkrlz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vnnxxtwe.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3ahzhfxkp.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3dtpwexig.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3oejgkbss.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3mdcvvofo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3ywxnutxa.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3gekbiwqg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3otlfwznz.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ccwlrlvf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3eqdyvhpx.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3eivjpglx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uopytjjp.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3wydhvtrv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gsnbzzvr.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3taxxjdgj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lrqdpgfs.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3mwawfsgk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xgrifpbz.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3shxqgiyu.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3chsnlqlw.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3srfebgml.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3bajqmisf.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3soazozyq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3htuhpyel.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3dhdjgqxc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3twzzmshv.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3tvjedupc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3fskyadqe.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yhvcfrbw.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3alknywtk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3hkirccvj.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3jdagrxox.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3udeetmve.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hoortrkm.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3weooglsj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ayuttull.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3lgpndikx.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3mvpwfvhs.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3vogqzevs.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3tmfrfakw.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3dnjgcbpf.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3iyawydpk.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3vbtbroxa.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3kzslhwlm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3cctqwzaj.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3dhqqqsng.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3vmduhhgu.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3njeyqmnf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3cwyqgyuf.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3vfidnbjz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3ljgotdfz.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3zyymacgc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3uxdqfefl.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3sratocwd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wtnixbjp.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3eqcsnxwg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hucsudib.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3fymbzuxh.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3iijpozvo.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3pgoctwkz.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3xyopwcot.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3tthrpbnb.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3xajhxlqp.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3ighclrbs.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3oexmdebl.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3qpejivfw.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3fuwbqntd.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3pighwwbn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3eyhbnnhd.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kfuuazpr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gzlummeu.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3rntxpbms.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3qyipreym.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3suzkpryd.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3hnxuedst.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3csrljvyf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3aeblyiim.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3hktsnsrg.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3rdgmgadn.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3qnypnmzq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3coohmido.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3shvfvons.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3swwxbuhm.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3mbggvmqe.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3xgedrgsg.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3kzshyyld.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3pzdgdbcm.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3tiastjos.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3rjbzuvcn.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3iprcmpoo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3oskseuze.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3izqvmyor.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3tgakutuk.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3wrhrjlso.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3saxmpzqd.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3ucbheinm.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3xfhvqaoa.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3lvedykdp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3cujrbtcr.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3lvuahevw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3nwepxveg.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3nvovvpzl.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gfkqbuym.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3syvaqwxc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3dietoccc.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3aysltsrm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3nzzrtkdr.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3jfhryapl.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3mijfddcl.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3zwahxhzf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3rqocvzvo.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3nuehgblx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3uhxnalac.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3mfxqlkbh.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3zavmuyvx.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3rqbafnyz.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3vffxlbkw.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3hslkyiay.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3kxoibdju.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3ezjfcigs.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3xrvlvish.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3yxjvhnrx.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3drfpzllr.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3ixvsomtb.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rouefful.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3ajfbwusu.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ubxhyhwm.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3mgyofpfq.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3eqazpask.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3karxjnql.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3lshyeicq.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3sjuqraxb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3hjyatzdf.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3abdkmpgf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kpvqqqnw.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3jemlqmle.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rpghkelt.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3cvhxohox.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3jwcnkvwi.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3uldqdntn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3lpnxfyno.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3klobsewt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3lvsenoei.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3qnujrjsa.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bhpdbxci.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3jivwouif.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3azymqxde.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3evowllxg.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3oqaluoag.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3sjfsmstm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3sonuvbxg.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nncjzzeb.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3slaluazn.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3mxatpnkk.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3obeduhwt.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3amanpngz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3cnsewanl.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zyimxivg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ivhflupq.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3nbbhgiea.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3hpehcnmq.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3xkjyzure.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3asrbukmz.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3jbmzwosw.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3avbwrcct.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3oigknznk.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3riwkgynd.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3wtopdogd.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3xkmxvelc.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3ukdtiahs.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3ipoivurk.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ektjhgez.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3clapglct.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3irfgowsf.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3hgfyvccq.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3pbjymnib.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3syghydgp.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3dubhhwqk.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3qrmlwvgy.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3xkrnzvom.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3usmryhxo.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jzukevwn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3nhskvolz.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3kroxpmrk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ugqpdjtr.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ooxzddop.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3vkxavfav.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3mtrviqan.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3birmqvhw.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3yqxbqaat.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3wqkcvewa.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3vtmgosqr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3aslfmbxv.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3rlloavsh.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3ekgipxft.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3sdrpemzo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3lrawlvsr.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3kyyglolg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3ctgybnyb.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3walaqvaw.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3nkezgbcp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nofaxhxh.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3xsykzxub.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yvlkmdpc.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yymijalc.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3jtlidqkw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3xnnqjpjc.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3oywzyhnn.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3loitqkvg.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3wfmeufdw.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3ntyckzbm.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3bfwnkifm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3tcvqtmlp.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3aljovmze.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ivuabmpr.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3cfmzqekp.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3cxbklakt.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3vbrocevn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ursnokgp.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3xljsnwia.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ddaffrwc.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3zlznoedc.html


<!-- 参考信息 -->