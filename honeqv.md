代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3zbzagpvw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3kghfplmp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3eillplcj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3jmvrpbyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mphnxapt.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3ruycnbiu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nyqqntxm.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3onuezyrz.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3ixkwbkns.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3wmlvvptc.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3gfsddbgo.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3yhwkhhyo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3nscbnpac.html

);
来源：http://www.52xcode.cn/Article/details/gt3lqugkqct.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3tdkcbjpt.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3aqrndhay.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3onwmmqwk.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3gwriqhdl.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3shdcaqkg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3voegqyic.html

);
来源：http://www.52xcode.cn/Article/details/gt3jyccqwcn.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3jiokbsac.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3fsgwjbhi.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3wrzecezr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3siidrqrz.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3fvmqkiwv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3gkxmsizi.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3udqkizja.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3gvedgktj.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3fjttfoff.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ssocuedi.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3idfpttaw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3arabpxkl.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3wrqyjrjn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3mbrhmkwv.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3xnhxufcw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3tirwvuuc.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3rrcxsqkc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3quwvdswo.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3xrzglbde.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3ppslzfsm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3vipekgvy.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3pkliduka.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3qdhatmhm.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3jinveqzr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3uaprzlae.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3hbyahdep.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3abhyblbn.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3doxklhdz.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3shyunoyh.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nvzrpbna.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3ukdtpdwi.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3liszrdtb.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cljmrbiy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3aumsdkmf.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3wlcnmmwr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3eegzsaws.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3zgsypbae.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eyoqpoeh.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3zqbrvbrs.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3hhxqaoyh.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3xoxoouty.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3xidppzbm.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3cmsvwzyp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3zlsfqipk.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3tevvdxaa.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ymkvbkly.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3cmvexiqw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3lllmjcch.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3crbegiag.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jvewbred.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3npsjfdct.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zaiheggm.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3fidtpyyi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xyuyhjnt.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3lfwhlgga.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ncasqhbm.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3tvvdsqba.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3klfvueom.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jdkpnzuc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ecuwkcwi.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3fsdleyuk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ixulsbbd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3vauatmrb.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3ifxilydb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3fafrgbqq.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3qbkploag.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3bmeehulx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3aslmbbjs.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fzepfmqr.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3gbrlaplo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3atkulixk.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3ykfkkbvw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3anekguvd.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3tvaarapo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3nyfltzaw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3lmyfylnb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3iaujvnzz.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3mxfweicp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3xrvkadsy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3vulyehym.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3edxysnjr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3ybkcjpjy.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3ornujvnb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3fogrkxrf.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3xrbdabib.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3kyiekywq.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3itakienn.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3nuducdfd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3qlcxibri.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3aimpifrh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3bkeyedcm.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3fddzhprq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3qqreerik.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3xwposizv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3qeoeenih.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3kibqfwjq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3vjdoievm.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3xxatyjcy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3tlunzshl.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bublcxyi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3govtnmul.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3vilehxgj.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3fwgfvmce.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3hjsiwsfp.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3agojogfv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3aauzovjz.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3fdfzubch.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3rwzzvosq.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3olccrahq.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3devujvze.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3dngmdwpe.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3aztkehzz.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3grminwpq.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3ctkpggux.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3ksqvghdo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3wrquuyip.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ukwyygmx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3szjvkjep.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3ubcvapfy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nrduozkd.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3geyjxugo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3muqynxtl.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3enpmzsrq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bodmuvrh.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3tdrajmtk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3vqxhmvlb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ogjyetjk.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3slfhvdzk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cbnklrqv.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3cojudehn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3sbsvefzf.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3bmjnlpgy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3kthzpxlb.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3iyqqeupg.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3omcgijjo.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3yofkdgud.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3gsikzvww.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3sscyqxos.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3hjowerpy.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3fkwmidjd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3ibbukzqd.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3bgfkpfhw.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3pvvpkywp.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3awskmate.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3bkdmbnxr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3gmtobbgf.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3nrwdjhnt.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3shalylzp.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3udoypjxr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3nptxuyjs.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3ajvrfzgz.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oygacnvl.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3wggtghgi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3ovkhwfdj.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3oijgpxjf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3aqeogwkx.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jmtvuvas.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mykcrgrd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3vldeoozp.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3jdncmrgi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3vkhtgqpg.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3mrgxfocp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3jgohvkfx.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3sdublvmr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3rewgjzot.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3fmvlaecx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3bubiqoul.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3btlxxxwd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3umyuifir.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3xnbgguyg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vzgxayas.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3rafujnac.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sefkkgal.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3tgxpijfy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aicocojy.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ykjrfguy.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uyksilhr.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3ulnxkutf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3pcpywamr.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3ipmcnahl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3gzwtviam.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3saiwvrwc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3cljaesor.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3mnmenqer.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3czvkytka.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jvcoytab.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3durmitco.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3tphgydqs.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3thaxzrfn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3ivarplgf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yolyhhlk.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3burymunn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yuicaeno.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3vildnkmn.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3hikggtvq.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3eehuwpzu.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3rinbdtws.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3vecawdcy.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3beihukfb.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3xwofoidw.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3zuxfaiox.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3krmvugwk.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3qbibjyyx.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3avrovqdx.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3wihkxldo.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufjispdk.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3yyipkdjr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3gshnnzep.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3xgupazdl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3rsbueldc.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3lksztajo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3rdpnbnkw.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3kaxibeyy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jpemitno.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3ocfaasqf.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3loyfuaat.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3llukhbov.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3epadkexp.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ghsehbts.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3mbcehooj.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3jolslzxt.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3bqokjtop.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3hvmcsbgd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3pyqffogt.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3clmwnjka.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vzfxlwkh.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qgetjkjt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3nimdsquw.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3uadbgtuc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3suwvnhah.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3ssymixii.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ffftfihb.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3xxhvpduc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3twjsvvwa.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3anapfzgk.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3kxpmoyox.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3ftskfguf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3kfdwqqcj.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3aetrcbwi.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3zfqzwawp.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3uxbbvvln.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ethqljow.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3txoadjyr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3uweieohf.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3wljwztzo.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3wuqainfr.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3nlytuvnm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3xosgohrt.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3alnjmovi.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3llclszxg.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3tkkdvldk.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ncdgecta.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3hibalgvm.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3txthffut.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ljqoihgs.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3dpbezwfo.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3avdbfqvn.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3rmkilocf.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3mbfsgrgp.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mokxxkks.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3djfrazch.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3oslktmry.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3fqswplik.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3gjctyfzi.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3gkcqzksy.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3wtduxifc.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3cdqidbeo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3qyspmdgc.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3mitrsnhn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3hnjzipup.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3hgomykzx.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3pyewzoit.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3kdnhxhir.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3isuzscut.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3zfmgtaea.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ngupfwbh.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3dadezjsi.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3hjmmnvqk.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3giqflfmw.html


<!-- 参考信息 -->