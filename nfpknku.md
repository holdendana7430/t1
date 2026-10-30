代发 wailian999

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvefpofr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fanxiaobao.xyz/Article/details/gywyamyzx.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ghhbsttol.sHtML

[Q01] 创建表
来源：http://www.share.fanxiaobao.xyz/Article/details/givxlzvpr.sHtML

CREATE TABLE users (
来源：http://www.blog.fanxiaobao.xyz/Article/details/glweqtmsy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakhyktze.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fanxiaobao.xyz/Article/details/gtwelwwpw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fanxiaobao.xyz/Article/details/gbsuhtwrp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fanxiaobao.xyz/Article/details/guwymsbcw.sHtML

);
来源：http://3g.fanxiaobao.xyz/Article/details/gvqaztpcn.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrgcyitk.sHtML

CREATE TABLE orders (
来源：http://m.share.fanxiaobao.xyz/Article/details/gsiwgsfso.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fanxiaobao.xyz/Article/details/gyuipmnjm.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwwqgcsm.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fanxiaobao.xyz/Article/details/gypnkaeiw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fanxiaobao.xyz/Article/details/gmheotypr.sHtML

);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtgdqntj.sHtML

[Q03] 增加列
来源：http://3g.fanxiaobao.xyz/Article/details/gqwkmppue.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlarukja.sHtML

[Q04] 修改列类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdbtcceg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fanxiaobao.xyz/Article/details/gcogpvwgy.sHtML

[Q05] 重命名列
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrpyohcn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqawoolw.sHtML

[Q06] 删除列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwhqxbbb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fanxiaobao.xyz/Article/details/grbepqzqy.sHtML

[Q07] 删除表
来源：http://wap.fanxiaobao.xyz/Article/details/golfngykx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvimfkgcn.sHtML

[Q08] 创建普通索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfrjlawf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fanxiaobao.xyz/Article/details/gkysnvnqz.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkebsumn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fanxiaobao.xyz/Article/details/gugvhdyog.sHtML

[Q10] 插入单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gturasfag.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gxytfdwnl.sHtML

[Q11] 一次插入多行
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkiqpobv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fanxiaobao.xyz/Article/details/genzgjime.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagaqbkiy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fanxiaobao.xyz/Article/details/gblohrtce.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fanxiaobao.xyz/Article/details/gkxbrucmg.sHtML

[Q13] 忽略重复插入
来源：http://wap.fanxiaobao.xyz/Article/details/glusdjakm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/gceclqtfc.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fanxiaobao.xyz/Article/details/gokqbnufw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fanxiaobao.xyz/Article/details/gslznoijc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyallxmwv.sHtML

[Q15] 查询全部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtpdxqwd.sHtML

SELECT * FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrbypxkt.sHtML

[Q16] 查询指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggafptzzp.sHtML

SELECT id, name FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/guscdzxzx.sHtML

[Q17] 条件查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gekgjajjf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/glxtishsa.sHtML

[Q18] 模糊匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gwikfjbdq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fanxiaobao.xyz/Article/details/ggpnxkkkl.sHtML

[Q19] 范围查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gobtusyhj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fanxiaobao.xyz/Article/details/gswowshjh.sHtML

[Q20] IN 列表
来源：http://blog.fanxiaobao.xyz/Article/details/gxckzcogn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlojmqcv.sHtML

[Q21] 空值判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbtcwjyy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/gshxavovj.sHtML

[Q22] 排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gliryqngw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhifnzfu.sHtML

[Q23] 分页
来源：http://read.share.fanxiaobao.xyz/Article/details/grasudiop.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fanxiaobao.xyz/Article/details/glocawtmo.sHtML

[Q24] 去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwtbdlbo.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpblmuniy.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsczzmkyl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fanxiaobao.xyz/Article/details/gxlnxcpwk.sHtML

