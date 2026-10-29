代发 wailian999

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/gtzfspudr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gklrypxjx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gbhljtein.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/gtvslijtc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.hesvh.cn/Article/details/goklshepq.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gkqpjelgs.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/gghgnnbpp.sHtML

CREATE TABLE orders (
来源：http://wap.zdbjq.cn/Article/details/gframuhhd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gikyporet.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/ghqvvanzy.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/gaqmikwtb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.zdbjq.cn/Article/details/gmsedjnoz.sHtML

);
来源：http://blog.fehbvm.com/Article/details/guxuemjpw.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/gptdzikga.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fehbvm.com/Article/details/gkwohjfnu.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/gwnggxnzs.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/goinppmwb.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/gstqcqsal.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/ggptnyvfw.sHtML

[Q06] 删除列
来源：http://blog.fehbvm.com/Article/details/grvgdzzdz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/gbxzelrry.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/ghqhxqpyp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.hesvh.cn/Article/details/gqxzedywr.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gffcrajwm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gqaxjnehu.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/gsjhnfjqz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gwyydlpnl.sHtML

[Q10] 插入单行
来源：http://read.share.zdbjq.cn/Article/details/gziubosox.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gpmtxwbex.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/gdqjzdbjl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/guxrajufm.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/gqspskreh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/gctgjtxof.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/gsclrdbsq.sHtML

[Q13] 忽略重复插入
来源：http://wap.hesvh.cn/Article/details/gnkruauys.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fehbvm.com/Article/details/gstklqjyj.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.zdbjq.cn/Article/details/ghxeomzui.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/gebjwwrdv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/gfvojtpxh.sHtML

[Q15] 查询全部
来源：http://blog.fehbvm.com/Article/details/gxcumvpdo.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/galayijie.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/gophnorjs.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gakpknrru.sHtML

[Q17] 条件查询
来源：http://baike.fehbvm.com/Article/details/gbdvtkybm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/gweleyhlg.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/geekwsfgy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.zdbjq.cn/Article/details/gtnoaurvq.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/gquyiaxkp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.hesvh.cn/Article/details/gmxjbubla.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/gusesxdiy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.hesvh.cn/Article/details/gubkzqfyb.sHtML

[Q21] 空值判断
来源：http://www.blog.hesvh.cn/Article/details/gndhikkvr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fehbvm.com/Article/details/gibxwnoyc.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/gsywnbbed.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gdyhzngqx.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/gocjalmjo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/gikpljrsv.sHtML

[Q24] 去重
来源：http://blog.zdbjq.cn/Article/details/gsljecqer.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.zdbjq.cn/Article/details/gvbrifctd.sHtML

[Q25] 只取前 N 条
来源：http://baike.hesvh.cn/Article/details/gugifmytj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.hesvh.cn/Article/details/gvlkdaoau.sHtML

[Q26] 计数
来源：http://read.share.hesvh.cn/Article/details/geujovcen.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gcqhxymau.sHtML

[Q27] 条件计数
来源：http://mobile.zdbjq.cn/Article/details/gteaqrlie.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/giwldkacc.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/gkiyfhzle.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gxspumzez.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gcvvctlab.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.hesvh.cn/Article/details/guarvzmga.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/gcjqwjrrf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gcchaojtr.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/ghfsbljpi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.hesvh.cn/Article/details/gvpnlnybt.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gfeijeuts.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/glltmwlgb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/guuvpzzkd.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/gcoeaxjsb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.hesvh.cn/Article/details/gdzvmxuib.sHtML

[Q34] 每组取第一条
来源：http://www.share.fehbvm.com/Article/details/gaghhxdtz.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gfrvanizs.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fehbvm.com/Article/details/gfehvfakt.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/gcezabsvv.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/gdadboeqj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gnuoepkiq.sHtML

[Q36] 左连接
来源：http://read.share.fehbvm.com/Article/details/gluhfndki.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gqcrfyyox.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/gdgvilbwz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gfehkpkxi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.zdbjq.cn/Article/details/gwdnwfmxq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.hesvh.cn/Article/details/gmomkriyp.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.zdbjq.cn/Article/details/gljdphahn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/gfkqzurvp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/gqhbsmppg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/gpleycovh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gyqkuccbb.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gephzsuyr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/gjvmapoue.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.zdbjq.cn/Article/details/gzduuwcrj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fehbvm.com/Article/details/gjfmjqcnf.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/gjguclqct.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.hesvh.cn/Article/details/gdtikgwtk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gvpuugfkm.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gbhcrwabj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gxmflbemb.sHtML

