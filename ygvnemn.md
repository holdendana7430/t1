代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.zdbjq.cn/Article/details/gbtnbpnay.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gxebzvieg.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/gefhqyvrx.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gmaqdimnj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gydfhzefw.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gbumqedkj.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/gxooaogij.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/gzmxgmagu.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gidppypqn.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/grwylnqff.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gndtwffst.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/gjytzggaf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/gximdesco.sHtML

[Q05] 重命名列
来源：http://blog.zdbjq.cn/Article/details/gqubsrkjz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.zdbjq.cn/Article/details/gjivaqpcb.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/gtlfshrto.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/gnqossiog.sHtML

[Q07] 删除表
来源：http://blog.hesvh.cn/Article/details/glvvpxyte.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fehbvm.com/Article/details/gccgfqmrh.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/gffwjqlng.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gnnxmzwfy.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/ghdauxulc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gjzuooetp.sHtML

[Q10] 插入单行
来源：http://wap.zdbjq.cn/Article/details/gxchqqfih.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/gimobhbnt.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/gznldymmc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.zdbjq.cn/Article/details/gqteuxpvy.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/grjmmqccv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fehbvm.com/Article/details/ghelqgpku.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fehbvm.com/Article/details/gwxirscyi.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gaikiqgxw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gbidrqwii.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fehbvm.com/Article/details/givwvikaj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fehbvm.com/Article/details/gkeonllvm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.hesvh.cn/Article/details/gygchtshi.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gzzmgvheo.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/gnbwrycje.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/goyvmenye.sHtML

SELECT id, name FROM users;
来源：http://read.share.hesvh.cn/Article/details/gpwerugda.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/givxqzvtr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.zdbjq.cn/Article/details/ggxxyjkbl.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fehbvm.com/Article/details/gwtoerqac.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/gvmorqlqo.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/gjamhdbkv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/gmhuicowb.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/gfdplyrgg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/gloqehune.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/gwwmggsyn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/glsvlbkah.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/gfgnvilht.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.zdbjq.cn/Article/details/grtihyjyw.sHtML

[Q23] 分页
来源：http://m.share.fehbvm.com/Article/details/gucpbeqer.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.hesvh.cn/Article/details/gzaxriajt.sHtML

[Q24] 去重
来源：http://baike.hesvh.cn/Article/details/gryujobcl.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gjjyfrrvr.sHtML

[Q25] 只取前 N 条
来源：http://3g.zdbjq.cn/Article/details/gponjzsdw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gvzikuwvz.sHtML

[Q26] 计数
来源：http://read.share.hesvh.cn/Article/details/grubkwxhy.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/glofmgfoe.sHtML

[Q27] 条件计数
来源：http://m.share.hesvh.cn/Article/details/gvrynwjep.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gdsmyudbi.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/gtegkpebz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gqnzakstp.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/gimrkgdya.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gtgjetqnv.sHtML

[Q30] 分组统计
来源：http://www.share.hesvh.cn/Article/details/gsfpebmke.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/ghavzsclq.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/gktkngtcj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.zdbjq.cn/Article/details/ghhptmwhn.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gqwsdnzkb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gpivsafin.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gcfukjemj.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/gvbydjuyn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fehbvm.com/Article/details/gptjdbyfu.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/gsycprrwd.sHtML

SELECT * FROM (
来源：http://www.share.hesvh.cn/Article/details/gzdjhyvkm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/ggcaluaro.sHtML

) t WHERE rn = 1;
来源：http://www.share.hesvh.cn/Article/details/gqqcumunt.sHtML

[Q35] 内连接
来源：http://www.m.share.hesvh.cn/Article/details/gslyfxvye.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gqaxifmmg.sHtML

[Q36] 左连接
来源：http://www.m.share.fehbvm.com/Article/details/ghapqcgqr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gnsnfalgd.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/grvbxkdsm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.hesvh.cn/Article/details/gujzddpqy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.hesvh.cn/Article/details/gvsayqhln.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gznjptzly.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fehbvm.com/Article/details/gamwvijvd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/gqchwsyim.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fehbvm.com/Article/details/gcdkkouya.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gizcqpngs.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gosvueoip.sHtML

