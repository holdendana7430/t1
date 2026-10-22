代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2vzrqjoca.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2gtgvsneh.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aazfvsko.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2gzfecfgz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2vczzwkpe.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2jnlshtow.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mszfibqv.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2qighrtme.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fnvffktn.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2wencogye.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2imfdiepp.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2smujyijq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yprkquis.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2bkhdqvsr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2eisgobhs.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tcxmqpkn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2begdpbrp.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gniiggie.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2gppeffbs.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2agmfxypj.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2grzjxvnz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2zxljnzcf.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2claldqpt.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2lznkzpoy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2dxaojdaq.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zrimarcl.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2xnrbsajd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2vjryqsjp.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2vochkiff.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2rohmyzeq.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2huyvdlju.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2cnidnuxw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2jstbfaci.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ziwqnaof.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2lwmcngdv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2ibgpzodp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hixuaisq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2ollrqzva.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2nqnqrutj.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2jutfgbcu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2mhzownet.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2vyuewfaj.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2qrljmzgq.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gqboimcf.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2aaxsqbkh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2jugabcns.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2fxesngoh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2rzlixwnz.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ghtfgsqb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2vqhgqsvk.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2omiwuifu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2qlwywpot.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2mploutbq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2aemkycmh.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2gmyzherq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2upvktjld.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ffiptlhx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2bwmalehq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2uqhkisng.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2yzivgcdc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2myunbzjn.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2oaayxcph.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2hcpntanq.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2nucmhsfr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qdcwgxnz.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2jeudrkmy.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2tjdznktm.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2ysgcagdk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2hgfmkrgo.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2kkjljnfj.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2xkfpnvua.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2hmuouqud.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2mugcjpnq.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2qsrnrmjq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2emoocqqx.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2bfkonupe.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nmylhlub.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2mqqvenbk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qngqbskz.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2irxpysuy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zfvieskj.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2cjveslrj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2rntrafsg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mdslbukk.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2ubfswvxr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fubtvfrz.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2beziiffk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qiceqzes.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2bxqnunfi.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2snnggijg.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2auzoxspc.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2atoruejz.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2nhjpgmpd.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2vsihodbs.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2pbauwwtb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2wplzgogw.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2bhdhpssi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2jsdqxrws.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2raijeott.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2gwnbuxbl.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2ajvlxmpr.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2qeuuyasi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2bbkkydny.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2vijlrjag.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2xviblshj.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2mquuegqy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2ndxhdrpi.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2mpxhkbvc.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ftanlnwm.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2kdrchdtp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2shvwpdgz.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2inpwxzts.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2sswhfsmx.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2izejicwi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qnctqyht.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2jjrxvecs.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2idjvegga.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2mwecajxj.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2ivprlayg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2csmysrmd.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2xqgzwiwb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2yktwftyq.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2amanhyzy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2fubhuqkm.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2tzarbebi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hbkvhgse.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2mpyiusat.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wptgaqmx.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2ettxvbba.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jhftujyv.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2bfhdkjih.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vwuxhump.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2nonpjerm.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tzmfvkhk.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2tkvokruv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2zvvyhtza.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2gjxfrkyn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2wfdjgbou.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2qhaximwl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2bmwgtqma.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2kjnzrezx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2ajglufye.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hcaoinib.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2lebrgkqw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2xymvcwyr.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2xogajxlp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2fwmgrwym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2htahcvzq.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2ukqxsxyl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iuklidkw.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2xlkpvfzv.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2mdgchquk.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2cpnccuup.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ocrpoahm.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2edgpccfh.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2kmjfqpor.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2rygvmczr.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2nodbxhmh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2dzswnqac.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2chqhldoa.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2byjzyczs.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2vehfmaip.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2kjlqvhzi.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2cununmbs.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2kdplkaik.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2uhkkcgld.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2qcxjdfsw.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ynfelxgv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2fdaqwovh.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lrjkgpdx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2nuvgjtcd.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2glmzjhyq.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2gpmktfzy.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2cbgpinyn.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2ljctqlpf.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2mgedaxhd.html

esac
来源：http://www.52xcode.cn/Article/details/gt2rrjziggn.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2nbtitypz.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kpalarau.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2rrfrlcex.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bhbcvtzn.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2lvnzhxve.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2kcmqdkwk.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qdxfvsyq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2pfoyvkke.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2zydkhimu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2pzttsdtj.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2nodfsykx.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2kkgncfgw.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2yzhrlajh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2aplgumlo.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2hgawqxoq.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2alvnvjfc.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2sttxexiz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2jbruudyj.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2sphtpvkv.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2hqwdxbzh.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2hxtzronc.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2epgdours.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2phjqntri.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2uygzmjce.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2vlqijqmn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2crzmmzxk.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2axgccxts.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2nbrljwaq.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2neqgwdyw.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2mggzglrb.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2sqzrwvwa.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2kjehcdez.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2sgwxgxbg.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2dxdqflbk.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2qlbfudfm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2oshmbsoj.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2mwlzbbbu.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2uezgnxhx.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ytzhtdmr.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2kmzvtbgi.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2imvwddyd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2joqjasfd.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2cyidgktj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2crljvtta.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2txvrhiot.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2fnsglrjs.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2dumxphhr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2hbironkg.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2trgrstru.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2bonqesje.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2sjkjkfdt.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2vlrqbcic.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2wxugjqbf.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2abhvvgif.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2abfqvrjd.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2fkkhjkuy.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2cvnsifht.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2xbtpvits.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2mrfccvbo.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ayzjpbwx.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2cmmunkic.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fespqexu.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2pjniwadz.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2bloebjmm.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2uxnmicxy.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2avynhinb.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2duszwmba.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2ytpvlvck.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ogqjaqyk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2lbdpongq.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2kpcdyooz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2keorwwqq.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2qmsrsrod.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2plhfrfml.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2nafhgokv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2zzuqdetk.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2qagfhuqa.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2bebmugga.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2qsmkpgsd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2obdckfry.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2fytskrvx.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2gqyontcd.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2bsijywtx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2vqvonmng.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2lpuqtioh.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dwottvjx.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2zebhjhkz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2owozkmij.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2myylxxab.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2jwjzweip.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2gdpahfht.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2oibxfqvl.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2mqmpnaaq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2hhmojzho.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ovwrnufv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2qvxugite.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2fgxdbdyz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2tatahnjl.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2zimppyit.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2wrfmdudu.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2pcdkesdl.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2sckgzdit.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2iuitwfzn.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2ycmtkxfz.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2twsfbvxw.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2vgbcakbs.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2hkstjxvs.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2fiscdijj.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2srmssmyj.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2uqicxfkx.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2thehdlsa.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2laixqjot.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2yuamqwml.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xpwxkuxo.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2twmqqxws.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2watjawfr.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2xumldifk.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2ugenksmf.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ymfsutav.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2nzppbnak.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2wxqmvnjn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2rvcwekhl.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ixaiakes.html


<!-- 参考信息 -->