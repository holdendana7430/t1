代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fanxiaobao.xyz/Article/details/ghysikbdj.sHtML

);
来源：http://baike.fanxiaobao.xyz/Article/details/gqrmbasiu.sHtML

[Q02] 创建带外键的表
来源：http://blog.fanxiaobao.xyz/Article/details/ghqvpxkth.sHtML

CREATE TABLE orders (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyodejjmt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkqnihvy.sHtML

user_id INT NOT NULL,
来源：http://www.share.fanxiaobao.xyz/Article/details/gsduwbtrg.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fanxiaobao.xyz/Article/details/gxponxjko.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fanxiaobao.xyz/Article/details/gucezpcgk.sHtML

);
来源：http://3g.fanxiaobao.xyz/Article/details/grbuvrlnn.sHtML

[Q03] 增加列
来源：http://blog.fanxiaobao.xyz/Article/details/grqeivxet.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkapxsmqn.sHtML

[Q04] 修改列类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gqluiosaw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqwksryn.sHtML

[Q05] 重命名列
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwdvhuth.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fanxiaobao.xyz/Article/details/gknrhgkcw.sHtML

[Q06] 删除列
来源：http://read.share.fanxiaobao.xyz/Article/details/geqysoqpl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcboftudk.sHtML

[Q07] 删除表
来源：http://mobile.fanxiaobao.xyz/Article/details/gyziabcze.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrjwmptl.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdgfxggk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fanxiaobao.xyz/Article/details/gfharuhqo.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fanxiaobao.xyz/Article/details/ggocfcnkc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fanxiaobao.xyz/Article/details/gtiurgrax.sHtML

[Q10] 插入单行
来源：http://baike.fanxiaobao.xyz/Article/details/gcxmyzryf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/gremgekcl.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjzoeenh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/ghnhkppnc.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fanxiaobao.xyz/Article/details/galzxhmlu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fanxiaobao.xyz/Article/details/gnlvemnfq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fanxiaobao.xyz/Article/details/gqzkwdpex.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqvbxbvo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyogvhqzn.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fanxiaobao.xyz/Article/details/guvvfammc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyzubeyq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlwmfdia.sHtML

[Q15] 查询全部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxiravcah.sHtML

SELECT * FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpdpffpm.sHtML

[Q16] 查询指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gnnsdwrzb.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcphblpon.sHtML

[Q17] 条件查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gliflwzsq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/ggfmqiobd.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqccgkfgs.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fanxiaobao.xyz/Article/details/gkhsgnlzb.sHtML

[Q19] 范围查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzwekbgh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvgqdqsq.sHtML

[Q20] IN 列表
来源：http://baike.fanxiaobao.xyz/Article/details/gsngllmaf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fanxiaobao.xyz/Article/details/glpzqjrvb.sHtML

[Q21] 空值判断
来源：http://3g.fanxiaobao.xyz/Article/details/gpajlryih.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghergslgc.sHtML

[Q22] 排序
来源：http://wap.fanxiaobao.xyz/Article/details/gqcwrqnpl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhthmjhe.sHtML

[Q23] 分页
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjncfecn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxncqyyh.sHtML

[Q24] 去重
来源：http://read.share.fanxiaobao.xyz/Article/details/gkatvhqxp.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gpaelzsvm.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvwlphzl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fanxiaobao.xyz/Article/details/gcbykeuxk.sHtML

[Q26] 计数
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyfaegii.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/giqlekrlf.sHtML

[Q27] 条件计数
来源：http://www.share.fanxiaobao.xyz/Article/details/gsczodiir.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gocypbbvi.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsouwlzzq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvukkfkm.sHtML

[Q29] 最大最小值
来源：http://blog.fanxiaobao.xyz/Article/details/gnxopyaed.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gtgvoeucl.sHtML

[Q30] 分组统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gncpxpvuw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqtlkytu.sHtML

