代发 wailian999

CREATE TABLE users (
来源：http://blog.zdbjq.cn/Article/details/gbqbybyge.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gfsrrfbxy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/glcwrchpr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.zdbjq.cn/Article/details/gksrqjlre.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/gkdldfhuk.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gotyvbmib.sHtML

[Q02] 创建带外键的表
来源：http://baike.fehbvm.com/Article/details/ghiagfkql.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/gehjkgqdx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gwjhlsmmy.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gnkqugqoo.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.zdbjq.cn/Article/details/gkxxzmbfd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gajfxlmse.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gmfglnrym.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/gxudgflaa.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.hesvh.cn/Article/details/gcnaqlodf.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/gpcxtfunb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fehbvm.com/Article/details/gdfmnafct.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/gwqjdltvm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fehbvm.com/Article/details/gtmrkpltm.sHtML

[Q06] 删除列
来源：http://3g.fehbvm.com/Article/details/gucgbenmr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/gdhodzmwk.sHtML

[Q07] 删除表
来源：http://read.share.fehbvm.com/Article/details/gzahkurhe.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/gcuqnlkhw.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gvunmmlce.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gvkiygiho.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.hesvh.cn/Article/details/gvdxnshvl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gwsegragr.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/ggqcjismk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/ghxksirfd.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/gsuuwgtnt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.zdbjq.cn/Article/details/gvszjkgkc.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.zdbjq.cn/Article/details/gmzmklkxt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fehbvm.com/Article/details/gtqudhpsj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.hesvh.cn/Article/details/gugrbdgfs.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/gulqkphzw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gmanpgrwr.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/gjliggyad.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.hesvh.cn/Article/details/gojwfhelc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/ghkqztqeo.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/geksxzwvh.sHtML

SELECT * FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ggwzfwsua.sHtML

[Q16] 查询指定列
来源：http://3g.hesvh.cn/Article/details/gewvxjdbk.sHtML

SELECT id, name FROM users;
来源：http://m.share.fehbvm.com/Article/details/gimwujqjm.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/gmdeenopk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fehbvm.com/Article/details/gocfizkwp.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/ggnuaibhv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.zdbjq.cn/Article/details/gemhuukpm.sHtML

[Q19] 范围查询
来源：http://baike.fehbvm.com/Article/details/ghukqxtck.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fehbvm.com/Article/details/gsauqecgp.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/gbthqufaw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/gqlolpfrt.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/gpqjnxgbg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fehbvm.com/Article/details/gonwyzfog.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/ggngbrxcp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gqdgkvpbi.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/gcmxhxozu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fehbvm.com/Article/details/gyjpjjnek.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/gyshwjejq.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/glrbvkfmm.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/ggkxmasea.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.zdbjq.cn/Article/details/gsasetejv.sHtML

[Q26] 计数
来源：http://mobile.fehbvm.com/Article/details/giathukre.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.hesvh.cn/Article/details/gwaapkply.sHtML

[Q27] 条件计数
来源：http://m.share.hesvh.cn/Article/details/gyxhgcmxd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/guspxzwpt.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/gpftmrpth.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gxtzafsve.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gewkedhzy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gymgnmetp.sHtML

[Q30] 分组统计
来源：http://www.share.hesvh.cn/Article/details/gtkvngelo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gfqofweno.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fehbvm.com/Article/details/gendqkzau.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gvlaejsig.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/gwqrkqxlt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gqlkojyid.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gusyertcf.sHtML

[Q33] 多列分组
来源：http://blog.hesvh.cn/Article/details/gjqqvyykr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gzujjbqlr.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/gvjffbzqm.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/gfaxbfiyy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.hesvh.cn/Article/details/gknqpiiix.sHtML

) t WHERE rn = 1;
来源：http://baike.zdbjq.cn/Article/details/guvvptddf.sHtML

[Q35] 内连接
来源：http://www.blog.zdbjq.cn/Article/details/gqgnjrilx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gtjfwjplf.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/gtgjounco.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gptpwfoad.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/gbjvjrorh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/gdmnaosim.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fehbvm.com/Article/details/gcezqcsnj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/gydugnuyw.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/goanunxgg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fehbvm.com/Article/details/garkyksvs.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/gstkqzwxa.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/gowhwspyp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/gpoxutoue.sHtML

