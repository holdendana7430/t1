代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkupcvld.sHtML

);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqotsknol.sHtML

[Q02] 创建带外键的表
来源：http://blog.fanxiaobao.xyz/Article/details/gxchlkwzb.sHtML

CREATE TABLE orders (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgdrutxu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fanxiaobao.xyz/Article/details/gjthqhhzp.sHtML

user_id INT NOT NULL,
来源：http://blog.fanxiaobao.xyz/Article/details/gefmkmlet.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fanxiaobao.xyz/Article/details/gcupnsint.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwfktsdq.sHtML

);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giabpsper.sHtML

[Q03] 增加列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumfncbgz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkajhjzlj.sHtML

[Q04] 修改列类型
来源：http://baike.fanxiaobao.xyz/Article/details/gowyqtimy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwwpqrqf.sHtML

[Q05] 重命名列
来源：http://blog.fanxiaobao.xyz/Article/details/grhhbiisi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbixqarn.sHtML

[Q06] 删除列
来源：http://blog.fanxiaobao.xyz/Article/details/gbcbeamik.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfsydtah.sHtML

[Q07] 删除表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvibevxw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbozqiywb.sHtML

[Q08] 创建普通索引
来源：http://wap.fanxiaobao.xyz/Article/details/gxtpgpmlv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzdwsrtb.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhsweavf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvfobrmw.sHtML

[Q10] 插入单行
来源：http://blog.fanxiaobao.xyz/Article/details/goqlspzjh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gwrguiunm.sHtML

[Q11] 一次插入多行
来源：http://baike.fanxiaobao.xyz/Article/details/glznjqrvh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/grolijfzo.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fanxiaobao.xyz/Article/details/gotdlwyvz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnreexfj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fanxiaobao.xyz/Article/details/grbddibgf.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fanxiaobao.xyz/Article/details/gesztsoiz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/grrjdroyt.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fanxiaobao.xyz/Article/details/gmumuuaiw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fanxiaobao.xyz/Article/details/gpydkishd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fanxiaobao.xyz/Article/details/gumhcxmyf.sHtML

[Q15] 查询全部
来源：http://mobile.fanxiaobao.xyz/Article/details/garlbuqhu.sHtML

SELECT * FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gfrkflktc.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giulteibq.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galipggmu.sHtML

[Q17] 条件查询
来源：http://blog.fanxiaobao.xyz/Article/details/gxxchntto.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gnangxklw.sHtML

[Q18] 模糊匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gkpbxuadd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fanxiaobao.xyz/Article/details/gvetkhqhc.sHtML

[Q19] 范围查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgiojnez.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmhxcydd.sHtML

[Q20] IN 列表
来源：http://3g.fanxiaobao.xyz/Article/details/gfihoprgb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkykorhwz.sHtML

[Q21] 空值判断
来源：http://wap.fanxiaobao.xyz/Article/details/gzwgwnjhy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fanxiaobao.xyz/Article/details/gysepvlag.sHtML

[Q22] 排序
来源：http://baike.fanxiaobao.xyz/Article/details/gmxsxcalu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsonzjggs.sHtML

[Q23] 分页
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbeugjid.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgdbfhtr.sHtML

[Q24] 去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gtshxvmpx.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gudikhqbp.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gpllgkjgl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwipzyte.sHtML

[Q26] 计数
来源：http://read.share.fanxiaobao.xyz/Article/details/gctxapdwn.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbwmbfru.sHtML

[Q27] 条件计数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrogshyz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gpzejhahp.sHtML

[Q28] 求和与平均
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmxdfjsy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/ghdtdpurr.sHtML

[Q29] 最大最小值
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxngndez.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gartfonmi.sHtML

[Q30] 分组统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gxugrwhhc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gdahzyuko.sHtML

[Q31] 分组后过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gykwhjnnz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fanxiaobao.xyz/Article/details/grkddhrke.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbrfrwme.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/giviikfmn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fanxiaobao.xyz/Article/details/gotpuihhe.sHtML

[Q33] 多列分组
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvrahewb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fanxiaobao.xyz/Article/details/gamqdhiua.sHtML

[Q34] 每组取第一条
来源：http://read.share.fanxiaobao.xyz/Article/details/guorpntfs.sHtML

