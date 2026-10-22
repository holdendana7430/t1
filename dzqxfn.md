代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2qvepqvpi.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2gkxivclx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2idszvqpe.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2xavxsmsv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2txqkfuds.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2nanxtlqt.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2qkerscng.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2nhtjagoi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2mmvrxcfv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2refctjam.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2darlltxk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2wnylwnzr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eacucjqz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2rkaxcjqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ucsoylhq.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2geuzczlt.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2fuakmscf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2nvqcbevu.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ztaqajkt.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2iokqvrkv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2njavhsne.html

);
来源：http://www.52xcode.cn/Article/details/gt2qamjwxwz.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2sccjswpg.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2llfvnlnv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2qrdppjtb.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2bakqvqov.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2epljaljz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2kucfcegy.html

);
来源：http://www.52xcode.cn/Article/details/gt2hmpyjvyn.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2khjeinwi.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2bsyyprrj.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2usmfsmws.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2dfgrgnxk.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2quggxwna.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2ndmfwqoy.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2jmyjwfjn.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2ijurxykj.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2rjginqug.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2lmqgtkyi.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2ckgjukbj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2aimjyexc.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2xiwbwlnl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2creynocl.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2qzgathxo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2yzdfcdnm.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2arwxvady.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vrgcakxq.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2cmypyebq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2bvyitaoj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2nangdrzq.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2cdmlhqyf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vouozudm.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2lvsfkywh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2fjstzqzc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2gboinepj.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2kgmnrnue.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lwlmhvle.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2nxnqacmj.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2woapezci.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2tfgetlyk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nwyrprlj.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qgzayhcu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2jwkzwyis.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2srzvieqd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2ewpniraa.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2kxzqvidb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cawczqjx.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2rnhzfbhy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ndktiexv.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2opxajpvd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2nmfelkwi.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2jbzmfuxr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ifnfjkyg.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2poakkawi.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hfczueqj.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2kubpgfcz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2muvixqbx.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2jfaseocv.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pjjhiylc.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2expjpatk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wpblgopj.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2ytyptozu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zrxbpjfo.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2vmreoakg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uwyiuvht.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2yjozekxl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nhsuyjfa.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2yovewlsx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2wqrlywpb.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2nnfmyjlj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2pkcrypvc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2piygoywv.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2hcyluivs.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2mvypeoiw.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2vdpzatyp.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2vhjhrrnn.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2aqzmfrij.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2lqiweejr.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2hovotqsh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2mixtefjs.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2bcqyfxyf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2crlhahxe.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2rthlddsv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2srbdpoic.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2npesyuzv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2vfpusevs.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2tpjyemxk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2hggemygh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2jfuaksdy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2xdzffflw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2blyuakup.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2lkrekwwz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2kaurrcgu.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2gilrraoc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2asxcfpxa.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jyllfuhd.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2ygqfcdmc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2vpezybfp.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2hxnbnfii.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2iwuutumm.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2mzvgvmvc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2udfklcsn.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2yftqvsfu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2awxkvsly.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2koyzhjzg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ahzqmpjw.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2ehqbjflm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2yluioksa.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ricmenco.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2sfylbxte.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2scmuuxrl.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2kfliqfli.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vkvnbuss.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2aggidzaz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2awrndpcs.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2qkamjzbt.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2zgbtbphv.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2gohuxkej.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2fwuvnzuk.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2zrpjpcjf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2noreiczz.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2lkpmpftl.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2pakmblhw.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2fyksfert.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2awgqgdbg.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2uktpdpnd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ftaptirn.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2tyumvqaf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tjpdokqy.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2qlibyrbr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qjwhmyoo.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2qvmnugcn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2sceuiiad.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2bgipnzfo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2kpbpzitq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nhwrbmoj.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2ivuvfrrw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ejkcnird.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2cwrpznqr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ucvamlle.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2wyocsblk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2ddcfryob.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2bjrobjag.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2ghsakckj.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2beboeybu.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2fpmwebkn.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2tbvyqqep.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2bveazpvh.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2bxrnzbrz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2iiuxilla.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2pwytghrv.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2ntbirffn.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2pqeyqrxp.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2lpfcwfjl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2wsypepyf.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2vbbyyqyt.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2zmshwtqi.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2yglvafyx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2hhztblil.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2amaushms.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2izjplign.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2nonqysoq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2cvktakyd.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2lsbssjec.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2pgwnseyz.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2iqvcdrln.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ujwatzla.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2csqcatxk.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2nycbvjbk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2bvrcdefl.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2ehuaayku.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2hdvknuja.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2enbwftbp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2cyqrhzyy.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2kqueybxm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2hjtzxrrn.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2lpqhunph.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yyhantbs.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ulakbfqp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ygzzacna.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2dcdsfojp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ftvsxwlg.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rdreuics.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pnlwvkrr.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2nbniamrk.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wsdfgips.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2qknnhyse.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2ripctsoa.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2eluiswjg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2kplkrvpz.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2yjelufju.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2tdrdhklq.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2qqkqurtt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2dbvkjidh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gydfmpjf.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2onpxxcpm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2qpsueskn.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2rqgzuypk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2tjlmgcid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ldcwrqmb.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2dkifssye.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eggxxczh.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2cntpczfn.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2jqlfczhy.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2uqpjgruw.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2xynqclyb.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2qcnuimvd.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2wnqcsfwz.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2isudidsg.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2sahmicqi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2wllnsxtu.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2hrjncizp.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2vuvzrfhp.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2mnutphqv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2yidxvytm.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2dhojeziv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2ytckgkib.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2vtelhwxn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2aostjije.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2prlfepkh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zqnhmyci.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2ywoiaqnx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2huxisrtz.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2vrourbmr.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ofzyzhst.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2nanqjgsf.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2nxkzpari.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2irvwmqav.html

esac
来源：http://www.52xcode.cn/Article/details/gt2uimzchli.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2sztqdtiy.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2tcyoezpu.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2yvibqagb.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qrsqdcui.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ikdnxemp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2pdfaojoa.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lmlphuxh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2xuhrbmpw.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2nenfvmba.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2wzchxfaj.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ercdjcuu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2kyoqoews.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2lhrgqofx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2hruqtzng.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2wkbuitun.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2axxtwghy.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2jkpmwzac.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2vtcbckwc.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2dmvxubld.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2juamusut.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2bsdovaqf.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2vqadcpjf.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2afhelvdx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2twfwtedl.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2aauabijz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2ypvqnmat.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2jwwauzuj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2eqcbwbpz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2szxcuitw.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ormmakzc.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2tbohpkyb.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2nhdidhbh.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2suhlduyz.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2wezwgpca.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2vmxqbhap.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2kfprpnun.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2aytwbaur.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2vezdzgpz.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2nbepujkk.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2jegyhsym.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2utoatgid.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2qksusvpz.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2yeqnefta.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2iptjtukq.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2raqbpnwh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2xkcvuzgx.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2gulvbdsr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2spasznfg.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2qpxeypzm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2ndduxxuz.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2giataysb.html


<!-- 参考信息 -->