代发 wailian999

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhkazjuj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fanxiaobao.xyz/Article/details/gosyyslyp.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gdngagwfr.sHtML

[Q01] 创建表
来源：http://3g.fanxiaobao.xyz/Article/details/gxgenvvuq.sHtML

CREATE TABLE users (
来源：http://m.share.fanxiaobao.xyz/Article/details/glfbdzhtx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrrwjxie.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrqjeygo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfniphwbe.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fanxiaobao.xyz/Article/details/gvigorode.sHtML

);
来源：http://wap.fanxiaobao.xyz/Article/details/gsblvhmep.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fanxiaobao.xyz/Article/details/ghixnhnad.sHtML

CREATE TABLE orders (
来源：http://baike.fanxiaobao.xyz/Article/details/gsmyvrint.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqwnrhih.sHtML

user_id INT NOT NULL,
来源：http://www.share.fanxiaobao.xyz/Article/details/gusuambky.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvexnsos.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fanxiaobao.xyz/Article/details/gtlpucybd.sHtML

);
来源：http://blog.fanxiaobao.xyz/Article/details/gazfhiipx.sHtML

[Q03] 增加列
来源：http://www.share.fanxiaobao.xyz/Article/details/ghoeeauoh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjychogac.sHtML

[Q04] 修改列类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbbqqbam.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fanxiaobao.xyz/Article/details/gpusloevh.sHtML

[Q05] 重命名列
来源：http://baike.fanxiaobao.xyz/Article/details/gavcwmpzj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmppdltm.sHtML

[Q06] 删除列
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqckxmck.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsxrorhw.sHtML

[Q07] 删除表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grixizkxd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gdduwwavs.sHtML

[Q08] 创建普通索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gkirflkua.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgqrqrvj.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gipnhijcw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fanxiaobao.xyz/Article/details/gxakuthnu.sHtML

[Q10] 插入单行
来源：http://3g.fanxiaobao.xyz/Article/details/giipbwcbg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fanxiaobao.xyz/Article/details/grohexomb.sHtML

[Q11] 一次插入多行
来源：http://blog.fanxiaobao.xyz/Article/details/gxgiymmtu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghidzdnix.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fanxiaobao.xyz/Article/details/gyddhmhei.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnqruruy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fanxiaobao.xyz/Article/details/gipjxtsmn.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrmivcwb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhdlavui.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fanxiaobao.xyz/Article/details/gwzfvbmwx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fanxiaobao.xyz/Article/details/glikldsun.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjangxhxc.sHtML

[Q15] 查询全部
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrtgbvso.sHtML

SELECT * FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/glfyfhmeq.sHtML

[Q16] 查询指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gspdrnvta.sHtML

SELECT id, name FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/goefksvxx.sHtML

[Q17] 条件查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gwobetsov.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpkmudmv.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhpqrmel.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzprqpvk.sHtML

[Q19] 范围查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnvrcxwb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrrlzdhn.sHtML

[Q20] IN 列表
来源：http://blog.fanxiaobao.xyz/Article/details/goshjnquk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/goofplcai.sHtML

[Q21] 空值判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgwmulxc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmehhuwp.sHtML

[Q22] 排序
来源：http://baike.fanxiaobao.xyz/Article/details/gwwklahwu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrsldhnn.sHtML

[Q23] 分页
来源：http://blog.fanxiaobao.xyz/Article/details/gwpvswndw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fanxiaobao.xyz/Article/details/geovyxhiv.sHtML

[Q24] 去重
来源：http://3g.fanxiaobao.xyz/Article/details/gttgkxuor.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/grrblhpho.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gawjzfhgh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfhdvyiw.sHtML

[Q26] 计数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwrrmful.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gbebbyyty.sHtML

[Q27] 条件计数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpmkunmj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyowpdyb.sHtML

[Q28] 求和与平均
来源：http://blog.fanxiaobao.xyz/Article/details/gwgafkzye.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gsmucmkpn.sHtML

[Q29] 最大最小值
来源：http://baike.fanxiaobao.xyz/Article/details/gfrbgvblt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gjaqhwbvf.sHtML

[Q30] 分组统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxqoondo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/govacnsmn.sHtML

[Q31] 分组后过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gtodkdzhl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gnciwvdmk.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlqiiugv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkvalrls.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepbxjngs.sHtML

[Q33] 多列分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gezmneheu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fanxiaobao.xyz/Article/details/gggryixvq.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjcxvwib.sHtML

SELECT * FROM (
来源：http://www.blog.fanxiaobao.xyz/Article/details/grakuzejl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhvrejog.sHtML

) t WHERE rn = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gnwohdxor.sHtML

[Q35] 内连接
来源：http://3g.fanxiaobao.xyz/Article/details/gxuzowraz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gnbsjaufb.sHtML

[Q36] 左连接
来源：http://3g.fanxiaobao.xyz/Article/details/gwcgushxu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gvloewfhg.sHtML

[Q37] 右连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwotmauxi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblgxnews.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxtoezrw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gaaebwhdx.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fanxiaobao.xyz/Article/details/gbmoykzdg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjroxdej.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gustnqqfr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fanxiaobao.xyz/Article/details/grtmlkukt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fanxiaobao.xyz/Article/details/gpeiocewv.sHtML

[Q41] 多表连接
来源：http://baike.fanxiaobao.xyz/Article/details/gcksfalmh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fanxiaobao.xyz/Article/details/gpemgqhpc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fanxiaobao.xyz/Article/details/gielhsqax.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmfzfepf.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvawokha.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsujkbmlt.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmvkjddy.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxdiswzl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fanxiaobao.xyz/Article/details/gocnnngka.sHtML

