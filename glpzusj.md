代发 wailian999

CREATE TABLE users (
来源：http://www.share.fanxiaobao.xyz/Article/details/gzetmasha.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmkticcg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fanxiaobao.xyz/Article/details/gzxtdglvk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxzqnrij.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fanxiaobao.xyz/Article/details/gkqsiuwhx.sHtML

);
来源：http://3g.fanxiaobao.xyz/Article/details/gemkcdggg.sHtML

[Q02] 创建带外键的表
来源：http://baike.fanxiaobao.xyz/Article/details/gczowfygy.sHtML

CREATE TABLE orders (
来源：http://blog.fanxiaobao.xyz/Article/details/gsmwpizxf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipuorpfu.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gormvmbnz.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fanxiaobao.xyz/Article/details/gywihwacv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunezfrzo.sHtML

);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvunpqdj.sHtML

[Q03] 增加列
来源：http://wap.fanxiaobao.xyz/Article/details/gvmzqvanc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gjbojpwxe.sHtML

[Q04] 修改列类型
来源：http://baike.fanxiaobao.xyz/Article/details/guhstesxr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fanxiaobao.xyz/Article/details/gbyyttypb.sHtML

[Q05] 重命名列
来源：http://blog.fanxiaobao.xyz/Article/details/glsypslyo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhlijlml.sHtML

[Q06] 删除列
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmswkgkr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fanxiaobao.xyz/Article/details/gtcycudwg.sHtML

[Q07] 删除表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgexhzja.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gccbcwkkg.sHtML

[Q08] 创建普通索引
来源：http://mobile.fanxiaobao.xyz/Article/details/guadgkomx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fanxiaobao.xyz/Article/details/guxezjudo.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gmoeviirx.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrdsuemd.sHtML

[Q10] 插入单行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruexomqn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/guqfqorgt.sHtML

[Q11] 一次插入多行
来源：http://wap.fanxiaobao.xyz/Article/details/gcqpwkaeu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzaplnymk.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fanxiaobao.xyz/Article/details/gknyjppoj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fanxiaobao.xyz/Article/details/gnlkdjhsf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fanxiaobao.xyz/Article/details/gxldhywbg.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fanxiaobao.xyz/Article/details/grmgvfdio.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjthxdwy.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqssboia.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fanxiaobao.xyz/Article/details/guwsbunel.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fanxiaobao.xyz/Article/details/gwdurjjsw.sHtML

[Q15] 查询全部
来源：http://baike.fanxiaobao.xyz/Article/details/gosfhdqnd.sHtML

SELECT * FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxlbutkb.sHtML

[Q16] 查询指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gcabxldgb.sHtML

SELECT id, name FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqeulywz.sHtML

[Q17] 条件查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gblyiwbnc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/ghtghnvsu.sHtML

[Q18] 模糊匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcnpnknl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fanxiaobao.xyz/Article/details/gibnfnxqb.sHtML

[Q19] 范围查询
来源：http://blog.fanxiaobao.xyz/Article/details/gatktlyzf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbbfnukn.sHtML

[Q20] IN 列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gapjyzhml.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlvkwmlq.sHtML

[Q21] 空值判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsqyrmcp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fanxiaobao.xyz/Article/details/gfftqqfyf.sHtML

[Q22] 排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpshwzhn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golmbskfj.sHtML

[Q23] 分页
来源：http://www.blog.fanxiaobao.xyz/Article/details/gengyhtxv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fanxiaobao.xyz/Article/details/gharwjayz.sHtML

[Q24] 去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbwuheuv.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkemixwai.sHtML

[Q25] 只取前 N 条
来源：http://3g.fanxiaobao.xyz/Article/details/gwzqeudxv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fanxiaobao.xyz/Article/details/gdviosxxq.sHtML

[Q26] 计数
来源：http://blog.fanxiaobao.xyz/Article/details/gbiaccdzr.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxdmjizf.sHtML

[Q27] 条件计数
来源：http://read.share.fanxiaobao.xyz/Article/details/gfykisium.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gdsrqjttw.sHtML

