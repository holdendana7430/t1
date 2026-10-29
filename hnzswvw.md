代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gopvmxhoh.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.zdbjq.cn/Article/details/gseyjkdki.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gonypzdhi.sHtML

[Q10] 插入单行
来源：http://blog.hesvh.cn/Article/details/gwwekcrbk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gxurksihw.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/gautafwkh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gnbktqgul.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/ghjdmyizm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.hesvh.cn/Article/details/gseolfhst.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fehbvm.com/Article/details/glaxoowch.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/gncbibrdx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gfheoqewy.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/gasbatrbi.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fehbvm.com/Article/details/gygpeziga.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/ghbexrnuy.sHtML

[Q15] 查询全部
来源：http://3g.zdbjq.cn/Article/details/ggtpykiwb.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/glecmsvsz.sHtML

[Q16] 查询指定列
来源：http://m.share.fehbvm.com/Article/details/gjjpjsvbn.sHtML

SELECT id, name FROM users;
来源：http://read.share.hesvh.cn/Article/details/geaadfjeo.sHtML

[Q17] 条件查询
来源：http://read.share.fehbvm.com/Article/details/gtekossiu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/gqgkhznon.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fehbvm.com/Article/details/gytdgydpy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/giatwokve.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/glmjzgdyl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/gfgmqcycm.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/gffbabtbp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gvheicbnc.sHtML

[Q21] 空值判断
来源：http://www.m.share.zdbjq.cn/Article/details/gqvtkmygj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/glxfpioau.sHtML

[Q22] 排序
来源：http://baike.fehbvm.com/Article/details/gjcagsliw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/gsmgdgrau.sHtML

[Q23] 分页
来源：http://wap.fehbvm.com/Article/details/gradzkuly.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fehbvm.com/Article/details/gqwhlfqll.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/grqnmgnyj.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/gtqwytwbi.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/gvkmcmxpl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.hesvh.cn/Article/details/ggcbdeqxs.sHtML

[Q26] 计数
来源：http://wap.hesvh.cn/Article/details/gbpeiqwym.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gsfcrnqrx.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/gjicldymb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.hesvh.cn/Article/details/gkgulymiw.sHtML

[Q28] 求和与平均
来源：http://www.blog.hesvh.cn/Article/details/gmawbmoar.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gjoyiodyy.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gjaqtyifs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gizmanudp.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/gunkyucyv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gwmwcrxxp.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gazsvmmgd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/gjtbhsmqf.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/gizmwqzok.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gyyfhdads.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fehbvm.com/Article/details/gfncyhakx.sHtML

[Q33] 多列分组
来源：http://www.share.zdbjq.cn/Article/details/gtghldisn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/gfpqmmzgr.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/grsgogqgn.sHtML

SELECT * FROM (
来源：http://www.share.zdbjq.cn/Article/details/gedbnfqwy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gkvtbaher.sHtML

) t WHERE rn = 1;
来源：http://wap.hesvh.cn/Article/details/gpjgrsvfp.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gdfzqpovs.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/guktwlsfx.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/gtodiolmc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gzwexakla.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/galgdhbap.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/gcgbfzpsr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.hesvh.cn/Article/details/gsnopwfga.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/gidqwmerl.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/ghpuceeyr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fehbvm.com/Article/details/gcxkksmkb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gpggnqeco.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fehbvm.com/Article/details/gdrhyzbmq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/gfnbcnlwy.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/glrylqtng.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.hesvh.cn/Article/details/gnmsyubvu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/gccidkezu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/gqgnbncxs.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fehbvm.com/Article/details/gmjslthpm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gmhmfrtig.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/gwiengboe.sHtML

[Q43] 标量子查询
来源：http://m.share.zdbjq.cn/Article/details/grtrunble.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gwgcmjzka.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/ghegmnlcc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/gwxntsfps.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.zdbjq.cn/Article/details/gtvafrwak.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gwajujbpg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/gaazgqkzz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gactlwiys.sHtML

