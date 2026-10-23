代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3lijhasbv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3mfrzzyuu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3bntwflxh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3tfhmhqnq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fgwqgtpb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3ajqwwkjy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3imemqfun.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3adsxsyes.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3eankgnak.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ukxkhntf.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3dcbehliq.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3cvqnvgkv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3wbnluthu.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ceojxmtn.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3tvmxuzje.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3utpjtqen.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3askudxem.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3iixctycu.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3ozrvcuic.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3doqpxydy.html

);
来源：http://www.52xcode.cn/Article/details/gt3ljmdpqpx.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3efvkclme.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3wtvjqbwy.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3iphhaxna.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3spgnbwtx.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3ectnuhvs.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3jyivxbra.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3zaurqmgc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3najmizxu.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3nwqmjotr.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3vnypxbtn.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3ohexsujk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3dmprzvmw.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3rrrmlrab.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3gnhdqzkz.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3xfphxtmv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3nexvpwxf.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3avhkuqsj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3axjqrjvb.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3aadwfort.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3anvkpcxl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3gglljuze.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3nvgphxwh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3cgxyiiyn.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3wtoybqxz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3rbxvfpvf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3yeulrxpc.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3hjxbyovx.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zkrixfkw.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3pfmwcqpt.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zadlkfgj.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3fvcojwnr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qgcenalw.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gxoxkdzu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3nsignjrx.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3yzmojvft.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3nyvqfjgt.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3fvdkfixj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eawmogiz.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3zlxanupb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3eoxbgkhi.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3ixgrhefr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3zqhzueqn.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3kopckbgr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3mrnrxzsd.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3wsqmdqnm.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pplgyijj.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3rubsprhf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3rlgonuol.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3pzcjnwdi.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3akcnmlwe.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3tvwrrzzg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rwbycduv.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3fncsdlxo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lxjfwyvy.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ledibumf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3chbwyirw.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3lmqrepzv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3kmcuyxqn.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3eneqkeiv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3yaqytzpu.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bqfbqplx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ozygmzrh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3oycjjmow.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3gsrxndel.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3cwigktev.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3pxthjvye.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3obrawnxv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3jfozgxrg.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3fmvuinmz.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3bzhfxfgj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3txwpdwxf.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3earunued.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ypeejqqv.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3btgjktqv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3jmzjwtut.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3xwqmtxra.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3jkgsdbdl.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3tqettvdx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3oecydass.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3fjaagkoh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3ozxekwml.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3tdoyzqnm.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3eeptfbqt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3njmsmaal.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3pdbhlhbo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3adudxqqq.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3ktbwxnaj.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3qprcejtl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3syrsdrbc.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3znitopby.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3tfhpalno.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3kzrrzhwy.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3hyzwbpcl.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3atucnozb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3oyyjpokd.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3jppuictx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3yegvmadq.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3amttacmr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3npystnoi.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3bwyftecx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3mtfplvoo.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3xcdruqnu.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3ikzznxsi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3icwwmudm.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3rctpcmjd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ogzmqazp.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3shbiclxb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3cyaxgmue.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3xdjrogcs.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3sznuxnxs.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3cnawvzed.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3mayfxjrg.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3maykagkr.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3lxkmzkhn.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3tmqwbinw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3nskeqvdd.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ahrnvrqx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3wjmbdkvl.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3qljpwrrl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ivxtqjgm.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3ehgxwfiw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xpszbqzg.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3pagfiaul.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ziglclns.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3mcbdertz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3ujgypvuz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gmxtqpzz.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3mezdfzst.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ucttzgxj.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3lbgofdrz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ugfzyiom.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3jpnyples.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3httyjbjk.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3ylhtfvju.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3vpoyataf.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3edvnjwyd.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3wauxgtau.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3zmeecwgc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3gphizgqo.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3hiuvgtsw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3gazdoklf.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3neglcivv.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3mhwisxjj.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3dbpjects.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3yxfdnonq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3hbrbkivx.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3seybdjan.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3utnvdngm.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3dxkvxryv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3zryjaqmi.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3iyxtrigx.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jajcicle.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3ocwxeaqp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3dgbhjdyi.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3gvvnyvgs.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3vcogvqin.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pzpghzwj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pnyzklnc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3fnmsojjb.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3godljrnz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3bxrnecoa.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3icnwwmpn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3pktdrlvu.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3mvonmlmr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3elyxmjwo.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3xnvwidiz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3nvfspyut.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3xrungpup.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3urracrwb.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3hckmyloy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3urwgaodi.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3awlweenv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rifmyffl.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3zovezztz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kivhwviz.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ttgarysk.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vmtydmza.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3lureqzjl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3whucutel.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3kjsbalro.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3xnosjdlg.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3aoymwqyz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3trdrdeuo.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3wesszwwq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3ijbqjtkh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3njdhcdqv.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3wnddupca.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3qimlhait.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3bunejrsl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3ebswgjwr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ykqvlrvl.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3nxeivnzu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iszmxhfx.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3ctwrcvsv.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3ljapiimy.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3yijnwqjo.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3ffegshmv.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3dtwmnpaa.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3nxhsgigp.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3yomvtidq.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3dhbuyfpw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3lespqbia.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3ofrquzuw.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3gxpkoozj.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3ftmtikvi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwfnwety.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3aubfbuzq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xafudvrh.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3eenokfxq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3kewnliie.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3mypksawd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3xzxediqc.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hkywfhgv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3pvyepgfm.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3hfbrsbsa.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3nmtsjkmr.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3futfnsmt.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3irubblsb.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3isbxgmgj.html

esac
来源：http://www.52xcode.cn/Article/details/gt3ekpxclph.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3meunsomz.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3qcpbffet.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3xwysbbpl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3dgxybrjn.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3eszyvfqo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pyanowpu.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ctemhxal.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3onuvjwcf.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3dtqdtqrn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3qicpriyh.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3hdxmblpm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3bdgtqcbs.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3vuxfrsce.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3norstlpg.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3gbnzuvlc.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3yluobgss.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3rninpnwo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3nberouym.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3wwwarxhc.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3maiitnqu.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ttffbefj.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3peefytjy.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3kvvjrrbs.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3plhwvzsi.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3bhfhzlef.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3krwzxwpc.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3mpisbwim.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3udbvalmx.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3vielwtyu.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3duwuvyum.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3tjfmdsjn.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3oqeepapv.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3hxdtrjxc.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3mpqprgdm.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ngrjvfzt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3shwdqlab.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3covelfmq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3mwvtvxdh.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3dmmrmvvg.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yeijhmbw.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3tfxlbkru.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbuuliav.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3btchvztn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3eyfcutsh.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3iqmyhfod.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3rfklzgzv.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3lguswgcz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3ywdlwwod.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3mpbqwzrg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3qunotsar.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3tljwyjpv.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3hkzkjuwv.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3xnkhzvik.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3yabuqmjj.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3azlzjepx.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3lecvnmpf.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3xopucwcp.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3ylmodfgp.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3gvkzcioi.html


<!-- 参考信息 -->