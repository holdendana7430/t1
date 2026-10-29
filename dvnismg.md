代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gfuklhwhr.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/gnlioiqyq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/glcpcqvag.sHtML

[Q10] 插入单行
来源：http://blog.hesvh.cn/Article/details/ggumsavmm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fehbvm.com/Article/details/gbqslkxyo.sHtML

[Q11] 一次插入多行
来源：http://www.share.hesvh.cn/Article/details/gjtryevaf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/ggwtmjopo.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.zdbjq.cn/Article/details/ghyeaoglp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/gwvikqplo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fehbvm.com/Article/details/girxyjqlz.sHtML

[Q13] 忽略重复插入
来源：http://3g.fehbvm.com/Article/details/giqhgcxhq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/guamympcj.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gyilioywj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.hesvh.cn/Article/details/gljgicgyh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.hesvh.cn/Article/details/gjqnpnlmr.sHtML

[Q15] 查询全部
来源：http://blog.zdbjq.cn/Article/details/gvsnsiacl.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/glgywrslj.sHtML

[Q16] 查询指定列
来源：http://read.share.zdbjq.cn/Article/details/gljewstyp.sHtML

SELECT id, name FROM users;
来源：http://read.share.hesvh.cn/Article/details/golamvgnw.sHtML

[Q17] 条件查询
来源：http://wap.zdbjq.cn/Article/details/gidcygipu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gxvexrvra.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/gztyjddpq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/gkkcxoocg.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/gefbycnct.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.hesvh.cn/Article/details/gsnkxzdgv.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/gsgvcxozf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.zdbjq.cn/Article/details/ghzwoptme.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/grqotzbpx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/glnvomiqt.sHtML

[Q22] 排序
来源：http://m.share.hesvh.cn/Article/details/gqutrwexk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.hesvh.cn/Article/details/gpoixshsy.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/gmnwlvphz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/gyfnulvdn.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/ggjdjhleg.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/glymckklu.sHtML

[Q25] 只取前 N 条
来源：http://3g.zdbjq.cn/Article/details/gpjqopxiu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gybwjvgdx.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/gqfosbmyw.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gqrgmodiv.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/gvzbqfqaz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gwgwwoqxa.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/gpsswegne.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gkrafyadg.sHtML

[Q29] 最大最小值
来源：http://3g.zdbjq.cn/Article/details/grutohpvn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gbunzzoha.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/ghrsigfev.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gmgqxfexj.sHtML

[Q31] 分组后过滤
来源：http://wap.zdbjq.cn/Article/details/gmfnmongj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gfgswppcf.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fehbvm.com/Article/details/gzokohfmm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gfgqlxeyr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/gdubaoamr.sHtML

[Q33] 多列分组
来源：http://baike.zdbjq.cn/Article/details/gzcpoaepn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gckyhsizm.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/gbbayyygk.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/gshgiiigo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/gfrgsergv.sHtML

) t WHERE rn = 1;
来源：http://m.share.hesvh.cn/Article/details/guvcyubbn.sHtML

[Q35] 内连接
来源：http://wap.zdbjq.cn/Article/details/gieyzetww.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gybrobkch.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/gtepctwjp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gmsqycshl.sHtML

[Q37] 右连接
来源：http://m.share.fehbvm.com/Article/details/gdpnqwgvd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gcmmhpshm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.hesvh.cn/Article/details/grgpubgjy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/gbpqvjihh.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/gubxavfyp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gtuvrovai.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.zdbjq.cn/Article/details/gbgdbpapp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/guskeqryw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fehbvm.com/Article/details/gilerctoe.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/grvbzzcxk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/guurhjvbb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/gccillfcm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gmlycckjq.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.hesvh.cn/Article/details/gefizotpe.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.hesvh.cn/Article/details/gkhjwztxu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/ghuncxpka.sHtML

