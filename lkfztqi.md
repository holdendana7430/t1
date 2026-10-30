代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fanxiaobao.xyz/Article/details/guogvcljv.sHtML

);
来源：http://3g.fanxiaobao.xyz/Article/details/geejdjvoj.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgrhbepm.sHtML

CREATE TABLE orders (
来源：http://wap.fanxiaobao.xyz/Article/details/gmybjleip.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fanxiaobao.xyz/Article/details/gclaxsnbi.sHtML

user_id INT NOT NULL,
来源：http://www.share.fanxiaobao.xyz/Article/details/gyosszvec.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fanxiaobao.xyz/Article/details/gcinpfxlc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpgkmzqq.sHtML

);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhfbuvnd.sHtML

[Q03] 增加列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqjoqjzo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuqrekmp.sHtML

[Q04] 修改列类型
来源：http://baike.fanxiaobao.xyz/Article/details/gwnbckoyl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkhueorr.sHtML

[Q05] 重命名列
来源：http://3g.fanxiaobao.xyz/Article/details/ggkxwnhsb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjlwlzzd.sHtML

[Q06] 删除列
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkouseks.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunjhfzjd.sHtML

[Q07] 删除表
来源：http://blog.fanxiaobao.xyz/Article/details/gnjdtuytt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gnlpqldfo.sHtML

[Q08] 创建普通索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gskoxhhjm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxteufcr.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtospedo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzvqjrlr.sHtML

[Q10] 插入单行
来源：http://blog.fanxiaobao.xyz/Article/details/grikgabvw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gvozlwssw.sHtML

[Q11] 一次插入多行
来源：http://wap.fanxiaobao.xyz/Article/details/gqpkviobx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczgtephb.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fanxiaobao.xyz/Article/details/gxhuauhhf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhbuchwu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fanxiaobao.xyz/Article/details/gxegteizo.sHtML

[Q13] 忽略重复插入
来源：http://blog.fanxiaobao.xyz/Article/details/gdhefglft.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gmhalsnjo.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fanxiaobao.xyz/Article/details/gijkvbdjv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fanxiaobao.xyz/Article/details/gecqzwrpi.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fanxiaobao.xyz/Article/details/gpmanhxyv.sHtML

[Q15] 查询全部
来源：http://baike.fanxiaobao.xyz/Article/details/gtmvmvwry.sHtML

SELECT * FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gescihbye.sHtML

[Q16] 查询指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gplwilxwr.sHtML

SELECT id, name FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gibqpwcix.sHtML

[Q17] 条件查询
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrlkqmuk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdudquqnx.sHtML

[Q18] 模糊匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkcernsw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkwntxbc.sHtML

[Q19] 范围查询
来源：http://www.share.fanxiaobao.xyz/Article/details/ggulmxqzh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fanxiaobao.xyz/Article/details/gtemyvonc.sHtML

[Q20] IN 列表
来源：http://wap.fanxiaobao.xyz/Article/details/geeiurdyg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqyobwhzj.sHtML

[Q21] 空值判断
来源：http://www.share.fanxiaobao.xyz/Article/details/glnzplugb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fanxiaobao.xyz/Article/details/gnsiasnpp.sHtML

[Q22] 排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgbxuret.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fanxiaobao.xyz/Article/details/gpunvjcfj.sHtML

[Q23] 分页
来源：http://blog.fanxiaobao.xyz/Article/details/gvtlizhju.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fanxiaobao.xyz/Article/details/gvbzznhca.sHtML

[Q24] 去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbtdorag.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyssnnmlf.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlvwdyid.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fanxiaobao.xyz/Article/details/grmrjhvlo.sHtML

[Q26] 计数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjxkpgld.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gubickmpn.sHtML

[Q27] 条件计数
来源：http://mobile.fanxiaobao.xyz/Article/details/gafocqfzd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gywbrptei.sHtML

[Q28] 求和与平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsquentb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/geeaihdtv.sHtML

[Q29] 最大最小值
来源：http://3g.fanxiaobao.xyz/Article/details/gmaiymlpi.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/grseizomd.sHtML

[Q30] 分组统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gndtqklxt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gencrefkb.sHtML

[Q31] 分组后过滤
来源：http://baike.fanxiaobao.xyz/Article/details/ghyzgtxdi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gkyrfgikl.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrmfluvb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjjvmalw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgdtjqil.sHtML

[Q33] 多列分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqpdhwev.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fanxiaobao.xyz/Article/details/gjimcsgwe.sHtML

[Q34] 每组取第一条
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwmiespe.sHtML

SELECT * FROM (
来源：http://wap.fanxiaobao.xyz/Article/details/gkxchgjcg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fanxiaobao.xyz/Article/details/ghdsmlold.sHtML

) t WHERE rn = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gfcevifzb.sHtML

[Q35] 内连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyqkasad.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrbfqnvq.sHtML

[Q36] 左连接
来源：http://blog.fanxiaobao.xyz/Article/details/glbkmgtgv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmubnngjf.sHtML

[Q37] 右连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcktnhvl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gffklysuu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fanxiaobao.xyz/Article/details/gyjhavdhv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fanxiaobao.xyz/Article/details/ggajxbyvf.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvaixkde.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fanxiaobao.xyz/Article/details/gkreaphyy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fanxiaobao.xyz/Article/details/grxsehpvt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fanxiaobao.xyz/Article/details/gxfbvltwv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtxwgdai.sHtML

[Q41] 多表连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmytmhuf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzycvlkeo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdngfhuna.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmpkjiyv.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/glmbzhkhz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fanxiaobao.xyz/Article/details/gdmqfyxve.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/ginpvpdwn.sHtML