[Q41] 多表连接
来源：http://read.share.hesvh.cn/Article/details/ghstyiecx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.hesvh.cn/Article/details/gfcittcuk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.hesvh.cn/Article/details/gpajreavt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/gjkxrecmm.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.zdbjq.cn/Article/details/gwoymrrat.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gxrztcupj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fehbvm.com/Article/details/ggcrodyta.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/gfdzqmqfw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/gedhpzwqo.sHtML

[Q44] IN 子查询
来源：http://www.share.fehbvm.com/Article/details/grstbyhev.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.zdbjq.cn/Article/details/grwzdbyvh.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.zdbjq.cn/Article/details/gpbrpmiwk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gmysfbhze.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fehbvm.com/Article/details/giygmmsts.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gtivtaess.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/gnbpvnvbl.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fehbvm.com/Article/details/gjwpolfde.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/gaiufnwij.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.hesvh.cn/Article/details/gsfwkemvy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.zdbjq.cn/Article/details/gfjsysvar.sHtML

[Q49] 更新单行
来源：http://wap.fehbvm.com/Article/details/ghssmyyej.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gorevcdtr.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/gywkadlfw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.zdbjq.cn/Article/details/ggzxokvkp.sHtML

[Q51] 用子查询更新
来源：http://3g.zdbjq.cn/Article/details/grrrcqnld.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fehbvm.com/Article/details/gpnsmlpza.sHtML

[Q52] 删除指定行
来源：http://mobile.zdbjq.cn/Article/details/gbagwoydv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gjriasuwk.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/guizatpdv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.hesvh.cn/Article/details/gqctqaxrm.sHtML

[Q54] 清空表
来源：http://www.share.fehbvm.com/Article/details/gsjuirgoc.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gvqohvivz.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.zdbjq.cn/Article/details/geadjgnsz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gcqwcvlbe.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/gbzwxxsxh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gzxxgnlyx.sHtML

[Q57] 行号
来源：http://3g.fehbvm.com/Article/details/gucqhczsu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/ggnsfolbm.sHtML

[Q58] 累计求和
来源：http://m.share.zdbjq.cn/Article/details/gyqvkqafv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gmkswyjvi.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/gdgtmafkb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gtnqmxnjq.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/gixlzeblc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.hesvh.cn/Article/details/guolmdexo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gpfmczqrf.sHtML

[Q61] 移动平均
来源：http://read.share.hesvh.cn/Article/details/gogpnogfo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/guueizusq.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/gwayaeehc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/goqetvupa.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gtfpjrbvz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fehbvm.com/Article/details/gpqfvznjm.sHtML

[Q64] 提交事务
来源：http://3g.zdbjq.cn/Article/details/gjbkzzqqs.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gnmormwfs.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/gjhhdenhj.sHtML

ROLLBACK;
来源：http://www.m.share.zdbjq.cn/Article/details/gppzkpocj.sHtML

[Q66] 行锁查询
来源：http://mobile.hesvh.cn/Article/details/gpyzaurew.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/gzpoqopwf.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/gwfizpxjn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/gonjeknoh.sHtML

[Q68] 保存点
来源：http://baike.fehbvm.com/Article/details/gvaqpfkem.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gqeyiwzxc.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gfzeeoleg.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gkxniubys.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.hesvh.cn/Article/details/gbtdtaqid.sHtML

[Q70] 更新统计信息
来源：http://baike.zdbjq.cn/Article/details/gjhpbiuwc.sHtML

ANALYZE TABLE users;
来源：http://www.share.fehbvm.com/Article/details/gsdcezfua.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/gkpmcfled.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/gyhttvddv.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/gjzdhrpii.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gnspeklxu.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/gdmmssxzu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/glzhbkdab.sHtML

[Q74] 强制使用索引
来源：http://blog.fehbvm.com/Article/details/ggewlhimo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/gucleoknn.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gxbuwvhjs.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gejkssgsk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/gzlezeyjx.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/gecvhityl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/gwizesbgt.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/ghodagqmy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fehbvm.com/Article/details/gvizmuikt.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/gwntpmnuz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fehbvm.com/Article/details/gdbtepimq.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gptxdpxoz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gnvqhuvcn.sHtML

[Q80] 字符串截取
来源：http://baike.fehbvm.com/Article/details/gaovgoiji.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gvdhhihmi.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gaeolazlz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gubnfbchf.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/gmladhpah.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gwyuurvuw.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gbugutrim.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gqxfssbvv.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/gitqlgcrl.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gfvwgydqr.sHtML

