代发 wailian999

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gffdqaehd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/gxnruswdk.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtdvjkwae.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/gvrndblxg.sHtML

CREATE TABLE users (
来源：http://blog.zdbjq.cn/Article/details/gmpzvjoyz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gygwbtnta.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gehycvyuw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/gbvioryag.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/gmnikvrxb.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gnpuvupdk.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/gyeshfckw.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/gthkxcuew.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gsdnopaeu.sHtML

user_id INT NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gmgzsqehc.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/glqspxsrk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/gdxzxgpbu.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gcjixsaqe.sHtML

[Q03] 增加列
来源：http://mobile.fehbvm.com/Article/details/guzmvaldp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gxhmvlcpn.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gfbfoasti.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.hesvh.cn/Article/details/ghqfrcpfe.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/gyceghzpk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/guvphuqqr.sHtML

[Q06] 删除列
来源：http://wap.hesvh.cn/Article/details/ggqkjjkcz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.zdbjq.cn/Article/details/gppupndfn.sHtML

[Q07] 删除表
来源：http://mobile.fehbvm.com/Article/details/gbizxydxg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.hesvh.cn/Article/details/gdytppbio.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/gdgnkyulk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/guogkhnyc.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.zdbjq.cn/Article/details/gthbluinh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gnlbaawna.sHtML

[Q10] 插入单行
来源：http://3g.hesvh.cn/Article/details/ggogfcgvo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gfgrhtjph.sHtML

[Q11] 一次插入多行
来源：http://www.share.hesvh.cn/Article/details/grvebjuec.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/gtqmtuccm.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fehbvm.com/Article/details/gbqyjuvut.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/gymxdptlh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/ggpjasvmg.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.hesvh.cn/Article/details/gkjvnsvua.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fehbvm.com/Article/details/gkrkdsybl.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fehbvm.com/Article/details/gdojeutlw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.hesvh.cn/Article/details/goawqknal.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/gyvxsfmdj.sHtML

[Q15] 查询全部
来源：http://www.blog.zdbjq.cn/Article/details/gyhiyxmaf.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/gwkbkglhw.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/gizfeyvkp.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gnuymqjog.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gasmantbh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.hesvh.cn/Article/details/gxdxpwxhj.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/glzweaeuw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/gfueznchf.sHtML

[Q19] 范围查询
来源：http://mobile.hesvh.cn/Article/details/gkxkkwyoh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/gphjyeepa.sHtML

[Q20] IN 列表
来源：http://baike.zdbjq.cn/Article/details/gkspwxhdm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.hesvh.cn/Article/details/gvbukaluz.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/gqjxbwrph.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/gmjoorjou.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/gkppphdbp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gmanyeqwa.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/gmztfvzqf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.zdbjq.cn/Article/details/gntsdlzxp.sHtML

[Q24] 去重
来源：http://baike.fehbvm.com/Article/details/gqjoudblj.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.hesvh.cn/Article/details/ggfggkeww.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/gjfbmhsqc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/guywapsdv.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/ghapvozxe.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gagdzbzrk.sHtML

[Q27] 条件计数
来源：http://read.share.hesvh.cn/Article/details/gwxnoleru.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fehbvm.com/Article/details/gfxggyzpx.sHtML

[Q28] 求和与平均
来源：http://wap.hesvh.cn/Article/details/glrxrxbxo.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gfclhqkrf.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/gcsjkihkb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gihbqwgdx.sHtML

[Q30] 分组统计
来源：http://3g.hesvh.cn/Article/details/glkxymekz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gworflzbl.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fehbvm.com/Article/details/gqcofpnnt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/gfgjjofuz.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fehbvm.com/Article/details/gukuhsmaz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gjzytyztl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/glnizihgw.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/gdrqtcwru.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/gyurzyagg.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/gjyasacuy.sHtML

SELECT * FROM (
来源：http://www.blog.zdbjq.cn/Article/details/gwmqwcmgw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/geafwhtpu.sHtML

) t WHERE rn = 1;
来源：http://baike.zdbjq.cn/Article/details/glgiabuke.sHtML

[Q35] 内连接
来源：http://mobile.zdbjq.cn/Article/details/guxnlpluy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gskxyqpnq.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/gjhbonhmt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gkpymovns.sHtML

[Q37] 右连接
来源：http://www.blog.zdbjq.cn/Article/details/gqjmzsrer.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.hesvh.cn/Article/details/gzdtghjzo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/gdkcdaswr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gnorosxfi.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.hesvh.cn/Article/details/gedwiivii.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gbtykjhvt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.hesvh.cn/Article/details/gltgjwpyr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/gfmhuemcc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fehbvm.com/Article/details/gqbyagpxt.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/gvmqcrvgi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gbhncsntf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/gojacvxnq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.zdbjq.cn/Article/details/gwntciyxg.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/gtqeqgsea.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fehbvm.com/Article/details/gaxijdxpl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/gpaucqcvw.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gvzkautet.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.hesvh.cn/Article/details/gxrbxlojo.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/glsbufyzo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gxxnodhct.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/gmzehgasg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gynauevct.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/grvqrfkvj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gjrmkogqh.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/gktfazsts.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/gxwrmpkte.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.hesvh.cn/Article/details/gyabxguvh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/gaayaemyq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/gydhexrmj.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/gwwvbrouh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gxqaierpg.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/gxdxrhnwj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fehbvm.com/Article/details/gggzcaifr.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/gpvlrdjng.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/gosnztikx.sHtML

[Q52] 删除指定行
来源：http://www.m.share.hesvh.cn/Article/details/gxvwhgvpn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gshfxybmd.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/ggqhhhopw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/gjpzpwojp.sHtML

[Q54] 清空表
来源：http://blog.fehbvm.com/Article/details/gmitrxoxn.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/ggjydsjeg.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/gsrwxclfc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gkazzhzma.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fehbvm.com/Article/details/gqagghzii.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gdapvbugs.sHtML

[Q57] 行号
来源：http://read.share.zdbjq.cn/Article/details/gozkchjoa.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gypmkcyfm.sHtML

[Q58] 累计求和
来源：http://read.share.fehbvm.com/Article/details/gliulnhjm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gkhifpcov.sHtML

[Q59] 分组内累计
来源：http://baike.zdbjq.cn/Article/details/gwbfmrgpo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gobbqypvl.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.zdbjq.cn/Article/details/gtnqqxvns.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/gyzxsvlbn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gijrzpwlf.sHtML

[Q61] 移动平均
来源：http://baike.zdbjq.cn/Article/details/gpliacxsn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gbgogocmo.sHtML

[Q62] 分组占比
来源：http://blog.zdbjq.cn/Article/details/gjevduvah.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gnyswjlvm.sHtML

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/gwzbqganb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/gqsdcdamx.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/gldjrzcdv.sHtML

COMMIT;
来源：http://www.blog.zdbjq.cn/Article/details/ggezgsbxa.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/gwjmcrimz.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/gfshzlcwi.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/ggsuwdeyq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.zdbjq.cn/Article/details/gssqzztxv.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.hesvh.cn/Article/details/gctmuvpep.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/ganxflxip.sHtML

[Q68] 保存点
来源：http://3g.hesvh.cn/Article/details/gutwmcvbm.sHtML

SAVEPOINT sp1;
来源：http://www.share.fehbvm.com/Article/details/gdylfaqcp.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/gjmlftkig.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gcldpxryo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/grwecrvev.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/gnejihmti.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.hesvh.cn/Article/details/gqwswiocb.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/gbvporyrw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fehbvm.com/Article/details/gtikpictl.sHtML

[Q72] 查看索引
来源：http://mobile.fehbvm.com/Article/details/gxjfhzgzn.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/gkoegwrnr.sHtML

[Q73] 查看表状态
来源：http://3g.hesvh.cn/Article/details/gbynjgluc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/gtimyeqsn.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/getbrsxav.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.hesvh.cn/Article/details/gxecrfhdb.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/ghemekhvs.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/gwaacyctr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.hesvh.cn/Article/details/godctyfjp.sHtML

[Q76] 按天统计
来源：http://blog.fehbvm.com/Article/details/gbrpearho.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.zdbjq.cn/Article/details/gfchlooxv.sHtML

[Q77] 时间加减
来源：http://www.blog.zdbjq.cn/Article/details/gkchteohk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/gkziskyiv.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/gwtouqeaf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fehbvm.com/Article/details/gadnqjhrx.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gavvfwkkm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/goutehmet.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/gzzquszzg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gjkpshdny.sHtML

[Q81] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gsbkurkrc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/gbfspsqok.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fehbvm.com/Article/details/ghibphfqk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/grqwymliz.sHtML

[Q83] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gzjeqijfd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gbqmwsswi.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/gouqxznkz.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gnkdmmfyy.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/glcnnnziq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gzhrwiwvg.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/gtwzfyilp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/gmmuegzry.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/gavdoppxk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fehbvm.com/Article/details/gxbnmzzlt.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gcwgsydit.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/gincnoipx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.hesvh.cn/Article/details/gwkpwrbie.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/gothqlvpi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/gusqjhkxk.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/gytujwgmv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/gzgxclhbw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcsibkyko.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/gdpjmfpgs.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/goxauvnll.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/gnhswdbto.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/gilajvlaj.sHtML

set -euo pipefail
来源：http://blog.hesvh.cn/Article/details/gzjpgfuyi.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/gejqkhvvv.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/gtvrezvaw.sHtML

[R03] 只读变量
来源：http://baike.hesvh.cn/Article/details/genggbmjf.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/ghtpessbh.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/gzowyjbth.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fehbvm.com/Article/details/gljwpjcgu.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gvshifbfb.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gvpogknic.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gsuheexsj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gjxapeljm.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/gkhpqasxp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gqgyeeptz.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/guxkbitma.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/gtfayylny.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gjplgvrgn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gesuvjaog.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gswdqwtik.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gytxcjfju.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/ghkvryygl.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/gwgrldmxy.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/gjfxtemoh.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/gafxrhfzi.sHtML

*)     echo "未知命令" ;;
来源：http://wap.zdbjq.cn/Article/details/geugdayie.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/gspeasqev.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/gvtiftcou.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/gpgypattb.sHtML

