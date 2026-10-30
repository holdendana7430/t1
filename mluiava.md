代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fanxiaobao.xyz/Article/details/goisxghus.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gipedaljt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glueihelu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fanxiaobao.xyz/Article/details/goekcinqe.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fanxiaobao.xyz/Article/details/gmzzmockw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fanxiaobao.xyz/Article/details/ggoqgeigv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fanxiaobao.xyz/Article/details/gynnnmbpa.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghhkbddq.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gkpkppxbw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fanxiaobao.xyz/Article/details/gpppbdrni.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gmtdhmxjl.sHtML

[Q01] 创建表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwyzgzcp.sHtML

CREATE TABLE users (
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqgwppmn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbykxqsa.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fanxiaobao.xyz/Article/details/gbftwrzvt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnqpymzb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtonlnzc.sHtML

);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gganpzecm.sHtML

[Q02] 创建带外键的表
来源：http://3g.fanxiaobao.xyz/Article/details/gyplkzbag.sHtML

CREATE TABLE orders (
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqmkptou.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fanxiaobao.xyz/Article/details/gjftlnwfb.sHtML

user_id INT NOT NULL,
来源：http://blog.fanxiaobao.xyz/Article/details/gsvnfshda.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqiljuww.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fanxiaobao.xyz/Article/details/gziddvemy.sHtML

);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbxcmwyt.sHtML

[Q03] 增加列
来源：http://baike.fanxiaobao.xyz/Article/details/gkxcpdmua.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glspyihqh.sHtML

[Q04] 修改列类型
来源：http://baike.fanxiaobao.xyz/Article/details/gjgulhlvh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fanxiaobao.xyz/Article/details/gcdncjvfq.sHtML

[Q05] 重命名列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvystchvt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcckxhnze.sHtML

[Q06] 删除列
来源：http://wap.fanxiaobao.xyz/Article/details/gcbsmfhxo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fanxiaobao.xyz/Article/details/gwdaggphi.sHtML

[Q07] 删除表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpdsabyw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbjlxxxh.sHtML

[Q08] 创建普通索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgysdbwe.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjtvdvrl.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlgnmiod.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fanxiaobao.xyz/Article/details/gilqolgxl.sHtML

[Q10] 插入单行
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbqmpjrp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/givtvltnb.sHtML

[Q11] 一次插入多行
来源：http://3g.fanxiaobao.xyz/Article/details/gacanoyzw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gndnlmkjk.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmusctyd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fanxiaobao.xyz/Article/details/grolxiyjo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fanxiaobao.xyz/Article/details/grolxgqij.sHtML

[Q13] 忽略重复插入
来源：http://3g.fanxiaobao.xyz/Article/details/ghdbulhzw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/ggounaoob.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqyadxbj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fanxiaobao.xyz/Article/details/ghitiepmd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fanxiaobao.xyz/Article/details/gcejzhkev.sHtML

[Q15] 查询全部
来源：http://mobile.fanxiaobao.xyz/Article/details/gynmjgmgz.sHtML

SELECT * FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpwczyce.sHtML

[Q16] 查询指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gmvkydlrc.sHtML

SELECT id, name FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjpjeqti.sHtML

[Q17] 条件查询
来源：http://baike.fanxiaobao.xyz/Article/details/giwtaxnui.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhptuxft.sHtML

[Q18] 模糊匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gwysrpwso.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fanxiaobao.xyz/Article/details/gjifkkvqb.sHtML

[Q19] 范围查询
来源：http://wap.fanxiaobao.xyz/Article/details/glunctupu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fanxiaobao.xyz/Article/details/gatmlltyk.sHtML

[Q20] IN 列表
来源：http://blog.fanxiaobao.xyz/Article/details/ghedobsdw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/guwofmssm.sHtML

[Q21] 空值判断
来源：http://wap.fanxiaobao.xyz/Article/details/gbpfywhbz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/gedanvzll.sHtML

[Q22] 排序
来源：http://www.share.fanxiaobao.xyz/Article/details/guzztwolu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fanxiaobao.xyz/Article/details/glxhmqeie.sHtML