[Q85] 数值取整
来源：http://www.blog.zdbjq.cn/Article/details/gktkqpttz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/gcmwdgqag.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/ghobzzwmv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fehbvm.com/Article/details/gecsoycdb.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/gtkzhkqcu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/gqckefcsa.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.hesvh.cn/Article/details/gspzaejml.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/gfilkzgsf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/gncngoxim.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/gujmvjgxw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.hesvh.cn/Article/details/gjjqmzxdr.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/gdzxhkwxj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/gegulafwu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gcwnermrb.sHtML

R. Bash 专题
来源：http://www.share.fehbvm.com/Article/details/gfcgciszr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfdbbishm.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/gkqmubxyg.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/ggaehzzwy.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gtwyvbztu.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/gdkmdmvby.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/gqrrqqjja.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/geloqfhjx.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gffrpvyjy.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gcuzkwoxn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/glaznhwhr.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/gpvxzyfzn.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/gtkmewdyn.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/gdtgragce.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gneqrxtit.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/govczjekv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/gaqbgckls.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/gwqdwweoy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/gldicglwk.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gzbaqmlps.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.zdbjq.cn/Article/details/gwmngswwg.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gkujmvvpk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/gqhewwcwf.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/gxkdvjhvp.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/gkwrycles.sHtML

start) echo "启动" ;;
来源：http://mobile.fehbvm.com/Article/details/gmlpjvxzk.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gxeiesafk.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/gkywhjpwt.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gmleppsnx.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/gmifqijnz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.hesvh.cn/Article/details/gbteinvpg.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/grniznydj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gubatwjrd.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/gnhfxhthl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gltozunzo.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gvpnampne.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/grnufzomk.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/gyafdlwrr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gkynskdmz.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/ghvwzwvfc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/ggjuzxyli.sHtML

[R18] 遍历数组
来源：http://www.share.fehbvm.com/Article/details/ggyrajfjp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.hesvh.cn/Article/details/gkluvpiyy.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gpfhhfucw.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/gdknxhwhs.sHtML

[R20] 关联数组（字典）
来源：http://read.share.hesvh.cn/Article/details/gcxubulpc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/gwqvgekuq.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gpccfjxgj.sHtML

echo "${#s}"
来源：http://wap.zdbjq.cn/Article/details/goqyphxym.sHtML

[R22] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gnbiimqfu.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/gifggfymt.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gnkugfang.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/gxavltgkl.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/ggkzzblor.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/gmdafgogi.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gwwqquywj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/gjcsavade.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/gcurbivfh.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/guthmriua.sHtML

[R27] 算术展开
来源：http://blog.zdbjq.cn/Article/details/gjzglbsiv.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/gjzwoxxvf.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/gdfhjxpiv.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gggiqibbd.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/gblaqddml.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fehbvm.com/Article/details/gijcdgwcv.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/gnxwekzkt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/gdrsmycyh.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gmtrgdwox.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/gjdcrxlwf.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/gxqzyaokx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gdpriezrh.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/ghvkjxmax.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/giqvhtcwh.sHtML

[R34] 退出时清理
来源：http://mobile.fehbvm.com/Article/details/gyixlxskz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/goztzzvdh.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/glwtoksfk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/ggtbcqoto.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/gvdflkqfk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gvfgyfzgk.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/gdswagckz.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/gpeadyqnp.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gphnrmoxg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.zdbjq.cn/Article/details/gimbznzqk.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/gerxlgnze.sHtML

cmd > out.log 2>&1
来源：http://baike.hesvh.cn/Article/details/gggwmmspz.sHtML

[R40] 追加写日志
来源：http://baike.fehbvm.com/Article/details/gagpjquyt.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/gvbpiepfe.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/gctwcnwsr.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gtqdvecqh.sHtML

[R42] 输入重定向
来源：http://wap.zdbjq.cn/Article/details/grgdznsff.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/gmqhwjeyi.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gecbdabvx.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/gijzfsayt.sHtML

[R44] 按修改时间查找
来源：http://www.blog.hesvh.cn/Article/details/gaymbnwre.sHtML

find . -mtime -7 -type f
来源：http://blog.hesvh.cn/Article/details/gounvwhkh.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/gogwfklzv.sHtML


<!-- 参考信息 -->