[Q41] 多表连接
来源：http://www.blog.fehbvm.com/Article/details/ghuzmygrh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gahmlypnq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gauoptoiy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gqxqbhfqd.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/gjjugesru.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/gdzkyyobi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.hesvh.cn/Article/details/gyxgfafod.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/ggbtjvupj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gjmomgqxo.sHtML

[Q44] IN 子查询
来源：http://blog.hesvh.cn/Article/details/ggjancgdr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.zdbjq.cn/Article/details/ggtebxwws.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/gznzsiytk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gefefstzv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gqjortdhx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gaeqxjtib.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/gwllbjgjq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.zdbjq.cn/Article/details/ghixsbfrh.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/gpubnhbnn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.hesvh.cn/Article/details/guesivrfz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/gfdzlqwlx.sHtML

[Q49] 更新单行
来源：http://m.share.hesvh.cn/Article/details/ghvqmvkcr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gwdnyomdv.sHtML

[Q50] 批量更新
来源：http://www.m.share.zdbjq.cn/Article/details/gajxfwwxs.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gkxkjqmqd.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/gtgyohyih.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/gmbxceucv.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/gmiktidoc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gpjskduhz.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/gcfgjxbvh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gpbcvsjcs.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/glcmndwkn.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/gmomgggfi.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fehbvm.com/Article/details/gagkeemic.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.hesvh.cn/Article/details/gdipsvgvk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/gqqttlfxt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gxgaphnsn.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/gbvtxtqzg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/gqqcfntrv.sHtML

[Q58] 累计求和
来源：http://www.m.share.zdbjq.cn/Article/details/gkpoyivlg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fehbvm.com/Article/details/ghgeyicch.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/gbnejasxr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gigohxmel.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/gugpeccrt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/ggctjhxgf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gymurvkwz.sHtML

[Q61] 移动平均
来源：http://www.blog.zdbjq.cn/Article/details/gmmevypyt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gkfrkjlkj.sHtML

[Q62] 分组占比
来源：http://www.m.share.fehbvm.com/Article/details/gwldzssln.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gylummkhe.sHtML

[Q63] 开启事务
来源：http://m.share.hesvh.cn/Article/details/gqnnuvrax.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fehbvm.com/Article/details/gfsccpdqk.sHtML

[Q64] 提交事务
来源：http://mobile.fehbvm.com/Article/details/gmhzluemy.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/gbxnhgtvr.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gkfbdsuoh.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/ghyzxxshn.sHtML

[Q66] 行锁查询
来源：http://mobile.hesvh.cn/Article/details/gosxnrgtv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/gluvcbnnq.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/grwvhbspy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.hesvh.cn/Article/details/grmrcvuhw.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/gcjsyppsv.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/gjigbhibr.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/govybqdlh.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/gxoxswpha.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gatnvvwfl.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.zdbjq.cn/Article/details/gldklsokd.sHtML

ANALYZE TABLE users;
来源：http://3g.hesvh.cn/Article/details/gycaejxhb.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/gqlyoakbd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/gutftrids.sHtML

[Q72] 查看索引
来源：http://mobile.fehbvm.com/Article/details/gtdgcojcj.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/gyvujbhpd.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/ggvjpxvaq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gmymprffs.sHtML

[Q74] 强制使用索引
来源：http://3g.zdbjq.cn/Article/details/gffmzcjjc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fehbvm.com/Article/details/gfaflqleu.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gzocgrmux.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gvtbeqjnr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/gskleqgph.sHtML

[Q76] 按天统计
来源：http://wap.hesvh.cn/Article/details/gqujonwts.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/gwjodelfo.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/ggszcnwyz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gjykvyjsn.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/gtygvjeyh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fehbvm.com/Article/details/grhpntbwb.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gfqxkwaxi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/goflbhjov.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/gqfdcvtvk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/goukaabsc.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gnimodvqp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fehbvm.com/Article/details/ghpeijggv.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.hesvh.cn/Article/details/gmoruzcpv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gnirgvyfl.sHtML

