代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.hesvh.cn/Article/details/gzpxggmyy.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gcmekmoqw.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gkeiknvnv.sHtML

CREATE TABLE orders (
来源：http://m.share.hesvh.cn/Article/details/gtujlkxwb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gxxqeaqxn.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gsdsrbzfn.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/gffpaemws.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.zdbjq.cn/Article/details/gyjloaiph.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gqarnasus.sHtML

[Q03] 增加列
来源：http://3g.fehbvm.com/Article/details/goeahhcdx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/glrlvhfxp.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/gnohiolmi.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.hesvh.cn/Article/details/giubgsutc.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/gistetsan.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/gvltlrmwc.sHtML

[Q06] 删除列
来源：http://3g.fehbvm.com/Article/details/gkjxtmaaj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.hesvh.cn/Article/details/gjreppcsf.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/gtxfyvgxf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gcxsatjqd.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/gkavsnnlg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gcumhvchv.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/glilukdnk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gjxaqggpy.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/gzhgitiog.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gxwnicqzm.sHtML

[Q11] 一次插入多行
来源：http://mobile.fehbvm.com/Article/details/groahvhee.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gnzeszqib.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.hesvh.cn/Article/details/gxpxvpvrh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/gbbmuynkc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.hesvh.cn/Article/details/gjgmmxmdv.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/gswyhvwoe.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fehbvm.com/Article/details/gpncyepqr.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/ggvoslkee.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.zdbjq.cn/Article/details/gxhkoywmh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/gvdzdljwh.sHtML

[Q15] 查询全部
来源：http://www.share.fehbvm.com/Article/details/grgpsetgg.sHtML

SELECT * FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gtecgehev.sHtML

[Q16] 查询指定列
来源：http://mobile.hesvh.cn/Article/details/gjhuqaqgz.sHtML

SELECT id, name FROM users;
来源：http://mobile.hesvh.cn/Article/details/ghntopefb.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/gydqbxhil.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.hesvh.cn/Article/details/gboqoklwm.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/gmihngqrc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/ggxagtfxc.sHtML

[Q19] 范围查询
来源：http://mobile.hesvh.cn/Article/details/gnpahftma.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/gfcqbxglk.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/gchakegma.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gcrxiwghj.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/gukhwwosq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/gjfrmnwrr.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/gdjliionz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.hesvh.cn/Article/details/grybfbmlk.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/gvpokluiz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.hesvh.cn/Article/details/grplzoewj.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/guhuelnix.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gmyqrtebh.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gwmqliidh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fehbvm.com/Article/details/gjpglysel.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/glfwrtqzw.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gtexgnima.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/gkdrhaius.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fehbvm.com/Article/details/gvhvdkdku.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/gvvuromsv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gouesphso.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/grfzshxci.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gdbzttwjz.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/gywlcaqie.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/goffiggvq.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/gjvlsbuwi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.hesvh.cn/Article/details/gmfnkpggp.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gqqmcrivv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gjvyywlby.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/gautbtudp.sHtML

[Q33] 多列分组
来源：http://baike.zdbjq.cn/Article/details/gpxwuegfa.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fehbvm.com/Article/details/gfknnwqnj.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/gthuubpvt.sHtML

SELECT * FROM (
来源：http://m.share.fehbvm.com/Article/details/gfwunfddg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/gymfzlxfw.sHtML

) t WHERE rn = 1;
来源：http://wap.hesvh.cn/Article/details/ggnznuksn.sHtML

[Q35] 内连接
来源：http://baike.zdbjq.cn/Article/details/gpgynrsoj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gnudrfugz.sHtML

[Q36] 左连接
来源：http://read.share.fehbvm.com/Article/details/gdtpbbsim.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gxiyiahmq.sHtML

[Q37] 右连接
来源：http://blog.fehbvm.com/Article/details/gadtzudmr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/gthibrduf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/gulxuoumz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gybvwwjel.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/gilnxnekc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.zdbjq.cn/Article/details/gdcxfvbdp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/gslormhvd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/gmbizqkmc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.hesvh.cn/Article/details/gyfvgxmds.sHtML

[Q41] 多表连接
来源：http://m.share.zdbjq.cn/Article/details/grisdylge.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/ghuiqlzvr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/gtgmlgawb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gfzlwzndr.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/gkylcghzu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/gmkenesve.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/gufiyxirz.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gafyouqir.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fehbvm.com/Article/details/gcvewspxe.sHtML

[Q44] IN 子查询
来源：http://3g.hesvh.cn/Article/details/gjnzlnkjl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/gaogdoonx.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/grxaqslbb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gbvjgeuoi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.hesvh.cn/Article/details/goqpolyvb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gvpyknbat.sHtML

[Q47] 与平均值比较
来源：http://read.share.hesvh.cn/Article/details/ggblbagcy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.zdbjq.cn/Article/details/gppdkysbx.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.hesvh.cn/Article/details/gqwgalrqp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/gkrgscnjw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.hesvh.cn/Article/details/gfosylkbz.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/gpplmkids.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gvhvavywr.sHtML

[Q50] 批量更新
来源：http://blog.zdbjq.cn/Article/details/gwbloeiyr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.zdbjq.cn/Article/details/ggksfzesv.sHtML

[Q51] 用子查询更新
来源：http://www.blog.hesvh.cn/Article/details/gpgujnfyv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fehbvm.com/Article/details/gppzqspcu.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/ggqeitwiu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/goiievndj.sHtML

[Q53] 按条件删除
来源：http://read.share.fehbvm.com/Article/details/gmmoiyvtm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gplmhvymx.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/gfbwdnemh.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/gbktgzghr.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/gwumfhgtq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.hesvh.cn/Article/details/ghyzmugww.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.zdbjq.cn/Article/details/gjvnzvlit.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gjlxiclgn.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gyapsftko.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gtmyuifzm.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/gigprjwkp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fehbvm.com/Article/details/gxkabcxkx.sHtML

[Q59] 分组内累计
来源：http://mobile.hesvh.cn/Article/details/gsgsdsjjd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gjkgdltjr.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/gxpgmtkqs.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/geuzntxns.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gmsnqmzrn.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/glthuoksl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gqxaxyepl.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/gxktlreis.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gldoevxls.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gtpwyqgfo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/goukoianh.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gtbphginu.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/gjvoielln.sHtML

[Q65] 回滚事务
来源：http://www.m.share.hesvh.cn/Article/details/gyeimnyty.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/giudwwiwo.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/gmzbikewu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gecwtnlyl.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/ggjctdhpp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.zdbjq.cn/Article/details/guetderuw.sHtML

[Q68] 保存点
来源：http://blog.fehbvm.com/Article/details/gfhlynxqq.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/gvbfjtvsx.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/gwiyaejvh.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/gwvuspdan.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/glredogsk.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/gwlzmblui.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/gcultkhya.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/gsramohkm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.hesvh.cn/Article/details/grhdmcxrl.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/gitfpyqas.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gxaemiohx.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/guhgdnwju.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/gmchybasu.sHtML

[Q74] 强制使用索引
来源：http://mobile.zdbjq.cn/Article/details/gkppfwnwt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/gsnzrjpno.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gnlydtbzt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gfeouwfsf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gpctkgqsq.sHtML

[Q76] 按天统计
来源：http://wap.hesvh.cn/Article/details/gocrpimdr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/gousrmpxp.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/gthuduszg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/gpwaszuca.sHtML

[Q78] 当前时间
来源：http://blog.fehbvm.com/Article/details/gpzcqeuek.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/gpuiypxja.sHtML

[Q79] 字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gcakgiaib.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/gytgqbhnv.sHtML

[Q80] 字符串截取
来源：http://read.share.zdbjq.cn/Article/details/gxncgijsp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gibxcwfyl.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gjyigqqid.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gtlbmmaoy.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.zdbjq.cn/Article/details/gmpdbcvjb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gjeggshwx.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gqaaggvsr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/grligevgk.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/glykspmuo.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gddgwmrmu.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/glpjgthqj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/gzulafifu.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/gywwxfzry.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/gkveliwfi.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/gcbkvbuww.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.hesvh.cn/Article/details/guibsxzpq.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/gntdkztag.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/ggwxegmgf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/gxsltstlr.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gjxwhlpva.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/gvmffpwtt.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/grhycsxnz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gpuvgufoq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvmmaalqp.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/ggdomrvkv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkkjxjcbo.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/gcrfnbkta.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/gacfvrfhx.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gazmgnhzy.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/gvrspbvfu.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gwmlwnzzx.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gznvjjzsn.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gkifmwzlm.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/glkbenqot.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/geickaojz.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/ghxnlttmi.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/glwhlfvwd.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gogsxbjsu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gcynnuuzn.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/grgnocbaa.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gzqtgmbkw.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/gmvqwiflc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/guauhrpan.sHtML

[R09] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/gcekrewzh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/gffesdhob.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gcjumfmed.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/giggnrobk.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gdmazaiud.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/glvclxpfr.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gdvekrfmu.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/gjtoairno.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/grvkufopr.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gjgezzvnx.sHtML

[R12] for 遍历文件
来源：http://blog.hesvh.cn/Article/details/giwcnujgn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/gevlhiyyl.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/grgloqkdl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gtoruyniq.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/gnmrswsum.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gaixhflov.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gvogzseie.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/gmxigeuee.sHtML

[R16] until 等待条件
来源：http://www.m.share.hesvh.cn/Article/details/gmkfbqwxx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gdfgztgak.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/gibimghse.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/gzfbttpdb.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gbqpzqlfq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/gazfgjiyb.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gtkrqrgxe.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/grpimsqrj.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/gjookaacn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fehbvm.com/Article/details/gordhtnnt.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gylhmqpxy.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/ghjxtwnbg.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/grfxwdqmf.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/gvstwlzwn.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gqekjvqme.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/gjlcojybb.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gnlvhsemk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/gvkgegaxm.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/gqpazecii.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/gaiqwklid.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/gnjxjusem.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/gnkrnijts.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/gxumsurvn.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.zdbjq.cn/Article/details/gjvnmbfgx.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/gnbkmivvj.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/gumfgfyiw.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gdosgyank.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fehbvm.com/Article/details/gwfwyxnnb.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/gmhopomqk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gafbputke.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gtxeqzdmo.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/gmkmkjzdb.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/gdhvzeinq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gvyrvluwk.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.hesvh.cn/Article/details/gdijemdnt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/gsletojxm.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/gvfljxoea.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gzqnwkzep.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/gybemgrqb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.zdbjq.cn/Article/details/gnzjbcywj.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/gskojtwpy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fehbvm.com/Article/details/gmdcbdxev.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/gyvnoooms.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/gbepoqith.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/gokdplyjz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/gewhmthdv.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gopqabund.sHtML

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/gdbxqsqfa.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gbkrpfqrj.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/gdegimdpg.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/gaxztmnmz.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.hesvh.cn/Article/details/gdqyhbvnj.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/gvbpnzzow.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gfcytbiuv.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/guikbiomf.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/gzexdiewr.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/ggihyeher.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/ghxkkmjya.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/gdywwmrdd.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/gwmegnvyh.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gwxcexymy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/giqzijsgt.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gzoyfppgt.sHtML


<!-- 参考信息 -->