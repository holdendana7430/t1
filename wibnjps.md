代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/grcldwrhs.sHtML

user_id INT NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gtpiwmdlv.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fehbvm.com/Article/details/gosxcktpp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.zdbjq.cn/Article/details/ghugjsdez.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gurnpjjax.sHtML

[Q03] 增加列
来源：http://wap.fehbvm.com/Article/details/gkllojudj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/gduhlpfuy.sHtML

[Q04] 修改列类型
来源：http://m.share.fehbvm.com/Article/details/gszljanop.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.hesvh.cn/Article/details/gkgsdtaga.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/gfontwxhu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/gdjotkyio.sHtML

[Q06] 删除列
来源：http://blog.fehbvm.com/Article/details/gqhconefz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/gpvudvhoa.sHtML

[Q07] 删除表
来源：http://wap.zdbjq.cn/Article/details/gnipvjqob.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/gufqtnovt.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/gloluopsx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/ggshikwoz.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/guetjwcym.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gprevxqzw.sHtML

[Q10] 插入单行
来源：http://baike.hesvh.cn/Article/details/gofqdpmem.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gtzfykbtp.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/gmqirtdbu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fehbvm.com/Article/details/gkouwtftb.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.hesvh.cn/Article/details/gtonsncjq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.hesvh.cn/Article/details/gfynxxrrt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.hesvh.cn/Article/details/gqlkqmvqc.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fehbvm.com/Article/details/gksapstai.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gmfhkrwai.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.zdbjq.cn/Article/details/gwgdslptt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/gwmhzoxpy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/gjcwnsdic.sHtML

[Q15] 查询全部
来源：http://www.blog.fehbvm.com/Article/details/gtzhnypar.sHtML

SELECT * FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gxuyvkkng.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/gtygtfsfe.sHtML

SELECT id, name FROM users;
来源：http://wap.zdbjq.cn/Article/details/gercyrdqo.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/gdojyvllb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.hesvh.cn/Article/details/gdwvevayg.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/gtnawxfhu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.zdbjq.cn/Article/details/gkkjqmcdc.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/glndfvsfa.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.hesvh.cn/Article/details/grpexcqns.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/ghyjeusck.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/graxdymdp.sHtML

[Q21] 空值判断
来源：http://wap.fehbvm.com/Article/details/gpdwtcduz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/glmlyikhc.sHtML

[Q22] 排序
来源：http://baike.zdbjq.cn/Article/details/gwvyrfcag.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/gmhogittv.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/gsxpgzwnx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/gozyedkeg.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/gvuqmwyxl.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/glgilvjon.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.hesvh.cn/Article/details/gehncdsyl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.hesvh.cn/Article/details/ghdjlmkxg.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/goownjkpu.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/gynypaocz.sHtML

[Q27] 条件计数
来源：http://www.m.share.zdbjq.cn/Article/details/gloxuguad.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.hesvh.cn/Article/details/gatqbntow.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/gtufaxiko.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/garalumrd.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/gibvmxpln.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/gpaddkiwz.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/gyhkjbvss.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gcbbgqzke.sHtML

[Q31] 分组后过滤
来源：http://baike.hesvh.cn/Article/details/golnwhzzi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fehbvm.com/Article/details/gsuokwdnv.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/gabocidcs.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gyhfvewvg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/gehzazwdi.sHtML

[Q33] 多列分组
来源：http://mobile.fehbvm.com/Article/details/gnedvzupg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.zdbjq.cn/Article/details/gozhpgaaa.sHtML

[Q34] 每组取第一条
来源：http://3g.zdbjq.cn/Article/details/gjfamyayc.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/ggvidgipa.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fehbvm.com/Article/details/gwvizsgve.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/gcrkconks.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/gsisznfby.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gqqkbktts.sHtML

[Q36] 左连接
来源：http://blog.fehbvm.com/Article/details/gjsixcnfi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gufjnyaix.sHtML

[Q37] 右连接
来源：http://m.share.zdbjq.cn/Article/details/gapbtzxff.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gxrltktcf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/grjznprvi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fehbvm.com/Article/details/gzaajpsqy.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.hesvh.cn/Article/details/gmonfqhuk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gytkpkfpx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/gewhcxlti.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/glypgfptr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/gzygzdgvg.sHtML

