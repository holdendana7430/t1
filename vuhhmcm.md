代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.zdbjq.cn/Article/details/gmsyctcut.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gejzuqvtm.sHtML

[Q02] 创建带外键的表
来源：http://read.share.hesvh.cn/Article/details/gewtubyeu.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/gqfxeocyk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gshtwdoqn.sHtML

user_id INT NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gtperdkek.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/ghpmfyeyi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/gvxuhurfc.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gvzmmjvmp.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/ginrmzdvo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.hesvh.cn/Article/details/gckhtmjyo.sHtML

[Q04] 修改列类型
来源：http://m.share.fehbvm.com/Article/details/glxrmpkif.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.zdbjq.cn/Article/details/gsydstubf.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/gkeztgghb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.hesvh.cn/Article/details/gdzcfqqhg.sHtML

[Q06] 删除列
来源：http://mobile.fehbvm.com/Article/details/gwpboczqy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.hesvh.cn/Article/details/gsndtxmoy.sHtML

[Q07] 删除表
来源：http://blog.hesvh.cn/Article/details/gzmnkduup.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/gnudukmgv.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gprkbgqac.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/glgdvcyaj.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/gstulznvv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gsvwtkonk.sHtML

[Q10] 插入单行
来源：http://mobile.fehbvm.com/Article/details/gwwyzmavk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/ghrvoncmt.sHtML

[Q11] 一次插入多行
来源：http://blog.fehbvm.com/Article/details/ggcdizspa.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.zdbjq.cn/Article/details/gyohvnjoa.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.hesvh.cn/Article/details/gyzbhajkv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/ggegykwuv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gsvostnmc.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/gmguknrnq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/gheaugcxd.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.zdbjq.cn/Article/details/gpnojkjfg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gpqlffmfg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/gkvcmdjah.sHtML

[Q15] 查询全部
来源：http://blog.fehbvm.com/Article/details/gvdxgvrxu.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gmjsppokq.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/gbxmcqpzl.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ghsxcfjsi.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gwllldacl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.hesvh.cn/Article/details/gtkzdxmqk.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/gayrrqqxk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/gjpimymkr.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/gfqvjdkad.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.hesvh.cn/Article/details/gnpgdgbpo.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/gqlcmugnz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fehbvm.com/Article/details/ghsrelpdl.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/gwajxgivk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gybfjhwox.sHtML

[Q22] 排序
来源：http://m.share.fehbvm.com/Article/details/gqombqsdd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.zdbjq.cn/Article/details/grsbslwqu.sHtML

[Q23] 分页
来源：http://wap.hesvh.cn/Article/details/gunavhhjs.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/gddnhvgaz.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/gopovcxbl.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.hesvh.cn/Article/details/gfrzjtzsn.sHtML

[Q25] 只取前 N 条
来源：http://wap.fehbvm.com/Article/details/gjbtqubky.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fehbvm.com/Article/details/gouktqubb.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/gtihgeyfp.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gvxeqsiej.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/gafeatdzy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gdmogmhan.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gxmteotme.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gjuyrhwun.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/gjrnbqrre.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/grbpsffwa.sHtML

[Q30] 分组统计
来源：http://3g.fehbvm.com/Article/details/gbznmvora.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gmiergece.sHtML

[Q31] 分组后过滤
来源：http://wap.fehbvm.com/Article/details/gzlubljco.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/gifjphxhl.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fehbvm.com/Article/details/gchpimdde.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gppotqsjz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/ghxlnsjvc.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/gkdrqcvgb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/geeoafmui.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/gmbdmnvys.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gphnssgzf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/gcjicsdws.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/gbduvgtbg.sHtML

[Q35] 内连接
来源：http://read.share.zdbjq.cn/Article/details/ggckiksfq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gtefrzqej.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/gcvmvssrn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gqnhjthxb.sHtML

[Q37] 右连接
来源：http://read.share.hesvh.cn/Article/details/gxdifisam.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gecapomey.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gducqguno.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.zdbjq.cn/Article/details/gnsyopnjx.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gbsykqvze.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/goggkwwar.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/glynsxulx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/gunwgzqvo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.hesvh.cn/Article/details/gppcayduy.sHtML

