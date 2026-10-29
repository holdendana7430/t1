代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://3g.hesvh.cn/Article/details/gqcgdemku.sHtML

[Q07] 删除表
来源：http://3g.zdbjq.cn/Article/details/gerinccep.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fehbvm.com/Article/details/gtxavecuu.sHtML

[Q08] 创建普通索引
来源：http://mobile.zdbjq.cn/Article/details/glbgtwpht.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gpaswsqjv.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/gquocvemz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gxlbzglqe.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/gdqytebsl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.zdbjq.cn/Article/details/gfdqcqvjs.sHtML

[Q11] 一次插入多行
来源：http://mobile.hesvh.cn/Article/details/gkyvnxxnv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gyhjojmqn.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/giahlfzsr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/gureyaagd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/giomvhrxl.sHtML

[Q13] 忽略重复插入
来源：http://baike.hesvh.cn/Article/details/gpixzlmzb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/glakuwczp.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/gjeshsqqf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/gnpovlngv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fehbvm.com/Article/details/gcmjmswvt.sHtML

[Q15] 查询全部
来源：http://www.share.zdbjq.cn/Article/details/geexlcwvv.sHtML

SELECT * FROM users;
来源：http://www.share.hesvh.cn/Article/details/gpkkhmsfu.sHtML

[Q16] 查询指定列
来源：http://3g.fehbvm.com/Article/details/gfrnkllbb.sHtML

SELECT id, name FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gzczeqsit.sHtML

[Q17] 条件查询
来源：http://read.share.fehbvm.com/Article/details/gvfysxzkp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.zdbjq.cn/Article/details/gmfqorqoa.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/gbrvjkppo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/gyxohbqxx.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/gjniwuumn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/ggcavvumg.sHtML

[Q20] IN 列表
来源：http://3g.hesvh.cn/Article/details/gxvrjynxo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/gnpbsgklp.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gezknuqfg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.zdbjq.cn/Article/details/grczrtlmw.sHtML

[Q22] 排序
来源：http://www.blog.zdbjq.cn/Article/details/gsrhflrlp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.hesvh.cn/Article/details/gfpkkzbor.sHtML

[Q23] 分页
来源：http://wap.hesvh.cn/Article/details/ghtwasfja.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/grsdbkfqq.sHtML

[Q24] 去重
来源：http://3g.hesvh.cn/Article/details/ggqxqpbio.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gfpsuyqae.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/gsyjkilxg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.hesvh.cn/Article/details/gdrcxxgeb.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/gftjjxutz.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/gvxhjpxub.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/gtfcednwt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fehbvm.com/Article/details/ghkneprlt.sHtML

[Q28] 求和与平均
来源：http://www.blog.hesvh.cn/Article/details/gwxyvuvym.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gfpfqndxp.sHtML

[Q29] 最大最小值
来源：http://3g.zdbjq.cn/Article/details/gfjkgwlam.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gpylbhuzh.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/ggnqxefkw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gpintazmx.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/gpbbehqtc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gfrsiwqxh.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/goixhibyz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gbeospudm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.hesvh.cn/Article/details/gsllzczsm.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gqdwzlspr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.hesvh.cn/Article/details/glpojkmqo.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/gredfrjqc.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/ghsuaspst.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fehbvm.com/Article/details/gzpcxktkh.sHtML

) t WHERE rn = 1;
来源：http://mobile.fehbvm.com/Article/details/gfysdomiz.sHtML

[Q35] 内连接
来源：http://read.share.zdbjq.cn/Article/details/gsphsgjbl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gstevtoex.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/gzidpcrxn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/goaatyblq.sHtML

[Q37] 右连接
来源：http://m.share.hesvh.cn/Article/details/gtwxefnyr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.zdbjq.cn/Article/details/gpscnymtu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/gmqapwbip.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gvsqrpezo.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gogdghywh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gcavbwife.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/glfqahiyp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/gffeuafdk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.zdbjq.cn/Article/details/gnmdsizhc.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gyefezywo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.zdbjq.cn/Article/details/gadmkeatr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fehbvm.com/Article/details/gpognifcd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gsjqcawcy.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gcvkwdwez.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gasgsylzo.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.hesvh.cn/Article/details/gujvwqlxc.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gjztwyzdi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/guvhfjuyp.sHtML

