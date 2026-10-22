代发 wailian999

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2zvztvgby.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2hifflydz.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2xzddvthu.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2lriestum.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2ldhandxx.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ygabrwde.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2axceuwtf.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2jtvszbls.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2fgunmymv.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ffwlhorl.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2qtpslfjo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2qrskfksc.html

);
来源：http://www.52xcode.cn/Article/details/gt2rvssaeat.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2jghrsyik.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2oswhrogy.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2mrutdlwu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2dosgxpso.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2frsdcufh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2rmhfrppi.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2abymbene.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2uhqkqbnb.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2wrrkzwhy.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ulsydqxw.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2pcimilgq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2nuorcyuf.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2axxbhlhb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2icwhulgu.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2qmgzkapg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2bahhxdkj.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2wgceeise.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2gbypmolo.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2gvkxcqky.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2rtjidmlg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2tbjpekpg.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2rfaiwjhl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2nzgmhqva.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2bdsmgvbk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2uhsabecv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2actqssct.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2jhxbwbga.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2huseklmh.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ccquwgko.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ytkzcssx.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2huznqczl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2ficfixid.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wcfofeig.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2vgeuhrna.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2tbyrvxtk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2ithhzchc.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2upzywblv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2qdthktcj.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2sodzjuqt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2flknfgvg.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2krrmlnll.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2pqcrdtat.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2qnnqdfxg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2exukiuhe.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2kuiuqjde.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ggpeuvea.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2puphkksi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2fybhzbkk.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2lyqnbdga.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jvgbjgtb.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2jmczaqfl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vystkeje.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2itldhbml.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yqdejukh.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2pooqvcpv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xugudqot.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2uqwlnlia.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2swdqrpfc.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2mttdtsvv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2udashkjw.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wushlrvb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ltrdbcgb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2scdpfzub.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2aoafkzsc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2wgxhnigd.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2dtwqwtds.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2sahazlrr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2vkyfcqtz.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2abxnawax.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2ldutyrcf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2vakrkrkz.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2bgvllxzc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2rkmdflrj.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2wdqrbptx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2fhosoaao.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2utsfkqgn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2noybayxy.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2uhasxhtr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2gkexbfvf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2kijhqndt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2srppbhjb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2gqxbpljc.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2jjvlhyqz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2mqfgghez.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2rlgikesv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2lrfifufb.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ouaisbyd.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2naqonhsd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2yqafiypn.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ewsiayuq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2gbzuwpgn.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2ftxnrkes.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2fftmmqsq.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2yglxfpco.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2bpcxygir.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2psfzppiv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2wvekkhbi.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2qreusufd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2kqaqmplq.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2sjuuynxf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2ebxzwkta.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2hmkqgelp.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2tryjokkp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2bfghqixn.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2rfdzozrq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2aswwdvke.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2msnkucyt.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2uxwoxkpg.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2tpgotpiy.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2rbvfnjha.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2bbhrbeul.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2xmywidqz.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2ihmviblr.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2pievalwn.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2zldrpswr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2pnwhudee.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2oxfukhgq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2oduhqyzx.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2awarhulo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dirwlqqt.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2kjiravrs.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2olxawzox.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2auhuvalq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bexkxndr.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2lwfxwuvc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2lygvwuwm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ihvhpnse.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2ykgpwisd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xzshkvdc.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2bxboqzrf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2abtrmwjm.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2heraqgva.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2cgqsrkyu.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2aouaphxj.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2xvhfgbyh.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2cmrswdrr.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2dthbxgtu.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2qjpclupm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2azsysglw.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2gjerhxta.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2pfzixmmt.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2vyqssxgk.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2rycadtkr.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2ievldwwh.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2asxnosgp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2zurclmph.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2xtdwufwl.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2prveoosq.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ucsnvnbr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2byqwfjyy.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2elxizjaq.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2illvytrs.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2izcgcrbu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2nxhgqanp.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2longstsz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2srkfjwtm.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2npniilec.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zaogmaxr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2gfclbqcv.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2xnargzvj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2hyhzjcve.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2kwaitepe.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2fiqalsaz.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2gkqedbom.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2rkrqljrv.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2rkxmipyi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2hdkwmlws.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2mutfdtos.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rgequhsf.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2syppihmg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mxpybrvo.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2gdllvkhp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pzvtylgx.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2iudnsjle.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qmjhwfia.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2hntyktpz.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ljfjvrlf.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2msyyuvup.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2huxythtc.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2szomglys.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2sbdfsvey.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2xtxkkyao.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2dmuzkokq.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2fsoxssbl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2jtcjqjym.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2osesvkic.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2evfamjmq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2dtbifqtl.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2mcnemlnj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2bxckwppn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2runxhrtk.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2vmlcecjx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kpryzfaz.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2eponfqpo.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2ymohidne.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2gqfstdjw.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2krrjrskq.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2waftslwa.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2nygawgsa.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2vgmbiiah.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ujdsehzu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2gtuygvbr.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2bbnmmagi.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2ihjinzsk.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2vhohsyip.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ceohqueu.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2uvzomktl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fqjbszyx.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2huluofua.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2gxruysmv.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2bixdogrg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2jqvtoaju.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2odpsvxzo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vldseblv.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2dfjaixij.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2rgnmicfv.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2jtirnonw.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2gkpjebwo.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2poxanfqw.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2wwnlaqto.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2llxmemyr.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hpgmbkou.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2kfmcmvho.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2eoidefhr.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2urbvzext.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ofkkkrce.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dxjrrnfx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2jarmuldw.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2brsyzstx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2xcpeirhe.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2oarozzhs.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2cdwhkxhe.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2padajvev.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2cuemnpdt.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2rqzkdbqp.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2jdurekeg.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2bcnuughg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2gjbifoib.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2samcspaw.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2ykbfksab.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2qgohizxu.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2ojljvtnu.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2qczxsoxr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2wzyjfvjn.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2vnpvveqh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ahlyeunk.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2oytvhtkc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2zgbbqtfq.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2cryiyfva.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2zeguknnw.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2ezquopzz.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2bjhidaqg.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2qmbiqitu.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2avhkyukq.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2vsrcbnqt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2nypozuku.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2etdwnoxu.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2qjhyxbcy.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2qbnilqng.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2vgdyojjy.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2hlbjuomd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2kcpwukbx.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2cpxovzlz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2qwfyfnxw.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2jzabrfqm.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2uevjgyyy.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2rsdbzdek.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2nlswvlyi.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2vrhzftgm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2kfgbunea.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2uoyiftfw.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ttmeojkg.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2yjbpfzgg.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2ssjumetk.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2ucycbcab.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2djinlkwj.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2zfjfbxxl.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2brjskith.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2zvremurq.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ecpfttrh.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2smfrdwbq.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2gjuipixu.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2eqzkrire.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2tqvwhidg.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2jbfqwlbb.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2amlxvyfx.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2ofqdecfy.html


<!-- 参考信息 -->