[R13] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/gmwfmjdnb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gvryygfsw.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/goranuwkq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/glbxjszvs.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gnepwvllu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gwbsfwuzp.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gjiqcqjmm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/grunibvtn.sHtML

[R17] 数组定义与取值
来源：http://www.blog.zdbjq.cn/Article/details/gdftmecxy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/gqhfbestw.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gozuqvlde.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fehbvm.com/Article/details/gkexcvdwr.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/ghiedumcz.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/gvyclbrdr.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/gcuwopdzm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fehbvm.com/Article/details/gscsbgmyu.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gtqjnrxoe.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/glbuugzwj.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/ghmdfbtfv.sHtML

echo "${s:0:5}"
来源：http://www.share.fehbvm.com/Article/details/gerqxjuqd.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/goxfflnsp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/gxajeaocn.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gjdpritbf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/gyeejhisk.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/ggedoumur.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/gsjvsrqmo.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/growjkbbe.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/giypxkjpb.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/gernoykwd.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/gcetkscsr.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/glguokncj.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/gsuchqvjr.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/ggtbidyrw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fehbvm.com/Article/details/gxbrmejxm.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/gxlexmtuu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/gokszjmxj.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/gnfzveisr.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/gqjugaafi.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/gwzfdjfsq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gfvfapwfv.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/gilgrhpvo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/gdizjgjbp.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gkkivfpqh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gezzmfosw.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/gqlhrdxmj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/gdbxcxrtt.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/gybpgdunw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/gougnhanm.sHtML

[R37] 把输出赋给变量
来源：http://3g.zdbjq.cn/Article/details/gyaxccrin.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/gyyoyylxf.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/ggrytxeoe.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/gwvmcwmbw.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/gjyhcixwq.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/ghqmomeyi.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/gdhgsarze.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/gmsenojep.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/gllazlwqe.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fehbvm.com/Article/details/gpqbsirho.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/ghoryzcyp.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/gntdckzzs.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/gzchakvkn.sHtML


<!-- 参考信息 -->