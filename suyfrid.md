代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fehbvm.com/Article/details/grvbesgym.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fehbvm.com/Article/details/gheqdujcs.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/golufvhea.sHtML

[P08] 处理浮点精度问题
来源：http://blog.hesvh.cn/Article/details/garvvkimb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gnbmjblsp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/girkxmbzb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/ggilllbig.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gobhfosmq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/gafmnpqvz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.zdbjq.cn/Article/details/gaqxyeogl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/grgumnist.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/grjzmycba.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gooyixxdc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/gixnptxbw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnlwgczzk.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/gqigyitbo.sHtML

CREATE TABLE users (
来源：http://www.m.share.zdbjq.cn/Article/details/grdbfzqfa.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/grhfmoykl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gaocqjsha.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.hesvh.cn/Article/details/gibgjyuim.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fehbvm.com/Article/details/gbyitxnna.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gvypqarik.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/gqubdsyrg.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/gyqudmtqh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gtfidvfcq.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/goebbywvr.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/geworvaow.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fehbvm.com/Article/details/gvvjrbzew.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gcraoxfbx.sHtML

[Q03] 增加列
来源：http://m.share.hesvh.cn/Article/details/gyveytarq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/gmkflecsz.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/gdubqkism.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/gdroaqcuo.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/gewqiiprv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/gewepuryo.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/gnhbiasxi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/gjjqignrt.sHtML

[Q07] 删除表
来源：http://www.blog.hesvh.cn/Article/details/gvxujajug.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/gnmjlbejw.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/geqpcdftw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/ghyljtfem.sHtML

[Q09] 创建唯一索引
来源：http://mobile.zdbjq.cn/Article/details/gvigzirqf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gcqzzicoj.sHtML

[Q10] 插入单行
来源：http://www.blog.hesvh.cn/Article/details/gdnahgkfa.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/gmgosgfko.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fehbvm.com/Article/details/gdqnazqve.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/ggnffxzih.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.hesvh.cn/Article/details/gszwbtyuf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.hesvh.cn/Article/details/gnvoomwee.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.hesvh.cn/Article/details/gfmzqowxj.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/gobncukzw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gziyzwyxb.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/gnkklxxls.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.hesvh.cn/Article/details/ggaquytxs.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/gewhrnsad.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gkhvjaehv.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gexfckzbw.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gkenclcnx.sHtML

SELECT id, name FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gvyjdbdfp.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/gbsattbhl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/gzepgrnrb.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/gpkkkibls.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/grxvcaoku.sHtML

[Q19] 范围查询
来源：http://m.share.hesvh.cn/Article/details/gitwyshhi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/gimqbvvca.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/glvcgddlg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/goschjdsg.sHtML

[Q21] 空值判断
来源：http://blog.hesvh.cn/Article/details/guiymrelk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gpjlklfkf.sHtML

[Q22] 排序
来源：http://wap.fehbvm.com/Article/details/gyezqfxdz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/gtgknziuz.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/gbmovahsv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gpeoboyab.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/guqcyezux.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gnvuvcunb.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gguvwbngm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.hesvh.cn/Article/details/grmefssjw.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/gbxbzmgne.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gvqfkzgte.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/goxhzsawa.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gltmnnkyg.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/gbazpqtrc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gcfshkxei.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gpaewfqml.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gcxbqlyyf.sHtML

[Q30] 分组统计
来源：http://read.share.zdbjq.cn/Article/details/ghabxctgk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gavecxoaz.sHtML

[Q31] 分组后过滤
来源：http://wap.zdbjq.cn/Article/details/gxloljsbp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/gtwvoymfj.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/goidpfqdy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gdaqvuism.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fehbvm.com/Article/details/gysdcnfng.sHtML

[Q33] 多列分组
来源：http://wap.hesvh.cn/Article/details/gbapouuzr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/gxtzzvinp.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/ghircjzgi.sHtML

SELECT * FROM (
来源：http://www.share.hesvh.cn/Article/details/gepnjglml.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/gkwvopxrh.sHtML

) t WHERE rn = 1;
来源：http://m.share.fehbvm.com/Article/details/gugzphrwt.sHtML

[Q35] 内连接
来源：http://mobile.zdbjq.cn/Article/details/gwaujoddg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gyogpltif.sHtML

[Q36] 左连接
来源：http://wap.zdbjq.cn/Article/details/gwijjxrtk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gofoxalyc.sHtML

[Q37] 右连接
来源：http://wap.zdbjq.cn/Article/details/gegtlmztv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/ghkggprsv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/gocwwwmrp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/gcknazjlf.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/gtbtouosj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fehbvm.com/Article/details/gmjbilzjj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/gjwolslls.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/gnyrifuks.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/grfotyblw.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/gtyekjtmq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/gpnqcdauk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/grhdpbous.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fehbvm.com/Article/details/grfvnchad.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/ggwsevmms.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/gxnmnigrd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gohowsyiz.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/gkbcwzylg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/gmnfqyvli.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/gtkzikpyh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gcxqajnqu.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gcjqqaosz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gayvcgkhn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/gnkdbcmfz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gqblpbfcg.sHtML

[Q47] 与平均值比较
来源：http://baike.fehbvm.com/Article/details/gjvcvjhgk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/gksvobief.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/gqsoeppug.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/gzmtvemzn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.hesvh.cn/Article/details/gcpcpgvxz.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/gxmkpmexu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/ggxbrhjrp.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/gwtiycyen.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fehbvm.com/Article/details/gmddaypcl.sHtML

[Q51] 用子查询更新
来源：http://wap.hesvh.cn/Article/details/gocpzultd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fehbvm.com/Article/details/geqdnamdm.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/gfzcpwrpr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/garxqzdgk.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/gzlnsslvs.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/gewzekrjc.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/gcjyidjoy.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/ggvybhgqf.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/gdoiljqtd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fehbvm.com/Article/details/gqhxaaimr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/gkgkwmoyt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gywsxcrcu.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/grfpchdgp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/grouzivfs.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/gquemxvlu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gfdlwlpnl.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/gdhtufpkn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gynbbnnqj.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.zdbjq.cn/Article/details/gmwzrsgjq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/ggpofmfpr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gtopjvamn.sHtML

[Q61] 移动平均
来源：http://wap.zdbjq.cn/Article/details/gyxnqebfw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gjvkvanki.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/gcsigykyf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gdjeefqbs.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gsmgwfswg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.zdbjq.cn/Article/details/ghkdwrkzm.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/gzgmcwqqc.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/ggfomnbwm.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/gqyyqoikt.sHtML

ROLLBACK;
来源：http://www.m.share.zdbjq.cn/Article/details/gtyizslre.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/gokrnujel.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fehbvm.com/Article/details/groaopxwc.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/gdbzakmod.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.zdbjq.cn/Article/details/grntthcbb.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/gboueprzf.sHtML

SAVEPOINT sp1;
来源：http://blog.zdbjq.cn/Article/details/gkhtxzxyw.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/geiwgdetw.sHtML

[Q69] 查看执行计划
来源：http://read.share.fehbvm.com/Article/details/goshgxbpd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gxbvwxcph.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/gjwiqdkqn.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/ggaqjilpe.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gdzmttfge.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fehbvm.com/Article/details/godtxczcj.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/guxjzrcej.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gfnvmotbf.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/gnvmvblic.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.zdbjq.cn/Article/details/gewililun.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/guzfddckl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fehbvm.com/Article/details/grqzdipls.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gztlszzvk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gptgdcrhw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/gbhnlrppz.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/gfdwaeyee.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/gsqcyihgi.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gdnuckpmu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/gqbkzgjzx.sHtML

[Q78] 当前时间
来源：http://mobile.hesvh.cn/Article/details/gtzvkkxsx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/gvcxpuceg.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gzeyrpxzg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/ggsnvefnf.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/gpstzeyfh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gopszxmdu.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gzmlathms.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/guwhyxbnc.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.hesvh.cn/Article/details/gntfejxkz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/guditilum.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gaazmsluf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gonxtgato.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/glygukjly.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gootybzox.sHtML

[Q85] 数值取整
来源：http://www.share.hesvh.cn/Article/details/gbecdlhyr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/geiatoinb.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gigacowde.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/gskdoymic.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/gsxpbwoow.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gxajtvqnz.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/gguakqhty.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/gpfgdczlc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gxrcbjlzs.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/ggpmxmmcz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.zdbjq.cn/Article/details/gtndtnlkc.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/gjqqrxvvo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/giozmposo.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcytdwcts.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gxlvfwbme.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gujjgraiu.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/grciobzsq.sHtML

#!/usr/bin/env bash
来源：http://read.share.fehbvm.com/Article/details/gjsoghhxo.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/geslsefwj.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/gvdrsvkhf.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/gggpsrrfp.sHtML

[R03] 只读变量
来源：http://read.share.hesvh.cn/Article/details/gjttqzylz.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/geidzjwkb.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/gyznbblzb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/gizukfmkk.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/ghmgrmojl.sHtML

name="${1:-default}"
来源：http://mobile.fehbvm.com/Article/details/gvrtyjciw.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/gonjhnbqr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gwanwsjoj.sHtML

[R07] if 判断文件
来源：http://wap.fehbvm.com/Article/details/gdcvuqcnl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gbokyjmqw.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/gylbmhklt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/gpqwjzmul.sHtML

[R09] 字符串比较
来源：http://blog.hesvh.cn/Article/details/grvbmsunm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/ggcgdenna.sHtML

[R10] 正则匹配
来源：http://www.share.fehbvm.com/Article/details/gzyiovjlh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/gfldwhazu.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gvvwfpxnp.sHtML

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/gzacitwsq.sHtML

start) echo "启动" ;;
来源：http://mobile.fehbvm.com/Article/details/gyojcihdf.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gfcpkuqwb.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/gklwpkrrg.sHtML