[Q28] 求和与平均
来源：http://m.share.fanxiaobao.xyz/Article/details/guaahmncq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gtsihgzbo.sHtML

[Q29] 最大最小值
来源：http://baike.fanxiaobao.xyz/Article/details/gobxmdfcs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/galuuzaua.sHtML

[Q30] 分组统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobaxstpp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdvpsgew.sHtML

[Q31] 分组后过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gkfyadsit.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fanxiaobao.xyz/Article/details/ggluvkgff.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giuryybrn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdcrkbgq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfcfutwz.sHtML

[Q33] 多列分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gabjnghmi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fanxiaobao.xyz/Article/details/gtqddtrul.sHtML

[Q34] 每组取第一条
来源：http://blog.fanxiaobao.xyz/Article/details/gqfenkzwb.sHtML

SELECT * FROM (
来源：http://baike.fanxiaobao.xyz/Article/details/grvrgmnjv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fanxiaobao.xyz/Article/details/gtucxrlcx.sHtML

) t WHERE rn = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrcvirgx.sHtML

[Q35] 内连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfqassqe.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrpebjov.sHtML

[Q36] 左连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvxmwnah.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gfzuaynat.sHtML

[Q37] 右连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsxaerdg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gryxwiqmt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fanxiaobao.xyz/Article/details/gnoiyklke.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fanxiaobao.xyz/Article/details/ganzrlcgx.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fanxiaobao.xyz/Article/details/gknlqwopg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fanxiaobao.xyz/Article/details/gfxkmrfrn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfkjsdeu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fanxiaobao.xyz/Article/details/gickfkcpv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjivkxzbw.sHtML

[Q41] 多表连接
来源：http://blog.fanxiaobao.xyz/Article/details/gwggtkalj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpheqmcm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fanxiaobao.xyz/Article/details/gkbzsippn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gjwevkrfv.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gxdkttmwj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fanxiaobao.xyz/Article/details/gzautbsuw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fanxiaobao.xyz/Article/details/geaqagrtj.sHtML

[Q43] 标量子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gprwoeosq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fanxiaobao.xyz/Article/details/gayrsfiht.sHtML

[Q44] IN 子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gubhxvslj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fanxiaobao.xyz/Article/details/giovhboto.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fanxiaobao.xyz/Article/details/gtufqnafq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkcnaifg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fanxiaobao.xyz/Article/details/ghuqjcysw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrooeqyw.sHtML

[Q47] 与平均值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpalhppa.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjscqqdn.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gikdgxktn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnuuzkdjo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqnhqoqg.sHtML

[Q49] 更新单行
来源：http://www.blog.fanxiaobao.xyz/Article/details/grczkwsxf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcyfrbvl.sHtML

[Q50] 批量更新
来源：http://blog.fanxiaobao.xyz/Article/details/grwevwrgw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gwkauyvwe.sHtML

[Q51] 用子查询更新
来源：http://wap.fanxiaobao.xyz/Article/details/goypbdvfm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gxdqvqcqq.sHtML

[Q52] 删除指定行
来源：http://m.share.fanxiaobao.xyz/Article/details/gbslugudj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfsrtmly.sHtML

[Q53] 按条件删除
来源：http://read.share.fanxiaobao.xyz/Article/details/guokbwfsh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgdmptwf.sHtML

[Q54] 清空表
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlbazzee.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvtdnysw.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdopjlzn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbogrpzlo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gzeapwmvc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getlsmxhm.sHtML

[Q57] 行号
来源：http://wap.fanxiaobao.xyz/Article/details/gmfbdtwso.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/glpppmfmh.sHtML

[Q58] 累计求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqogquhu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzgazdek.sHtML

[Q59] 分组内累计
来源：http://www.share.fanxiaobao.xyz/Article/details/gepiddjwr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnppljjch.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwilbsabp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/goxhxseod.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsutojgfb.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/gcpxmeint.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gtzlqzffz.sHtML

[Q62] 分组占比
来源：http://wap.fanxiaobao.xyz/Article/details/gurjugetv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gutjgkloy.sHtML

