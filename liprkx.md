代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3qwqeprky.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3gjndolah.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3rhovcwoi.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3tpaukpnl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3nvasfonk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3npvxgdwh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3zvauikee.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wzagfyyu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3rgjczmys.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3swarjpoa.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3zfbdocnk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3xwemxmnh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fdehjimp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3vrzgslvh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3egbhucjh.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3wfotacxa.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3kmpejwbo.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3zqmstmat.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3pfefhbjs.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3hqtjrkpn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3brluwkkd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3eaievfqj.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3ddebcagl.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3vllndfcc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3qxtosdir.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3fgcinurb.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3xwuyqoax.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3dmtdsjgu.html

);
来源：http://www.52xcode.cn/Article/details/gt3gqorikhp.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3avpntsyc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3ymnffldt.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3lgygblat.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3rvleuhgf.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3jvnsweup.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3wqlhtmgs.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3nkotnsyc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3pyqqwhxk.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3oootylxc.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kblstvnk.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3owwgbybo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3jrnvbdwq.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3vafznbnu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3vbgajtzu.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3oczokzqh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3pgxydcxr.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3eqsvgeuv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3dkgoxvli.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3ynckvfyj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3qotpvbob.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3cvmbjaoe.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3yortxlqq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3kjkvkdkh.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3epwzodur.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3szisyxzl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3afhncupt.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ujulwgcj.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qbpbgwwd.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3hdjyopzo.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vdumufcv.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3vccfegdc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mntcgkwr.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ynwqhnxu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3tdkekitm.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3xayvdzux.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3ucivpzsx.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3gubetimr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3pdabclzg.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3qkuytkfm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3twpfnolg.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3lxccaiwo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3irjswryv.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3lyakwpcu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3advmdltr.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3rnmvdxck.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yzrwwskm.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3fuyevneg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3fqskcdsu.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3gycmtufp.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3enulktdg.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3akajxfuk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3seiihuif.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3zoyfwkmj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3sqrwqkll.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3avaxhjlc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qpkqfgbj.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3qskhyvny.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3rmfdvumg.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3bsxixurq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3sfbgykfp.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3riowhuvx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3rhmoapln.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3ckkuxkud.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3humcvcin.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3xwbijprl.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3ofnpfmae.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3nbntdmkw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3wtbaftlq.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3utnsgjya.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3eblbkbhl.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3mqbxzbht.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3ubtcxjbp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3tmyocdqp.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3vnrtkwhw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3wbaehiqy.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3auwyfnuu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3sbcmvyuy.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3tpgaauul.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3ipeesmoh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3secewhev.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3carrmsrf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3lcthoeug.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3ciarmfdj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3qevcwhti.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3esqoexfp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ivaxkddr.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hqfenhif.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3jfpdhlzx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3swjenrlh.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3watxjhnj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3jaizqsfp.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3gffdugwc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3lsjowjqz.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3dwviavod.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3cjogzfxl.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3kceqxqvf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3gzsbhtdv.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3swsqteku.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3jryrpvvb.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jnyzghio.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3hwecnlym.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3gtmhpqeh.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3vqubkrfh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wtwsbjeo.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3kqwhhkvb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3jgpvsapi.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3lquebesz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xzdciygl.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3kmxqwwjd.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ybsyiwhu.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3ljvxduxe.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3yqbvkvzn.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3hncsdgjx.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3dawxvjkz.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3gglcfqiq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3rjcpcogg.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ggvrjwnk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3huxujpzb.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3fverrwws.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3npttgdri.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3vlluqbrs.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3oroulkqo.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3yhmnsfio.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nmvxpfif.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3klsftpkk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3ebzufqqt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dxfmmtac.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3drhcwzkn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xzdnlvpy.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3nofxaeur.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3gbhfmacc.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3gntjchiy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3utwjfkvi.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3ptxydspq.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3kubexthw.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3zposbkjo.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3kkzchhbj.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3stckluhk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3tfrgejaz.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3hieznnta.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3zdvbadyn.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3zoemnekb.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3kdwqpgxn.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3rdynqhku.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3uxfmawag.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3tkalvofo.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3ltvcwlnz.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3fiedjqef.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3wusfnios.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3hevpvcdk.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3jwconrjm.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3alkeazxx.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3wmrxygjh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3tbtnyzrc.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3emumvgcn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3sqpfykoq.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kyzkhbgi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nakgnftp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3atngvodw.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3lljbwmxj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3kqkutgia.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3poswvvew.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3khdhznwh.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3fcebhvvq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3wktmrrkf.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3lqbagvfc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3yddtnxww.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3zgfpgcrd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wcgfohlq.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3dligwonp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sdsaevjy.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3vbgsmnzz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dkefziyh.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3mirknexi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ifrkpqwo.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3zmiuryfp.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ikdxawqo.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3qkcqdshx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3wrbmunbi.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3qwdvjoet.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3wcsilxgy.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3cnwlrxkj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3cwzndsiw.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3gdaghepx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3hkfqiisi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jpoieyee.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3fyrzotde.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3sdtunnrj.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3mlkeurqw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3pzbtydwx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fefpykvg.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3djvmzcad.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gjddxgrn.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3ihxordlp.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3crqdhuxi.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3wkxnasxr.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3rbqtaveu.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3myyydnqh.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3oqshssal.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3rzrqsejr.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3nhpxoilw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3chlcirhp.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3wdahhtus.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3zvdrffyn.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ovzugshr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdgnwstw.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3pamcexwy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bareqoel.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3zkgkfipr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3qpormntj.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3fuaxykgh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3srsbgnzs.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zkqxuwso.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3idqbzoku.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3zbkaahfd.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3ebsosrbg.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vmiwaipn.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3tnsotckm.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3inpbpgwi.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3nchplaod.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3jjquwswt.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3appjtzfw.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3kxbqmkjx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3jpocmzhc.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3htlumdrl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3bebusasw.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3uhagjrzp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zomqtvaw.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3knwxxylm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3eqeonnmu.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3lbwmfefv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3kfxpgdvr.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3stumwlcz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3tkboympx.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3lrxfrapn.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3bnbvdjae.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3mttgupdo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3dztllxgm.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3cmsnsugk.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3ccjxtrqo.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3qcbkhfxo.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3eoqhgaay.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3mxqrqnsb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3kobxrcok.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3gfsplnfl.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3yczmjdvh.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3htuqivmc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3nwjlvmur.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3hnfkjhif.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3cnnechkg.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3ipxpddye.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3fnwfshjv.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3txawnjla.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3wrajthpv.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3jmttcfqt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3enqvvxzo.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3unviuoyw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3pprorqdw.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3nuusfmot.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3fadhjizq.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3cochdtqr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjvcmotd.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3egezenqr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3gihoznhq.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3icrcvdmn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3dyalaglx.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3tqjpwbby.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3hwoqopeh.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3hixdurle.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3zivksanf.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3kllxgvxq.html


<!-- 参考信息 -->