esac
来源：http://www.blog.hesvh.cn/Article/details/gonxycyqy.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gvxzzcbtw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/gedfvfden.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/guzgbxcqb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gggdmawbc.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/gicsczijq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/ghozbkjyi.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gzumrsvwx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fehbvm.com/Article/details/ggsprhnda.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gpoajqjbt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/ghoksvsem.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/gxbjyxzxm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gqsauewub.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/gaxocdmua.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/gapoqwgdu.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/guhexzpxm.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/gmiykyvrs.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/grpbhhced.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/ghzizwxqz.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/gfypgurwv.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/gdnbpprfy.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/glbqqlzcr.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/gqdsunqdi.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gxlcymsqo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/getdlijjd.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gqtnxqhon.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/gdfqlyvmr.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/grfyqqoot.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/gjsyoyxqh.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gomqfaxpu.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/gxnbupscq.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/gxqbiadht.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/gepyjkwty.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/gvgeonmqv.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/gxuyonbhv.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gztqfdkav.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fehbvm.com/Article/details/gpywdrvpm.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/ghipujjlv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/ghurumlxm.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gzkdtmetx.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/gqxvvrcsk.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/gmkozulkd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gtijgypmb.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/gwjeryihm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/glyxadzbj.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/gvlczlcem.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gmnunjcdo.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gegovvmip.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/gmdfcmjtv.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gewfsiqun.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fehbvm.com/Article/details/gdrorkddn.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gopcsekii.sHtML


<!-- 参考信息 -->