[Q26] 计数
来源：http://mobile.fanxiaobao.xyz/Article/details/gixhpcesa.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/ghpcxnjoa.sHtML

[Q27] 条件计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitytcebx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtongkewc.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdiqjisuj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gajyhyqbr.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrktghac.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdhaexgn.sHtML

[Q30] 分组统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrkvmtvt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwddiplu.sHtML

[Q31] 分组后过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/ggaxysgok.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjiqsafac.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzuqogir.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpeyaaqn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdrtelaz.sHtML

[Q33] 多列分组
来源：http://blog.fanxiaobao.xyz/Article/details/gzcwqojsm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjirdfsq.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdywwgwst.sHtML

SELECT * FROM (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxaxlahb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssllktio.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrwgobol.sHtML

[Q35] 内连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbtefaae.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgmxehjg.sHtML

[Q36] 左连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gmragmoxr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gtdgpctfk.sHtML

[Q37] 右连接
来源：http://www.share.fanxiaobao.xyz/Article/details/giqkqqdjt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfowotxmz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnnfteze.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzproapss.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fanxiaobao.xyz/Article/details/gedcnlpft.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fanxiaobao.xyz/Article/details/gpysghvqg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fanxiaobao.xyz/Article/details/giwvypeix.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fanxiaobao.xyz/Article/details/gldwzkrab.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fanxiaobao.xyz/Article/details/gnleapdaq.sHtML

[Q41] 多表连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geravplpc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fanxiaobao.xyz/Article/details/gzosscoev.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobiysaiw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gaqnhbyek.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gxsuldxul.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpkxgnde.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gefostejc.sHtML

[Q43] 标量子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gdefvzcqx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytnjqrbl.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbcnsdwp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgpkxfax.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fanxiaobao.xyz/Article/details/geqrjoktv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gshbrfnwp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fanxiaobao.xyz/Article/details/gfegeijmy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxsufoba.sHtML

[Q47] 与平均值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gybaztkpb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpftpbkld.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gzaoxkocn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcdeutgn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gmbcoheqb.sHtML

[Q49] 更新单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyfpwlbk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gmyenurxt.sHtML

[Q50] 批量更新
来源：http://baike.fanxiaobao.xyz/Article/details/gduvcajzn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gpmecuzcq.sHtML

[Q51] 用子查询更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlfnbezh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpascxzl.sHtML

[Q52] 删除指定行
来源：http://3g.fanxiaobao.xyz/Article/details/gzservobq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gcfkzdnxm.sHtML

[Q53] 按条件删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakwwwmbj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkobldpq.sHtML

[Q54] 清空表
来源：http://blog.fanxiaobao.xyz/Article/details/ghjrxtzos.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fanxiaobao.xyz/Article/details/ggqmoxert.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gyepbqfte.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbltzfgma.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fanxiaobao.xyz/Article/details/givnrwyiy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gzggghvdi.sHtML

[Q57] 行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzpktfnv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhwquwpi.sHtML

[Q58] 累计求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbdjscjo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmrfoaog.sHtML

[Q59] 分组内累计
来源：http://read.share.fanxiaobao.xyz/Article/details/gpyrqucic.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsahkdjqk.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdliuhub.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbfxrzyx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gapiddewo.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqtxbvmj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gissmiskx.sHtML

[Q62] 分组占比
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqepclfq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/graebpinq.sHtML

[Q63] 开启事务
来源：http://baike.fanxiaobao.xyz/Article/details/gsgiorbbd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fanxiaobao.xyz/Article/details/gakvupvrc.sHtML

[Q64] 提交事务
来源：http://3g.fanxiaobao.xyz/Article/details/gzdgtyvww.sHtML

COMMIT;
来源：http://www.share.fanxiaobao.xyz/Article/details/godawodwi.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/gfrmcffdw.sHtML

ROLLBACK;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhbtprkk.sHtML

[Q66] 行锁查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttcmxmds.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fanxiaobao.xyz/Article/details/gjlbbdivn.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fanxiaobao.xyz/Article/details/gazzyzqel.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/gubeejlfp.sHtML

[Q68] 保存点
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzpsnaam.sHtML

SAVEPOINT sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gwzhskmrt.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwladafqw.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/gwmmsgqhw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fanxiaobao.xyz/Article/details/gsrnpfcpn.sHtML

[Q70] 更新统计信息
来源：http://m.share.fanxiaobao.xyz/Article/details/glpnyjhqu.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxahxyvgs.sHtML

[Q71] 查看建表语句
来源：http://blog.fanxiaobao.xyz/Article/details/gccguitcr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/guolrxklw.sHtML

[Q72] 查看索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gguhvojcp.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzrhjhwj.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyysosmuj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxfsdtib.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/goxdmoepp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/grvuhbhua.sHtML

[Q75] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gnjcrtyhf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/giupvklmx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/guqvefpel.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggivtmxeb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gexhtfrie.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/grnmqpqxi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpnkomre.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gldimqlok.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fanxiaobao.xyz/Article/details/gjgmebmio.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gllampcrt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrhbkcgq.sHtML

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/gnjntfqvt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwrpezfu.sHtML

[Q81] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/guerckjon.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/grdpyecqs.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/grlshnrfj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtegjects.sHtML

[Q83] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gywbhrjjt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gruginosh.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gpolnfejl.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gdvxwairq.sHtML

[Q85] 数值取整
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzpiorqw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/gnqugeqqc.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gescqpvpi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/gdxhthehh.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/ggzlwilnr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/grotcugkm.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grivrqpvc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gvitnguyn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhkhczfi.sHtML

[Q89] 判断表是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gadqwjlam.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gqorqtptr.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmicdouu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gyqbualzt.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkaevcib.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gdjufhukw.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gackhfexc.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdbniqlq.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gltirzpbe.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gcpsnnjej.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gqljkmbuw.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlftgxzd.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/ggevapppe.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gbmdrsqxq.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/gxxersqdl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/goqarfnmf.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gbtijhwxx.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/glqahtlou.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccxyiiwt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggvhgvzct.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gdxtfifzu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gcwsphuxu.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gchderzzk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/glfxvjxct.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/girgatmhd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gqtohcowz.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjrxwonk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryfzsnhn.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzjwgecl.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgnhbwrr.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/guopjvoos.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gchbtlhzr.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gftmcuymu.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gyvjhostc.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gibktlmzq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gjfkqkvxu.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/gurmcjyqm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvswxqxg.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gvjesahqx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpomcolw.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gakgrbnpr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxrduzmf.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfntjybb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gojxvhwkv.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/gjbxznwyy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmvjwdqm.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghilkcixv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gyjtdlwvf.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbhrnxvq.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gbsaxzjio.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gnznvmopv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtnhwqgj.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjresmux.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/ggtjkcoxy.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gqaaemwwo.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbcjgwsa.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gnbcnbfvo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmpgltvz.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gnlwfqqli.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcbvowql.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxxhanem.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnofcyzjd.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/gxltnpdli.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gmypglhpa.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzezbdsg.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsckoecch.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gymjhlntv.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmkddmve.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gxgxmopnc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gmndpzass.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfrggcps.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjnmfmjd.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gscanlwpn.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkvmtyar.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gbsurqklu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggphnnlcf.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gttgrwhsb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/ghxxunvne.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyyekdos.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gyahfitse.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqrxepzx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gumqzuvgn.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmwktube.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gthxoayup.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/guppczmnh.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gsqxdiizv.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/garpvazew.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gkjrcunzd.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gcniqkefl.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrgpqyyr.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gttnrkkvp.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjtdcrbb.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gztxldfol.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gepvxbugn.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gwymhwsmk.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gvplnmonn.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhcwyewz.sHtML


<!-- 参考信息 -->