[Q23] 分页
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqwpxsge.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fanxiaobao.xyz/Article/details/geiykqiyw.sHtML

[Q24] 去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyuqqtsq.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdwtvbej.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwylluvk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fanxiaobao.xyz/Article/details/garkjnsmr.sHtML

[Q26] 计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqwuhkwe.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/glmivyjzt.sHtML

[Q27] 条件计数
来源：http://3g.fanxiaobao.xyz/Article/details/ghylagkjw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/grmpohoja.sHtML

[Q28] 求和与平均
来源：http://blog.fanxiaobao.xyz/Article/details/gyvrmpotr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/guzqlmfyq.sHtML

[Q29] 最大最小值
来源：http://wap.fanxiaobao.xyz/Article/details/gvembrmhx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gqvymzqtl.sHtML

[Q30] 分组统计
来源：http://3g.fanxiaobao.xyz/Article/details/gzisajhze.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/guptlmxom.sHtML

[Q31] 分组后过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gufiqewac.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbrqqkaj.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamwkkdht.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzljnvdgi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fanxiaobao.xyz/Article/details/gvvfmghla.sHtML

[Q33] 多列分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgyndhpl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvxlvgaj.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxwhsulp.sHtML

SELECT * FROM (
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwzzouiy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fanxiaobao.xyz/Article/details/gjbdiznry.sHtML

) t WHERE rn = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gwzoiljct.sHtML

[Q35] 内连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gungoykxv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnjufdcr.sHtML

[Q36] 左连接
来源：http://baike.fanxiaobao.xyz/Article/details/gnjrhrgct.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gpeqgxxlc.sHtML

[Q37] 右连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdlxebly.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gergcmkcz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fanxiaobao.xyz/Article/details/glubtosqs.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gvpcbngia.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlsoysqo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fanxiaobao.xyz/Article/details/gtwnidjvy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gxvunvalm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fanxiaobao.xyz/Article/details/geravoypv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fanxiaobao.xyz/Article/details/gbswlxxwg.sHtML

[Q41] 多表连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gepvkjqhy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fanxiaobao.xyz/Article/details/gykxpvxbc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fanxiaobao.xyz/Article/details/gxumiicny.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzrswpwm.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fanxiaobao.xyz/Article/details/ghexxblqs.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fanxiaobao.xyz/Article/details/gvtgnpsbb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gumwkwcxf.sHtML

[Q43] 标量子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gmqnrvaeu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhcxnkjn.sHtML

[Q44] IN 子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gasacllkl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfpkdxvk.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fanxiaobao.xyz/Article/details/grvsgisgi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/govhevnye.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fanxiaobao.xyz/Article/details/ggkfvutaj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkayxulxv.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxlkvpnf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fanxiaobao.xyz/Article/details/gydpnytxw.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gydyqrmuu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwloclcr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpjuixgu.sHtML

[Q49] 更新单行
来源：http://blog.fanxiaobao.xyz/Article/details/gzfmyhecg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gunkerbmb.sHtML

[Q50] 批量更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/goizzszqx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqnzvazg.sHtML

[Q51] 用子查询更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gtuwaqjky.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcliwpkvq.sHtML

[Q52] 删除指定行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gildyeain.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gozdrczxh.sHtML

[Q53] 按条件删除
来源：http://wap.fanxiaobao.xyz/Article/details/guehkxldn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyktzjdd.sHtML

[Q54] 清空表
来源：http://3g.fanxiaobao.xyz/Article/details/gflfxsqny.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfndkjhx.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/grtvlrumu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gyeunogrx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gdouaapoa.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gcippggvm.sHtML

[Q57] 行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggejhlefy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzavypyeb.sHtML

[Q58] 累计求和
来源：http://wap.fanxiaobao.xyz/Article/details/gjjxeltct.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/glntysomx.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscoujvuk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/ghjrxudhn.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fanxiaobao.xyz/Article/details/gmpvollno.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfresvgl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gfjdqncku.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/glxqhwtqb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gxhtapubk.sHtML