[Q44] IN 子查询
来源：http://blog.fehbvm.com/Article/details/guporqyqx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gyqymtcji.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/gngiejxet.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gkcojplng.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.hesvh.cn/Article/details/gmateoqvx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gaukeqfnu.sHtML

[Q47] 与平均值比较
来源：http://www.share.fehbvm.com/Article/details/gvgixlimw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gcyzdikba.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.zdbjq.cn/Article/details/gqdvamjvq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/gpjepamcu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/gicvrjhzo.sHtML

[Q49] 更新单行
来源：http://www.m.share.fehbvm.com/Article/details/ghjjljiqu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/grqjlyksh.sHtML

[Q50] 批量更新
来源：http://baike.fehbvm.com/Article/details/gmcwudvtf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gjdkxtxzl.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/gdgmazxix.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/gdswvuore.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/gwjzkztfh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gdivnrwuc.sHtML

[Q53] 按条件删除
来源：http://blog.zdbjq.cn/Article/details/grocbukdw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fehbvm.com/Article/details/gorxbjhxn.sHtML

[Q54] 清空表
来源：http://3g.fehbvm.com/Article/details/gxiuqsbrd.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/gzpssfsjr.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.hesvh.cn/Article/details/gsrmxsgjo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.hesvh.cn/Article/details/gyhkjuyky.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.zdbjq.cn/Article/details/gxmnzliss.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/ghwgtwgbd.sHtML

[Q57] 行号
来源：http://blog.hesvh.cn/Article/details/ghlaprhmo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.hesvh.cn/Article/details/gizbcolvl.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gsuosjeal.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gxcvhukyk.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/grxzxbpgl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gzhagvbxm.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/griiyugym.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/gesalkwiz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gjtqwrliv.sHtML

[Q61] 移动平均
来源：http://baike.hesvh.cn/Article/details/gzurdcmuk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gotqqsjni.sHtML

[Q62] 分组占比
来源：http://mobile.hesvh.cn/Article/details/gjmoqiuqu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gxvlxczns.sHtML

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/gcmjcvrmc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.zdbjq.cn/Article/details/gvahoolra.sHtML

[Q64] 提交事务
来源：http://m.share.hesvh.cn/Article/details/gemwmapfb.sHtML

COMMIT;
来源：http://wap.zdbjq.cn/Article/details/gtlfoitve.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gvssmkiab.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/gwwjbpopt.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/gmejmqosm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.zdbjq.cn/Article/details/gauvyippu.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/gwygctpbk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.zdbjq.cn/Article/details/gsaouthwi.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gjxpceifr.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/gcfootnee.sHtML

ROLLBACK TO sp1;
来源：http://3g.fehbvm.com/Article/details/gdghunqng.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/gmfororbb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/geaqjuduk.sHtML

[Q70] 更新统计信息
来源：http://baike.zdbjq.cn/Article/details/gklqcnggd.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/gcythyhhk.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/gumkpvpbp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.hesvh.cn/Article/details/gotecnmfw.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/gizudpmcr.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gyomosmpk.sHtML

[Q73] 查看表状态
来源：http://3g.zdbjq.cn/Article/details/glmdxmqwq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.zdbjq.cn/Article/details/glonnixra.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gpflbsnhw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/glngvvkzf.sHtML

[Q75] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gthmsbzgz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gkhtgmcqi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/gfbzsojum.sHtML

[Q76] 按天统计
来源：http://baike.zdbjq.cn/Article/details/glbtybgry.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fehbvm.com/Article/details/gnazfqpui.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gfsrgofwx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.zdbjq.cn/Article/details/goqcizvdh.sHtML

[Q78] 当前时间
来源：http://m.share.fehbvm.com/Article/details/gaeyrlvad.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.hesvh.cn/Article/details/gntliaual.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/glckeildf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/gbbthopes.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/gaedvqova.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gnunakbby.sHtML

