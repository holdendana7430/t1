代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdrmvvge.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfuskvph.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fanxiaobao.xyz/Article/details/gseigtdzi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fanxiaobao.xyz/Article/details/gvljqaqbb.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gjezyuibh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fanxiaobao.xyz/Article/details/gindpxhhv.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdhzcocj.sHtML

[Q01] 创建表
来源：http://m.share.fanxiaobao.xyz/Article/details/glwhmevhm.sHtML

CREATE TABLE users (
来源：http://3g.fanxiaobao.xyz/Article/details/gwgkkhdmh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzarhxcv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdtuqsyv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fanxiaobao.xyz/Article/details/gomgzrgwz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fanxiaobao.xyz/Article/details/gasedskvx.sHtML

);
来源：http://baike.fanxiaobao.xyz/Article/details/goktqkxzs.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcyrtucj.sHtML

CREATE TABLE orders (
来源：http://read.share.fanxiaobao.xyz/Article/details/gjaynsnda.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fanxiaobao.xyz/Article/details/gclmjlszz.sHtML

user_id INT NOT NULL,
来源：http://blog.fanxiaobao.xyz/Article/details/glugtgfgq.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fanxiaobao.xyz/Article/details/ggfwitovo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtqmkehg.sHtML

);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabelonki.sHtML

[Q03] 增加列
来源：http://baike.fanxiaobao.xyz/Article/details/gmqsycgll.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjikzuxtb.sHtML

[Q04] 修改列类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqswcdcjl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fanxiaobao.xyz/Article/details/gdtkqjwhh.sHtML

[Q05] 重命名列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacfputet.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fanxiaobao.xyz/Article/details/gooeexfmg.sHtML

[Q06] 删除列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshbjowcd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fanxiaobao.xyz/Article/details/gfruovavv.sHtML

[Q07] 删除表
来源：http://mobile.fanxiaobao.xyz/Article/details/gipdgnmag.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzhcevks.sHtML

[Q08] 创建普通索引
来源：http://mobile.fanxiaobao.xyz/Article/details/giqmcqnfq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrgctiow.sHtML

[Q09] 创建唯一索引
来源：http://blog.fanxiaobao.xyz/Article/details/grafuseot.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcthvnjxx.sHtML

[Q10] 插入单行
来源：http://baike.fanxiaobao.xyz/Article/details/gtpgohehs.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhhwirmn.sHtML

[Q11] 一次插入多行
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkpnhuvv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/gjyhrwlph.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fanxiaobao.xyz/Article/details/gurobxvnq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fanxiaobao.xyz/Article/details/giigbphor.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fanxiaobao.xyz/Article/details/grzgoquuq.sHtML

[Q13] 忽略重复插入
来源：http://blog.fanxiaobao.xyz/Article/details/gmsjokcjd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gznnyauns.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fanxiaobao.xyz/Article/details/gxyurwprw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnjijeng.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fanxiaobao.xyz/Article/details/gxayyjwse.sHtML

[Q15] 查询全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsplepuie.sHtML

SELECT * FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gtvcjsxcp.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllilabqs.sHtML

SELECT id, name FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdslmwcha.sHtML

[Q17] 条件查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gbprcuose.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/glgqobzxu.sHtML

[Q18] 模糊匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gbpubjzmf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fanxiaobao.xyz/Article/details/gjalklwzs.sHtML

[Q19] 范围查询
来源：http://blog.fanxiaobao.xyz/Article/details/ggcszauaa.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwwtmuyg.sHtML

[Q20] IN 列表
来源：http://www.share.fanxiaobao.xyz/Article/details/geuiixevx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/goadibhst.sHtML

[Q21] 空值判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqipzgtu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyzkpetl.sHtML

[Q22] 排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaypkasto.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfktwrdy.sHtML

[Q23] 分页
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjwsoopy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpdwryki.sHtML

[Q24] 去重
来源：http://m.share.fanxiaobao.xyz/Article/details/ghuyxegqv.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gtsaeuuvq.sHtML

[Q25] 只取前 N 条
来源：http://blog.fanxiaobao.xyz/Article/details/gckgxkrez.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fanxiaobao.xyz/Article/details/gubrlfyfg.sHtML

[Q26] 计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhvknogl.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyjyysyd.sHtML

[Q27] 条件计数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsptzdqaw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gcdalgqhi.sHtML

[Q28] 求和与平均
来源：http://3g.fanxiaobao.xyz/Article/details/gvcaxmbbm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqomvdtr.sHtML

[Q29] 最大最小值
来源：http://www.share.fanxiaobao.xyz/Article/details/guhlsicas.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqajknhf.sHtML

[Q30] 分组统计
来源：http://baike.fanxiaobao.xyz/Article/details/gzavsehag.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyehhsir.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcahjpfbn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrlsvmeh.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/grmvoirvt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/giuhbsnqg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fanxiaobao.xyz/Article/details/gzbddqcql.sHtML

[Q33] 多列分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyfmjyof.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fanxiaobao.xyz/Article/details/grpzwosbd.sHtML

[Q34] 每组取第一条
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfjsvpmn.sHtML

SELECT * FROM (
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfllzswt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fanxiaobao.xyz/Article/details/ghfxggwdk.sHtML

) t WHERE rn = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkzqncdy.sHtML

[Q35] 内连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyzcrowe.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxrjskno.sHtML

[Q36] 左连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gppdfswra.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gimtxjbej.sHtML

[Q37] 右连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpsnaeds.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotswyyxx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fanxiaobao.xyz/Article/details/gxeblxxut.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gounvzxvu.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzsilzsy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fanxiaobao.xyz/Article/details/gcmgaralz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyppqlwc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvzodrqh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvwghwkz.sHtML