[Q44] IN 子查询
来源：http://3g.hesvh.cn/Article/details/gqghvmbzg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.zdbjq.cn/Article/details/gipgdyxgu.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/geliszvbs.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gpfbkngcb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gxhxzjval.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gwzvokicb.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/gfvvyivjj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.zdbjq.cn/Article/details/grhlrkabm.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.zdbjq.cn/Article/details/gixsmbhww.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/geenaldvc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.zdbjq.cn/Article/details/giqjrveqz.sHtML

[Q49] 更新单行
来源：http://read.share.zdbjq.cn/Article/details/gxsauaqfu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/geejhwpzr.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/gvsvbfpys.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/gybmeekpm.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gvfwueird.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fehbvm.com/Article/details/ggvjsufth.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/gbbyzdqta.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gdakjtcvi.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/gkuyopgti.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gxpwkryrv.sHtML

[Q54] 清空表
来源：http://m.share.hesvh.cn/Article/details/gwifabgmj.sHtML

TRUNCATE TABLE logs;
来源：http://wap.hesvh.cn/Article/details/gkzsergxd.sHtML

[Q55] 排名（并列占位）
来源：http://baike.hesvh.cn/Article/details/gftqcvjwq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gekbswhrd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/gpeyiayom.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gymehjmhg.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/gjxxdydvp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gtwqrxcpp.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/gjljgjqfv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/grwlkhjkz.sHtML

[Q59] 分组内累计
来源：http://blog.fehbvm.com/Article/details/gwdorczcu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gzyzjhocf.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.zdbjq.cn/Article/details/gyuugvenl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.hesvh.cn/Article/details/ggzxdtnoc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gowkxelep.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/gfetcaprk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gegbaveud.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/gzmvwvkkx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/ghejnmdyg.sHtML

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/gvwmxydcn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/ghqphnhky.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/gelmuqorz.sHtML

COMMIT;
来源：http://m.share.fehbvm.com/Article/details/giyltxklh.sHtML

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/gnujxsdyz.sHtML

ROLLBACK;
来源：http://baike.hesvh.cn/Article/details/gmxofhanw.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/gyletoinc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/gctavvyrd.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/gjwupmhfe.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/gdcvivgrb.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/gmgzutiap.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fehbvm.com/Article/details/gvxbeukkq.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/gktjenjey.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/gfykardfb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/gahwfyfvr.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/gejufsoft.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/gvsouvobh.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/gsnvidouv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/gqznevhvi.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/gaxjvmmlw.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/gfvjofain.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/gziyadceh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gfqxkpary.sHtML

[Q74] 强制使用索引
来源：http://m.share.hesvh.cn/Article/details/gejmrmkbc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/gcolbitnu.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/ghwwzqggl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/gygejdeuy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.zdbjq.cn/Article/details/ggpjhijce.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/glwmvqcke.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/gqsbvcyze.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/gaocltczu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/gjtgukvcf.sHtML

[Q78] 当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gmazpxyqm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gavnolrkd.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gfesvwetr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gsyuilfng.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/gbdtivelw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gabfnonat.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/geuqhhole.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gbjsmmhnr.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/gdxvbqtsd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gidgjzcth.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gbsjrvclj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gkpvfzdvu.sHtML

[Q84] 去除首尾空格
来源：http://3g.fehbvm.com/Article/details/grfnivpsy.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gznijwjcb.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/gohcqlyei.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/gtqqdxrni.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fehbvm.com/Article/details/gmhfsokiy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/gfeycbzed.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/gdpckaigo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/grjxgmznl.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/gigtfedzy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/gefbwbqoh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/giptnbjon.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fehbvm.com/Article/details/gspetcgsb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/gcbtieoul.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gzkhqsdhg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/gbiiqutpz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghuteanqw.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/grjrmpujx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gyuygsoco.sHtML

[R01] shebang 与严格模式
来源：http://m.share.hesvh.cn/Article/details/gksvnqhym.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.hesvh.cn/Article/details/ggrwpbmeh.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/gqmeutrmp.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/gsokjuqpb.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/gmmaffobw.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/gxvdbdsak.sHtML

