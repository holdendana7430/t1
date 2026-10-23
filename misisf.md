代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3ograakov.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3dayzyjcg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3cxbzbnea.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3tafnzkae.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3osncquel.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3cukgsvkb.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xfghdykf.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3bpzdnojw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3gocjrwuy.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3detpkjzw.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jhxdyyba.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3rncqplqe.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3prpipvur.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3yzfurhpo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ryjxverw.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3hyqzqffe.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lnluzpyh.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3bodgmeef.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fcirlrtk.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3mfebsxxl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fviiioss.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3cqrpnqlv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3olpmazth.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3tbfzmaoa.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3aohzimnh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3bmctaoac.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3drfijjzp.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3egwpbkgp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3uqgummap.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3doirntbl.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3zhgxkfpz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3qdesorvu.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3ptfoctqu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3rnpokvdw.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3riymlxfq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3jvvgmgyn.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3cjqmoyjn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3mxjuznws.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3vibhszwu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3qbgrhtpe.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3pptkokos.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3vhorzxvv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3szrnkpje.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3ilwemlif.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3bquimamo.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3dfbcdlnj.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ekrannbz.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3zgldplnt.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3endjmnjl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3rhhwobyq.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3edpqqwzq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3podittot.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3zrmlevym.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3chrqsoxj.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3ihssbuei.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3fxxyfnku.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3ndulctlq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3swlbtpny.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3uhxlsrhf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3ngevrobx.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3innakptv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3kthllqzd.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3aghrxvjw.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3zkkfniup.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wickktxu.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3rjgcfumb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3kruzswic.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3afcynxde.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ukesromu.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3rmyymbrg.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3cpvxizqw.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3ikyymnzu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3yixytnnt.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3rxoygbkc.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3wkxnrmqg.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ahzpmhaj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3kkebvqss.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ypnizbdg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3znqrjvrl.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3xwnxcdci.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tbpocjyz.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3ywjnmrsp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wvrxfufu.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3xxhftgdi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fimojilp.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3vytobroj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3lhmkodge.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lyveqhoq.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3dpvobljh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rxoshbko.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3eycbscyr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hatkaixm.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3sxlttihj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3vfebujlc.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3piezwxjc.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3ezufhfbd.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3jsztzwjr.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3rhackahr.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3fzvjicwu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3nqfrlmah.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3cgjhkpjm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3lzfmblpm.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3bfmndfib.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3cywhpidp.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ijipuhye.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3etlqtorc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3kzpfqtgc.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3dflwbmks.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3zdwktzvt.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3ejqekanb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3axssvjkd.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3bdkzxymk.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uboelzsw.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3qdequyak.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3sxntfthi.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3rcbgkxhp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3hhstnqey.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3nxfhcjny.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3havzqdbo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3phuquacm.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3xykrdukl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3yfyvuixp.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ajvbuymq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3lwzusdyw.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3crkjcuct.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3hftfzhgq.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ltymginy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3asqsmmea.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3tuiikueg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sbyegosv.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3lmzesdse.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3genxdqut.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3ymjrmbbw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3giihacvj.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3dkofgnrh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ixzruuqp.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3lietoynn.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wslewzts.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3gphsylft.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3rdwbmfax.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3drlcxvuf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3ckrbuaed.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ogtilxpr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3uzyfazvv.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3hgjsqveg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3lqeegfjq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3czepjnch.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3skarvdes.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3qnvjuhoh.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3ixjafvta.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3gnhtufgk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eofvbcfy.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3syrdbntb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nzieuogo.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3mnknqrvs.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3eiatvxql.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3crqozakm.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3cingajue.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3xeqythst.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3cakjgolr.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3tmyzerdu.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3nigvbcfo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3mwbgnrhs.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3wklvnmkk.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3pcqkmhnl.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3kuxtovzg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3nxfowkfv.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ommspwwg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3tbovzqea.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3dfcrsfnb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3edixgdry.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3okohsmhw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3rhsfzenc.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nyqoyqad.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3hspkiann.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3tvzpkgnn.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3mzqcqzbj.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3ehrtqagp.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zjwwgjip.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zwzrhdxk.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3izpoafgd.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3oplzbkod.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3xhjlkttk.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ufavsnpn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3spgrrdul.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3esjnedrw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3mwdswxbi.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fyxsxlls.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mbrjirsg.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3oimjczex.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3bremtsrc.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3movgiuly.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3cpclmdxe.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3acooucfg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3gqztikij.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3kprxqxma.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3oqehfcxa.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3ffohlnpe.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3pjzwtwfb.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3saxwhikb.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3jktqjntw.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3cyeyqydg.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3bhcwitou.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3oeakssde.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3qcngsrnz.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3grhmtkxf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3cskvivwd.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3tcybuuuz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3wjsekdxe.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3yajbceuv.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3thizptcd.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3snmuvdnt.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3wlcldoih.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3dgfsylxb.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3eicvddyv.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3dquguxcj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3zkfkxuxd.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3bxohfujc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3iicikmyn.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3zhewmgws.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3xtbqwyyy.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3puyndwys.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3kpguvjzy.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3vldcfugp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3msllxmrt.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3bjskeiio.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3zedqfgpa.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3vfktutij.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3upuglnew.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3usagqrye.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3prdaogju.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3dtrssqmp.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3nrzwvkrv.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3alfgijsf.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3iwodcnyj.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3nwfjrulk.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3sfyndiji.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3ffbawdvz.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3mbrfwqya.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3omruwepk.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ajuigspc.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3vfsjjmmd.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ljsbgynf.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3aehwuwah.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3afkosxbs.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3vhkbttpa.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3swzwvgxf.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3ynxuowhk.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3eszksvxw.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3tkhzjebk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3qncaozkm.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3mxkbtwqu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pobrzrgy.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3fwqusuag.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3abfekfwp.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3zuxkgrpz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3vaxqvcmp.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3fxtjnmee.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ciudyteu.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3qnpqhwtc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3utpryzvg.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3trehlrrk.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3jykthwse.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3umiryssf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3soseufoj.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3bkcdnnml.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3dblehold.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3buxxqdxk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3niieqpja.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3zawoykxz.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3hiopheog.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3wqpwgbmu.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3gkhttjnp.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3ddencnjc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3fdbpbcea.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3bbjiirio.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3pppfsrgq.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ryllcflz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3lajlrpwv.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3bclfkdgv.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3lnywtvhi.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3trjzjjer.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3kwqzotdt.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3pbgdmqxo.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3fvvrhbxj.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3fvjxexat.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3dhldrqpx.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3tlvztamg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3njoeatca.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3oykjncdf.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3fuyodtdr.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3pqmvssgj.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3zrlylcou.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3zskqvjqx.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ulxfswql.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3mydglomm.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3bmqxklyx.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3tasrwwzh.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3ufixwtdc.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3wopzoxpq.html


<!-- 参考信息 -->