[Q43] 标量子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfdxkpec.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmeiakupn.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayrnaozu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fanxiaobao.xyz/Article/details/gvatxoklo.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzwbrgfd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gjlqyytvv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjrmaxan.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gwalipjis.sHtML

[Q47] 与平均值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gfebpkvap.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fanxiaobao.xyz/Article/details/gnaejmlqx.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gkaxweule.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fanxiaobao.xyz/Article/details/gblncgklq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwvaostq.sHtML

[Q49] 更新单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goalafhrf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gmofbaygt.sHtML

[Q50] 批量更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gocxutyav.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlaatdna.sHtML

[Q51] 用子查询更新
来源：http://3g.fanxiaobao.xyz/Article/details/gydbyhwxy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gzomrfbol.sHtML

[Q52] 删除指定行
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcigrjqy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/ggmocuelm.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhxtsydx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gdttuhvdm.sHtML

[Q54] 清空表
来源：http://baike.fanxiaobao.xyz/Article/details/gzomvxpuv.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gindikepm.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsgoxcby.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gnogoxktu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugkyvzqb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gwaexckrk.sHtML

[Q57] 行号
来源：http://blog.fanxiaobao.xyz/Article/details/godjyhjie.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckeyqbdb.sHtML

[Q58] 累计求和
来源：http://3g.fanxiaobao.xyz/Article/details/gcwtdklvl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gegqhqgme.sHtML

[Q59] 分组内累计
来源：http://m.share.fanxiaobao.xyz/Article/details/granbzzuk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqborgzc.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/gpjaiosvr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fanxiaobao.xyz/Article/details/gapzbdzdt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxahbvhj.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/gwfrbpsns.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhifjkzq.sHtML

[Q62] 分组占比
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvmcbqaz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gzeczgylj.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/gaquzmblr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxcnbcuo.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/gsppjtucp.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/gyhmcwfcg.sHtML

[Q65] 回滚事务
来源：http://wap.fanxiaobao.xyz/Article/details/grhnyorye.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/gbclviatj.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/gitguqwms.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrceqxmi.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibjhracp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/gekzvuebv.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkwafchf.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmevinoj.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwosisrk.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/gftfatqgc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnqywqnb.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/gxnhvgrps.sHtML

ANALYZE TABLE users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgnpkydp.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gjalkqysp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gsljwqcty.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/grtxwaqxl.sHtML

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gxliuiqen.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/gjimahndl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gdezwwxzi.sHtML

[Q74] 强制使用索引
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcwdicyv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqtgpeix.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxppzzkgk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gublwqqqk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/gumyryqhs.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gotvuooec.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqyeaprj.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/gghbyelfg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbcmlmey.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdyxdldr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxczaduw.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gxibqeemx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gweyhnjfj.sHtML

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/gjvnfnpad.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzsvgxor.sHtML

[Q81] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/guxkhkqxz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwbqxcle.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gkodlgnns.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gwyhfbpnd.sHtML

[Q83] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gzjonnaha.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gerehiprk.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/gpamjykma.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gehjaeogl.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/gbphhdzyi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsffursq.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbtxungs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgkkrotk.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklumgexq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gpvvuvltq.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gkxcnezor.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/giusxblln.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gqgjjwrxq.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpynqmon.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gbttctyku.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/glkzoddli.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfteipasc.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gzkmcrkhe.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyxppejd.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/giukgevsv.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqnteuwp.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/ghwjkbqmj.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gkldzmpad.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/guqjpazpi.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfsnzlxb.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfkkpgpy.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/glfqdajzs.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gomsezjbh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gydjzgvbj.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcnypgck.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gddrjpary.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxkvjoze.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnukoscpc.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqvsapws.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gpeajulzu.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gnsmsznbg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gcumoxjbw.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/ggxfpsaaa.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/glbdglmtr.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/glcqimkrm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gorygyyzx.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrmrbpee.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/guxdgvnoq.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcrehcyk.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnoejyiul.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfprusdfe.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gnogzvihu.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvljklarz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gmatscugr.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gyoxecxbh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gejfutxsf.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvtdxxsy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gjopppsrh.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gzrpzzklc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/girvirfan.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gxngnqows.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfcpxhjv.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/ghlaszujq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfptdmsbq.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gturczrvw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gstmgzcxq.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gkiwdqzzd.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/govwpokcb.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfwadhhu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxohboegf.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmianwwc.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtbiadit.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gikzpkhwd.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gzrxevxid.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/grvzrmwqv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfwouadi.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnuqgkrb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gefaexdpw.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gxwsxkxxd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gitgqnudy.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gnavoyfah.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbvhjggs.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gqeumtcyd.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgeajvzc.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gdvmjywms.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gpqdrkjcm.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gftyotnvw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/ggmpjyltq.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gvslqsbww.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/guocbaadd.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gljdvqobw.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdiakqvaa.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gcitrdhqf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjnnqcpf.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gkauwtzdz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gxkvndacm.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazxwwctg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gdaioqtgi.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfywythj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/geojsyddt.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gebuutqcu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gropqkugh.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gspbxrbth.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gkfflxuzb.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gkazxspsp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gbqpvycqf.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gxnsgtwvv.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gvoeyyatm.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gzahpbnnw.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdyssoem.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjdegmcf.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gmyccexwn.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqiuioihp.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gzkardlos.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gnixyvwjm.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gabybizlt.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysdypxbx.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gjaudkwkg.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdzybjcb.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gefmnvivm.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmnmfhyn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwavqssg.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gpktkzuxv.sHtML


<!-- 参考信息 -->