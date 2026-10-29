代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.zdbjq.cn/Article/details/gcgxyusvg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/gbbyercej.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/gxlnqfmaq.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/gbbzqlcze.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.zdbjq.cn/Article/details/gxdyumdiq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/gqsazmbts.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/gfhcplnpy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gedewkstn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.zdbjq.cn/Article/details/gzcadroye.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.hesvh.cn/Article/details/gmznisbfo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.zdbjq.cn/Article/details/gvrewrplc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fehbvm.com/Article/details/gbbkuadms.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnqafacmc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/gnnjqzplv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxdasqiwn.sHtML

[Q01] 创建表
来源：http://baike.hesvh.cn/Article/details/gdjlrnshr.sHtML

CREATE TABLE users (
来源：http://www.blog.fehbvm.com/Article/details/gvzcsdxvq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gxqdohfuz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gneiccjcf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.hesvh.cn/Article/details/gougdgyhp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/gnnfjfkgr.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gzxcuihpr.sHtML

[Q02] 创建带外键的表
来源：http://m.share.zdbjq.cn/Article/details/gpsqgnjrt.sHtML

CREATE TABLE orders (
来源：http://baike.fehbvm.com/Article/details/ggvsweqkd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gfotpfday.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gjdkokhoj.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/gevtycpct.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/gtjdebjqx.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/giesllzuu.sHtML

[Q03] 增加列
来源：http://mobile.hesvh.cn/Article/details/gxskivkce.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/gqqcczrto.sHtML

[Q04] 修改列类型
来源：http://read.share.fehbvm.com/Article/details/gcqtihzlo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.hesvh.cn/Article/details/gslrqjqvf.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/gykipuile.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.hesvh.cn/Article/details/gdcwfxhkq.sHtML

[Q06] 删除列
来源：http://baike.zdbjq.cn/Article/details/ggohhpyvd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/gqhlnkwmt.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/gzwirzzqi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/gckwvylqn.sHtML

[Q08] 创建普通索引
来源：http://3g.zdbjq.cn/Article/details/gdaobsjah.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/guigqnltp.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/guvmcymwq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gpimghhxh.sHtML

[Q10] 插入单行
来源：http://wap.zdbjq.cn/Article/details/gdofugtjm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/gmxdgahuo.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/gprncteke.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.hesvh.cn/Article/details/gttqwawmo.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/goyzpqaxi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.hesvh.cn/Article/details/gozflbxkv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gcpvjklnr.sHtML

[Q13] 忽略重复插入
来源：http://wap.zdbjq.cn/Article/details/ggazokrhj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/gmuarmnnn.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.zdbjq.cn/Article/details/gsygazewq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/gviygphvt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/gldvoejve.sHtML

[Q15] 查询全部
来源：http://wap.fehbvm.com/Article/details/guyqkvuno.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gtuakriqw.sHtML

[Q16] 查询指定列
来源：http://www.m.share.hesvh.cn/Article/details/gutjdpctj.sHtML

SELECT id, name FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gquauucul.sHtML

[Q17] 条件查询
来源：http://m.share.zdbjq.cn/Article/details/gdsgkbcic.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.hesvh.cn/Article/details/gwfyjcyzz.sHtML

[Q18] 模糊匹配
来源：http://wap.hesvh.cn/Article/details/gpwxbdbey.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.zdbjq.cn/Article/details/gqmrhvmtj.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/gldqelrjj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.zdbjq.cn/Article/details/gicttwuwb.sHtML

[Q20] IN 列表
来源：http://read.share.hesvh.cn/Article/details/gcprwihip.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/gxeixuflg.sHtML

[Q21] 空值判断
来源：http://baike.fehbvm.com/Article/details/ggqtupcmq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.zdbjq.cn/Article/details/ghdivexis.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/gkedhhmdy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/gbvhtgtmk.sHtML

[Q23] 分页
来源：http://www.share.fehbvm.com/Article/details/gmrdnxqgh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/gysiruaoc.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/gzggwmlkv.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/gxyyyxslr.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/gihrqnlzh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/gnaptvqmb.sHtML

[Q26] 计数
来源：http://read.share.zdbjq.cn/Article/details/guhkoclqp.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gyjekyzvi.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/gqyujkyzw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gnisdgrpa.sHtML

[Q28] 求和与平均
来源：http://baike.zdbjq.cn/Article/details/ggwquctdj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gyfaozrbv.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/gwvjnwdye.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/gtfduvzsg.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/gezvcwgqb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gwldkktrh.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/gwvdeacjc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fehbvm.com/Article/details/gnqzixuoz.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fehbvm.com/Article/details/gmfrkwnga.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gmjvqdzlx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.zdbjq.cn/Article/details/gtkygdbvp.sHtML

[Q33] 多列分组
来源：http://www.m.share.fehbvm.com/Article/details/gfadcuvew.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/glmblksuk.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/giclciotj.sHtML

SELECT * FROM (
来源：http://www.blog.zdbjq.cn/Article/details/gzombjppu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/gjulktogk.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/gfireggmq.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/gdtwqmgtb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gglpjzbeq.sHtML

[Q36] 左连接
来源：http://m.share.fehbvm.com/Article/details/gkopctdzf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gmtzaujkp.sHtML

[Q37] 右连接
来源：http://wap.zdbjq.cn/Article/details/gtpwhzpxz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/gncposrfk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fehbvm.com/Article/details/gkjdbwzbc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/gdibskmsh.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gnijxsbla.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/gbplyqobo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gqrrrzasd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/gjxgmdhkn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.hesvh.cn/Article/details/ghebxkrbc.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/gnuwepbyb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/gbjurtxhf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/gyonnukbz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/gtodnzquh.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/gltxusskc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gosnsxpep.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/gtefkuwqt.sHtML

[Q43] 标量子查询
来源：http://3g.hesvh.cn/Article/details/giknlkvll.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fehbvm.com/Article/details/gsqkhdlpt.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/gaubhsyqc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.hesvh.cn/Article/details/gfrxkproe.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.zdbjq.cn/Article/details/gnxuvynjv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/grmpuahgr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.zdbjq.cn/Article/details/gepuhwkbo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gzvieserg.sHtML

[Q47] 与平均值比较
来源：http://www.share.fehbvm.com/Article/details/gdovlyaiy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fehbvm.com/Article/details/gcfuuvibq.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gnvngprjz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fehbvm.com/Article/details/genntbzwp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.hesvh.cn/Article/details/glyfhaefd.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/gqorebcnw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gtsxegdqv.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gulbdtvbe.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/gwxhxlbcm.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/gbxqytzdx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.hesvh.cn/Article/details/gdljhyoty.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/gghvdohho.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gsgbihmfi.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fehbvm.com/Article/details/gbmgdopyn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fehbvm.com/Article/details/gvpnerlgq.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/gumdssvat.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/gdmksnehj.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/gmjoqwwzt.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gzsawloxs.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.hesvh.cn/Article/details/gcqdjmjut.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gkvressgn.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/gxbgikuqz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ghkzjfiej.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/grtdieqmk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gbmdlksbe.sHtML

[Q59] 分组内累计
来源：http://mobile.hesvh.cn/Article/details/gaisvjuyg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gmqspjuwe.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/glqbostku.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.zdbjq.cn/Article/details/gghbonblo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/grizwfxld.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/gtedcdkdd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gtjegfpmx.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/gicawyelj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gpkuwsvju.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/gsodxiahj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gtcibempp.sHtML

[Q64] 提交事务
来源：http://www.share.fehbvm.com/Article/details/goauuhelz.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/gtwcjeorc.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gfqqkrqbn.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/giplekpki.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/gyvrmxfnv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/gftirmxvp.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gwvddaaqh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/ggaypmrjn.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/gwvyhbnvc.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/geepaleic.sHtML

ROLLBACK TO sp1;
来源：http://blog.zdbjq.cn/Article/details/gultqstyz.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fehbvm.com/Article/details/gdrikbkfy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/gljnpgoqg.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/gwmwnmbbh.sHtML

ANALYZE TABLE users;
来源：http://m.share.hesvh.cn/Article/details/gxbmohsxn.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/gbwyjwrib.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/gecovsecx.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gdnjrxiwy.sHtML

SHOW INDEX FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gpbqclfks.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gryzndecp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/gbfknovyl.sHtML

[Q74] 强制使用索引
来源：http://wap.fehbvm.com/Article/details/gasisjann.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/gmuskrbuv.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gjpwyokoc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gtwkglmvm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.hesvh.cn/Article/details/gnhivqwts.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/gvijslffu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/glwmjzcqm.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/gmaygjgxb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/gisfxttam.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gtkxnwvrp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fehbvm.com/Article/details/gonimsbjq.sHtML

[Q79] 字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/guxigplwg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/ghumolcso.sHtML

[Q80] 字符串截取
来源：http://www.blog.hesvh.cn/Article/details/gkfyvazrj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gapqdqaur.sHtML

[Q81] 字符串替换
来源：http://baike.fehbvm.com/Article/details/ggibdbrvh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/gjhokldbr.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/gemhnobbm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/ghfzifvva.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/glncfukzk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gvojcuohb.sHtML

[Q84] 去除首尾空格
来源：http://m.share.zdbjq.cn/Article/details/gnnndjmmd.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/grteroyrh.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/gmvxqanpo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/gfmarotjb.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/gnxlezizr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/gbawlkvfj.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/gusgsugmz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/ggkkknzvf.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.zdbjq.cn/Article/details/gginsqdlg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/gkvudlqvn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/gawqlkwee.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/gbkizuigb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.zdbjq.cn/Article/details/gnmuutrae.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/gwmdmpxvm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/gshcljphf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/guutxqxsn.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/gughjfuca.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwwnwwpmf.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/gkoiwczlh.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/gtixobayh.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/grncohmng.sHtML

[R02] 变量赋值与使用
来源：http://wap.fehbvm.com/Article/details/gpnohptfv.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/gvjglzqjk.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/gslynjgjn.sHtML

readonly PI=3.14
来源：http://www.m.share.zdbjq.cn/Article/details/gzzdasaqd.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gwvrhtmjz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/gwnptmpax.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gzehyrrhu.sHtML

name="${1:-default}"
来源：http://blog.hesvh.cn/Article/details/gsequsurs.sHtML

[R06] 判断命令是否存在
来源：http://mobile.zdbjq.cn/Article/details/gdeezxijr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gunrrkgpd.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/gqdlzkjip.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/grgskyvof.sHtML

[R08] 数值比较
来源：http://www.blog.fehbvm.com/Article/details/gwgifqljj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/genicgosf.sHtML

[R09] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gxskxbaam.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gbglhtrlz.sHtML

[R10] 正则匹配
来源：http://blog.fehbvm.com/Article/details/gqwtqglhy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/gtrpptwfu.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gtufmtbmh.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/gjloghvkg.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/geslnhfxo.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/gtoimnnwo.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gphwfiivw.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/gpchcmamv.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/ggbafdpkr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/glyeydrzg.sHtML

[R13] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gslfkowqv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gdahueiix.sHtML

[R14] C 风格 for
来源：http://blog.fehbvm.com/Article/details/gcqxyqkvr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gqggopltr.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/gszsrxcax.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/gpyfktaqs.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/ggfyfedhf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/goxwylsjr.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/gsopzqbon.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.hesvh.cn/Article/details/ghkdwjjyj.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/gxcdrxkqk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/ggwoclehr.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gpggranyc.sHtML

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/gmknmynun.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/gphgjpdgr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/gmgetxwdq.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gzfolrkhz.sHtML

echo "${#s}"
来源：http://www.blog.zdbjq.cn/Article/details/giumicptx.sHtML

[R22] 截取子串
来源：http://baike.fehbvm.com/Article/details/gybspdfnq.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/gblefdfjf.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gksvowhcu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/glspcxuwx.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gtzcbodrl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/gsnthgnxm.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.zdbjq.cn/Article/details/gmahnkynm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/gzlqfdavw.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/gdzldeorq.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.zdbjq.cn/Article/details/gibhngyvr.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/gryftealg.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gnwkvcbwd.sHtML

[R28] 浮点运算
来源：http://www.m.share.fehbvm.com/Article/details/gxzflzcrk.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/gjtkvmlzp.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gurtchrjl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/gozqpgydm.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gcowinbbp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/gadsbldyk.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/gaiioyicv.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/gtzoseldp.sHtML

[R32] 参数个数校验
来源：http://read.share.fehbvm.com/Article/details/gnkasyazu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gkozsuvyi.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/gxzutxqfs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/genccpczs.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gdwrvyjvw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gxmeaadml.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/gxkrjvaxe.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/gkrzmioom.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/gvjmvdems.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fehbvm.com/Article/details/gsedxjtjj.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/gzlabzpvj.sHtML


<!-- 参考信息 -->