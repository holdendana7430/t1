代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3cbptvcxe.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ehvvkwnx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3stoikztk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3cdvxcmnv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3grcydlyx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3ynyszrvq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3smwjrmcq.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3zauukdjz.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3lxsodnag.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3uyiplxii.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3sllwhepu.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3aecnkbwy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3hseltsjp.html

);
来源：http://www.52xcode.cn/Article/details/gt3ywekvgca.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3njrfozam.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3myazyeen.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3xikrpwbc.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3vvzeafwi.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3yoccypxo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3eyatdaah.html

);
来源：http://www.52xcode.cn/Article/details/gt3wtososry.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ylxfxugb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3scqfjqbo.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3eixbhwrr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3lchaoylh.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3okvtrgdy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3tfliwzii.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3whupcmvd.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3uxzrtydd.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3jkymwlvt.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ppvjqgzt.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3ephnaqhm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3jtttdmfr.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3hwjmyetc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3slentadr.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3jylujyfi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3frbhafre.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3tvgkpevm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3jzvfczis.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3icvkuvvb.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3amkdgatx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3xzyrkiui.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3mqksyczq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ugmaoghg.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3ohlcenri.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3hgkqcjrv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3jhdcpons.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3ydpmyfsv.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3meygtcje.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3xiugypkl.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cgykxocx.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3havfupgq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ygnfljnm.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3pacygnes.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3ibuvmohs.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3xugzrxlp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3dqpcmeui.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3wkcxpuut.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3cstuszuf.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3wlsgzgkp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3rzzvlwgt.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3uvzsstuw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3ecyqfymy.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3zrvlcisu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3szszztjh.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3aoqvnqwl.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dfwckwab.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3uerqshuq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3ifvgnzgj.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3aansmhxo.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aepyfihv.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3ynxzfquq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xdhcaqpv.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ahcegekr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nahohcvf.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3jlzwjdii.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vofaqbrz.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3cdzlepjh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3qhepswwn.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3jucztlwd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3mktfixsh.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3olvhimww.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3jupfpszp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3tihnlywm.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3gfhdbuid.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3yfebuphl.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3mxeqtzhj.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3hrsqhdqr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3gjymkhzt.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3kirrqury.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3msdzzvwx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3gaqdpmyg.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3bccljzfn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ncdixttl.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3dwfyjzme.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3zaocsuks.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3gkbohbbp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3dmryeryp.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3nfuwaaxg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3sfsfrars.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3vqhkmpvo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3dmlffluf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3wvwbyytd.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3isnmbluc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3uxbmruum.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3ofhhcszk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3muqiuvlg.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3hwljdozj.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3rciqqgqf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3thjoqgkp.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3ocicgamk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3mqmlmlus.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3bfmcbodd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3jijgokcs.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3enskjjpv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3xdjfogvw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3nehsiyxw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3dalbzjfd.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3vadkusxx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3aacplwbz.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3skszjmul.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3gavoglmz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3hvhewvfv.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3givbruec.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3uipczfkq.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3qwdrhivj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3mqmsxkbu.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3lyzmjkak.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3guabpntj.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3nuzctypy.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3oxystwuv.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3gqcvjtpr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3rmrifvoh.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3cgobetfp.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3mjhqrcwe.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3dddumpwg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ksqsbvlb.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3nitvejow.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3dzwzfxbw.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3tchbivin.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3odficvyh.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3thpjusjq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ioqmysbu.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3mjgmmscv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ynjjlemc.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3dmbhaahm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3aegholvy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vcjziafl.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3wsiswdkn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dhcdmqdj.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3qagcanuq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3qtxlqjjx.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3sqorszkc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3biheahuv.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3gdruaerj.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3jvsqfyod.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3squbyctn.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3qvrsukmm.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3szcitjpi.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3jnamakdf.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3umyvxouy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3ioillmog.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3gdwseurs.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3yzjsorpd.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3jwkwmqre.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3pvjcuoax.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3bxcmmuwr.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3aszbiwbx.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3nldkbvcg.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3ccylyfcz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3xwyjuwrn.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3tjuxlvlj.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3orcctbme.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3ugbhbjme.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3oejlbbpl.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3obqwhcui.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3bomwnoup.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3szouabfj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gnyzpczr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3fegcbkuk.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3hmzpziqk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3koaeqbqo.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3tspxbums.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3dixzaqiv.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3qrbhebbm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3plmxlxqo.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3flodjrxf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3bpdznhps.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3hknyjnxh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tcmhtdnc.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3yphvnxfz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3esljiuwf.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3uexavhxg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wwnaqqzy.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ertdpeec.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3szzgzwlk.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3skdgcdfz.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3osdzvqrg.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3muotrnes.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3ayxzzdyv.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3vbyhordu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3zihknexq.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ruvpsbvj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3wazcigdq.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3krxzbzmg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3esyqviiy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uakuafyq.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3iqneohck.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3txcyixtd.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3pvulcxiz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3vkrbpnkp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ldykvzyt.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3kocprbkt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gwrbjhjr.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3mmaosvqw.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3itrqsaef.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3rucpstdf.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3dfvrfuwx.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3byttiulf.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3givxkrxk.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3uebjqgsm.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3cnygmjjl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3vartltlq.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3twhbhugj.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3tdnfqzpc.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3dsuelpnh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3dpgjbbxq.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3wkrrmmad.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3roetntlr.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3oznraawz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3aaxhwaee.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3cjhazivl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3jxosyxuz.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3xtkidssk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3xyqwfmhn.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ppgiimkx.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3ayyjufoi.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ueulbsbj.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3aasazjaa.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vbszwrda.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3dftyusau.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3mgyclndr.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3mgnlcjck.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3oipqdemw.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3srxojgqe.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3cuxqzllb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3bemtozhw.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xykjjhrc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3tqvtfvyj.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3jcddlifu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3lorcnnao.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3bupgmtgi.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3ntuovfwr.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3doyuafuo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rekgzaop.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3nrekgxlk.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3fbculvzc.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3vejhajhe.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3tgmiyycd.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3kbvocovx.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3lziulvgj.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3pagxeubc.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3eemzlchn.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3gycsvbub.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3vilfcpag.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3djfmvqxa.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3qmtznals.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3bpkgdfbq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3kvfpvgol.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3tuoypzsd.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3ophvqpim.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3mpfaauuk.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3cnprqsxb.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3lnrzxhvz.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3pmwvemhq.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ywagfswo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3sjproivy.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3yvzsnwbb.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3dtefrecb.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3bdqjuylt.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndbirhbc.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3czkuktua.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3rtsafgom.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3pjxfhxjz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3doowoudj.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3ngacecgy.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3mfuznabf.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3outjanns.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3dfmkvmqt.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3fnboohlz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3dmqmuuje.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3ibhqpwvd.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3yzqngskw.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3wkhqvzfw.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3jpomahmd.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3cslmlwrw.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3zkqheknl.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3qmmqvabl.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3faswjywt.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3ipzftvef.html


<!-- 参考信息 -->