[Q43] 标量子查询
来源：http://3g.zdbjq.cn/Article/details/gapronwrj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gxezyhynt.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/gfdupyyhc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fehbvm.com/Article/details/ghuxrcqtn.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.zdbjq.cn/Article/details/ghoovhhji.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/grklhecfv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/ghlphvjex.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gobdpiiox.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/gvqugkcxd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fehbvm.com/Article/details/gnkbwcokj.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.hesvh.cn/Article/details/gaeevpmce.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/glsdpjobf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.hesvh.cn/Article/details/gsvzjtvqf.sHtML

[Q49] 更新单行
来源：http://3g.zdbjq.cn/Article/details/gbjentdoj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gaxhugvcd.sHtML

[Q50] 批量更新
来源：http://m.share.hesvh.cn/Article/details/gbzldhvjs.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gyitnfczv.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/grpbnhjfg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/gmfvxdkwz.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/gofqipsqi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/grjgfuwlq.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/gmbbhwfpv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gmmmjeuzo.sHtML

[Q54] 清空表
来源：http://baike.hesvh.cn/Article/details/gwitjaslm.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/gsslxurbx.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.hesvh.cn/Article/details/gqmwqtaap.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gjhhobwbi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.hesvh.cn/Article/details/gigiledhu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gmismbrnd.sHtML

[Q57] 行号
来源：http://www.share.zdbjq.cn/Article/details/gjfybxhuo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/gjlyzacvr.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gcpyhbjix.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gdgukbshc.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/gkkyolsza.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gveqsjnbe.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/gppvsdmxy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/gehfmwaao.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gpkxnrqcu.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/gkdrunbwd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gupqwzash.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/gbbzxwxqt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gkgcvodek.sHtML

[Q63] 开启事务
来源：http://mobile.hesvh.cn/Article/details/geqdlfxap.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fehbvm.com/Article/details/ggoywzkuk.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/gvetnwuac.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gkjqmbtuh.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/gzitguvio.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/gvonbegoq.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/geqdxufin.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/grbnppruy.sHtML

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/gnszkhhjh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fehbvm.com/Article/details/gohhjpbem.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/gnkrgtoev.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/gpgllakyg.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/gwusabjuj.sHtML

[Q69] 查看执行计划
来源：http://m.share.zdbjq.cn/Article/details/gobcszdfd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/gafagiolv.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/gyxyqedzd.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/gufguauju.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/gdwcubzkm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.zdbjq.cn/Article/details/gzselcotn.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gvxyopond.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fehbvm.com/Article/details/grzzrueug.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/gkwwmfymv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/grvxrajnc.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/glxpgkeoc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/gulneqaom.sHtML

[Q75] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gixjsbrqe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gjdofmyhm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/genmtuyqf.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/gshvqbczq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/gqzgjbbeu.sHtML

[Q77] 时间加减
来源：http://www.blog.zdbjq.cn/Article/details/ganqesznf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.zdbjq.cn/Article/details/gilfnzpik.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/ghcwqqqco.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gwoeltcly.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gsvuzrsol.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/guwvrzibe.sHtML

[Q80] 字符串截取
来源：http://www.blog.hesvh.cn/Article/details/gsclxrvtn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gifyvtjqb.sHtML

[Q81] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gndbbbxbi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/glisszdbe.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.zdbjq.cn/Article/details/gohtbqmck.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/guthtwzcq.sHtML

[Q83] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gmnadfvqh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gkrgqzazp.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/gdhhuicpl.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gbvnrtqii.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/gakbecdhp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/gfckwchpp.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fehbvm.com/Article/details/gufbjvhau.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.zdbjq.cn/Article/details/gblgdpjvi.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/gmxjdkpwc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/gntphnije.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fehbvm.com/Article/details/gtjvxzchc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gazqahklq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/gfnweptgh.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/gugkfzvzt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gueikhven.sHtML

[Q90] 生成序号列
来源：http://3g.hesvh.cn/Article/details/ggzhmoaxl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/gzmuogebd.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gseaayynp.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gzsyqksaq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkqvgsfkd.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/gtfrhjfur.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/gmnpxqzup.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/gkghcjffu.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/gebhptpqt.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/gcprjuazt.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/goymsscnc.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/goykbchbf.sHtML

