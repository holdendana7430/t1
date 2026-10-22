代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2uzsoccen.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2xztedrpn.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nysmfosw.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2yqtkuudi.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2xoosfwjh.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2xrpybrpb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2svmvtejc.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2isltcecg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2upnjiopz.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2kyfrjghv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2umfwyqmw.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2ebbpqfml.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2flyjmxeo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2pswpmccy.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2zrvhpzbd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xeirxgur.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2ensntple.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2ctfawnrt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2rxckxlho.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2abkmnlqh.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vbftoyyb.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2xoyyyfpj.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jerfwoed.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2cdemyrzl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2henfqppb.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2tvexfhge.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2lkehwdgk.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2tjssdgog.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2zxpyuryx.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2iugrnrte.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qoearqio.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2gfdsjfnh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2dabngzer.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2iyhbnbek.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2qjoqxdfo.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2oeijgthf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2wutzpilo.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2gtoyvkzp.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lplrvsti.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2zbcvxbih.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2zdaanpzn.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2sibfzibs.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zubofgak.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2xvkdkayf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2soabvzjh.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2anhtrsfx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fwzrabtk.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2iznlhcpg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2prixcpfo.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2wwxpzlug.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2wlocsiox.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hvxvnyzo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2ioateodh.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gbqfqpro.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ufhjnzhs.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2vaigxhrj.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2mrmlntdm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2tqqqmrhl.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2qjqeqfyj.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2vkzvjtca.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2bbiziafj.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2rhphjjsh.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2qisnxxyp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2yqajbprl.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2vmgeprvw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2itmxyetq.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2qeusxbhe.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2aqxaiadl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2dnqjpubh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2dbqlvbnh.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2oaxpnozd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2hwifycvl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ojxfskmi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2ndrawgtx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2bnmcebdn.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2ervmquhh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2haagjdgb.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2zbraotiw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2bpcgmlml.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2avnscswk.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2epefrkzk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2emportot.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ihcujivi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2slgayybb.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2prfktsri.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2pqaolllh.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2xsfhjkzn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2cqsmmjix.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2awggcmzb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2qejuvleq.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2mdozaiqu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2lwxrodev.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rjhiszsg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2rwjmwbjs.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2ztaltfzr.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2jtepxlyv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2wggjnbkd.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2utdqyjbf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2bzhjpwhn.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2rqqnzjem.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2iwdvzdaq.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2gecynnsg.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2psvavgyk.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2vengnyvs.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2mhffootz.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2kwqanyyq.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2jgoufwql.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2uknnwpiu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2xggmxjhb.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2yrqdclnw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2qhqtdxen.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2lzhpbrqv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gvptgqjb.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2mzxwwira.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bpzswltt.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2ixfntgee.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yxixxfvm.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2jckwlfju.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2lnibgbxr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fkftxuta.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2naynwfmk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gnioncsg.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2ylxfltjz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2pwjuoetv.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2ahqunysu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2lrpjvkgx.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2xctmjash.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2tlgrvzli.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2wxqpuxnw.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2twrdehoc.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2penaudaq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2jmmxvvjx.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2zclrxbnm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2tzzazlua.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2yluijcww.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2gcuypxlz.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ghhipukt.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2aefotado.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2imcjwiyd.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2iiexdngt.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2jeqdebbp.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2juxhxqwa.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2lfmdietb.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2uddzxczx.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wqmsqhbb.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2limwxmvb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2bzibtwyk.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2xpozkauo.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2vfcmgnfc.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xunfxgsp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2osmuwfhd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2dxrdongu.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2nekeczuo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2rwfaalqp.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2dqlaytts.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2jjtgtwjq.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2nwyuomdl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2cdfucxtt.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2milohqjg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2dcnnujsb.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2kxslocgu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kwhaaifs.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2zizowyxd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2avwisock.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2ddwryewu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2acnirazc.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2krkhrslv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2adhvcukt.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2fzxvvwog.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sewvacog.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2fvrgxrwh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2zvwaxuvg.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2jvcusyiw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2zganakcf.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2doxbwpaj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2trpuvkns.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2wggszzur.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2tasxttuu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lyacevxq.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2dkohnuxo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2kbijmwqr.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2wksvbakl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2zfhlcoos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lsuofyie.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2pkvchnfl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2azyxkywf.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2vyckucoa.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2bezpqtzc.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2sdmvvbxq.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2kwvckenw.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2zkscnojd.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2akseyucn.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ghflfpuu.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ntbbqkiv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2evlvzesa.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2lrcevnas.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2flkqbkkg.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2ofwprknt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2brwaayke.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2vngriapb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2idqpganj.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2ihqzbtpa.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2bnsockoh.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2kaouxqdi.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2xxjxseil.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2roteutxw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ebdjqeib.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2nvancasl.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2rguxfogl.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2brxpnrcj.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2dmbdwtme.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2mxgipqrb.html

esac
来源：http://www.52xcode.cn/Article/details/gt2fnrkxgsy.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2nxpmcnhj.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xuaccjky.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2mhmuaiac.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dbiwugcx.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2dnqdieks.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2adteupeo.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2flathomq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mevxrksi.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2zyoeokkn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2qximphkh.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2rjxsccwp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2burqvkff.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2nedyhqcg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bzgumdup.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2pkinafph.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2bwizveuq.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2lhzuztmk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2dgrdtmpl.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2vslgqkmb.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2lmogpnyr.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ljbcgmuo.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2revxdxfo.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2hlowsvzj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2qnrdsdnt.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2tqvuqkwh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ywticblv.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2cqcoefhw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2bujhwtes.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2jrwdofqc.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2afqsnmfo.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2hjfwqfau.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2yforlmvo.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2aulxkxrg.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2hxqzuzou.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ymhqbriq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2egfmrfvb.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2cvetqbvr.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2wwwrdzrt.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2rnguiion.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2nxhzqdrq.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2rivndcww.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhdgfrxn.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2aafejezb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2sfnvfuto.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2xfwokitc.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2tlwgkigl.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2rvlnsozm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2pjgwvwqa.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2rlevzobq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2peruybxw.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2elmhmlmw.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ouncggqw.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2xgvzmxyq.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2fieexmxp.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2ypmeheli.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2gpguuugs.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2tkwbkoht.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2kvnleqba.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2lwyryjsz.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2fdqbmrcz.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2jftmxlbw.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2chhsamtv.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2iuofsjgo.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2kbmxcavo.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2iswshwzj.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2akheackq.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2zyrxuirq.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2uzhsrvpd.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2qntwzabn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2hrrtynmp.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2xllcnbca.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2lzxusdma.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ibqallxc.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fhcgzvve.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2gckdvgqa.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2iclwlnfm.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2vfqrdeuh.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gcgcivhz.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2kbuporqi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2jyfyfbzf.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2fefxfdoe.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2yhfcposl.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2cojuetvl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2hkgukppv.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2zmwcqofm.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2pdkaxgsi.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2orrcpqxd.html


<!-- 参考信息 -->