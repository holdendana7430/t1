代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/gifqbrdvs.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/gwksmncbv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/ghggpvakt.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/guqxrgtsh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/gcudxyfvl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.hesvh.cn/Article/details/golipllqi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.zdbjq.cn/Article/details/grzwgerxq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/gznngsugt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.zdbjq.cn/Article/details/gfdakdpkh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/gmbrngisu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/grmusdgps.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.hesvh.cn/Article/details/ghuzqhmmh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjzntwwsd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/grojrlgsx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gutqdfhqz.sHtML

[Q01] 创建表
来源：http://mobile.hesvh.cn/Article/details/gktxhshxl.sHtML

CREATE TABLE users (
来源：http://blog.zdbjq.cn/Article/details/gejxziiup.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gfgjjqyhx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gayewypul.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.zdbjq.cn/Article/details/gmnjjivto.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/gbvjvxdor.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gnrfrloqg.sHtML

[Q02] 创建带外键的表
来源：http://baike.hesvh.cn/Article/details/gwaqaocne.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/gjwmpsmkm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/grtxpsrqf.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/guxtownme.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fehbvm.com/Article/details/gddmedhut.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/gtteeouwb.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gbjrztiwo.sHtML

[Q03] 增加列
来源：http://3g.fehbvm.com/Article/details/gqafopibw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/gtwgwoypy.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/grzbztlsd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/gvgbeeqsp.sHtML

[Q05] 重命名列
来源：http://m.share.hesvh.cn/Article/details/gthohzqfl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.hesvh.cn/Article/details/giqahhjyj.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/glchjzuoo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/gqvgswmit.sHtML

[Q07] 删除表
来源：http://www.blog.zdbjq.cn/Article/details/gccbujhzq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gzwfpzkjt.sHtML

[Q08] 创建普通索引
来源：http://baike.hesvh.cn/Article/details/gviipodak.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gutruqery.sHtML

[Q09] 创建唯一索引
来源：http://baike.fehbvm.com/Article/details/gugkqekeo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gqgxpixpd.sHtML

[Q10] 插入单行
来源：http://baike.hesvh.cn/Article/details/gtaaoitlc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/guvxjydrq.sHtML

[Q11] 一次插入多行
来源：http://mobile.fehbvm.com/Article/details/gtxrsiykr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gfqwutqlk.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.zdbjq.cn/Article/details/glrbcqmcf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fehbvm.com/Article/details/gamfoypao.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/grzbhseuk.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/grucdeakl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/gmjfvdckw.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gdfzzbrdf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/gaeuxrfsd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.hesvh.cn/Article/details/gfjkwincn.sHtML

[Q15] 查询全部
来源：http://www.share.fehbvm.com/Article/details/gpqzvfctd.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/gktlakyol.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/gmlpbpeih.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/gssokraff.sHtML

[Q17] 条件查询
来源：http://m.share.zdbjq.cn/Article/details/guputulau.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/gwgffgdqo.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/gkhcffcdu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.hesvh.cn/Article/details/gfnolzwob.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/giygbeijq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/gqtbajwei.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/ggxcxgdxq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/gkwoqyuro.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/gqfzkrsyo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/ggjncyshd.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/gooewjejh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/ginirgycz.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/glvyrdrpw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.hesvh.cn/Article/details/ghwbbaiwl.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/gjmhsousz.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gtfbupjvr.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/gahcuyzjv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/gokeleeln.sHtML

[Q26] 计数
来源：http://wap.hesvh.cn/Article/details/gdiemovhu.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.hesvh.cn/Article/details/guxbvqhff.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/gmxbpbioy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gsfnkqliu.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/gfhanuxdq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/ghekubpqs.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/gvwvozdin.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/ggjcjmmai.sHtML

[Q30] 分组统计
来源：http://mobile.hesvh.cn/Article/details/gudcdhyvp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gszojknyb.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/gkfsrtgsd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.hesvh.cn/Article/details/gpptqmktz.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gxkzxtcmw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gpujarcxa.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.zdbjq.cn/Article/details/gyxhdfgcq.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gdfasliab.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/gtnuxwfwv.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/gpfvonhfj.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/guewzpeua.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.zdbjq.cn/Article/details/ghmciwsth.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/gbfesgoos.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gasajfojs.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gxkqcjqmr.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/gxvapmkes.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gzsosvrmx.sHtML

[Q37] 右连接
来源：http://www.share.zdbjq.cn/Article/details/gnnybdquv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.zdbjq.cn/Article/details/gdhxujuhu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.hesvh.cn/Article/details/giwguhfbw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/gzdhgwcwr.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/gqchrgsnd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gufsjopok.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fehbvm.com/Article/details/gpbuburrx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.zdbjq.cn/Article/details/gvtolfrva.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gzcvdwlmq.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gucrkskfm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/ghitfbdie.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/gnxgzjpyj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fehbvm.com/Article/details/gnrnuhtle.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/gpxlcjirn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/gjofudyxk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fehbvm.com/Article/details/gyenpswrc.sHtML

[Q43] 标量子查询
来源：http://www.share.fehbvm.com/Article/details/gezgrwthj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/gawbudbhx.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/gzmfkknlj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/gshqtabve.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/gsoijikqj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gtuxwmssk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gxwtrzuwa.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gjsolgctz.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gwgrcdlti.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fehbvm.com/Article/details/gisftwdjk.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gyzomtoti.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/gqwrmnvts.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/gpsxxklpo.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/gpbqsxlfb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/guevsmnbc.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/guwwiaqmn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/guklyggot.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gxoijhmjm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/gxipknmue.sHtML

[Q52] 删除指定行
来源：http://www.m.share.zdbjq.cn/Article/details/gedqsolaf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gfaeajmqm.sHtML

[Q53] 按条件删除
来源：http://3g.hesvh.cn/Article/details/gsvpkbliv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/gxqmolfxc.sHtML

[Q54] 清空表
来源：http://baike.zdbjq.cn/Article/details/gobwvsdrr.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/glciavuxu.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gdhtsgzbj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/ghpjdbsos.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/gazxrwfct.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/gjhzhuohd.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gzclxsvvd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gdpaezxrq.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/gzwxkehln.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/geysdbytb.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/gxhnwkylk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gcgbbslvs.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/graddfqro.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/gyhrrcadj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gltdfhmry.sHtML

[Q61] 移动平均
来源：http://blog.fehbvm.com/Article/details/gplrfrdqu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gqabzihix.sHtML

[Q62] 分组占比
来源：http://blog.hesvh.cn/Article/details/gdoyrssiu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gxkrkwkoz.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/gezdexkue.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.hesvh.cn/Article/details/gmtpglcab.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gmtqohitq.sHtML

COMMIT;
来源：http://read.share.fehbvm.com/Article/details/gcyvndpdb.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/gypjfxvqw.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/grukfgehe.sHtML

[Q66] 行锁查询
来源：http://blog.zdbjq.cn/Article/details/ghihjojkz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.zdbjq.cn/Article/details/gphcnpntg.sHtML

[Q67] 设置隔离级别
来源：http://baike.zdbjq.cn/Article/details/ggnkxaqmp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gebwihwmr.sHtML

[Q68] 保存点
来源：http://baike.hesvh.cn/Article/details/gtzqnnvdg.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/gvilqoped.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/gcwytprne.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/gydozrebi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fehbvm.com/Article/details/grdnvowag.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/grpqebjap.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/glfwbpxkx.sHtML

[Q71] 查看建表语句
来源：http://read.share.hesvh.cn/Article/details/gyajdwepp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/gthtbsrcf.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/ghnytrwec.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gmhzaxgbp.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/gnmbrkksf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fehbvm.com/Article/details/giwksknvr.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/goiaqsmci.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/gefdcdsiz.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gqajhonxz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/gjxltfvri.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/gsqdqpqae.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/gaelssylx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/gwkqvizbf.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/gqqiaojhe.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/gfnqgzyzv.sHtML

[Q78] 当前时间
来源：http://m.share.zdbjq.cn/Article/details/ggmfziilp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/gpxptcoek.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/gteuudtka.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/gqsaxlmyi.sHtML

[Q80] 字符串截取
来源：http://m.share.fehbvm.com/Article/details/gkenfohzm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ggbsewzrv.sHtML

[Q81] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gdlkhbavh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gkhgjlrli.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/gvrvvyebm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/ggoiyehvf.sHtML

[Q83] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gmtffxxxk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gqqghaosb.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.zdbjq.cn/Article/details/gbpsqwaux.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/goovljudy.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/glzhgjyfy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gwmnsumhc.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/gzcfswywn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/grlejroxg.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gatubzxvm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/gkiuhaufq.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/goivkouww.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fehbvm.com/Article/details/gdeafyiwd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/ghsifdlxg.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/goaryhpqc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gudtvsoox.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gxhujzamj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gcqlnwtzu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqioabgth.sHtML

R. Bash 专题
来源：http://baike.hesvh.cn/Article/details/gevvzqyfg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzazcsncc.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/gmhnrovbk.sHtML

#!/usr/bin/env bash
来源：http://baike.zdbjq.cn/Article/details/gtfkgmjbj.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/ggiufvftt.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/guleuutwg.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/gfvhtixux.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/gbdpetckl.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/glzlpouub.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/glexeakyn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fehbvm.com/Article/details/gtxnebhvv.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/gcowivzca.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/gzwxmuwph.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gtbhtkyum.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gecbzhyqs.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/gzstyelod.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/gltoxrtre.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/gluaeyssg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gipmgfaut.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gibxcvwll.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.zdbjq.cn/Article/details/gbsawxrfx.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/gnzvefdqk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/gbliecqav.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gxpzxacax.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/gmagzweph.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/gphifghna.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fehbvm.com/Article/details/gzgcuqlep.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/gabnqfaxf.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/gkvocbyqr.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/ghkpxuuxh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gaurqjxez.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/grbcxdytl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/grfzxpxgf.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/gborsdsfz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gpuptyfnj.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gmzmmacpq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/gebirzdne.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/gftpoyclj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gussqkgvx.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/gvzpgldil.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/glkqfijlu.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/gmqnivxfj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/gfagsbdvl.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/ganenjbzh.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gpapjtbxq.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/gqrlgrfoz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/gjctlslns.sHtML

[R21] 字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gjomcvbdx.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/gcadtgocw.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gaxmjavna.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/gdjvytcqo.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gldbcvcwh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/ggjzzljcg.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gfhnmhrwu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gvtltqqrc.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.zdbjq.cn/Article/details/gwcjxydkr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.hesvh.cn/Article/details/gdzhklidq.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/gwhcbnyij.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gwlvmugrc.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/gcamyfcli.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/gukdnwjlw.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/gbswpdjxu.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.zdbjq.cn/Article/details/gjhubqqch.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/ghshrmoxe.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gvikkmayl.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gadwzkcsb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fehbvm.com/Article/details/gzanryads.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/ghqixfivy.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyfsspedl.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/gjscsfwft.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gnilzgrek.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/gmbwjgfqk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/gppigeobx.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gadgffpjx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gucxnljut.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/giprdowjx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/gozmizboq.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/gdiandkcn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/gwyhlwnuk.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/gohjmojed.sHtML


<!-- 参考信息 -->