SELECT * FROM (
来源：http://wap.fanxiaobao.xyz/Article/details/gtgkhcmzm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fanxiaobao.xyz/Article/details/gradkpjgl.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsjxsonh.sHtML

[Q35] 内连接
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzwnqzjk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhobwtme.sHtML

[Q36] 左连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giigbfxai.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/ginpzndfm.sHtML

[Q37] 右连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwesxravk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gskkkaltv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjatkpyn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fanxiaobao.xyz/Article/details/ghkedhakk.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyzpgxcz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fanxiaobao.xyz/Article/details/gyegwtkyw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gihqawugi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fanxiaobao.xyz/Article/details/glhviowrd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fanxiaobao.xyz/Article/details/gkrwlyplh.sHtML

[Q41] 多表连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtxgmexw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fanxiaobao.xyz/Article/details/grcojqcva.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnmiquin.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gprzqkgei.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gmwhrzxwc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fanxiaobao.xyz/Article/details/gvtdjxcib.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gnkoevdda.sHtML

[Q43] 标量子查询
来源：http://3g.fanxiaobao.xyz/Article/details/glpzkdwwl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fanxiaobao.xyz/Article/details/gwyekvrnq.sHtML

[Q44] IN 子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gtboobiyv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtrarzqf.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fanxiaobao.xyz/Article/details/galpozqev.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzliiqft.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fanxiaobao.xyz/Article/details/gziiykinh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/glniaollk.sHtML

[Q47] 与平均值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gebtkgbka.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcggdkrns.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvsqxcqc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fanxiaobao.xyz/Article/details/gnzgxrxos.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcedmhsfm.sHtML

[Q49] 更新单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvmbhpiv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyowduhm.sHtML

[Q50] 批量更新
来源：http://baike.fanxiaobao.xyz/Article/details/gemkhixbi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsretumb.sHtML

[Q51] 用子查询更新
来源：http://baike.fanxiaobao.xyz/Article/details/gwcrqdkqa.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gidrtanif.sHtML

[Q52] 删除指定行
来源：http://blog.fanxiaobao.xyz/Article/details/gdjkmbskm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gvkhbxnno.sHtML

[Q53] 按条件删除
来源：http://3g.fanxiaobao.xyz/Article/details/ghjjkjbbi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/ggcwehvzg.sHtML

[Q54] 清空表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwggevdah.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjodrblzw.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqemcltk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmwzghvn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhtyukvz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxuntgpt.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gjunqevik.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gfsuhccel.sHtML

[Q58] 累计求和
来源：http://3g.fanxiaobao.xyz/Article/details/gwzzehqwq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gechqpevb.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwxomvoe.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gyxindllp.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgwfmngn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmhhiwgu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gaafyciro.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqjrjsjf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxtivfuz.sHtML

[Q62] 分组占比
来源：http://mobile.fanxiaobao.xyz/Article/details/gsothrsbh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzotwlkwf.sHtML

[Q63] 开启事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwolxeuy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxzqjarn.sHtML

[Q64] 提交事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gqysfzauj.sHtML

COMMIT;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbogzkmlk.sHtML

[Q65] 回滚事务
来源：http://wap.fanxiaobao.xyz/Article/details/gllzuoxox.sHtML

ROLLBACK;
来源：http://read.share.fanxiaobao.xyz/Article/details/girzsucmz.sHtML

[Q66] 行锁查询
来源：http://blog.fanxiaobao.xyz/Article/details/gyiohwgju.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fanxiaobao.xyz/Article/details/gwypcgqlb.sHtML

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/gmkrotkqf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/gttvuuplx.sHtML

[Q68] 保存点
来源：http://3g.fanxiaobao.xyz/Article/details/gnptzghyh.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjxobhxm.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhygeumi.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwobqgrx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcokclhe.sHtML

[Q70] 更新统计信息
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxqgrlhc.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gnyvtnhfa.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfjijspi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fanxiaobao.xyz/Article/details/gspabotbw.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrambcaw.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjfttxrl.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghorpgmmm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gxjdrtyms.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujagxdze.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/gkiafkijc.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvyglxhz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggebamniy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzwbtesy.sHtML

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcecfnqus.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/gkkdlnbji.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/gndfdhkon.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpiaiqpa.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gbsmlcxot.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fanxiaobao.xyz/Article/details/gpslatswz.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjzdvxtg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsosghmm.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gdodgjzxc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ghweamaqj.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzaacjojo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gkvxnaspt.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gxsccfzjf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gkuktumac.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gchlibolo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpfhaitz.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqdiprnu.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbflpegx.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/gyjnayfya.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/gueceygzg.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphmepqke.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gbslbfmsg.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gpmgkzoeg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gxzehljcn.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gudueeriz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gpovifbky.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpznrtqnj.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/geeciznva.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpbkjkjv.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gqcwlxubz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gnmknkexf.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gqfinjlhv.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gjjbstbxv.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksttygsf.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxpmrrpl.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gqrpzxkam.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekcylqme.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/ghdvseavu.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gisazchea.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchxbmret.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gnitprvxr.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/grzpitigi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gkiwivqoo.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gzktabrug.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gdklvbefr.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gwezalqxd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmweevzw.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbqaihqp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwueppmtk.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gacqzuwzv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucuzzivt.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmjljjnu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gapupgapz.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvujultw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/ghnoiunlx.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzmbpxzf.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnmkpobh.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/geolvaloq.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvadmanun.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxchblbs.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpvzirwx.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gscnllbmx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gygpvscpk.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/ggchlqccs.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gqnwrtezk.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/ghkxydacm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gwnfwtibj.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gmshkhwgv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gkauactyq.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvphznfy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gshmdbtbc.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrsktfcp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gceqtntcz.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gbriuwhji.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpxqbxxy.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpkycigy.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/guhoqiptp.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwlkzvid.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gaxlmqhkz.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqczmkhh.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goftlzbyp.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/ghluvqbjh.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gafozqvby.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gyebwbkuo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvrxttta.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbvrhkbs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gjcozefra.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwjgyobc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gzbvyhdqh.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/gdeooilue.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/godnzijul.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gxbvvnawh.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfiundhi.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdruzbmn.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gdibwlujq.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gybjnitda.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjegjeml.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/glcevhhdz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gevzqzvyj.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gtdklaeeg.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/guzxawncp.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gayistohv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/galekcfwy.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/ggiguxxeh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gmdbuvrmf.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gikjfknqm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gvnnjcqpw.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gzaggveqo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvvsuiuz.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtinymjpu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkmoebrz.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gauvdfzpf.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gjslpnqsv.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gwboxmzqw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkyawuig.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdnuxnqi.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gnnviqiry.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxrsczyr.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/giajrpasm.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryuhuliv.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gpxjuotbk.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gfsqrsazw.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gvalqzrzi.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gktwlmalr.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnypqhbr.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqmanzfl.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gmezfyebs.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gnjurlmtn.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbsqxrpq.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/ghqiukhwo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gpfxaffcf.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/giryozkll.sHtML


<!-- 参考信息 -->