[Q81] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gogrgucsf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/gvdyqxjjl.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/gmprsidgf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/ghajzrsdo.sHtML

[Q83] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gwafyyurc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gvhsyppem.sHtML

[Q84] 去除首尾空格
来源：http://3g.zdbjq.cn/Article/details/gdjmundfn.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gfzhlsmni.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gucwhyunj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/glxczvlcp.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/giceywgkm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gisviznuu.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/gojaycogh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fehbvm.com/Article/details/gsouhxzco.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/ggjhmrund.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/giihafeqf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gfzpnxpat.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/gmmlcmddi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/gfzfamrsk.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/gakzzglay.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/gksoifqoq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gasnjklua.sHtML

R. Bash 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gppwbxgwu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gquepxxyy.sHtML

[R01] shebang 与严格模式
来源：http://m.share.zdbjq.cn/Article/details/gvrbzayqm.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/gyhaxaceo.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gvkuhttrp.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/gyizlmpzc.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/gmlduvkxe.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/gsdomyzwd.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gvreutiqr.sHtML

[R04] 位置参数
来源：http://www.m.share.hesvh.cn/Article/details/gqedntyzx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/ggevmmkgv.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gqffsiwrp.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gkeoriwzp.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/ghrdmnpkd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gmhdwidwa.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/gerugajfc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.zdbjq.cn/Article/details/guksfuptw.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/gqnlaspfs.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/gavydqhff.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gfuzafqxn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gwiazzjpf.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/gisxlkqkn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/gmumtcftr.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/gwaytmeio.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/gfadqhuok.sHtML

start) echo "启动" ;;
来源：http://read.share.hesvh.cn/Article/details/gfjssuzby.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/gtwsohkjk.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gexoeluop.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/gkpfbihan.sHtML

[R12] for 遍历文件
来源：http://wap.fehbvm.com/Article/details/gtszdsgsw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.hesvh.cn/Article/details/gnleeqpip.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gtgedqpgg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gplklbhbd.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/gabzgzgtb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gircjlher.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gichhmrcd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/gmkyaxrwi.sHtML

[R16] until 等待条件
来源：http://www.m.share.hesvh.cn/Article/details/gsavjamoc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gazjdrkcx.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/gshboikdj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gzwnkwhem.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gqmdxjyqp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/gtmzspwgx.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gxahqvchl.sHtML

echo "${#arr[@]}"
来源：http://mobile.fehbvm.com/Article/details/ghzdenere.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/guzwuqcop.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/gvhreuadn.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gvzwkwjmj.sHtML

echo "${#s}"
来源：http://www.m.share.fehbvm.com/Article/details/gmmfmhnxr.sHtML

[R22] 截取子串
来源：http://baike.fehbvm.com/Article/details/gfmvvmtii.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/ghssxryqq.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gjjnnggoz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/gyavrqsvi.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/geaszhwfd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/gfwoulxya.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/gpqupezrf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/gwbmcitis.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/gehgrifxq.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/gdbuvnnau.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/ghmutcmpm.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/gxmcdeszm.sHtML

[R28] 浮点运算
来源：http://www.share.hesvh.cn/Article/details/gdelywiia.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gkopuoyyb.sHtML

[R29] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gdqsdnpfx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/gkuzolcim.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/gkuwxyubs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/godbqpjmg.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/gtfeefdib.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/gibxjkenb.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/gpiqdsnxn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gjkihoawx.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gvvyxdhmj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/grgcyxlmg.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/gkmnvqrto.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gjssxaxyi.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/gwmvpxwpy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/gucemamzr.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/gfxcemqht.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.zdbjq.cn/Article/details/gkfuomizl.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/gkevwrqvz.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/gehuqmsrh.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/gommmuveh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/gbkmxjssa.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/gbslmguat.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gvywvrsak.sHtML

[R40] 追加写日志
来源：http://baike.zdbjq.cn/Article/details/gwflvwofu.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/gomqnrgew.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/gdztkeqmx.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/gdvokohsp.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/gparulmep.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gavzzkmha.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gsrdmwvza.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gpiiiifbz.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/gyhhoejtj.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/gaefvzbba.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/gyzqzfbvh.sHtML


<!-- 参考信息 -->