[Q62] 分组占比
来源：http://3g.fanxiaobao.xyz/Article/details/gapgitlui.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gonzivwdg.sHtML

[Q63] 开启事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxecwgtk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fanxiaobao.xyz/Article/details/geopzoljs.sHtML

[Q64] 提交事务
来源：http://blog.fanxiaobao.xyz/Article/details/gjoawmvah.sHtML

COMMIT;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmhkfsjz.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgcgapld.sHtML

ROLLBACK;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwkqzbpx.sHtML

[Q66] 行锁查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlczycvf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gloakamoq.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/gkqcpgbwt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnumuzdwd.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnkfkzkg.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwayfsvu.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtplruiox.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/gmltdiodf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxizegyv.sHtML

[Q70] 更新统计信息
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlentheq.sHtML

ANALYZE TABLE users;
来源：http://mobile.fanxiaobao.xyz/Article/details/guokiltib.sHtML

[Q71] 查看建表语句
来源：http://baike.fanxiaobao.xyz/Article/details/gsykjkkkv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fanxiaobao.xyz/Article/details/geptlfkvb.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/govmewivn.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnrzbgjt.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/gpchfzilw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geomlfdpf.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/geptxydri.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/grlhabifd.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gheanhwrc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gnfkbxxzk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbemdyfyj.sHtML

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlkhlnkf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxsahola.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypntlsau.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fanxiaobao.xyz/Article/details/gstcehgix.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gtcixglab.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/gcrizwmqy.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gamanqhru.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/govshripn.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnmnzszu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsruzavak.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gwqgjhhdp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/ggpdakblm.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fanxiaobao.xyz/Article/details/gczthawpu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gjvmsoakf.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gmjdbshfk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbrvntxh.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprawucip.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvsfczrl.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gbmziswdb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gghakqkwc.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhiirwev.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpttyhbp.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gzyrqyggg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/grnkxanwx.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/guoainlga.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgatgdmk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcxjgaoe.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/ghyuumjyi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginqminhz.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprxudgtt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/glkhslywc.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ganetrmqy.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgcgguey.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gsjidkhhd.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvsbpilu.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gwaozkzfy.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbdooceq.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxtwrdcj.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gthoqxjxe.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbjbkzbc.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gwszdlmwr.sHtML

[R04] 位置参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujgcqooj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfaryfuj.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/givwhdtfy.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gsaodrvtc.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbtmrtpk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkmnkpey.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqwqorlk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gfppiptch.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gkvvbqfru.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gqcdrbkxh.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gyrmtbiqv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcnijqje.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzuztyjw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gjjtfrkqp.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gerctxyay.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdqgbkyj.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gpvtlnmfz.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxagwixz.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfolighe.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gpduwwqnt.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/guzljbrwy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gtljcsvkl.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxqpwvhh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ggscbfync.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gnrhgfxoz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzqwwiiq.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/giyjybsoj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gepkrtudz.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcpvpuly.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gdxldfaws.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gmobkzwuj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/goobmshrv.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gsxwhoksl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gsosbqezb.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkajaqcw.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gappihhpb.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/ggyoaocbb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/glmvkxlcm.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gajalphbe.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gxdnebmfx.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/goouyhhat.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgvhmayk.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gzdsumujf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbyknvwl.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gloxosbpb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gujftcbms.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gbdwpdpwy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbybyqws.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/gpxrjcwml.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmwbggug.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gsjototcl.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/glwtndyxv.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbfaelrj.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/glqviylta.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gpooeyfbb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gckawnrid.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbjyhgsk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gateimkbo.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/grlcajsgh.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghofhhthm.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gswfynkgc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/golombxng.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gibxbhzmd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvacpnqq.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwjcnclu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gcflddtqf.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxlmmnbe.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gbtcivhua.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkxmxtwl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrrlmdsd.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjshsfiq.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/goxisbdsl.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdlqmmdu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gykysnsyq.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gapabdkkf.sHtML


<!-- 参考信息 -->