readonly PI=3.14
来源：http://wap.hesvh.cn/Article/details/gytjogrcn.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gitcaxevf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fehbvm.com/Article/details/gihdmjpch.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gtnoyikgw.sHtML

name="${1:-default}"
来源：http://3g.zdbjq.cn/Article/details/gmpumcemh.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/gdtzyqirg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/ggdxjmpzo.sHtML

[R07] if 判断文件
来源：http://www.share.zdbjq.cn/Article/details/gffbtxavg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gzeujwgtx.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gcynykget.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/gjqfappmz.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gjgvjbckp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/gmgrkcgwz.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/gveuwfico.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.hesvh.cn/Article/details/gzhyptttb.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gwdmjgjlg.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/gfhtsilpw.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/ghyqppngo.sHtML

stop)  echo "停止" ;;
来源：http://3g.hesvh.cn/Article/details/gimzkkyfc.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/gwyniwebx.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/gzzngvelo.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/ghgmsonkm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.zdbjq.cn/Article/details/gmhvqkxfo.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/gnuypqstn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gaflwwwvu.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/ggqmqhyks.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gcvzpaeez.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gbznmzkpe.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/gbcwypcju.sHtML

[R16] until 等待条件
来源：http://m.share.hesvh.cn/Article/details/gxrftavza.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gdcbldlpa.sHtML

[R17] 数组定义与取值
来源：http://baike.hesvh.cn/Article/details/gjectarvx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.hesvh.cn/Article/details/gpdlhrvnn.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/gzdrwsboj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/gjiptkvgk.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gfjxwunfz.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/gwaevtcfh.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/gchuedifl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/grunqbvit.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/glglueuhd.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/gygaqvkkc.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gvohxvyvc.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/godnzbaow.sHtML

[R23] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gsdpcvbth.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/gcfzdhvtj.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gsfbyxxud.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/gnojrkuzs.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/gwrczxbkl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gpnxkaqwb.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/gmdplfuht.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.zdbjq.cn/Article/details/gyebqvqdf.sHtML

[R27] 算术展开
来源：http://blog.zdbjq.cn/Article/details/gbnhapjnz.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.zdbjq.cn/Article/details/gawnxfjaa.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gqylatsmb.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/gvvgglcod.sHtML

[R29] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gifbitcal.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/govzefqzr.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/gilquobny.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/gybegsduw.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gugldmcye.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gfzandlsy.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/gekkhzxns.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gjcohemig.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/grfsgwlfs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/gmugtlrmi.sHtML

[R34] 退出时清理
来源：http://www.blog.zdbjq.cn/Article/details/gllqkdcut.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/ghfvkorff.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/goimkihar.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/gpcxzsadt.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fehbvm.com/Article/details/gjybqkclw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/gfitaokoe.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/gtyhjhyof.sHtML

files=$(ls -1)
来源：http://3g.hesvh.cn/Article/details/gaipoqusp.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/guptifvxa.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/gmiivajsv.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fehbvm.com/Article/details/gklaosiwv.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gdvxyudmv.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/goddhgcnh.sHtML

echo "log" >> out.log
来源：http://wap.zdbjq.cn/Article/details/gnwxfidim.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/gakpwgkli.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/gtfdpxndn.sHtML

[R42] 输入重定向
来源：http://m.share.fehbvm.com/Article/details/gaoqsrmjd.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gaxhhkxrm.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/ghywkbocc.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gdpbxpqoq.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/gxgvaaobv.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/gfarejmge.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/glycaapkz.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/gjgnhavzf.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/gknoxoset.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/gnfbjwjed.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fehbvm.com/Article/details/gvpysfihw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/gupkugcop.sHtML

[R48] awk 取指定列
来源：http://www.share.fehbvm.com/Article/details/gqwkutxpj.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/garzdmqfu.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/gyfdsyxos.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/gfqijspvr.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/goiuyepme.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/ghwjzetmg.sHtML

[R51] 排序去重取前几
来源：http://m.share.zdbjq.cn/Article/details/gqoswatdx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/gwrpspbvl.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/gxcocnyzc.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gzwsatjqi.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gupbtdvnx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/grhevrkfa.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/gbdzulokt.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gijpnuats.sHtML

[R55] 压缩与解压
来源：http://mobile.hesvh.cn/Article/details/gohzwlmyh.sHtML


<!-- 参考信息 -->