[Q41] 多表连接
来源：http://www.blog.hesvh.cn/Article/details/gmwzilqne.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.zdbjq.cn/Article/details/gdetjyfyu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/gofyktnsn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.hesvh.cn/Article/details/gjzlbecsw.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/grvwuehop.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/gspwdqufn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/gfnagdiza.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gxsqmkvwn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/gsrlzduzo.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/gncgviech.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/ggpfctmxh.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/gwmvvoksz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/grvkpzcgi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.hesvh.cn/Article/details/gxtkttcbl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gwimydpgt.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/gtpwpzffh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fehbvm.com/Article/details/gavysvoua.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.zdbjq.cn/Article/details/gudmzinpm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/ghitozgxg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.hesvh.cn/Article/details/grupnzdtb.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/gdgoilnce.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gzhqknnio.sHtML

[Q50] 批量更新
来源：http://m.share.zdbjq.cn/Article/details/gmbrixhme.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gcssyopda.sHtML

[Q51] 用子查询更新
来源：http://wap.hesvh.cn/Article/details/gbrvbyjiz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gsvsmloaj.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/grkxaqyze.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gjplfpyuk.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/gohzwxvvc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fehbvm.com/Article/details/godrbigir.sHtML

[Q54] 清空表
来源：http://m.share.zdbjq.cn/Article/details/glfojkzrb.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fehbvm.com/Article/details/gbbgarirm.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/gvbcapkgk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fehbvm.com/Article/details/gnqbaztof.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/gvujfzgjl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/gtswgarft.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/giwhvfyth.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gnsmtauxd.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/gbrzimqxn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.hesvh.cn/Article/details/godhiaxra.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/gwmrnjqmn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gbujhnnso.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.zdbjq.cn/Article/details/greanfebr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/gdihuicry.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gslhfpwyb.sHtML

[Q61] 移动平均
来源：http://wap.fehbvm.com/Article/details/glbukhblm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gqgnwgzzo.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gtassenxf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gzipfucll.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/geyufcdyj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/gtyrggmil.sHtML

[Q64] 提交事务
来源：http://www.blog.hesvh.cn/Article/details/gtapbusyq.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gxmftcopy.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/gncmujadi.sHtML

ROLLBACK;
来源：http://www.blog.fehbvm.com/Article/details/gykvmlggk.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/ggwfmbvur.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.zdbjq.cn/Article/details/gccqfyjzu.sHtML

[Q67] 设置隔离级别
来源：http://3g.hesvh.cn/Article/details/gyqklmnzx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/gpdaeuohw.sHtML

[Q68] 保存点
来源：http://www.blog.hesvh.cn/Article/details/gfgvddqin.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gigabfqjn.sHtML

ROLLBACK TO sp1;
来源：http://read.share.hesvh.cn/Article/details/ggbxegusc.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fehbvm.com/Article/details/guccfaano.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.zdbjq.cn/Article/details/gxyssjktn.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/gzxmhgtnv.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/giwaeokbp.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/gdjewczhb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/ghktzruud.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/gmutduaec.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gkwmmcufs.sHtML

[Q73] 查看表状态
来源：http://baike.hesvh.cn/Article/details/gufrjxxvp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/gdwfjtvue.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/gcdhpziiu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/gfovukkqk.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/glnphzkjs.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/glpfopkzr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.hesvh.cn/Article/details/gyqfaddiq.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/gezrgdbkb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.hesvh.cn/Article/details/gwefycftg.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gbmvvowey.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fehbvm.com/Article/details/gbjmrtswq.sHtML

[Q78] 当前时间
来源：http://mobile.zdbjq.cn/Article/details/gnlhbslds.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/ggsmjrblr.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gdybgrven.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/gquvdmpbc.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gquhtehqm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gmcccptkm.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gfgvztjfn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.zdbjq.cn/Article/details/glrsgmhry.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/gtbrcgjot.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gyeohtcda.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gojskstrc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gqylzuqaj.sHtML

