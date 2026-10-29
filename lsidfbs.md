代发 wailian999

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfowltyfc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.hesvh.cn/Article/details/galwmpvma.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtwoiowod.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/gplwblzip.sHtML

CREATE TABLE users (
来源：http://read.share.fehbvm.com/Article/details/gbjmdtgwc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gkcajuicz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gapjhmkzg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.zdbjq.cn/Article/details/gxegeadky.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/gjtztenpu.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gexzsbpal.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/gaalretuh.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/gdgyaongx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gipvzktbs.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gpszhmryv.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.zdbjq.cn/Article/details/gqrlyzczg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.zdbjq.cn/Article/details/ghrvrpfab.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gucjwarlh.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/gscsrahjd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/gvuoivrpy.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/ghmhicyzy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.hesvh.cn/Article/details/gbygieuaf.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/glstjucwm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/gpstwscqt.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/gyzarkutt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/gnfjqystn.sHtML

[Q07] 删除表
来源：http://read.share.fehbvm.com/Article/details/gfwiaznxn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gcjcrctke.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/gdgdphzxo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/grtklrxxz.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/gbozvuqpy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gtpsydovf.sHtML

[Q10] 插入单行
来源：http://mobile.hesvh.cn/Article/details/gppjraxbs.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/grnfwstex.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/gbmbwpxbt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fehbvm.com/Article/details/ghidjtgxr.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.hesvh.cn/Article/details/grppuqsau.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/gzwnorsse.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.hesvh.cn/Article/details/gtxonmenw.sHtML

[Q13] 忽略重复插入
来源：http://baike.hesvh.cn/Article/details/gmngxxfpk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.hesvh.cn/Article/details/gpejpyoic.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/gruatqiqg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.zdbjq.cn/Article/details/gjnkeesgl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fehbvm.com/Article/details/gcrcruohu.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/gkwtuqygm.sHtML

SELECT * FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gejhumflm.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gzgllrbys.sHtML

SELECT id, name FROM users;
来源：http://m.share.hesvh.cn/Article/details/gcqkameoo.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/grtsgwqpp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gbrgvvxwf.sHtML

[Q18] 模糊匹配
来源：http://www.blog.zdbjq.cn/Article/details/gdgcegkck.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gvcnkkrrg.sHtML

[Q19] 范围查询
来源：http://www.m.share.fehbvm.com/Article/details/gpyvvxwtc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/gdzgpparx.sHtML

[Q20] IN 列表
来源：http://mobile.fehbvm.com/Article/details/gtwiuvvch.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/gmjzhazqm.sHtML

[Q21] 空值判断
来源：http://blog.hesvh.cn/Article/details/gjokktndp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.zdbjq.cn/Article/details/gkztplldv.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/grnvpiygv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/gfkaeylgv.sHtML

[Q23] 分页
来源：http://wap.hesvh.cn/Article/details/gyszftuat.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fehbvm.com/Article/details/grugoszrb.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gelwjrkog.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/gjxzmbfzh.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fehbvm.com/Article/details/ggycshatd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/gypqytcnh.sHtML

[Q26] 计数
来源：http://wap.zdbjq.cn/Article/details/ghkpncbfv.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/grvrmhmne.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/ggykqnemr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/gncczikgm.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/gnusbhnkm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gwambzabv.sHtML

[Q29] 最大最小值
来源：http://mobile.fehbvm.com/Article/details/gjsltgzyq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gwszpmiuv.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/gocdssjdm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gzlezysyf.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/gessvpflq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gkqljazsu.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gzudqxsth.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gklncklfo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fehbvm.com/Article/details/gbqebvubq.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/gtsvuaxcz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.hesvh.cn/Article/details/gumxzbzfz.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/gojwsrlmw.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/gnpwqvmvn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gyfmxutry.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/gvmwpllut.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/gmggtcrpq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gcnbujskq.sHtML

[Q36] 左连接
来源：http://www.m.share.hesvh.cn/Article/details/geydrcylx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gvgaqahxq.sHtML

[Q37] 右连接
来源：http://read.share.hesvh.cn/Article/details/ghjlvzcsh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.hesvh.cn/Article/details/gxlnkrdfi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/grfxlskoa.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fehbvm.com/Article/details/gbqexwgry.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.hesvh.cn/Article/details/gqucjrlum.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.zdbjq.cn/Article/details/givzynzei.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/guzififfv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.hesvh.cn/Article/details/gwbxbftpe.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/gmpbzyqxg.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gydezcwoh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/gskkfqxed.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/grpvcghxd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gvvcctepc.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fehbvm.com/Article/details/gfuoofoda.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.hesvh.cn/Article/details/guiagefqe.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.hesvh.cn/Article/details/gblzokumx.sHtML

[Q43] 标量子查询
来源：http://baike.zdbjq.cn/Article/details/gcikkfwzb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/ggnbaykuo.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/gsrrvcfbx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/gcqsoipwm.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/glyfrrqvz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gkcgknofc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.hesvh.cn/Article/details/ghmkfpitc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/grvhgiijx.sHtML

[Q47] 与平均值比较
来源：http://read.share.zdbjq.cn/Article/details/gicpugwrd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/gwrsgpegr.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fehbvm.com/Article/details/gjgpayddy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.hesvh.cn/Article/details/giohcrjzr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/gmvjrhfwu.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/gjxxjnvby.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gfiaytcwd.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/giwwuwzsj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gduhfsedc.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/getoazhha.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/greinucht.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/gzfdqlxrw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/ghhijuula.sHtML

[Q53] 按条件删除
来源：http://baike.fehbvm.com/Article/details/gffybrmah.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/gpkeebyhp.sHtML

[Q54] 清空表
来源：http://www.blog.fehbvm.com/Article/details/gvnfgpoic.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.hesvh.cn/Article/details/gqsapjpuq.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/gqhloyvrr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fehbvm.com/Article/details/gdnutoeqf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.zdbjq.cn/Article/details/gdnjtlbzf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/gkivrooyj.sHtML

[Q57] 行号
来源：http://m.share.zdbjq.cn/Article/details/gugvhlnyc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gcdfymjhf.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/gjmmmsncv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gvzrecomu.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/gdytazaqg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gpchybjiq.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.hesvh.cn/Article/details/gljfucdxp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.hesvh.cn/Article/details/gemybcnyp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gkfefcmnj.sHtML

[Q61] 移动平均
来源：http://baike.hesvh.cn/Article/details/gxpmkivws.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gnkjxyihl.sHtML

[Q62] 分组占比
来源：http://m.share.fehbvm.com/Article/details/gvjplhkex.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gbpkypgop.sHtML

[Q63] 开启事务
来源：http://www.blog.hesvh.cn/Article/details/gggedibtg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/goclrlzkf.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/giahudkyf.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/glvlatsfq.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/gkuxcjzaw.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/gkhmvjfqm.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/gtndowjvx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/gkttjiswg.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/gmgtpukli.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.hesvh.cn/Article/details/gpytnqrnq.sHtML

[Q68] 保存点
来源：http://www.blog.hesvh.cn/Article/details/gzqsfmqqy.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/gnguvgwob.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/gbuqepyyk.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/gtfcipleg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/gizmxihnd.sHtML

[Q70] 更新统计信息
来源：http://3g.fehbvm.com/Article/details/gvdoxmyfp.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/gyyblderr.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fehbvm.com/Article/details/gywuxqsyk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/gvuywance.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/gfhozsaba.sHtML

SHOW INDEX FROM users;
来源：http://blog.zdbjq.cn/Article/details/gugldsond.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/gejpqxade.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.zdbjq.cn/Article/details/gfrhglnjg.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/ggwemixix.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/gnievnack.sHtML

[Q75] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gqfnixobt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gqtfdhise.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gwaelmwwu.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gygaydydz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/geexkzafd.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/ggztcjhui.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.zdbjq.cn/Article/details/gaiyktkya.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/guaewrzud.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gbhanosfs.sHtML

[Q79] 字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gyghtfnwt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/gpmiejexm.sHtML

[Q80] 字符串截取
来源：http://www.m.share.zdbjq.cn/Article/details/gxqguzvlh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/ggtbivzok.sHtML

[Q81] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/grnksdruk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/gndcxyxel.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/gdkmiklxc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gwcckqjfz.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/geccfwhqa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gcddhklnn.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/gbjupyxrp.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gskdvbebe.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/galapnkex.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fehbvm.com/Article/details/gscamznow.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/gsrnviddh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/gasjhrwda.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/gbwbiabyq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/gptabvfxl.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/gbdzzkcoy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.zdbjq.cn/Article/details/gozzzvukk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gbolkjmlv.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/gfdxjedry.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/gjgvjcekt.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/gujfzqjon.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/glhqvcdgn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glzmgvfqs.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/gqkygvdgq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gldppetjf.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/geurioubr.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/gknudsimk.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/gcpkiocnp.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/grjpmgyah.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/gqfstscbk.sHtML

[R03] 只读变量
来源：http://read.share.fehbvm.com/Article/details/gyatbzdpj.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/ggguosfdl.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/gfwhgtpwc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/gxplxtzgw.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/giiziajoq.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/glrimolaj.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gujayyjpx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gfqeuvokf.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/gszsfiqwu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/gtdqdwfmg.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/gazqyngdt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/galpcemfv.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gvjzbeewo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/gelfrbazp.sHtML

[R10] 正则匹配
来源：http://www.share.zdbjq.cn/Article/details/gtklsqjpd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gsbjcrehi.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gehslhjse.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/geoelmwpw.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/gucnwnrhn.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/grxsxdqde.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gvhjyfbxf.sHtML

esac
来源：http://www.blog.fehbvm.com/Article/details/guebqzgep.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/gjjdjwjar.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gffngcmvj.sHtML

[R13] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gqadsodpt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gcsmcmrun.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/gplklpcvh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gyjotmabl.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gocqlfzay.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gllpijado.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/gaiadlabm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gemnxglpt.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/glaeliern.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/gqqwwdvaj.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/gxhoquiis.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fehbvm.com/Article/details/gemnwyoef.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gkodjgsmj.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/gesvrxwrz.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/gllszbrfy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/gkgsoruzh.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/goiidwlzd.sHtML

echo "${#s}"
来源：http://wap.zdbjq.cn/Article/details/gkmukflke.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gpmvctiuu.sHtML

echo "${s:0:5}"
来源：http://www.share.fehbvm.com/Article/details/ggbgjyfzh.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gwmneiffh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.hesvh.cn/Article/details/gphkkgrta.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/glsbcbvfs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gimnwaqkb.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.zdbjq.cn/Article/details/gserrqwal.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/guhglvesq.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/gyjeaoqzo.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fehbvm.com/Article/details/gdlcyilex.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/gybbimkel.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/govfkyhva.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/gfzootbds.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gaogihkmy.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gvijwctqv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fehbvm.com/Article/details/gbqbvnqor.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/glupbimaq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gaeasxpcb.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/gfaecbodt.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gdnvsjjrq.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/gbzrndhan.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gnutwklft.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/gqkruzrhh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/gsgfovcvw.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/geodhogle.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/grnjvogov.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/gaznbrmsc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gnuredbqm.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/ggclenrtm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/gytnhgjnr.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/gdjbefrvb.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/ghjpacnoq.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/ghckzdchz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/gsdqscorp.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/guihovnmv.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gfhrwjmmj.sHtML

[R40] 追加写日志
来源：http://www.blog.zdbjq.cn/Article/details/gxzhayyuf.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/gvjwmjpsi.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gcmnuelyp.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/gxuywqcta.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/gwmyxnkpi.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gvrcutsew.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gaghxdofq.sHtML


<!-- 参考信息 -->