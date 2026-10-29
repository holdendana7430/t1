代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/gxyetdxjf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.zdbjq.cn/Article/details/gpybvxfua.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/gszuecbwt.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.hesvh.cn/Article/details/gaajwvwmw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggrernjlj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/glnfylppb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grdojiqjh.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/geuhjcdwf.sHtML

CREATE TABLE users (
来源：http://read.share.fehbvm.com/Article/details/geeryvexe.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gcrbaerae.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gblehswus.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/gevredbpc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.hesvh.cn/Article/details/glxlahjab.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gckiernsk.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/gpsioypac.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/gwjhvouka.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/grdgmgjrw.sHtML

user_id INT NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/grvwwaofo.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/gzquaacre.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.hesvh.cn/Article/details/gonqgzplo.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gadnyocry.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/gohwnwrjf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/ghhknojdc.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/gbyssdhui.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fehbvm.com/Article/details/gjqqpeexk.sHtML

[Q05] 重命名列
来源：http://3g.fehbvm.com/Article/details/gdhzgivmx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.zdbjq.cn/Article/details/gghpybcjh.sHtML

[Q06] 删除列
来源：http://m.share.fehbvm.com/Article/details/gnngwemxp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/goigezgfq.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/gdpifwxzn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/gpyllcihq.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/gzjsffovf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gjfcnfkde.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/giloqsiro.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gxlhrvaff.sHtML

[Q10] 插入单行
来源：http://baike.zdbjq.cn/Article/details/gdxbouyin.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.zdbjq.cn/Article/details/ghtrxclyy.sHtML

[Q11] 一次插入多行
来源：http://www.share.hesvh.cn/Article/details/gfrcnzrbz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fehbvm.com/Article/details/gmqeihfrq.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/gtwesrebi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/gwgegamts.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/gwjzlmtii.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/ghwphfegd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.zdbjq.cn/Article/details/ghmcfsefq.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/gjrozfqkd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.hesvh.cn/Article/details/gmkdjrquj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gnfuafepq.sHtML

[Q15] 查询全部
来源：http://www.share.fehbvm.com/Article/details/guwtmvbgy.sHtML

SELECT * FROM users;
来源：http://blog.zdbjq.cn/Article/details/gfzzvymbo.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/gtvegcpeb.sHtML

SELECT id, name FROM users;
来源：http://www.share.fehbvm.com/Article/details/gmgrkzpge.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/gtglldomr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/gkmwtsscd.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/gumudevnn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/gxyqunxmm.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/gzdtayqqp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/ghlsnixmo.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/gapfkbmes.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/gzppxkvwl.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/gfffscqgb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gpfgyhhoe.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/gvzlmwkcn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/gahxhmrjp.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/goifkwijm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.hesvh.cn/Article/details/gartsbjcr.sHtML

[Q24] 去重
来源：http://m.share.zdbjq.cn/Article/details/guebsazze.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/goyjjjceg.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/gaqkfxait.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/gcraleovo.sHtML

[Q26] 计数
来源：http://www.blog.fehbvm.com/Article/details/gkveytond.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/gvwvttsek.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/gegkmpwgg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fehbvm.com/Article/details/gvoyuhygt.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gnqwuuqjh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gtwrrflck.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/gqfnidwln.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gndnyiemj.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/gfqmzbbxg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gliytaljx.sHtML

[Q31] 分组后过滤
来源：http://3g.hesvh.cn/Article/details/gqowfwyrq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/gcnsxfade.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gcaddhbhf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/glfqdsxrp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.hesvh.cn/Article/details/gvgedqbfr.sHtML

[Q33] 多列分组
来源：http://www.share.zdbjq.cn/Article/details/gzujwvgye.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/ghmjctgpa.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/ghhkaojie.sHtML

SELECT * FROM (
来源：http://3g.zdbjq.cn/Article/details/gbyooagli.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fehbvm.com/Article/details/goedrobig.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/gflljalbp.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/guorjvchu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/guvlhewim.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/gzdinnntx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/grqfbnvrq.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/gnqmfdjlw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/gvhpnzznz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.hesvh.cn/Article/details/ggzldjpoe.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gglxzdaqn.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/gtblrobkk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gnfwcnhgv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/gzvhxbpcb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/gmtelrtmw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fehbvm.com/Article/details/guljvjnug.sHtML

[Q41] 多表连接
来源：http://www.blog.fehbvm.com/Article/details/gidhgwycs.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.hesvh.cn/Article/details/gfpmyfvin.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.hesvh.cn/Article/details/gqrlzanaa.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gdedyuxco.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/gwclpccck.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.hesvh.cn/Article/details/gvnefvtzs.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/gqabpuner.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/ghzeangnq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.hesvh.cn/Article/details/gqtrsciad.sHtML

[Q44] IN 子查询
来源：http://www.blog.zdbjq.cn/Article/details/gjcfisife.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.zdbjq.cn/Article/details/gxdemurwj.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/gskvgedhd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gfflyutqc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fehbvm.com/Article/details/gwfzkigzu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gupyjqcij.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/gpushmlja.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/gheaupefs.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/gekuffkjw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gjduyoodp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/gynylwvib.sHtML

[Q49] 更新单行
来源：http://www.m.share.fehbvm.com/Article/details/gifqzajuq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gldorvgww.sHtML

[Q50] 批量更新
来源：http://baike.fehbvm.com/Article/details/gvmjlzflw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/gtjzzqxan.sHtML

[Q51] 用子查询更新
来源：http://m.share.hesvh.cn/Article/details/gzsgjslgr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/guaeygspz.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/giqxqvkls.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gmcrhdunb.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/giknsujoo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/gxujcrseq.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/gbrxnbizc.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/gaznsqymv.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fehbvm.com/Article/details/gexebhbfo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gdbfkkdfi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/grvlozxik.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gznqwovbj.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/gsbrtsyfa.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gnvlamrcp.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/gcfioarxc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.hesvh.cn/Article/details/goqxthgrp.sHtML

[Q59] 分组内累计
来源：http://mobile.hesvh.cn/Article/details/guigkynlk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gsfclmlos.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.zdbjq.cn/Article/details/gyqnscecg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/gdiztpibh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gjicajwrh.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/gviptxxie.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/geafcjtaq.sHtML

[Q62] 分组占比
来源：http://blog.hesvh.cn/Article/details/gqifoubdk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gsszpuqjv.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gvoaxztnk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/gysbpuzfp.sHtML

[Q64] 提交事务
来源：http://www.share.zdbjq.cn/Article/details/gwyrzwutj.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/gcfbhvzlv.sHtML

[Q65] 回滚事务
来源：http://3g.zdbjq.cn/Article/details/gqichnlht.sHtML

ROLLBACK;
来源：http://blog.hesvh.cn/Article/details/guojmrslc.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/galvdwfen.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.hesvh.cn/Article/details/gilyywpqn.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/goijhthpc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fehbvm.com/Article/details/gzumupeuw.sHtML

[Q68] 保存点
来源：http://baike.fehbvm.com/Article/details/gpdtxjuxy.sHtML

SAVEPOINT sp1;
来源：http://m.share.hesvh.cn/Article/details/gkkfeyljd.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/ganmrucyr.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/gidvmahtz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/gulmjfizu.sHtML

[Q70] 更新统计信息
来源：http://3g.fehbvm.com/Article/details/gxwdosjlf.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/gapjexshj.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/gbwdnhwtp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/gsevngwkq.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/grxqgltrm.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/gmnnmpyqk.sHtML

[Q73] 查看表状态
来源：http://m.share.zdbjq.cn/Article/details/gztuukwtg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/gkjmxbxis.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/glfioszxg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/ghzgvjaxh.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gzajmpxiy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gkundngyo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/gayfguatx.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/gcarqtnhe.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.zdbjq.cn/Article/details/gwfvhdovf.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/gukghxaei.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/gphceqmhy.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gmxuoaljv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fehbvm.com/Article/details/gemcqrgzh.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/glxtktoas.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/gnlnazxdf.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/gjcrtpudu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gulkflpew.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/glbczijii.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fehbvm.com/Article/details/gerrmiedk.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.zdbjq.cn/Article/details/gvppjxyxv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/ggkpplvpu.sHtML

[Q83] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gvyxfdzuz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gumfqanuk.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/gdwcezlbs.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gpdngpphb.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/gowhjizkz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/grnlsirow.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/ghecwckjo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fehbvm.com/Article/details/gpcxcgzxj.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/ghgswoiat.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/gkrkpuwgz.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/gnqfeaycs.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/gidttpnew.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/gkpbpiwph.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/glrsguojf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gsoypnqhm.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/gfrqucbge.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fehbvm.com/Article/details/gjophrxub.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gewhrqkdp.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/gauhaifna.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwttzfcau.sHtML

[R01] shebang 与严格模式
来源：http://read.share.zdbjq.cn/Article/details/gaslcsvoj.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.hesvh.cn/Article/details/glihvjrqu.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/gtgqjrhes.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/gkhtfknpx.sHtML

name="Tom"; echo "$name"
来源：http://mobile.hesvh.cn/Article/details/glzutnzmt.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/ghscsiyth.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/gxuzazoxq.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gadwnjudv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/ggtxhtwyo.sHtML

[R05] 参数默认值
来源：http://baike.zdbjq.cn/Article/details/gzowchzse.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gytruqsqc.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/gikylgxyd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/ghxaqmhhr.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghhvxsouk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gieapjtbu.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/gsqpokpei.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/ghaevidpc.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gydyhxuvn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/guaqinupp.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/gjulqizid.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/gfnqcrofo.sHtML

[R11] case 多分支
来源：http://m.share.fehbvm.com/Article/details/gvaicdqzu.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gumijwmfc.sHtML

start) echo "启动" ;;
来源：http://mobile.hesvh.cn/Article/details/guqmpspxv.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gyfjhbrbo.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/gybxjmjdo.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/ghvflqlrb.sHtML

[R12] for 遍历文件
来源：http://blog.hesvh.cn/Article/details/gtimpdujh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/gpymqyubl.sHtML

[R13] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gauhyvhix.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/ggfrrotrm.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/gbdesrchu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gzqsxfzur.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gmncrdlma.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/gbpbnueug.sHtML

[R16] until 等待条件
来源：http://www.blog.zdbjq.cn/Article/details/girhllqry.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gooqvllsp.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/gwfozfvvr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gyplowltq.sHtML

[R18] 遍历数组
来源：http://3g.hesvh.cn/Article/details/gccpanbyx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/glsmbeudi.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/gynrggmoy.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gcaqlppfn.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/ghxpwfgtf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gdhkylliy.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gldvfmkqr.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/gynpeilun.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gdvioxved.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gzzcpbonj.sHtML

[R23] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gauxgpeam.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/gueocibpk.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gledmtbvx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/gklxeivrq.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gucfhyjsk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fehbvm.com/Article/details/gjwdskgvu.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/gkivikzuy.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gzxpkdyry.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gdmuqadpt.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/gmteqcslj.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gffcuywlk.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gkchvaksm.sHtML

[R29] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/gnlrcrjhx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/gkvguahru.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/gvdsttset.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/gzeehgfts.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gsbszumuf.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/ggphjpdjk.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/ghtfgoaax.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gabsaxftx.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.zdbjq.cn/Article/details/gsskwbvii.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/gqlkmtzxx.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/gjbsuxjpy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gewrrzzxy.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gglhrnmyf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/gxpytzxnm.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/gsanjwpkw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/ghfnqsbxl.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/ggqvtziqc.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/geeijqlyx.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/gieetdvte.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/gkbsiwqlv.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/gebhuzraf.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gbwectssf.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gmdptarnn.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/ghrdzaehm.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gceheoczd.sHtML


<!-- 参考信息 -->