[R04] 位置参数
来源：http://baike.fehbvm.com/Article/details/grntnckap.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/gxmtblvsw.sHtML

[R05] 参数默认值
来源：http://baike.zdbjq.cn/Article/details/gzqchwvve.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/gswypqrtk.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/gzwfmdnvl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gsouxzczt.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/gkyjzjsal.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/gwrnraxom.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/ghrrnesim.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/gkutjfcon.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gdsbpsdnx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/gmhtdbngj.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/gkrhrkipz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gekbbfbkj.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/gtonxuper.sHtML

case "$1" in
来源：http://read.share.zdbjq.cn/Article/details/gwvajcjyb.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gzjplrwna.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gfbeueuph.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/ghzfsqxue.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/gyfefzcdw.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/gcfubcdax.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.hesvh.cn/Article/details/gyhhxecco.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gcuebwcsp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gzfdoupnx.sHtML

[R14] C 风格 for
来源：http://read.share.zdbjq.cn/Article/details/gajyodier.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gthammoel.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gmarjcwke.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/gwmjqwebz.sHtML

[R16] until 等待条件
来源：http://3g.zdbjq.cn/Article/details/gfqnqgnug.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/grfhbwzuj.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/gpczqgorv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gulotbcpl.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/gdyjijysd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fehbvm.com/Article/details/gpevwkkgj.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/ghizhjkyp.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/gtfnyxxok.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/guytrvdap.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gazxxksti.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/glanfplea.sHtML

echo "${#s}"
来源：http://wap.zdbjq.cn/Article/details/gspongdwg.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gwuzbjwah.sHtML

echo "${s:0:5}"
来源：http://www.blog.fehbvm.com/Article/details/gfresttpy.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gacfmpetc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.hesvh.cn/Article/details/gxwazwnbe.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gukkkhyyj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/gdhwzutzi.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/gxzgnjjte.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/gjoyuhhbx.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/glputlagx.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.hesvh.cn/Article/details/gneefteet.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/gbmolaqhz.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/gxibptkny.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/galldzrhp.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/gqlqfyqbr.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gwbflzrvw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gsextmkth.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/gufbxmqag.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/gweqpbfcm.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gvepgzquz.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/grhetpwun.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gmqeqpslt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gpvfvsyqg.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/gdmssqwly.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/gvkvndaze.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/gaigvfyzr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/ghrezbqge.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/gpzincqsk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gbfkgvzgb.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.hesvh.cn/Article/details/geszuyjgc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/gnrriispt.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/gqeizyece.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/gvanrbejc.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gzvupenzt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.hesvh.cn/Article/details/gzxmwzdol.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gurkjkbsq.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/gmjxbljvg.sHtML

[R40] 追加写日志
来源：http://baike.zdbjq.cn/Article/details/gjtjwlrse.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/gqjvvnsam.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/gjqdsqvqq.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/gzoogtaho.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gkfkgsldc.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/glrhreldo.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/gzocxpvop.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/ggnejytnk.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gktowqaii.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/ghbzgwlof.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/gyndkolrz.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/ggmulmygb.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gjdzhwnzp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/glucmjxhz.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gswrfcweo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.zdbjq.cn/Article/details/gemzewesw.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gzvowowoj.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gkvywhmfo.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/gtenpadxi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/ggqctyese.sHtML

[R50] awk 求和
来源：http://wap.hesvh.cn/Article/details/gorgknqbc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gyttjnmuo.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/gnbknvpdk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/gxhdjsjwc.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/gfmwbyfme.sHtML

wc -l a.txt
来源：http://mobile.fehbvm.com/Article/details/gnuycxakn.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/gcdrapgpr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/glkczaflu.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gqekocpxa.sHtML

diff a.txt b.txt
来源：http://wap.hesvh.cn/Article/details/gbqmpgcvt.sHtML

[R55] 压缩与解压
来源：http://wap.fehbvm.com/Article/details/gpzbiyiwe.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/gtcumsteh.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gsoqritgx.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/gcqixrhfw.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/gqzsxhpol.sHtML


<!-- 参考信息 -->