[Q31] 分组后过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gsosmgoay.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gpvrezvsb.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyrwghgc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gzjrrcbjw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fanxiaobao.xyz/Article/details/gflyshftm.sHtML

[Q33] 多列分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpvjhfkz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fanxiaobao.xyz/Article/details/gijhezyet.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfcovuea.sHtML

SELECT * FROM (
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxvqlnkf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fanxiaobao.xyz/Article/details/grxzsskop.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkjrebpm.sHtML

[Q35] 内连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwivdiws.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorcslbgc.sHtML

[Q36] 左连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdxcjftn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfagxxbu.sHtML

[Q37] 右连接
来源：http://blog.fanxiaobao.xyz/Article/details/gvlqwwlga.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdwbnhvd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhqupmhw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gorxcsyhu.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fanxiaobao.xyz/Article/details/glastzcao.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fanxiaobao.xyz/Article/details/glrneahqe.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpteftkxe.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fanxiaobao.xyz/Article/details/gsyczequo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fanxiaobao.xyz/Article/details/gfjpceetr.sHtML

[Q41] 多表连接
来源：http://blog.fanxiaobao.xyz/Article/details/golrzyeaq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fanxiaobao.xyz/Article/details/gosfpcuox.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbepzlmzq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnswnhhqd.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjbnixpr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fanxiaobao.xyz/Article/details/gigutkfae.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gsejlldjl.sHtML

[Q43] 标量子查询
来源：http://wap.fanxiaobao.xyz/Article/details/grquaiydo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvrqiwbw.sHtML

[Q44] IN 子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gpujcoeov.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwmqfjny.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fanxiaobao.xyz/Article/details/gdgubswfw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqrvljyx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbkhgjra.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkndcyohe.sHtML

[Q47] 与平均值比较
来源：http://baike.fanxiaobao.xyz/Article/details/glfdzgesn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fanxiaobao.xyz/Article/details/guorsscrz.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gcxekkuxg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fanxiaobao.xyz/Article/details/gewshovte.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gqkwmmumz.sHtML

[Q49] 更新单行
来源：http://blog.fanxiaobao.xyz/Article/details/gfptuggiq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcskvjhnk.sHtML

[Q50] 批量更新
来源：http://blog.fanxiaobao.xyz/Article/details/govddaywl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbvcsucj.sHtML

[Q51] 用子查询更新
来源：http://wap.fanxiaobao.xyz/Article/details/gqnanwiae.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmncwxysp.sHtML

[Q52] 删除指定行
来源：http://baike.fanxiaobao.xyz/Article/details/gfwlygibl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbwuewkr.sHtML

[Q53] 按条件删除
来源：http://3g.fanxiaobao.xyz/Article/details/gppbwxcib.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/giglezsrw.sHtML

[Q54] 清空表
来源：http://3g.fanxiaobao.xyz/Article/details/gaztjnjhn.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fanxiaobao.xyz/Article/details/giqfroetq.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjesdizw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gqorzyffk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhgzfpsg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gvfgtaife.sHtML

[Q57] 行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gdesyecjf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gbjdcugws.sHtML

[Q58] 累计求和
来源：http://3g.fanxiaobao.xyz/Article/details/gprkqzrwq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwamsacws.sHtML

[Q59] 分组内累计
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbwwbgod.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/glxafpybv.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtcwqxyg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnbhplff.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gqrpbvzzb.sHtML

[Q61] 移动平均
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfneyyks.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/ghbaygpcm.sHtML

[Q62] 分组占比
来源：http://blog.fanxiaobao.xyz/Article/details/gbasjgtic.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gfwcsmwvt.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/geiesjlii.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjhzjkbj.sHtML

[Q64] 提交事务
来源：http://baike.fanxiaobao.xyz/Article/details/gkjtdrbzg.sHtML

COMMIT;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtigmyqhg.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/guercmqjw.sHtML

ROLLBACK;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrdrecmm.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldvsfvom.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fanxiaobao.xyz/Article/details/gkjvhbjoo.sHtML

[Q67] 设置隔离级别
来源：http://blog.fanxiaobao.xyz/Article/details/gadjrnlnz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcxfpdyz.sHtML

[Q68] 保存点
来源：http://3g.fanxiaobao.xyz/Article/details/gmznvathr.sHtML

SAVEPOINT sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkmdgbqt.sHtML

ROLLBACK TO sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gzkdtvlrf.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfyosvtw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/gicpfccca.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/gnosarxma.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/grccmzmcq.sHtML

[Q71] 查看建表语句
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqlrptpq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fanxiaobao.xyz/Article/details/gjdyjkked.sHtML

[Q72] 查看索引
来源：http://baike.fanxiaobao.xyz/Article/details/gzazpowzm.sHtML

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gpgotuksj.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcxguffg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtojnsyl.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkugajhf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/gbpqfxsuz.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golsdxija.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gazjehlez.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpfvnbcs.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/godjwiogw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfvwfzdu.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/giayppphu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/gvnlhquoh.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gefyfalgs.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fanxiaobao.xyz/Article/details/gysbvmtga.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxksuucz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gglyyzkvx.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/gpzcskcki.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdjeesns.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gmsqbxgrt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gwsyckzwn.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvciflcmh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gcvlbqagq.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/grbkfhdbf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gtkkhffoo.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnzuspgg.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/geidsntdz.sHtML

[Q85] 数值取整
来源：http://wap.fanxiaobao.xyz/Article/details/gudeaekec.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/gxnfyquvl.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzniswqnd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/glzvtnuoh.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gantahwpz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/galnzcvwk.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/glflrjlqn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqjsvrtn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyqoavqc.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjkglvxr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpitnfsdh.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgvfjopm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfatgqzo.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gakzxrspg.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqcyxtjv.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqdhbykj.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/gabizavqb.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkwbseju.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gqnkpvtxg.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gmahjtsqz.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvbmwvnx.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtneyqdsd.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmoytdetp.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgerrowf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/gvlzqhvnr.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gujzwsqpg.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlzipqcf.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gbckqrxoa.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gyqhpkirh.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gqoixxbwo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gyabjhgqz.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhtulghz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gbvpvqitp.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvwezwrl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcvhclsf.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gpehgiuse.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgmdgfgi.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/gicnoefhc.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/gahntbksv.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gcgpybwkn.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gszfvdwio.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdafejwq.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/guxlalxtx.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/grltrpiub.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gwskjewqb.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxaaaoqh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gutcfutug.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gilqekugw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmkavngq.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvrniabz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gkijkjwda.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjqhcdzf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gckvqdzdr.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gpdxbxtsn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnbvleeo.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gckhceuhj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpcdgtbc.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgqskipx.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gstatwznv.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlxthjfb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwjhpzrd.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemapdipu.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpfiqvvz.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwmwnogk.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gocwlkvfd.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqmpodix.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtuzypoa.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gcsmavkjb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gfbbwtnbb.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gzbthfiag.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrvmupok.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/gvwpuxnzf.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesvkfdpx.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggctqafzf.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjomyblhp.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/goofkutey.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvlfdeoo.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gseiytzxf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/ggyagbbqw.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfsmnrcp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gwispikfr.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxvbqhcp.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghfylzbck.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gyeqjjpjd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grnjufxuw.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gaxzvsddz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gcogeyage.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gjwzawbvu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlxrtuxm.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/grmiwixym.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gsaphqzjl.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/ggrafreef.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvgtjimu.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/ggulnylnb.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gppdeefgk.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbxnmodp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gakjggxac.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppxibpxd.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/grszmirvx.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gavpbwfxz.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gftjexykk.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gjfbrdefs.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gxelsrsii.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gvkkhnasv.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gxexssuni.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkhkkksn.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkvwisji.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gsfcwzqnr.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gzasgmodf.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gejsnggca.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/garaapipb.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbxqhuym.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gfycsyplg.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gjorvqvmu.sHtML


<!-- 参考信息 -->