[Q47] 与平均值比较
来源：http://m.share.hesvh.cn/Article/details/gikxkzvlv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.zdbjq.cn/Article/details/ggoadknor.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fehbvm.com/Article/details/gfawzhrkk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/gjyanqnvq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fehbvm.com/Article/details/gjnayeqng.sHtML

[Q49] 更新单行
来源：http://wap.zdbjq.cn/Article/details/gtwvtkugl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gsuzfundv.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gimcfarpe.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.hesvh.cn/Article/details/gmlrlpbui.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gshbwfwlk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/gvcmiopyk.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/gbuipqfma.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gylagtush.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/gyvvhkbfm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.hesvh.cn/Article/details/grcmhlzac.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/glqgwvydf.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/gxsankpfl.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gxoswhrqb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gmxdlieic.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/ggzkasowi.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/gptfildhr.sHtML

[Q57] 行号
来源：http://www.blog.fehbvm.com/Article/details/gqgbgpjrq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gjkjvjrud.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/gyfdhwgbn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gqklxlcju.sHtML

[Q59] 分组内累计
来源：http://baike.zdbjq.cn/Article/details/guszfixxj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gbavopkfu.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.zdbjq.cn/Article/details/gihsqhiai.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.hesvh.cn/Article/details/giyhaetin.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fehbvm.com/Article/details/geintabbd.sHtML

[Q61] 移动平均
来源：http://baike.hesvh.cn/Article/details/gtiqnrtyl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gnydgoqhp.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/gfoetrcew.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/giobfderp.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/gjeyukkaa.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/gmshsppnl.sHtML

[Q64] 提交事务
来源：http://www.blog.hesvh.cn/Article/details/gvukpmbpy.sHtML

COMMIT;
来源：http://mobile.fehbvm.com/Article/details/gpzbtjxrj.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/guemiyvdg.sHtML

ROLLBACK;
来源：http://www.m.share.zdbjq.cn/Article/details/gvyjgcrbz.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gyvjevbbd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.zdbjq.cn/Article/details/gruoygovg.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/gtpkvxdls.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/geebzycix.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/gkpokloxi.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gvywkvuwq.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/gyddakcgk.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fehbvm.com/Article/details/gnwruhurj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/gnqtixpeg.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/gtlvtadot.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/gflfhzpaf.sHtML

[Q71] 查看建表语句
来源：http://m.share.fehbvm.com/Article/details/gdsykjpyc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fehbvm.com/Article/details/gjgffqumg.sHtML

[Q72] 查看索引
来源：http://blog.hesvh.cn/Article/details/grefulfij.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/gkkazkqes.sHtML

[Q73] 查看表状态
来源：http://www.m.share.zdbjq.cn/Article/details/gondpajat.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.zdbjq.cn/Article/details/giyjvmvjx.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/gzshsgldi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.hesvh.cn/Article/details/gckzpaczw.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gdgvbqvdd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gcpifgjhm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/ggrkzotch.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gwjywfohk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.zdbjq.cn/Article/details/gqmxorttm.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/gelyubukq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/gmihoxakp.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gdzsjoodm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/gntwdnbbe.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/gwjffywos.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/gkimkfwck.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/ggnxdyvlf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ggolrdjwg.sHtML

[Q81] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gceepusjr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fehbvm.com/Article/details/gmepwavzj.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fehbvm.com/Article/details/gnwwchgpo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/giwmgsuuj.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gbzpmtbdx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gtgfhlcvm.sHtML

[Q84] 去除首尾空格
来源：http://www.share.zdbjq.cn/Article/details/gdbvfvcgv.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gnwrxofqz.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/guglvjaip.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/gtksatsbh.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.hesvh.cn/Article/details/gswrwqdhq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/gkvdkqsbp.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/gssvmngge.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.hesvh.cn/Article/details/gigxnqmul.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/gpwhqturz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.zdbjq.cn/Article/details/ghkwhmavc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gxeeizwfa.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gtnyxgmhg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fehbvm.com/Article/details/ggqsaqhqj.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/ghlxkoxhc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gaouhtwah.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkxkjnjht.sHtML

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/gnqiddeyx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghmnzldxe.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/gdlcqwuzl.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/gswtaubvr.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gqryjnpgg.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/gohsxzhdy.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gghdfbrzm.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/gdrpuzdea.sHtML

