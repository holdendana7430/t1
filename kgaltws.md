代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/gvizcqbfa.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/glomglfur.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.hesvh.cn/Article/details/grlhtiwef.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/gfjpwlypv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/gplmmrhjq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gygdbzzqc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gulgrycza.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gtladautj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/gnejgxkmi.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fehbvm.com/Article/details/gforowwia.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/ggeplixrg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fehbvm.com/Article/details/goupbadkz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyeavaxvu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/gksmfygwq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpqwcqiks.sHtML

[Q01] 创建表
来源：http://baike.hesvh.cn/Article/details/guseqlkdc.sHtML

CREATE TABLE users (
来源：http://www.m.share.hesvh.cn/Article/details/gwssnjndf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gyreqgqiu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gddtaiort.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fehbvm.com/Article/details/gtaokzzhp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/gnspafuxt.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/genabtwws.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gaottmfbb.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fehbvm.com/Article/details/gfkghvldr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/glszrzlwa.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gkvidirfk.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fehbvm.com/Article/details/gievviodv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/gatowkwjg.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gbuhsoixp.sHtML

[Q03] 增加列
来源：http://blog.hesvh.cn/Article/details/geunzdmqg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/gtovrfwgd.sHtML

[Q04] 修改列类型
来源：http://m.share.fehbvm.com/Article/details/gclqlanil.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/gpbkauotv.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/ghpxfbeen.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/giiobczkg.sHtML

[Q06] 删除列
来源：http://mobile.fehbvm.com/Article/details/gnlmhoteu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gwoyrfchr.sHtML

[Q07] 删除表
来源：http://baike.fehbvm.com/Article/details/getxswgtr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.zdbjq.cn/Article/details/gdhkljovu.sHtML

[Q08] 创建普通索引
来源：http://wap.fehbvm.com/Article/details/gbwefwowu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gycbwvuvl.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/glrahtpgv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gjjhpblvx.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/gcgwnxhfj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gugixozgq.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fehbvm.com/Article/details/gawsqrckx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/gdrgijuow.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.hesvh.cn/Article/details/gviorwhwh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/gwdtjdbgt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gaolatumo.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/glzdvnrwt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.hesvh.cn/Article/details/gllukgmpi.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/guawzirht.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/gfwzpjgmy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.zdbjq.cn/Article/details/ggetsaivw.sHtML

[Q15] 查询全部
来源：http://m.share.fehbvm.com/Article/details/gqmclvvxu.sHtML

SELECT * FROM users;
来源：http://3g.fehbvm.com/Article/details/gzxgimsvu.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/gylepwoxr.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gwzsmrtye.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/grmrhervf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.hesvh.cn/Article/details/gicgxargk.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/gppshrfnt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.hesvh.cn/Article/details/grreajork.sHtML

[Q19] 范围查询
来源：http://m.share.fehbvm.com/Article/details/gdzyzjddw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fehbvm.com/Article/details/gjimajanx.sHtML

[Q20] IN 列表
来源：http://www.m.share.hesvh.cn/Article/details/gmzjezbkj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.zdbjq.cn/Article/details/gjcinyqmp.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/gcxpycvpw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/glrbucqsy.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/giqkuguha.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/gfcnalixo.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/ggvzmvkqc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gsiuujzkx.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/ghmrnxvnv.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/gxgicbydw.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/gfovyxoig.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fehbvm.com/Article/details/gvqdlrqjz.sHtML

[Q26] 计数
来源：http://3g.zdbjq.cn/Article/details/gfpcrlkvj.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gdhkcxtha.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/gxywdskav.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gtfootjuo.sHtML

[Q28] 求和与平均
来源：http://baike.hesvh.cn/Article/details/gezwldwpb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gxoqbcqvz.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/giouoplgg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gxjhczova.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gmfpkoavu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/glrykqybg.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/gviubkkqf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/glynxxawa.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gaywrpbot.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/geajxcydq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fehbvm.com/Article/details/ghioddfob.sHtML

[Q33] 多列分组
来源：http://www.m.share.hesvh.cn/Article/details/gtbrlaunj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gajewrymn.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/gukwjagbp.sHtML

SELECT * FROM (
来源：http://m.share.hesvh.cn/Article/details/gexeagxhw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.hesvh.cn/Article/details/gemffvpfr.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/ghaqspyuv.sHtML

[Q35] 内连接
来源：http://wap.zdbjq.cn/Article/details/gaqxkxmfp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/guvcitmcs.sHtML

[Q36] 左连接
来源：http://m.share.fehbvm.com/Article/details/ghemkuthy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/guackchzj.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/gzywxoyja.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/gscsxpjzv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fehbvm.com/Article/details/ggcppdqyt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fehbvm.com/Article/details/guyusuzrs.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/ghdhhykqa.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.zdbjq.cn/Article/details/gkusdwwea.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.hesvh.cn/Article/details/gwbtzmwwk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gviezavuw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fehbvm.com/Article/details/gsuckjnxd.sHtML

[Q41] 多表连接
来源：http://baike.fehbvm.com/Article/details/gujiimdvm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/gkymwvcuc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.hesvh.cn/Article/details/gfnvlnflg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fehbvm.com/Article/details/gkoenawob.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/gtymekwpf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.hesvh.cn/Article/details/gxebjbasc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/gqotigulx.sHtML

[Q43] 标量子查询
来源：http://www.blog.fehbvm.com/Article/details/gfuvdhdsl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.hesvh.cn/Article/details/gqlhsqizr.sHtML

[Q44] IN 子查询
来源：http://www.share.fehbvm.com/Article/details/glzadlzrp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/gxeqqbyeg.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/gyopvxnlw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/ggjxdcsvq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.hesvh.cn/Article/details/gqjqjxjna.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/geddbgfaa.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fehbvm.com/Article/details/grsazqepl.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.hesvh.cn/Article/details/gejwlrodr.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.hesvh.cn/Article/details/gfywdxbqa.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gdeyartja.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/gkzqucilc.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/gqgupnzph.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/glvllmlsd.sHtML

[Q50] 批量更新
来源：http://m.share.zdbjq.cn/Article/details/gelslvlif.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gsapcvlff.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/gcmmqnilh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/gwpfpndws.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/garymevxf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/ggqfqyazg.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/graelgesx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/ggxjvvjqo.sHtML

[Q54] 清空表
来源：http://m.share.zdbjq.cn/Article/details/gmavsmkyk.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/gsjuatzle.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fehbvm.com/Article/details/ggcbqglnm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gsbgwsnvy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.hesvh.cn/Article/details/gzomyrzzr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/glebvmsvp.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/gbaodslpk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gouigglfn.sHtML

[Q58] 累计求和
来源：http://m.share.zdbjq.cn/Article/details/ghbgbxpmm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gwmqjfhkl.sHtML

[Q59] 分组内累计
来源：http://baike.zdbjq.cn/Article/details/gedzpnkyh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/ggevsxtdd.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.hesvh.cn/Article/details/gyjbkdpnu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.hesvh.cn/Article/details/gxbtaljui.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gzpihmzuk.sHtML

[Q61] 移动平均
来源：http://blog.fehbvm.com/Article/details/golltjukc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gsdedwbso.sHtML

[Q62] 分组占比
来源：http://blog.zdbjq.cn/Article/details/gzscvtuqt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gktiacxkk.sHtML

[Q63] 开启事务
来源：http://blog.hesvh.cn/Article/details/gmtyuphzz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.zdbjq.cn/Article/details/gdpslmxyc.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/ghqbedjrw.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gmhqasrvk.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gjsuzeilo.sHtML

ROLLBACK;
来源：http://read.share.zdbjq.cn/Article/details/gutafhbmz.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/gsunkbfyk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/gphrhhpbt.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/gxmmfnbzz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gserotaha.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/glbxejbgh.sHtML

SAVEPOINT sp1;
来源：http://3g.fehbvm.com/Article/details/gnhkhnprf.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/gntpvymhz.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fehbvm.com/Article/details/ghodfnfhw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/glqmtgkqp.sHtML

[Q70] 更新统计信息
来源：http://read.share.fehbvm.com/Article/details/gxzqnbeqf.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gelexcinn.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/gdydkjkhp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/gyfwuepoh.sHtML

[Q72] 查看索引
来源：http://mobile.zdbjq.cn/Article/details/gvaudofdf.sHtML

SHOW INDEX FROM users;
来源：http://www.share.zdbjq.cn/Article/details/giqjjrkbe.sHtML

[Q73] 查看表状态
来源：http://read.share.fehbvm.com/Article/details/gmyozmnes.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/gwmjbpedl.sHtML

[Q74] 强制使用索引
来源：http://www.blog.hesvh.cn/Article/details/gogmorgbo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fehbvm.com/Article/details/godvbgngl.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gybvugjwp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gbvzjrzeb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gdnuoqzaa.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/giarjkias.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/gmjjxmmyc.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/gancfkumv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.hesvh.cn/Article/details/gdhhgrgny.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/gxwjbjbyh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/gavvbvlbh.sHtML

[Q79] 字符串拼接
来源：http://wap.hesvh.cn/Article/details/gpdmgntxj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/gnpkcfkuy.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/gswlwslmz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gxmravvcl.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gumjfdqjs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ghyimgxfr.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.zdbjq.cn/Article/details/grrswtjjr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gmdcagsth.sHtML

[Q83] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gbhxsotmd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gmtqbzsnn.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/getznujsn.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gkekmikbd.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/ggnqhcmoa.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gnrgcexwy.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/guxzbwtjo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.hesvh.cn/Article/details/gqlmwawbb.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/ggrhvdgqo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gspdoseyx.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fehbvm.com/Article/details/gkejjizzv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gndwwfrzv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/gaczhpyty.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/gdlwosmyi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/gbnbqmcre.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/guqrlwogl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/geslicvvz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/geidhctco.sHtML

R. Bash 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gdmunwaai.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gstmixkpj.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/gqvrktylf.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gpsnngeqz.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/gzimixocr.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/ggeqqptsn.sHtML

name="Tom"; echo "$name"
来源：http://baike.fehbvm.com/Article/details/gtszfwnob.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/gdekgdxei.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gbxafnkbu.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/gbyaydsiw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/gfsyfiggj.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/gfmwvhaim.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/gzcbgphxd.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/gnpsrtztt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gjwcjgxbl.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/gebowdcuq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.zdbjq.cn/Article/details/gelzmafwp.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/gbzyzaaag.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/gfospewgg.sHtML

[R09] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/ginjjmbsi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gftbqdllc.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/gpijkgyan.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/gyvrecjsg.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gkezwxkpq.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/gcvpvvyqm.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/gxktbkeeb.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/gijnzcytb.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/gbujtwmbc.sHtML

esac
来源：http://wap.zdbjq.cn/Article/details/ghqneffvb.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gkfbdpxqh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gdvvpxloi.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/gfzykiwln.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gdduvypyx.sHtML

[R14] C 风格 for
来源：http://baike.hesvh.cn/Article/details/goeetjbcg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gbplmbyiq.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gplxagnbg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/grpdpbtie.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/gewggnlkq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gkkpwonzo.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/gyllrzvlh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/giyhiezle.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/gnylrvmet.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.hesvh.cn/Article/details/godpujtit.sHtML

[R19] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gcpvlzktw.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/gnvcrzozp.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gnwsnqhoy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/glhbxgxuc.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/gzjfqecnn.sHtML

echo "${#s}"
来源：http://www.m.share.fehbvm.com/Article/details/gpdozhunw.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/gquwnavkx.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/gmqpmljje.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gfdxrqdkb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/gdznnjeol.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gmotqgkix.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/gacgurlid.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/gtsdndioe.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gixyfuxfl.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gwamxyzza.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gonyulems.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/gaqaopzsu.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/gbernkssf.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/gnoyflkhz.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/gtgimlvkj.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gctpzgucx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/gcbnljsob.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gyztfkdzb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gkocqhrhb.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/gyksbvrkl.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gojbmjmih.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/grnrinetp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/grrruyfmv.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fehbvm.com/Article/details/gjpqpwjca.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gvolvfkjd.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gwwkkhdxm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gdjiawwwu.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/grqlyqjaw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/gnjomlywv.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/gutiafava.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/gwxxctipn.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gotxponxz.sHtML


<!-- 参考信息 -->