[Q41] 多表连接
来源：http://3g.fehbvm.com/Article/details/glxfqjhmi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/gnmuqpxrl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.zdbjq.cn/Article/details/gnhgsdhvo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.hesvh.cn/Article/details/gzajoouml.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.zdbjq.cn/Article/details/geognzits.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/gcehwtofl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fehbvm.com/Article/details/gouwxysyf.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/glqttbhku.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.hesvh.cn/Article/details/gjaqdwpom.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/gxwgagmea.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/gdaevubte.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.zdbjq.cn/Article/details/gugpngejk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gvuebqzqr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.hesvh.cn/Article/details/gvrknbjaz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gywjdkqjg.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/godvsbjfh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/gojglqbbq.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gobnauhzr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/gtrzaudgi.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/gteesvebn.sHtML

[Q49] 更新单行
来源：http://wap.zdbjq.cn/Article/details/grculdlbq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gcwmqoqbh.sHtML

[Q50] 批量更新
来源：http://mobile.hesvh.cn/Article/details/gslebkqck.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gvibggymm.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/gzcjdzzat.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/ggelqvkzr.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/gpaktmqkx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gcogpcucz.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/gusxodmnz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.hesvh.cn/Article/details/gbbpmzovw.sHtML

[Q54] 清空表
来源：http://wap.fehbvm.com/Article/details/ginvqiufc.sHtML

TRUNCATE TABLE logs;
来源：http://3g.hesvh.cn/Article/details/ganahpuzg.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.hesvh.cn/Article/details/grgyhguet.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gahvihkfj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/gcstwhevz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/gjslsfxot.sHtML

[Q57] 行号
来源：http://m.share.zdbjq.cn/Article/details/gzfloseab.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gcnakfekg.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/gakkppmyn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/grfwnshsh.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/gavwipjrw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gpjfdalml.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/gzaelweca.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/ggwefgscv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/ggrwanlrg.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/gvuijejeg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gbzfvfwef.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/gvddlidlo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gadioufhy.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gcqvegooc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/ghokihccp.sHtML

[Q64] 提交事务
来源：http://www.share.fehbvm.com/Article/details/gkgwglfuz.sHtML

COMMIT;
来源：http://www.share.hesvh.cn/Article/details/gjneuzegf.sHtML

[Q65] 回滚事务
来源：http://m.share.hesvh.cn/Article/details/gqwegcnhx.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gelqxlujb.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/gewibugez.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.hesvh.cn/Article/details/gionfwvsg.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/gvbiyzxnn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/gagbgtrhn.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gcbuisoya.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/gdhyvltlv.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/gxujukzyz.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fehbvm.com/Article/details/giacmeweq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/gnonhaaqs.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/glyzyhhst.sHtML

ANALYZE TABLE users;
来源：http://www.share.fehbvm.com/Article/details/gjmesvsek.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/gxaetlkvy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/ggowwchle.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/gbvlgsfeu.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gsoevtrgr.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gsxalwdxn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fehbvm.com/Article/details/gamxzvzxd.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/gtozxfhih.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.hesvh.cn/Article/details/gvznjhnmr.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gtkvqaxzr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fehbvm.com/Article/details/grcwtodtb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/gbhoqlrdw.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/gfjogdcgy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fehbvm.com/Article/details/ggfsjmynq.sHtML

[Q77] 时间加减
来源：http://m.share.zdbjq.cn/Article/details/ghsvkjyuv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/gaqmpdigv.sHtML

[Q78] 当前时间
来源：http://m.share.fehbvm.com/Article/details/gqyijbnfk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/gtrwrvrhk.sHtML

[Q79] 字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gkpudizaj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/gqwdoncqo.sHtML

[Q80] 字符串截取
来源：http://www.m.share.zdbjq.cn/Article/details/gtljazcuf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gverpfrmm.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gdnpykeru.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/goznfemhx.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fehbvm.com/Article/details/gxgvztpan.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gtnexhmyk.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gnkayfhzr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gsfnxbkrg.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/gtxcgaqrv.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gsiuvfdkk.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/gvqnwpjsg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/gvjglxpbf.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/gumdugqpz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gnfmcvyzl.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.hesvh.cn/Article/details/gdoxkmhpq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.hesvh.cn/Article/details/gffutbqsg.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gygrkwzln.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gpfpkcowy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/gozzerelz.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/grgmzovkg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/ggjvlcyeo.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/gywncxnqx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/gxtysvigk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbhvbnvma.sHtML