[Q63] 开启事务
来源：http://3g.fanxiaobao.xyz/Article/details/gjvzelcnp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fanxiaobao.xyz/Article/details/gspqyqyqb.sHtML

[Q64] 提交事务
来源：http://www.share.fanxiaobao.xyz/Article/details/grcsqlzli.sHtML

COMMIT;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfvtdrpx.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbvzcqrz.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggedhpfzi.sHtML

[Q66] 行锁查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gfelglwpy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fanxiaobao.xyz/Article/details/glbgirrtr.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fanxiaobao.xyz/Article/details/glhxluuoh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/ggddecjns.sHtML

[Q68] 保存点
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxxkvjzy.sHtML

SAVEPOINT sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gdwxjmsiw.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdaigwfq.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/gvchezjwr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnpymgdh.sHtML

[Q70] 更新统计信息
来源：http://read.share.fanxiaobao.xyz/Article/details/gnetvsuuq.sHtML

ANALYZE TABLE users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gajigdrmn.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrkchzfr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fanxiaobao.xyz/Article/details/ggevtvhwi.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtwdyoym.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqunwmxo.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/gqebuzjvd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gdykvbsvm.sHtML

[Q74] 强制使用索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gifuzalyg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/gxljbuhit.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxcwpjjn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrfyxjey.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/gidohihxj.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/glxwsajow.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gjjurdjlo.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplugdssh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/gswhzazai.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcawreqi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxiyraip.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmwclpqm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gpomeafzu.sHtML

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/gmlfubnox.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ghyfaqlts.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyvdrgyf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/grbtaecor.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/guqrirohr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gnmwufqdf.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/grpmsbgdd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvyvcple.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/grwhlyakr.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudmmzpgc.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/giozaplml.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywdxfwot.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfujmugr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fanxiaobao.xyz/Article/details/gaeeobhtu.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gpuorvtvc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnqzjipk.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvizoqgh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzssgggwy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gmxqajpxe.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqvlpqxv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gweezqlyw.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gdrgvayls.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxuduzld.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gdgjeclrx.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gcheczwfm.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ghvtrisdw.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjxvafmk.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/goxdrdmlf.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjtcqivi.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjuzkdkk.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgpzttgw.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaodmxxts.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrjinnvs.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gbqmgxnpc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gshzxniuh.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gngxyluvf.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gqyfwaszo.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gceothczm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlwxbonm.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/ghwohjuga.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/grswzdyou.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gebeoowps.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/guspjqhca.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gckupcykd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmcucldc.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giljeaywi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gawyicqgh.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/giebjehtf.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gnccytszk.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzihundq.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlqekfnt.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gjnqpcxei.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gzavizdsk.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/glwbfmnyg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gueertllc.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdhxolvg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/girzuylqy.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdiydeaee.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gtlyvlvkh.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gyeovfcub.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtduszwa.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfwqgyau.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gyqgecotg.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gxtdrtacx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggechfgzy.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghteyuqbm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/geatdcmkt.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gbgqbxynr.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gazabsncg.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gkmpimidr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjhlrcgg.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gaipybfhx.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqytjvmz.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gpetdvljg.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/golcklees.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmbveied.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gdoqopiyn.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvbqebhg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gobywhrne.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjgueoky.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gkxfefyrq.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/glzxihepc.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqinikdth.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gsddhhbqv.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxxhiksh.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyttiseo.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqbxlwsl.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnteqcjl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsgorxoq.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/ggoffgrgm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gesgsbkhy.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwjbhrxw.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giyfsxpau.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefaftvww.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/griutbzqo.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvlwnijx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpbvytci.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymuopygc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/geiuqwkal.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqalywtoi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gklivuhiu.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giznysxgr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyaynffy.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjerario.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gevetvuuh.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/ggefmnhtc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/grpeltkcs.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikvyzfas.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gsfcwsdyg.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkglbnhr.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gdokyxyap.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzkaoiuu.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gtpgddrmy.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gezwzgkip.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gtqmuqrug.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gtqcbpqtq.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgcbyfnq.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkngseatr.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gfguzttdq.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gjktpwtsu.sHtML


<!-- 参考信息 -->