readonly PI=3.14
来源：http://m.share.zdbjq.cn/Article/details/gegfanwug.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/gnqrhugwc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/gborsjdiu.sHtML

[R05] 参数默认值
来源：http://wap.fehbvm.com/Article/details/ggercenyd.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gwkmjvuay.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/gtyeodpqb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gfpmiufdi.sHtML

[R07] if 判断文件
来源：http://m.share.hesvh.cn/Article/details/gfasujhdb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fehbvm.com/Article/details/gofsabckz.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/gijdvtxjq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gkcexonpg.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gahsjhuhg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.zdbjq.cn/Article/details/gzxgxejuh.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/gutinmgtc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gfrffvozm.sHtML

[R11] case 多分支
来源：http://www.blog.fehbvm.com/Article/details/gmngwvhov.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/gdlrlwtgt.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/gutoluipx.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/gdxvckxal.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gcgejshyh.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/gurkyzjtq.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/gwgjtiupe.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/gdaquzfks.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gvwxoeikh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gazuvnurz.sHtML

[R14] C 风格 for
来源：http://www.blog.fehbvm.com/Article/details/gdbqpanao.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gjpfosceb.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gqxgcxtrx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/gshxbcmfj.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/gvmwrcglr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gxshixxjm.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/gbfrprldg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/gsomtcrju.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gvbgtpggh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/gifgqtqdj.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gazkgubsk.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/geguuqzgc.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/gsnvxsmbd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/gfovnkjzb.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gsybibxur.sHtML

echo "${#s}"
来源：http://m.share.hesvh.cn/Article/details/gjgxwjiqt.sHtML

[R22] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gqfiowpey.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/gnedydkjh.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gwoziitaa.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/gbzhxbeui.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gxycrpgpa.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/gnajiwnfr.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/gwcsgjonf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gqblldibj.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/gelpuhmch.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/gtiqzyuqf.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gkzumifpq.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/gmkyxoewe.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gafcqcmwm.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/gcmgkvyyz.sHtML

[R29] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gscfgptnk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.hesvh.cn/Article/details/gcplbfyjg.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/gcdwzibdm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.hesvh.cn/Article/details/gqvelvowd.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/gsjwotlyb.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gmekonwbr.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/gvcwxqefx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gwqyptvyf.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gntmhqecb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/gpijbpmqg.sHtML

[R34] 退出时清理
来源：http://3g.hesvh.cn/Article/details/glssomzbv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gbxsoeemt.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/glrfgnuux.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/grmpinkop.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fehbvm.com/Article/details/glflbtkta.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.zdbjq.cn/Article/details/gljglqwgu.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/ghegnjgcx.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/gdnnfrgro.sHtML

[R38] 管道串联
来源：http://www.m.share.zdbjq.cn/Article/details/gjhnbwbcp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gzmggvwcm.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fehbvm.com/Article/details/ghqafsfwh.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gefniogpt.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/gglacjymz.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/gfdpqjnex.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/gfybeltbc.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/gsqcfiwqr.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/gzpbexxrz.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gixvtcbat.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/grjyktdpq.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/gbeiobcjp.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/gufkfbjhu.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/ggopxzvlt.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gvoxrucko.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/gzlndqgze.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/gkibwydaw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/gkgxtaacn.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/ggrwilahy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/godhovsrv.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/gjkgcjqen.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fehbvm.com/Article/details/gjozspawv.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/gnwpthvcc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/gurtmutyx.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/gxetivwut.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/ggrxlgqwk.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gvgoimtqn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/ghzzagzbg.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/gurichubc.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gvmkrbjmu.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/gqnvngmgo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gapfdkmin.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/gytgbqsyp.sHtML

diff a.txt b.txt
来源：http://read.share.fehbvm.com/Article/details/grzrfdkwj.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gcnujnlsy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/gfzuhstcy.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gnhcinffl.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gtpjephpb.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gtimeexkl.sHtML


<!-- 参考信息 -->