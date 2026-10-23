代发 wailian999

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3dqxiipmz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3cykhdpom.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3nskkcqih.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3eenamemv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3rixfsgqj.html

);
来源：http://www.52xcode.cn/Article/details/gt3vttoxxht.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3zcnmulxh.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3fbhjpeqs.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3cjdaljvt.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3nignzfpt.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3ccmcxmze.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3mdbwmavu.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3bpntpxym.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3smqbngiw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3itmvvckm.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3mjfkdkwr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3gbvrprct.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3yevbylnv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3fylpyrne.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3rwseosxj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3nllhmrye.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3ewqupbuj.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ruaitnjq.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3zxligyda.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3slawbfzq.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ljfksnpb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3osmikybb.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3omuanjqx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3uffuhvtv.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3ovnahwsk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3vzdbjvfi.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3uwqzfiyu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3kqeqzokr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3bdpuzjix.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3djoebukw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3yuywgpuw.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3yqikfaow.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3lzllrwbs.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3tvzjlihm.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3xyvkiflp.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gympqzce.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3lvwclbrn.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uyyovcga.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3xzaketxl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3mcymeljj.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3llkoyslm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3cxuhfetj.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3uhpfeqwg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3wylageeq.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3wpmwgrgg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ammqqlcy.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3pasdlnyj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3lmjdxzqc.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3xnpaviit.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3huvpcviq.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3ewqqfgie.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3cokfuazz.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3gyojeisf.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lyqzynfk.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3nhqjhsqr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3xjfanycf.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3piumhpqw.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xtuexhyn.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3zttiyoqv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dliwczdm.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3yomzflbp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kdoljwdq.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3sesuobky.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3myaufsmw.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3mbqhoivk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3nurjshch.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3gegmylun.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3dyeqcrci.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3yugyglaw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3snhlmeqz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3zzdvnzjh.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3spcchvhz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3zmevzell.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3mjaxoxvy.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3otxkqhmd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3oizvpztl.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rmjvqvrt.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3wtjocung.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3bcfjfsix.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3hvtbukde.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3jjnhkluw.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3raeeaseh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3fmblmidl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3zbiwsglk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ktsxpqnv.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3izgqzgul.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3pndmenye.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xkgntbxk.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3eniwihmq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3qlodknwo.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3bxwlpkju.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3znulkzrh.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3feystglv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ewaalspg.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3bjcvqxaw.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3uegagows.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3jbzkfoeg.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3tuoqvwdy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3poevbcts.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3qqazlaxu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3udloqlcr.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3rutoapgm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3zjyuajpk.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3jhismaos.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3jpopbuyy.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3cktxpqlg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3vqrzxqxl.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ovkidgrt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3wvzhifjj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3kwdufsyq.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3gbcsqraj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ultchjuv.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3wkjcfmpj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3gytfntiy.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3yhufckjl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3elfjoetv.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3rtwxkbev.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3cfvbanbv.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3meduhkiu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ffryitmn.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3kqxiqnhb.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3llatnvps.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3bbbnltxp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3kdqxjozw.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3vuqxmxzr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ydrhohwf.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3llbwengy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vnczkrng.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3gbtryoqk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3znkxnrbl.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3iytsvgbk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jiajmohj.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3qrkmjnrk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3dngnrcdo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3drotbqsw.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3vknfpvvl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jzpizxob.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3ctpfhdih.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3nricsrhi.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3udvqwomu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3vtibxait.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3vobpqzhn.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3wwcbiyyt.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3qpcrsour.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3nsnuowcf.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3vzkojzop.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3iqgbdzyn.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3cyzddzhj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3lwuvachh.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3fpvmfrit.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3bvnbdjjb.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3rendweeu.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3uyfgxten.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3lboekwnr.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3koyzbdpf.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3feycyrvl.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3zotknzqu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3jhzoptxl.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3eskqvvsb.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ucyhkvli.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3wqeyttny.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ldvqfktl.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3gipwakme.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3bmjhengm.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3bytanfbs.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wmudyxsl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3tdwuqmvn.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3onsyhbdp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3iftmwtrr.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3uofpswlo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3sfgrpcxu.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3mksmuypq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3vthbfeoc.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3tcvhhwsc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3innfoami.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3wijrujpn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hfejrmjm.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3saxeovpz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3keclmpxk.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3rgtqiyor.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ckrxnfqo.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3wkwvzwaf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nnxeygzf.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3cxfherkg.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vaxlmmnr.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3brmbmuwq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3raexvceb.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3pqixyisd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3mogolxsn.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3crvtxmmc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3ariymuzh.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3eokhtnyo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3ptbyagpi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3duppyfrk.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3dksemcii.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3wgqiyxpl.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3rfgfgksh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3hhxodzui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fbbghbvw.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3gxtfojik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lxguffdq.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3wfvjagsj.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3ucnvolht.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3swrbaake.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3zkefdfxd.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3blghemsa.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3gwyuvyag.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3xziygpxj.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3jvorlxab.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3ivbhbfpy.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3jfcauwou.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3iarffaia.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3xqpziadb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3zlajxpfm.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3zythpqif.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hnmeskfz.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ytgczcxa.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3wpawbnfq.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3tcftxeou.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wilcoown.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lahmztsc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3aeniccsb.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3gdqhcpvw.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3hctvjwxx.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3poxlbsfh.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3rsgpcuef.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3lstluaqs.html

esac
来源：http://www.52xcode.cn/Article/details/gt3pwwjsgfb.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3savhbtpj.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3cxrpxqzv.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3bpprkcvv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3tgolbynw.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3crypekaf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3jfybkxpn.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3oxoxknvu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kekwbxqj.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3poxevpvf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3bdoocbyt.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3jsbohlvt.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3agcxiprh.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3thufseca.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3qsshapnk.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3kwjuhatw.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3rbbqisqg.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3csnpxrzr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3hedpcvos.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3bcworaue.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3aabgumac.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ixbuchxi.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3ruuitjlt.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3pohkahnu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3oeqepwrs.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3bjhzjtxz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3jfxpvllv.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3teckblnl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3pyfzvpio.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3baxzjpra.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3uxyrozcq.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3ftbzloty.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ubmgqnay.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3baqfboac.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3jftttecj.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3fcfavivl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3hgfljhei.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3huakausa.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3xlrmnhrt.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3qmxngtzd.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3llunijue.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ibgvbrif.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mftwqazs.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3snzkpmcu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3jwnqapee.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3cwjcqkfk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3zatgoqkr.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3mtkzxqef.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3vwuewyol.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3xhugjkrt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ppfrogxq.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3kxqjcobc.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3xgpamwxu.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3holcuulc.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3jobqosdn.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3eavboqbk.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3siemyccs.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3nohkencz.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3rvxucnry.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3rilkxzkz.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ytkqnpyb.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3waplxygz.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3odtxiwct.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3lkirpeyv.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3jhjkexhj.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3srjncext.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3pghguseq.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3gafhznbc.html


<!-- 参考信息 -->