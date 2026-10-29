代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/gecvjczpq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/gcjuiokoa.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.zdbjq.cn/Article/details/ghzpffowx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fehbvm.com/Article/details/guxdkyeer.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gffglalys.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/goorqnpxd.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpltdacpf.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/gjstoyjlo.sHtML

CREATE TABLE users (
来源：http://baike.fehbvm.com/Article/details/gyrqxqhmd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gtvrqbwlg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/guqzrfafb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.hesvh.cn/Article/details/gvnszmhkk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fehbvm.com/Article/details/gegnucokk.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gaqcmrcpg.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/gapqewgmd.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/gdrxcggmt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gddepille.sHtML

user_id INT NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gsuwfhxva.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/gmqbjpupy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/gdogposko.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gxiccoprx.sHtML

[Q03] 增加列
来源：http://wap.fehbvm.com/Article/details/gyyuvjvvl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fehbvm.com/Article/details/guzfdigit.sHtML

[Q04] 修改列类型
来源：http://baike.hesvh.cn/Article/details/gbexmrkjw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/gnbutgyhq.sHtML

[Q05] 重命名列
来源：http://www.blog.fehbvm.com/Article/details/gkdgqhlxz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/gkhyvwtju.sHtML

[Q06] 删除列
来源：http://wap.zdbjq.cn/Article/details/gekihlxot.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.zdbjq.cn/Article/details/goftoyxfc.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/gnpkddgmr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.hesvh.cn/Article/details/gnncmolqa.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/ggnmsbrrs.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gbdtwqvmr.sHtML

[Q09] 创建唯一索引
来源：http://www.share.zdbjq.cn/Article/details/gccdtwedl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/giykgnfui.sHtML

[Q10] 插入单行
来源：http://baike.zdbjq.cn/Article/details/gfagvclvh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.hesvh.cn/Article/details/gogexntyv.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/gmihysspg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/gvjluczdk.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.zdbjq.cn/Article/details/gdmegmyuz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/gycqgpicj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/gjcybhtbq.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.zdbjq.cn/Article/details/guwzldmso.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fehbvm.com/Article/details/gcluxecfs.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.hesvh.cn/Article/details/gnuyvkcws.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.hesvh.cn/Article/details/geuonrolo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/gggsnafok.sHtML

[Q15] 查询全部
来源：http://blog.hesvh.cn/Article/details/gegcpluzf.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gacayjpoj.sHtML

[Q16] 查询指定列
来源：http://www.m.share.hesvh.cn/Article/details/gidxeucvy.sHtML

SELECT id, name FROM users;
来源：http://mobile.hesvh.cn/Article/details/ggcwbtewl.sHtML

[Q17] 条件查询
来源：http://baike.fehbvm.com/Article/details/gwirtozmw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.hesvh.cn/Article/details/gfwthmgno.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/gzbsjqjhl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gmtbcnulw.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/ggenuzebh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/gltylneoo.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/gqzbvssxk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fehbvm.com/Article/details/guzmsgejc.sHtML

[Q21] 空值判断
来源：http://www.share.hesvh.cn/Article/details/gyqahwayd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/godutxrbr.sHtML

[Q22] 排序
来源：http://www.blog.zdbjq.cn/Article/details/gurbzcjpx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/gczoeldbb.sHtML

[Q23] 分页
来源：http://www.m.share.hesvh.cn/Article/details/gxqqxwgwq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fehbvm.com/Article/details/gignsemty.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/gjtltajqd.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/gfyalyzmq.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fehbvm.com/Article/details/glkzakszv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.hesvh.cn/Article/details/glnretuoo.sHtML

[Q26] 计数
来源：http://www.share.fehbvm.com/Article/details/gtjjohvsd.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/gckqlvgrn.sHtML

[Q27] 条件计数
来源：http://mobile.zdbjq.cn/Article/details/ggdgtxcws.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fehbvm.com/Article/details/gtswkccsf.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/grtuebqce.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gtldxacyj.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gjpdfdzep.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/ggpitotzp.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/gagjnxnba.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gqvreflje.sHtML

[Q31] 分组后过滤
来源：http://m.share.zdbjq.cn/Article/details/gnaunbcyp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/gdxsqmpru.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gjcsnukuo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gnrjrqicc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fehbvm.com/Article/details/glwkjxvda.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gbspdkmsg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.hesvh.cn/Article/details/gxmusokwa.sHtML

[Q34] 每组取第一条
来源：http://m.share.fehbvm.com/Article/details/gzabdcrzv.sHtML

SELECT * FROM (
来源：http://mobile.hesvh.cn/Article/details/gskwnecpo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gjvbjyysq.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/gmenjxypc.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/gfwovzioz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gyijhfaft.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/gijqlziea.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gtmvjagmt.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/glyajhzzn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.hesvh.cn/Article/details/gizpxqqcf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/gjobywktu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/gcugoyyzb.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.hesvh.cn/Article/details/grgtcegli.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/gkiijjviu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fehbvm.com/Article/details/geeivsjcd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/gjyrpoolk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fehbvm.com/Article/details/giqmpzbal.sHtML

[Q41] 多表连接
来源：http://www.blog.zdbjq.cn/Article/details/gldtdiwyk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/glezcggab.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fehbvm.com/Article/details/gqmvpnicu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fehbvm.com/Article/details/gcvkrepen.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.zdbjq.cn/Article/details/gqtbeyaqi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.hesvh.cn/Article/details/grymgvpki.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/gzdtttfmw.sHtML

[Q43] 标量子查询
来源：http://read.share.hesvh.cn/Article/details/gtilbxqxs.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.hesvh.cn/Article/details/gmjjtvoww.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/gukizkoyi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/gtpzlgqqg.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/gvhiibcmv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/geuvpgene.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.zdbjq.cn/Article/details/gtgryrtio.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/goviavfaw.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/gleqiffeo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gzffpllkp.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.hesvh.cn/Article/details/gzhtmquby.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fehbvm.com/Article/details/gqgyyqgcv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fehbvm.com/Article/details/gxqreeeiw.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gouwtkdqb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gqxsrynvr.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/gulploeca.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.zdbjq.cn/Article/details/ggwxrfkpd.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/gctcvspzo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gcwodltyr.sHtML

[Q52] 删除指定行
来源：http://baike.hesvh.cn/Article/details/glghkbaqp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gvhilbtkf.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/gtwwkwwxv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gbqkpuqxi.sHtML

[Q54] 清空表
来源：http://www.blog.fehbvm.com/Article/details/gxcvmookm.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/guojpvuvl.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gbsglzdbs.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gnmthofoe.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/gchsvcgmu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/grxbliyew.sHtML

[Q57] 行号
来源：http://3g.fehbvm.com/Article/details/gnpwnijgg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fehbvm.com/Article/details/gcjhxtpdl.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/ggsqnravu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gbtxmfhbh.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/gydgezbyc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gqofphrfy.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/ggkzeqsqp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/glvzdfydu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/ganieqamc.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/gzqozixlk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/ggkcdbelo.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gqwuvmaka.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gfhgbpvyr.sHtML

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/gzhsjkqws.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.zdbjq.cn/Article/details/gfoiuhegq.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/gztlxqlua.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/gwbatzocy.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/gqsnxwvzz.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/gphayhzge.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/gawyfroas.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/gfsqputve.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gstctbzdm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/gmcvhwirw.sHtML

[Q68] 保存点
来源：http://www.blog.fehbvm.com/Article/details/gokrpvfby.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/gfuhozvzn.sHtML

ROLLBACK TO sp1;
来源：http://blog.fehbvm.com/Article/details/giarwtall.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/gjqjuauvr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.zdbjq.cn/Article/details/gcfgceqtl.sHtML

[Q70] 更新统计信息
来源：http://3g.fehbvm.com/Article/details/gtpfcllab.sHtML

ANALYZE TABLE users;
来源：http://3g.hesvh.cn/Article/details/gilruzmly.sHtML

[Q71] 查看建表语句
来源：http://3g.fehbvm.com/Article/details/gpujwxlcl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.zdbjq.cn/Article/details/gdwqumpqm.sHtML

[Q72] 查看索引
来源：http://3g.zdbjq.cn/Article/details/gfvgtsvlm.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/ghydtbunr.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/gsaqtgiwl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/gcgvwrlhf.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/gwmvyqcwg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fehbvm.com/Article/details/gjwudbrni.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/ghvlmqvbw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gccijvuou.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/grefhofca.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/gskjxrsyu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gfalwoswv.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/gyajnrumm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/gullcganl.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gtwbftupm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/gpcamgilo.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/givduaqjf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/gzrfmdudq.sHtML

[Q80] 字符串截取
来源：http://3g.fehbvm.com/Article/details/goygdelcl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gfermrqer.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gcnmsgpbx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.zdbjq.cn/Article/details/gfdmmtins.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/gonvbajpb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gpawnopgz.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gsmjurgqd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gcyvnqejx.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/guhkvvyoi.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gnonnuhxw.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/gcbayastn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/gaawbjrdy.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gnalhnzdg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.zdbjq.cn/Article/details/gbjfvkdzk.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/gbhnkgmmk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fehbvm.com/Article/details/gddnhnyvi.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/guxmtchjf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.hesvh.cn/Article/details/gltdzzals.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gkrwpdjpj.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/gtpipyvkj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fehbvm.com/Article/details/gnrxnmchi.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/gusjnnsrm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/gribzldap.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkvcrkwon.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gprdinodd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfwstipco.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gclmuuogz.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/gheryypwq.sHtML

set -euo pipefail
来源：http://wap.fehbvm.com/Article/details/gnjfrmhcj.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/gynvmlpqu.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gptixgswl.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/gnmuizzfk.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/ggtvmympe.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gegubgthk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/gnmmkicsu.sHtML

[R05] 参数默认值
来源：http://wap.zdbjq.cn/Article/details/gwwslkpwq.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/goinkivpb.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/gvbateufw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnmkwdzgq.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/gwgiifzev.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/gpuvumaup.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gtjxqbxct.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/gonlzckfv.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gidcwpfxb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gecoccwpp.sHtML

[R10] 正则匹配
来源：http://www.m.share.hesvh.cn/Article/details/ghczssevy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/gpzpjndli.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/gsjupxdgp.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/gioowwjhb.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/gfxpihgzz.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/gyaluhifx.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gohujymuw.sHtML

esac
来源：http://wap.zdbjq.cn/Article/details/gacozhgmg.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/grkisgilm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/gkcpuqppb.sHtML

[R13] for 计数循环
来源：http://baike.fehbvm.com/Article/details/gaymllibl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gxbvwdoxr.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/gbdnjjwbu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gungsuvif.sHtML

[R15] while 逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gbksduktk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/gijevefye.sHtML

[R16] until 等待条件
来源：http://wap.fehbvm.com/Article/details/gjddemvde.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gfusvbwke.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gltetquxw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fehbvm.com/Article/details/gvldydasp.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/gofgwruki.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/gzoiquyrx.sHtML

[R19] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gtyfzartx.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/ggxujsvoh.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/gfzvygfcx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/gfswayxyg.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/glmymgjzo.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gsrcvuhci.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gmpzzitlf.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/gceirlode.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/guvmbgsto.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gvtzkyvpc.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gwhufojpj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/glenuigfm.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/gbkkxacgh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/ghzfsgsui.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/guowhttpd.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gvjvpheiw.sHtML

[R27] 算术展开
来源：http://blog.zdbjq.cn/Article/details/gcuvzctjz.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/gmtuolwsl.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/gxazhmevv.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/grpeoffmv.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gdlpaztmy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fehbvm.com/Article/details/gigfuzopm.sHtML

[R30] 函数返回状态码
来源：http://3g.zdbjq.cn/Article/details/gowozydxz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/gzcagizuy.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/gtyrsruui.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gykzxasxo.sHtML

[R32] 参数个数校验
来源：http://m.share.zdbjq.cn/Article/details/ghflkaxjk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gpnrmzutf.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gdyvdeoxk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.zdbjq.cn/Article/details/gaiqxqwoi.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/guxrjykkx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gnngfrhho.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gartglrgm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/giawhuxij.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/gtikgncki.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/gvpldnebb.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gbdhsssqp.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/gegzjulhq.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/grjxxjaed.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/gesadatxp.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/ghfeeiuxu.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/gbjfakpmu.sHtML

[R40] 追加写日志
来源：http://m.share.zdbjq.cn/Article/details/gdmkwusrg.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gkycflgfs.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/gxdyygdlm.sHtML


<!-- 参考信息 -->