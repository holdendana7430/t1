代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fanxiaobao.xyz/Article/details/geoorvzmn.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fanxiaobao.xyz/Article/details/geswaznfp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgjyurhy.sHtML

[Q10] 插入单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gjawymodh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsssmgikd.sHtML

[Q11] 一次插入多行
来源：http://baike.fanxiaobao.xyz/Article/details/gfjrlvqeq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/grtxtfjfu.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fanxiaobao.xyz/Article/details/gsapwccco.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fanxiaobao.xyz/Article/details/gofdskirx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fanxiaobao.xyz/Article/details/gyqirjabf.sHtML

[Q13] 忽略重复插入
来源：http://baike.fanxiaobao.xyz/Article/details/gzskjbagx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gumgabjbh.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fanxiaobao.xyz/Article/details/glzmcrgnm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fanxiaobao.xyz/Article/details/gzykxzqwd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fanxiaobao.xyz/Article/details/gossqpcnh.sHtML

[Q15] 查询全部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgjvsxgo.sHtML

SELECT * FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gkikwabap.sHtML

[Q16] 查询指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxzayuqe.sHtML

SELECT id, name FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gwetvleud.sHtML

[Q17] 条件查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzdrgrkl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupjhezno.sHtML

[Q18] 模糊匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gvrztqqbw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fanxiaobao.xyz/Article/details/gtplmoflz.sHtML

[Q19] 范围查询
来源：http://baike.fanxiaobao.xyz/Article/details/gakgeztcm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvscylqx.sHtML

[Q20] IN 列表
来源：http://wap.fanxiaobao.xyz/Article/details/goahclcme.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvouocks.sHtML

[Q21] 空值判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsjgumoy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fanxiaobao.xyz/Article/details/gbphjurzh.sHtML

[Q22] 排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdbzhahf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fanxiaobao.xyz/Article/details/gtfpmevat.sHtML

[Q23] 分页
来源：http://wap.fanxiaobao.xyz/Article/details/gueivotej.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzitxoapw.sHtML

[Q24] 去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gpipdeopu.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuzgjlxl.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcwslyul.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fanxiaobao.xyz/Article/details/gpdeljaey.sHtML

[Q26] 计数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkknzhvc.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjyvqllu.sHtML

[Q27] 条件计数
来源：http://www.share.fanxiaobao.xyz/Article/details/gaymvmomq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwmvslvq.sHtML

[Q28] 求和与平均
来源：http://3g.fanxiaobao.xyz/Article/details/gbomtnyiz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnmxzcog.sHtML

[Q29] 最大最小值
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmhfocen.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzjrlwhm.sHtML

[Q30] 分组统计
来源：http://3g.fanxiaobao.xyz/Article/details/gbbwvwxgj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gjyfmangn.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqnfpruc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gtbwxkvol.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/giyggjdaj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnavfjzwi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjkytowp.sHtML

[Q33] 多列分组
来源：http://blog.fanxiaobao.xyz/Article/details/gnjkqhcuz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fanxiaobao.xyz/Article/details/gkflpvneo.sHtML

[Q34] 每组取第一条
来源：http://m.share.fanxiaobao.xyz/Article/details/ginzulbpf.sHtML

SELECT * FROM (
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkbroodr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fanxiaobao.xyz/Article/details/gryxkbaye.sHtML

) t WHERE rn = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkczaxhb.sHtML

[Q35] 内连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftqtfxci.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gcgfrdgbz.sHtML

[Q36] 左连接
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqnzifao.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gqetazzlu.sHtML

[Q37] 右连接
来源：http://wap.fanxiaobao.xyz/Article/details/gniacwuqz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gbunzmpxf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtkntnsb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gectebkkm.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fanxiaobao.xyz/Article/details/gmswqkmbi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fanxiaobao.xyz/Article/details/gfspzjulh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdtzviig.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqqfqcap.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fanxiaobao.xyz/Article/details/gbxcvjmmc.sHtML

[Q41] 多表连接
来源：http://baike.fanxiaobao.xyz/Article/details/gejdaapuv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fanxiaobao.xyz/Article/details/gvwkofrxt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjdoihom.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fanxiaobao.xyz/Article/details/ghxyuruje.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjixcqfl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fanxiaobao.xyz/Article/details/gqntnbdom.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvsweglp.sHtML

[Q43] 标量子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gsizgvjde.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzkymklb.sHtML

[Q44] IN 子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/ghryyotlj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgbrkjtx.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxyginvc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdljnyzul.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fanxiaobao.xyz/Article/details/gftvfchdf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gibgivofc.sHtML

[Q47] 与平均值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gftkdltja.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkacawgq.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gamulifxg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fanxiaobao.xyz/Article/details/gwhcvtjme.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gbwgzuezt.sHtML

[Q49] 更新单行
来源：http://wap.fanxiaobao.xyz/Article/details/gurmhxzal.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gghrrlbnv.sHtML

[Q50] 批量更新
来源：http://baike.fanxiaobao.xyz/Article/details/gttigftnh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gufajcoxg.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnavgxbbm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidippibj.sHtML