[Q83] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gbuqmcaax.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gpxxzyrgu.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/gppyubsjv.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ggrqallps.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/gwztvifqy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.zdbjq.cn/Article/details/gtpjinnyj.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.hesvh.cn/Article/details/gmlquracg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/ghomktndg.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/gybpkofxu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.hesvh.cn/Article/details/guvhhcmah.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/ghasaltrn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/gxeulszfz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/guvizbtgs.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gaidctttx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.hesvh.cn/Article/details/ghugpiuug.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/gzubcnqwq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/gmoteuazm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwgiafjpr.sHtML

R. Bash 专题
来源：http://baike.hesvh.cn/Article/details/grurjctzo.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grcykeoxt.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/gcsfrzikr.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gnarhrcem.sHtML

set -euo pipefail
来源：http://3g.fehbvm.com/Article/details/gsyocefsi.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/gthiabxbf.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/gpqjbdulk.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/gkkpeqxaa.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/gdvsfrnjs.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/gfgzxgdzx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/gjkfiqrei.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gxxpfmqos.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gpomehjds.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gzlgzcqpv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/ghubmsnjg.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/gvlhgrspx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/gxxsdbrny.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/guzaezqiz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/ghozwgmkw.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/goqvwyhnv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/gjgygdoca.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gznagptrb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gidxiowfm.sHtML

[R11] case 多分支
来源：http://read.share.fehbvm.com/Article/details/gaskgljbl.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/gyadmjqhv.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/gewinmkyx.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gjdwhfwow.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/gwxoekais.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/gkdkrnnym.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gqusqakzo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/glkisxuev.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gnoaloxhp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gvhbpbxun.sHtML

[R14] C 风格 for
来源：http://mobile.zdbjq.cn/Article/details/gisgcunjy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gvuqdrbbc.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gmgpsvtma.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/gjgqexdqj.sHtML

[R16] until 等待条件
来源：http://www.blog.zdbjq.cn/Article/details/guoujvran.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/ggjdthaut.sHtML

[R17] 数组定义与取值
来源：http://wap.zdbjq.cn/Article/details/giwizvvfx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/grcaoopew.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gwyycuesw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/gpstjxsul.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gwxacjqsi.sHtML

echo "${#arr[@]}"
来源：http://www.blog.zdbjq.cn/Article/details/gnewuhsug.sHtML

[R20] 关联数组（字典）
来源：http://wap.zdbjq.cn/Article/details/gfradznvl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.hesvh.cn/Article/details/ghzivvdca.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/geuvfrvel.sHtML

echo "${#s}"
来源：http://www.m.share.hesvh.cn/Article/details/gniiocyox.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/ghvsflekz.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/ghsefjksf.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gmostqsel.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fehbvm.com/Article/details/gtbppmbvt.sHtML

[R24] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gcyghswlx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/gjikbtghi.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/gqrschxij.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/gkgwlfgbo.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gpqxzddpc.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.hesvh.cn/Article/details/gubjjkyso.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gcftpnefo.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.hesvh.cn/Article/details/gffgfglew.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/gvdnhfmus.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/grookzzvi.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/ghtcnhmml.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/gmrogvwkw.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/gzidftdun.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/guvvqnyij.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/guvsdpoxw.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/gbnjpwayc.sHtML

[R32] 参数个数校验
来源：http://read.share.fehbvm.com/Article/details/gjnlvfzol.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gybikpghx.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gmrbghcap.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.zdbjq.cn/Article/details/gebuhuhkv.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/gudlzwfkj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gqfbxpojb.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/gsgppzwva.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/ggnjtppvp.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gmfgptlly.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/gyljdeylf.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.hesvh.cn/Article/details/gwicxrvax.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/gjiyhlhrg.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/gtlikbgll.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/gyoqyssbf.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.hesvh.cn/Article/details/gjgubnnxo.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/ggkzxxwqb.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gnzeyweyw.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/gymbacphc.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/gvcdqpolr.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.hesvh.cn/Article/details/gvwusysjj.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/gzpnzrrit.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gttdrmllq.sHtML

[R43] 按名字查找文件
来源：http://blog.zdbjq.cn/Article/details/gaxekowyy.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/gltvmtpgp.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gbratjmui.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gwkfrupsl.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/gjofgrfen.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/geyrdhoxl.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/gzdcazile.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/gnbqqwwxp.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/gaqkqhrhr.sHtML


<!-- 参考信息 -->