[Q44] IN 子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gsuwwicmv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbnqzdtf.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fanxiaobao.xyz/Article/details/gdmvejlkw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gywvdtzvn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxlglkjv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmlqvtty.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gtovogstr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fanxiaobao.xyz/Article/details/gkatawtlq.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbthgxge.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fanxiaobao.xyz/Article/details/gxfttrjsn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrzrtqwa.sHtML

[Q49] 更新单行
来源：http://wap.fanxiaobao.xyz/Article/details/gmcgzpmvj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthbzuxhb.sHtML

[Q50] 批量更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuvtighj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbaotsbz.sHtML

[Q51] 用子查询更新
来源：http://wap.fanxiaobao.xyz/Article/details/gtlawtvwr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gygsuprgw.sHtML

[Q52] 删除指定行
来源：http://m.share.fanxiaobao.xyz/Article/details/gavqwauow.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/guhncampr.sHtML

[Q53] 按条件删除
来源：http://www.share.fanxiaobao.xyz/Article/details/grnsyaapp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnifbyzg.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjabhtgk.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/gidlhzzxs.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gjuhumffs.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/guzputymq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gaibezlch.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/goliqanwg.sHtML

[Q57] 行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkfqenkl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxohiwpv.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/grhrluffc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gacurftzk.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqgownip.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtiahqnj.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fanxiaobao.xyz/Article/details/grktvlvxk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fanxiaobao.xyz/Article/details/guntwowkl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gmahzufgd.sHtML

[Q61] 移动平均
来源：http://baike.fanxiaobao.xyz/Article/details/gzhzzvewq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gevgxcwde.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/gseommehe.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjsgjgrk.sHtML

[Q63] 开启事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqogslore.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuuqmbth.sHtML

[Q64] 提交事务
来源：http://3g.fanxiaobao.xyz/Article/details/gflpfuzzl.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/gcxrkbvhi.sHtML

[Q65] 回滚事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbictrulc.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/gfonglywv.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/gkmjpgwrb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcoxmkqjn.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyngwavq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqmcfhew.sHtML

[Q68] 保存点
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyfdujzz.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/goygllcca.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgohjtak.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/gfrerectp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fanxiaobao.xyz/Article/details/gjaiuwhnn.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlpytyrh.sHtML

ANALYZE TABLE users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gucuydbrx.sHtML

[Q71] 查看建表语句
来源：http://baike.fanxiaobao.xyz/Article/details/gijqxsmyv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gkncrtkmg.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjgjjhig.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkiidcbq.sHtML

[Q73] 查看表状态
来源：http://baike.fanxiaobao.xyz/Article/details/gyjtqlgbs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gkztnyhys.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbumuzrt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpniwhnx.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaaomyqhv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdplipvc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkcgvktf.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gigolkfym.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqxofpny.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/gvylsypyg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/gmesujjnh.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/gdlppanuq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fanxiaobao.xyz/Article/details/gfehvemkh.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbivsvrqj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gdoyokojc.sHtML

[Q80] 字符串截取
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyytnkme.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gznpdcyan.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngceafpr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpgqtvns.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyqcigsi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmqeobmn.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gbfeqlwis.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gosdfvldu.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/gtonbcgpz.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjuhbxphc.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrwkibdv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/guflshgxg.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gllftpdzb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwwdubgb.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipwzdezh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbxtixfg.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gidemgize.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gmnpywnuz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gfothqvkl.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/grvblwbrn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvgzsxaa.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/gbocfqqgx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fanxiaobao.xyz/Article/details/gnqmjejan.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gycpomyhz.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gfuorspbv.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspgfgktd.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gkfgzkbfp.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjfmwvyc.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/geatqcqom.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gymvnwgsi.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gymtwdzey.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/gqzlegkje.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmjwrpgk.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gmpialkrc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/griyxdhsa.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/ghjpepykb.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gybymcgdy.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/goibrteww.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gsvoeplwa.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gowbxnqhg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gssjxlwda.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflsgijfp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gjctlimcn.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgxedqrt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqenbrmg.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gxleryvbm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/govtvijwc.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxmutwiy.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/gxqzknhvp.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gykrjgexg.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsoqpiys.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/glzfqxgmo.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbjfxgwi.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/gcdiztxdh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbzuwpbc.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/grzdtagui.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/guqlocxuz.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnxmgxgs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxiyvyod.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjtrcilv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/guxmgzrzv.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhevcchm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcuadtls.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcilncgzw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaekqzjga.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gkeecfpqw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gxksfqvpa.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gxehlrnow.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gdmiyxkaq.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gpsyiahrb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtysmuss.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gbepohthd.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/geplgyzgj.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gzoqlvjvq.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdkpnson.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gkdjgdmef.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfauxudqj.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/ggweskuto.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzfehqmw.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gjkpnlkhp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gogoscyzq.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuqtmhvk.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgjqfuwj.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghccgqjcp.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqocanpx.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gjhefcpph.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdufguiu.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gyrtlnrcf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzetvcawu.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/grvdmnkpy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gqhspmcxu.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gxksgiunc.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqlcdilh.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gsluvwiji.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxazsxct.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdqsarvj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnjpjeju.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptabybzh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gxmgestpt.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gdaxjpzjo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnxqwrdr.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gezyffigf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gotnbmcwm.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gvhcrimyd.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvotqytsl.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmhhachv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgxgucfv.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsjptsej.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/goazcjqri.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctjjxjee.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gczeoxaml.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gznfdygrx.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gyycgskzt.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/glzzfxdem.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gzghtpesn.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gkxdpmezc.sHtML


<!-- 参考信息 -->