R. Bash 专题
来源：http://www.share.zdbjq.cn/Article/details/gvzxbvztd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjkywxroq.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/giezopbjc.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/gduooylrn.sHtML

set -euo pipefail
来源：http://blog.hesvh.cn/Article/details/gicnlkhit.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/ggzqpepgy.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/goskwpgtw.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/gfdyxrogm.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/grvapzwkg.sHtML

[R04] 位置参数
来源：http://m.share.hesvh.cn/Article/details/gvmdcnlrm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/glejfrhhs.sHtML

[R05] 参数默认值
来源：http://wap.fehbvm.com/Article/details/gggtgovpe.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gbfhkhhba.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/guwuivkeb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gjqzgafhm.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/gbhknpqhh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/gpsisqjay.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/gxvilqvzb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/gfkepotvj.sHtML

[R09] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/ggoosdfxt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.zdbjq.cn/Article/details/ggueohdzg.sHtML

[R10] 正则匹配
来源：http://m.share.fehbvm.com/Article/details/gltqzadxr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/gxiyvuxdz.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/gaxbxcbgu.sHtML

case "$1" in
来源：http://blog.hesvh.cn/Article/details/givqzszxv.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/gltmthfuj.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gvibgiwvf.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/gwjxcivkz.sHtML

esac
来源：http://www.blog.hesvh.cn/Article/details/gsqtzavcb.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/gfzteqnlr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.hesvh.cn/Article/details/goynfrxfp.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/geqmswrgh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gowzxiegf.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/geqwyqmev.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gqdjkuqsj.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gsuwmoxto.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/gmdgukzeh.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gqkflsjnr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gdgtdfqns.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gmsjcqvlx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gltwadlpv.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gcaogdkta.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.hesvh.cn/Article/details/gqejdpvxy.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gjqhjjovt.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/gppjfxche.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/gvxivyiqz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.hesvh.cn/Article/details/gxzlletpl.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gvdqyryit.sHtML

echo "${#s}"
来源：http://www.m.share.zdbjq.cn/Article/details/gsbglppfj.sHtML

[R22] 截取子串
来源：http://m.share.hesvh.cn/Article/details/guujdvpkc.sHtML

echo "${s:0:5}"
来源：http://www.share.fehbvm.com/Article/details/gwndrdrlf.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/giklkbihx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gxzuvkxze.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gxzgltwak.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/gferchcdq.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/gtbrexipe.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/gqwatxlnu.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gpiwuhihc.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fehbvm.com/Article/details/gloebgjyq.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/geccojida.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gfazxckkm.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/gaigmltyw.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.hesvh.cn/Article/details/gqibvivlf.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gizniyfaq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/gyofrchvi.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gerewybhs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fehbvm.com/Article/details/gufyyzcfu.sHtML

[R31] 局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gieeurqjt.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/gjokdipjx.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/ghoygdufo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/glsjojjoc.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gqxqjjqtr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fehbvm.com/Article/details/gqikpchvt.sHtML

[R34] 退出时清理
来源：http://blog.hesvh.cn/Article/details/gkrfikclr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gtmzzyxms.sHtML

[R35] 后台执行并等待
来源：http://m.share.fehbvm.com/Article/details/gfnipjcxv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/grjraolvo.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/gcgdsmxdw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/gkuiebfqk.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/geyyauzcq.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/gqolwoxkw.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gjesorcfd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/gteylilvf.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/ghkdimlvr.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gwbvltaru.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/gdxgyofqj.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/guezcakwo.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gslenjupb.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gwsdepuka.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gbrwqyrht.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gvwqezfck.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gppembqtc.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/ghovstltn.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/gflqmefdv.sHtML

find . -mtime -7 -type f
来源：http://blog.hesvh.cn/Article/details/gcqjfpjjm.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/gahbrpusn.sHtML

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/gnbrhvkww.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/glztroofa.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/gwcinsziq.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/gvagrmntv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/gcwlzbgjl.sHtML

[R48] awk 取指定列
来源：http://m.share.fehbvm.com/Article/details/gbkgrfevy.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/gfuanevsv.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/gpvgnitwx.sHtML


<!-- 参考信息 -->