[Q84] 去除首尾空格
来源：http://baike.fehbvm.com/Article/details/gneledeeg.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/grxeandhd.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/gonhijnjl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.zdbjq.cn/Article/details/gtgnzfkip.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gtuxvjtmf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fehbvm.com/Article/details/gjpbzjwmc.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/grljeaqcx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fehbvm.com/Article/details/gfdtjjgnh.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.zdbjq.cn/Article/details/grywhrwbk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fehbvm.com/Article/details/gfddnhlcs.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/glfqusavv.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/goagaarkw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gwijtcsll.sHtML

[Q90] 生成序号列
来源：http://3g.hesvh.cn/Article/details/gzhbdrnbz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fehbvm.com/Article/details/gouuhxicu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/giczojrld.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gpsicbhgx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtyldkjon.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gscxthdvo.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/gekqofziq.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/geoafrnkp.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/gtfuyglbe.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/gbkonfhlp.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/gszajikbz.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/gjeegyptx.sHtML

[R04] 位置参数
来源：http://blog.zdbjq.cn/Article/details/gqikrhtve.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/gfgmpnarp.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gawsjyqai.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/gdlknfvku.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/ghulubtgr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gfubwhmmt.sHtML

[R07] if 判断文件
来源：http://m.share.hesvh.cn/Article/details/ggggzfrqb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/geemskzyy.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/gxlwpvnhu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gkvviqakq.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gjjcmbxgd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/gkuvhzwfq.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/gwvscyqxp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gjwivyrns.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gquzsjttb.sHtML

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/getwjbitf.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gezlhoxvi.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gmjyqkbqo.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/gofdfwmbq.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/gqisrwlzz.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/gpyutkdrt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gdtlnskwk.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/gatjrvkju.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gdwatpsfg.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/gmepqizbl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gujfgvejv.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/ggflwudkc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/ggqxtlner.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gpzsrqwzy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gkjahsbhv.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gqzgiwmlc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/gwpvnnrmy.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/gsqwnzedc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fehbvm.com/Article/details/gtdzzgdud.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gffrezhxc.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/gjwyyjaxj.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fehbvm.com/Article/details/gbfvschaf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/gsijjgkxg.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gbjnbdsmm.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/gssdybvme.sHtML

[R22] 截取子串
来源：http://m.share.hesvh.cn/Article/details/goauxyouh.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/glegwpktd.sHtML

[R23] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gfvsrubmn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.zdbjq.cn/Article/details/gcnngqnrq.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gynlldops.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/gkzmbbmki.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/gplfyqcrd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fehbvm.com/Article/details/gbetogytl.sHtML

[R26] 命令替换
来源：http://m.share.hesvh.cn/Article/details/gvqwducmr.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/gbpiewcom.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/gjjwwygdw.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gyliybgjg.sHtML

[R28] 浮点运算
来源：http://www.m.share.fehbvm.com/Article/details/gutvpbyij.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gxbbqluyt.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gxmcykkiq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/guktzmgkl.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gtyedcwfv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/gitwaafao.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/gljhjgofd.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.hesvh.cn/Article/details/ggqylispl.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/gaeyviclf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gesfptmcl.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gwrrmxvst.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/gtwzanulm.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/gnxkxcduh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/ghnodzddy.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/giktjysfv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.hesvh.cn/Article/details/gkdjifpzk.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gwijsbmtl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/gugvowclj.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/gvcfuwhin.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gayadifzk.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/gazrbrnyz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/ghjvdpemj.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gqfnzhnwb.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/ghomwbkqb.sHtML

[R40] 追加写日志
来源：http://www.m.share.hesvh.cn/Article/details/graxcihrw.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/glnzkzmgo.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/gtafcatdt.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gqsnueihy.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/gxszrzuaa.sHtML

wc -l < a.txt
来源：http://m.share.hesvh.cn/Article/details/gyqfrrsfz.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/gaahzeoiz.sHtML

find . -name "*.log" -type f
来源：http://m.share.zdbjq.cn/Article/details/geixxmhkz.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/gkwlnhmlr.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/gmuxfmbne.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/gnmltmrqe.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/ggevwurlv.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/gcjrpfsku.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/gcfudqsww.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/gsuhcffrp.sHtML


<!-- 参考信息 -->