[Q52] 删除指定行
来源：http://3g.fanxiaobao.xyz/Article/details/ghcqtgbee.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gawfgvyal.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjklabgzn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxirjldp.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/gekwvfptv.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkyxmxju.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gslajlzqu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/goqyiryta.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjjkttbh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gxhmaxfjy.sHtML

[Q57] 行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgwqscno.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gmisiiftf.sHtML

[Q58] 累计求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gugmxzrsp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glahbjsbq.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpcwdlat.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gocxprfuz.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtvipypm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fanxiaobao.xyz/Article/details/gcqjelqcw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvcgdzbi.sHtML

[Q61] 移动平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojiktktq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbtgnbvi.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/gelxrikrs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gpdscuhil.sHtML

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyslbdny.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmnsgqzv.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwcisbjc.sHtML

COMMIT;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdbjojek.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gljgeodlt.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/gvqehhglg.sHtML

[Q66] 行锁查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gapyzzjfd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fanxiaobao.xyz/Article/details/gfkpbkgzk.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/gviaqpfev.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fanxiaobao.xyz/Article/details/gcubycxaf.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/gzcsugyvz.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gatvpyuzx.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnmlmpns.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/giybszmwv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsovuako.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkorfkifh.sHtML

ANALYZE TABLE users;
来源：http://3g.fanxiaobao.xyz/Article/details/gcopdsbpk.sHtML

[Q71] 查看建表语句
来源：http://read.share.fanxiaobao.xyz/Article/details/gsosmwoek.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgpdjlyt.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkenagtwq.sHtML

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gbwsuinng.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gesacsqnv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqicjsyrv.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/gurbmsmrv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcewgkvec.sHtML

[Q75] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gelrlavfu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyoqghubb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/gomthqzyj.sHtML

[Q76] 按天统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfxogvqf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbovyeft.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsydkuqjk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/gxexjxlvg.sHtML

[Q78] 当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/giosxinzh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fanxiaobao.xyz/Article/details/gilatpjal.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/glvwwhhoj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/gqfimfxkd.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/gljiudyns.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfmellov.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gqcojhxqa.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhxzjfdj.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gqitcgzyb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnaqlnddg.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlsupxdd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gptvnrjow.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/gavaawkjj.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqnjxpcv.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/glopmgqlz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgvvravs.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmijteqp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/glplhdkzo.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gctbkppif.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/girptshzd.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/glqzzzxsl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmvghyxq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/ginhyfmds.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfrewszu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gdmdrjupk.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/gefowrebu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fanxiaobao.xyz/Article/details/gzqpsgvlf.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/goshrikee.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrvsqooz.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gxpebyybg.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/grlrxmqsh.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzkziooa.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/girzcliez.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gottmsmaf.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gllslitqu.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/ggoqbddol.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glerlqfhi.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gvqnwbkfr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlpfydvi.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gyskvtnau.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gwrsnggxs.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gdduuzzjp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfwtjbrs.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbitvoul.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gautvnulb.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxvgivpq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/grrgfmwxr.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbttkyka.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvrmrqar.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxgkcwbk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfkryndn.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcqsfvkh.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/gixdzskvt.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgtwksbi.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/guhpbrave.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/geiidnqck.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gwwntrame.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvebgbcgz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gnbpyaihw.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gvuvolobq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/groxcvdqy.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/guzbjfjcm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gcfspihvy.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gaanmzfjm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/giesdvipy.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjysgdlz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqpzlbwr.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfbkdzvi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gdhzrookb.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/goxtxewek.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gvybndkjl.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gvbhixfyv.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gelrpewbp.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gazmxulop.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gjqrvwizd.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfbmjchi.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gybsvtqld.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgnbapyy.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvjpbthg.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gaiqznhwe.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gdomfprwu.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gpojrtmox.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gadlavyfz.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhniqteq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gaehuzhmg.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuzhyafg.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gcujhuemd.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gqiemwglh.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnmbqfun.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxibpkte.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gnvtxnzia.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gtqqhcmhy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtevrdouh.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gallqjake.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmveuxki.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgxhulgc.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gccwyftht.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjrmsqov.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsunxwpel.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gpfhaoupx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gfikmhpfm.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gxopdmaez.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjaxjkfs.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gdswrerbr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghuklemcb.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/giizorjha.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcgappbu.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gugzhmuyh.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjivfikkf.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gjgnzsusx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gomhnguhi.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/grsxmfypz.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuiwgjqu.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcgrcjeg.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gftqafejc.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gacbjiwed.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gqrofjugu.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhiajbrd.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/guzcaeism.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/giyktapwr.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gqouxikwo.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgjyifrc.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gtabiltde.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gybdccawd.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwuxzvwk.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glycyvpzi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/ghwvwnspz.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gfsichvla.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpuszjhx.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnovoymg.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjpgqybw.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/golttwnxl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfepivqly.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/grircrszf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ggvaacgij.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdzucfrd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gwxzubgkj.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwnqgvbi.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvosltxa.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gopbtwqfw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gisbrogqw.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gkzjcydbk.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gnsiibjiz.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxkwkfug.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gpcwructi.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gcavetlal.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/grgwnnutm.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhitpdby.sHtML


<!-- 参考信息 -->