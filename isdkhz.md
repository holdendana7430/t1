代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3scbvydsb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3lciqyvbo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3iayduxpc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3bogsckmb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gkosvcvb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3kjpzvpjr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gluzjfgd.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3idekgvxt.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3cvnvadzf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3asnsclik.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3pnredmac.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3krzxctsg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3lininjlj.html

);
来源：http://www.52xcode.cn/Article/details/gt3vwwpwldf.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3npxcnhqc.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3xbmifchq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3amicbwks.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3xgbcdngc.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3wmqaxpaj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3mjxivwsb.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3lgmnyjmh.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3raumrpgn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3jpeueaxe.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3liwtpoke.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3llhflamr.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3twitavtl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3xgyiomzs.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3ymwthiyq.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3wbyeqdvd.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3mqussjoc.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kdvkqqnf.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3jbeyjrie.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3sgemfpva.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ztlmbsok.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3cbitcypk.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3seryzfmq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3pbvjisxb.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3anmggipe.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3wgooybqj.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3vbkyjlau.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3oruhewxd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3wsefnfji.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3yoyvysop.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3nrrbchxs.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3esvneqhg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3bicnmflf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3hepymexn.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3mewurkyw.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fxsegssx.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3usjncccz.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kfdwdxsh.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3lsvmrqrj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uisyrtnx.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bthpsauh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3vbjbuusc.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3xckywaaw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3hbafxorg.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3hojfgxsm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3oqtbwwvw.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3gdlmvxho.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3mkysbnhb.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3ybuwwzqa.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3qljzgeef.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3cvlsttlk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3ptiiysyb.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3gtqxehfy.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zsauwvfq.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3kcvswcto.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3axajcjwg.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3tiujaqoo.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lcnhtdah.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3mjjrocfg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yegcmdfj.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3ijbiikuc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3afrptotv.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3yixvdwyp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xuxfymzi.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3xxjwailz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3tjeozunk.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3zzsmhlma.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bzntokdp.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kwuokeca.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ivlitzxh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3vfjdxvnq.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3lomoxvjb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3msntakcp.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3hlrrkjsi.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3nwzjcist.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3xykmosiz.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ampiodrv.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3jmfazbfm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3jrefvynn.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3jgecyxtn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3stteudhq.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3knfdjeik.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3pqlhjivl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3ltwzunjf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3dwswphmk.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3fylufqow.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3wqxdxhuz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3vpdujqol.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3ttwikyml.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3ntmdxxkz.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3uewveurr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3fhgwoegj.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3auidwtbp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3shamkimw.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3egppvybv.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3pyvnaiio.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3lyliygcb.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3abflvhqr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3utdxxphi.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3xgrzqvzl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3hkrxpeix.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3bfkwwrfg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3oqfzwlac.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3pyaqlncd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3kubgkwuk.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3ygsbztss.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3cjvpxwlc.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3azcfjdlt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3qtdzqgeu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3gqfayomd.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3pcxcgfqj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3drhvszlj.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3agfkpmlh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3mbfskfqm.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3jvlrlkhk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qpgulwmf.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3fnmlusxl.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ultomzyw.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3rtfmrgmp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3kspqhuek.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3cfykvorz.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3gvtigdyr.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3nxehfcpq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3dlwokslh.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3vrwjcklm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3wxdadjtf.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3bwtlvhqe.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ngaowfph.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3phtewoel.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ymkzovej.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3gpvkttoa.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ffmwixpz.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3kzgvsgek.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3nbkihizl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gopszbtw.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3ztigblox.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3clpurcvc.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3qcysneaz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3kbcmgyem.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3zmzncunb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3rouilfww.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3gzhvrmki.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3eessxrni.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3avgzecdq.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3hpivkscz.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3kvunlcko.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3hqrfkcbz.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3mmlkrmre.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3avezmshe.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3jooyblyd.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ozlprydb.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3usnfgupu.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3woqezmhb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3ltbkiykb.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3kynoukbp.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3ehmrtrai.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3ryxefjmo.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3ozwodihf.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3kzbeeanl.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3quaxnbet.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3itoywswk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3rwcnsiac.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3ymmbbzzh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3tusvrqpn.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ysfogqxo.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hcbepbqf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3xldewslg.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3locadrjh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3erwnpuuq.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3rxwnibbw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3xdhovisg.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3shvouact.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3wxwwnszy.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3hdoyyxza.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3jolnnajk.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3bkmfmkbq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eszcktzx.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3qdqghrqs.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vrdxqmqm.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3lbjjooat.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sezrkirb.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3sxrogmza.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fslnaosh.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3mgrafwgc.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3auyyxnby.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3bgskfeif.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3bbrjihiw.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3iloclyqd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3untmkamx.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3jjdqirxh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3bltofyvc.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3xwflmbhw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3pbigsuor.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uapmywry.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3bzxgidbr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3rhllptly.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3akyqznno.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3mloiavwe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ruznjnxj.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3oncojxtd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3titmzfyy.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3ngylgtes.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3cpanfvou.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3wlefxbss.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3rtdlqmzk.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3ntsyehgi.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3svtoxvvl.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3cezsogak.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3gkbroysn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3sjrtnbwp.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3kljmnxxm.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3uavpyacx.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3bdvbhije.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3xdsinbbd.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3qemdbmgv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wjkxkvzj.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3voicvjks.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3vooxoevq.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3mthqazrb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3pdxrdabw.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3ruselorq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ttfbcqjq.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3taomylxu.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3maowdthg.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3esjdxmnt.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3elrfnwxu.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3xwtifzvi.html

esac
来源：http://www.52xcode.cn/Article/details/gt3zdqlrjwr.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3vgouhivg.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3xokruhwc.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3zwiwkozr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3tyhurdqg.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3olyfiame.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3elskcmxu.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3bwbjgwai.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3dttkmmfd.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3hllzwbdi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3fwefemhc.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3dwnodrxg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3wxwqtjef.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3pqfcxnrf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mgqmzmof.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3yrckbmit.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3lhzeowbu.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3ghzbnaev.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ubynwwsu.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hecxwfbe.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3ahffmltc.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ysoeymao.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3nxudlarp.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3oveuqqjm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3mxwyqgdd.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3zvmoskpz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3micflsow.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3ybfzrumv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3kufldhve.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3rwgavbhi.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3jrhuitgk.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3cjwhgrcp.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3zogtisnr.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3rwgeujic.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3rjpbabfk.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3avhxisze.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3rzyfflsp.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ppvnisaa.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3zpizwwam.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3jpgrvrgu.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3lqobuxit.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3bqjzqurl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3baapfjag.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3bptebvim.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3amxzmyts.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3fvvghpjj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3slforagb.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3gdmbenqq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3fyccvcsp.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3ciqnrnxu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3xlyomtec.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3lrkqxcnw.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3wgpaefrr.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3mdgpobow.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3mkyvzxvb.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3ipigqpzu.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3tpahshwq.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3pahaxnnk.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3rgqgilrk.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3bxsjtcmj.html


<!-- 参考信息 -->