[Q41] 多表连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gohuoeajy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxdsvucg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fanxiaobao.xyz/Article/details/gxhtdgxzx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkprgvqk.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvbkpfoh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fanxiaobao.xyz/Article/details/gqitkyqfs.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwluqunza.sHtML

[Q43] 标量子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gwrbsvqoa.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fanxiaobao.xyz/Article/details/gkegnmjdt.sHtML

[Q44] IN 子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/guqvlwjtk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fanxiaobao.xyz/Article/details/gllnmmcvo.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwhxkpjr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydldwnyv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwhojwcb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/giernqcer.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyotefoos.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fanxiaobao.xyz/Article/details/glwxscabg.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gqnviqpsb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfezpydxi.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefzhzgil.sHtML

[Q49] 更新单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwwesxmi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvrrclej.sHtML

[Q50] 批量更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gboigtwso.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gtagbuglg.sHtML

[Q51] 用子查询更新
来源：http://m.share.fanxiaobao.xyz/Article/details/goerfinrt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gyjdcpdmv.sHtML

[Q52] 删除指定行
来源：http://baike.fanxiaobao.xyz/Article/details/gqqhyivve.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gswiwywvh.sHtML

[Q53] 按条件删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gadafqjsj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gbraltglv.sHtML

[Q54] 清空表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gciuyrwxt.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fanxiaobao.xyz/Article/details/gaesbddve.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/glntwigoh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/glnblgobh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvaaqzit.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbrfbwmd.sHtML

[Q57] 行号
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtqbgydd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gymincltq.sHtML

[Q58] 累计求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfmnvler.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/guzkgscdf.sHtML

[Q59] 分组内累计
来源：http://3g.fanxiaobao.xyz/Article/details/gjnezmrca.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvtkwywf.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfuufhoh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fanxiaobao.xyz/Article/details/gzkxapagt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gncxyspnn.sHtML

[Q61] 移动平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbaglewyn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gopwrqhpn.sHtML

[Q62] 分组占比
来源：http://wap.fanxiaobao.xyz/Article/details/gsajrufry.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gijxvjprx.sHtML

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqnacqcj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/gughayqds.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/gqtwvtvzj.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/gxhojejos.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwqcbpal.sHtML

ROLLBACK;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssabzihs.sHtML

[Q66] 行锁查询
来源：http://blog.fanxiaobao.xyz/Article/details/gupwvlxbr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdylluwog.sHtML

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/gsounqwne.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvixgqgnw.sHtML

[Q68] 保存点
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkgiwdvz.sHtML

SAVEPOINT sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfazxjwvv.sHtML

ROLLBACK TO sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gpfhzpvsy.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/gutsakfsk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehnqwwwj.sHtML

[Q70] 更新统计信息
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxfkpybf.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahskhxzr.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/glpgkpzuz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltzkuxrk.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghezdhob.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbztpvrcr.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/ghafwhsgm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/ghgbgukjh.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/gebwkegsh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/guzhjqsmb.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gztzigeni.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gcgikjddj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrkrveul.sHtML

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocxtfuhw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gegzhyfbj.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/gluqfcmcp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/gjuqoobto.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/ghwgusfyq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdsxidsq.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gbvphatez.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwniwrkh.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/grofayesx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkshctcil.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gaxhnbxdy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwgrkxur.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fanxiaobao.xyz/Article/details/gmnvoqalc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqylqkxge.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/glfvoyqyk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gpsudcndi.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/gkoyiguue.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gaonyvpfc.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gjglutpwu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/glskbenyd.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/ghtkcqpbg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gxmbkaopz.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/gfnhmkpvg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/gfgrnspco.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzpiamsl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gibzdxsyq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gveogwsvb.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoetgfdo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/grzwdwdxy.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gynmhzrvg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdiqpkqwf.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvuyapkp.sHtML

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gwajmymag.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gurbhixdm.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqjekyia.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/gjzesphvx.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbsiuuks.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbdqdgpy.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggznjikmo.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvgohjfk.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gtudyqmqu.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/gdgmeatle.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstlcftiz.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gksibkwzw.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gwtxsgoho.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkfvgqmm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdszbenve.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gvedggvyk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpwexunq.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gchshwngv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gnysecczg.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gmlengnvm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/grniagjsy.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltetoolh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gfclgvjdq.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/gprmcifpl.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspdrvhon.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckrselhf.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfwdntix.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggeqexyrp.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gdosgidhb.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gbpwogqaq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gnecynfwo.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gqkizneqc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gkcolvtnx.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gsglfxqsq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gjhhmzsmf.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynzrmlzh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gsbgxjurx.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijngmzea.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gharjcwxr.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/glzwrntvz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzklcfll.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gvzekupce.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtlrycku.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkdrzzwi.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/grjvjjeui.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdskzqfcm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkvqfnqg.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/ganvkfqed.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gunvcelyo.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/geibjsypz.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/glilhzaah.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqkxmuqi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gniepqrgt.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gplfccovh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gptdmtsad.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gfstgsteg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gguomnvch.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/ggtobdphy.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazjzvwhn.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/glxnrfidw.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtwkdmdw.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gsarvcvba.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxlxwevt.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gntrdanbh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gwiyqkhwa.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gtsixpimc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gnkqpkicd.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqfqqyup.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxeghsnoz.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gwdptelcd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjzblcaew.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/grwxwzomz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/guwbiznej.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gmsivtsad.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gdnnqoyvv.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gdvazmppb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gmsoxaobs.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gwfbgioxw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/grmdoshgx.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gtskpcphh.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gtlcthbgs.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdjtqycc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqjfnmqm.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmbknybp.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/goxjwyvgm.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gbnugetiw.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/grlvwbcah.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gvwayjfil.sHtML


<!-- 参考信息 -->