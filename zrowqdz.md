代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/gcupyhusc.sHtML

[Q05] 重命名列
来源：http://3g.zdbjq.cn/Article/details/gpwdivqui.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/gmzzmhmsj.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/goyssxmzi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.hesvh.cn/Article/details/gyufxaxat.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/geyrihwtv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/gqwtdoqdh.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/gssjxditu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gtxnwwhzr.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/gvpmbfxxx.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/guzxjwmlo.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/gqxhorzwu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.hesvh.cn/Article/details/gbmiqatku.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/gpufhatzk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/gthxjxjka.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/gxekrgccl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/giutnsrlw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.zdbjq.cn/Article/details/gwsdwihxl.sHtML

[Q13] 忽略重复插入
来源：http://baike.hesvh.cn/Article/details/gkfqfpmay.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gsyoxwmpg.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.zdbjq.cn/Article/details/gyaspdpce.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/gswfchetp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fehbvm.com/Article/details/gfuobblle.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/guxjjnuac.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/gkhqbmttw.sHtML

[Q16] 查询指定列
来源：http://blog.fehbvm.com/Article/details/gsszwyxox.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gygjrsemq.sHtML

[Q17] 条件查询
来源：http://read.share.zdbjq.cn/Article/details/gxvzlitpw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.hesvh.cn/Article/details/gaefmykvy.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gskdyvdiv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.hesvh.cn/Article/details/gqotyvyth.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/gqfrvmncl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.zdbjq.cn/Article/details/gvzqsicyy.sHtML

[Q20] IN 列表
来源：http://www.share.hesvh.cn/Article/details/gfyjdjvlq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.zdbjq.cn/Article/details/grcodabdn.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/goqjywftj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/gvmltiqlq.sHtML

[Q22] 排序
来源：http://www.blog.zdbjq.cn/Article/details/grycftfkf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.hesvh.cn/Article/details/gwewahxqj.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/gtwcaaitg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/gntqobrfy.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/guungzhaz.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.zdbjq.cn/Article/details/glpbbdgle.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/gvhvkvfic.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gmsednvko.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/gbkbrkghz.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gmztgkjne.sHtML

[Q27] 条件计数
来源：http://read.share.zdbjq.cn/Article/details/gftptlqse.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gayxwojwz.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/geatwllvq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/ghymgvjlk.sHtML

[Q29] 最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gbkrzzvjw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gkzhgicxj.sHtML

[Q30] 分组统计
来源：http://baike.fehbvm.com/Article/details/grzaoysqo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gxcruhltu.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/gnixcnerr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gjjnxmbxv.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fehbvm.com/Article/details/gcutyauaf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gyhozkmkq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.hesvh.cn/Article/details/gxkvjrbfr.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/gfwufbbcg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.zdbjq.cn/Article/details/gqpliccvi.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/gdlwriuhy.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gyprtuibv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fehbvm.com/Article/details/gprcnncfo.sHtML

) t WHERE rn = 1;
来源：http://baike.zdbjq.cn/Article/details/gbdfyqity.sHtML

[Q35] 内连接
来源：http://m.share.fehbvm.com/Article/details/gnwtldjgq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gyittchjr.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/gocjepeqf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gcakkiilm.sHtML

[Q37] 右连接
来源：http://read.share.hesvh.cn/Article/details/gigplhmgh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/gftqvycal.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/grhnblewf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/gckltsbmo.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/gghewvmmn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gajskybbc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/gvcufuaxz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fehbvm.com/Article/details/gddpyjjjf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/gjppbsmyr.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/gxvmkdynb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/glgidwvti.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fehbvm.com/Article/details/ggbdyaxim.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/glvoogmjp.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.hesvh.cn/Article/details/gnqqqytaw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.hesvh.cn/Article/details/guhttexxy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/gzgxeppoy.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gtcfxsnqw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/gpjzpefxo.sHtML

[Q44] IN 子查询
来源：http://read.share.fehbvm.com/Article/details/guymiaiti.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gpukhrpzt.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/gorqkvuvw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gjqcvhbev.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gpgrezxui.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gcwdluvho.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/gffesaopc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gimwfxwib.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/grbhpjrzw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/grsfwbuaw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/gugklolgn.sHtML

[Q49] 更新单行
来源：http://www.m.share.zdbjq.cn/Article/details/gdurggjse.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gzbponckc.sHtML

[Q50] 批量更新
来源：http://3g.zdbjq.cn/Article/details/gjlocvcfp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fehbvm.com/Article/details/gwllpcwgf.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.hesvh.cn/Article/details/gbpxlknwv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/grmjouvpz.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/ghllmnrmb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gltlrbwek.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/gghbxkdhw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/gqjmujgim.sHtML

[Q54] 清空表
来源：http://wap.fehbvm.com/Article/details/gdpwdxsdj.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/geefxqjls.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.hesvh.cn/Article/details/gcuidzkbk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.hesvh.cn/Article/details/gdhptuqfu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.hesvh.cn/Article/details/gwgabwumh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gthaclskp.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/gygfkasle.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.hesvh.cn/Article/details/gfiseocqn.sHtML

[Q58] 累计求和
来源：http://www.m.share.zdbjq.cn/Article/details/gmyopxtah.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gsgvesktn.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/guliaxnkn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/ggcolyogv.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.zdbjq.cn/Article/details/gkelhkecy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.zdbjq.cn/Article/details/granxvkuf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/ghydtlukb.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/gskokkixw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/grkjvkjad.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/gixxjtdlz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gahwkjsbd.sHtML

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/ggsnkandg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fehbvm.com/Article/details/gufabvuuc.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/gqdowyizv.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gtrfynicy.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gkpsiizrm.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/gycrghlai.sHtML

[Q66] 行锁查询
来源：http://read.share.fehbvm.com/Article/details/gwqdkhpqd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.zdbjq.cn/Article/details/gstiavcpi.sHtML

[Q67] 设置隔离级别
来源：http://3g.fehbvm.com/Article/details/gtkiezxvn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/grxbjyjrn.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gnrhouupg.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gwcuplsdd.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/gcfkkpqll.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gnwjljzzd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gqcuckreo.sHtML

[Q70] 更新统计信息
来源：http://m.share.hesvh.cn/Article/details/gqbjezzvf.sHtML

ANALYZE TABLE users;
来源：http://3g.fehbvm.com/Article/details/gcerzhjjw.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/gmsgnfqcf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/gqnktjgwx.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/gfenjcebh.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gwgxrqhkn.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gxukbabbk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fehbvm.com/Article/details/gounxrmrs.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/gejegpbcs.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gafxunncw.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gnrjkranp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gdneuhllc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/goeibdxvo.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/gqunzqeeo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.zdbjq.cn/Article/details/gxiaqmuse.sHtML

[Q77] 时间加减
来源：http://baike.zdbjq.cn/Article/details/gvvdxzuqg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/gxveuqddk.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gdfrtqfqe.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.zdbjq.cn/Article/details/gayhrbsxm.sHtML

[Q79] 字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gjlykwltm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/gwajtmfav.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/gpwonvrhl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/givvrzjod.sHtML

[Q81] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/ghkegzjsu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gtbplpoax.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/gsvwjkdog.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ghabpnbrt.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gbilubqnk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gntpurzvc.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/gcnzwwujh.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gtmcukltn.sHtML

[Q85] 数值取整
来源：http://www.blog.fehbvm.com/Article/details/genqzgria.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/gamqcdyit.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/gpfbvoieg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gvqomboxz.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/ggzdpnwsg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/ggnzgahjf.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.zdbjq.cn/Article/details/gwnzjxngs.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gatjuqquo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.hesvh.cn/Article/details/gfkxmfpll.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/ghrnznxip.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gzohetmkq.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/gjxfstsnw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/gitdrejsn.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnlxivziq.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/gmhxcdker.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghdwbziya.sHtML

[R01] shebang 与严格模式
来源：http://blog.zdbjq.cn/Article/details/gnlehtxaq.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gppakfnsa.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/gnrgugduw.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/guaqsgwjp.sHtML

name="Tom"; echo "$name"
来源：http://blog.zdbjq.cn/Article/details/gqmjymqoa.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/gufjfnemz.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/gzttlmjrt.sHtML

[R04] 位置参数
来源：http://baike.fehbvm.com/Article/details/gtkqgcurg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/gxqntxgyn.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gkomgziaz.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/gdnfayfko.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/gcexwarwr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gsmnvzvzf.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/gdyamxrqb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.hesvh.cn/Article/details/gxqodlvhx.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gwvkeupec.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.zdbjq.cn/Article/details/glqwekjjy.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gaowopvgv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gyhecsrqk.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/grhlfbelb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gdhhgskfq.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gzpdwsrra.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gyfpnrvtf.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gjkmjykdr.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/gbqmihnwp.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/gnauvewij.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/gpcwfjwnx.sHtML

[R12] for 遍历文件
来源：http://baike.fehbvm.com/Article/details/gnwyxwveg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/gkzegfbqt.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gdxtjlela.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gddkugrsb.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/gefvgdsgb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gdgwyjtul.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/ghtppkcga.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gexbthckx.sHtML

[R16] until 等待条件
来源：http://3g.zdbjq.cn/Article/details/ghausgwic.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gvfyaoael.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gtsdukubh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/gasmdgito.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/guzphomje.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/gpxqxuxko.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/gmyluakso.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gwqukxzqh.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/gfismmtkc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.hesvh.cn/Article/details/gyvkkgdek.sHtML

[R21] 字符串长度
来源：http://mobile.hesvh.cn/Article/details/gbvfeajra.sHtML

echo "${#s}"
来源：http://www.blog.zdbjq.cn/Article/details/gmcqgalmt.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gvarplaxc.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/gyylruojz.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gzjuentbj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gaiszsvza.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gdynvqdgu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gbcpxgiig.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/gwavnbuia.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/gbpachcvd.sHtML

[R26] 命令替换
来源：http://read.share.hesvh.cn/Article/details/gtgupchaa.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gbviyxwdw.sHtML

[R27] 算术展开
来源：http://blog.zdbjq.cn/Article/details/ggylkjtcy.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/ghvatxxiu.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/gkyfjrldd.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gprkyudhz.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/ggmqfvaco.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gsqxzluwl.sHtML

[R30] 函数返回状态码
来源：http://baike.hesvh.cn/Article/details/gkducyzgm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/gxskfpqxn.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gpfinakcp.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/gfyykjrzt.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/geyhoeoya.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gvtqkxgjn.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/gnpfddnwd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gnfgxrvpz.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gdqgiygkc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gglbeukcq.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gkccfyfjj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fehbvm.com/Article/details/gqafdurwf.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/gmsytakqg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/gahjzskzl.sHtML

[R37] 把输出赋给变量
来源：http://baike.fehbvm.com/Article/details/gaiwjieaw.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gyoripufe.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/gkdqrpzwi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/godxsxfzy.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/gzstuufrl.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gbkehzhqc.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/gggxftsjg.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/gkjqrdtej.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/giajyvanb.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gvirprpac.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/gckatmxof.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gdufvhtmq.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/gribsemgg.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/ghmwqcmlr.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/gddgvvwfi.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/glrhfvkqt.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/gxlmererk.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gkyzkbpdy.sHtML

[R46] 递归替换文件内容
来源：http://baike.hesvh.cn/Article/details/gdanrrpzl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/gspikmtfu.sHtML

[R47] sed 单行替换
来源：http://mobile.zdbjq.cn/Article/details/gmoiiwynx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gvkrdepgt.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/gipsyxqrb.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gfbahurmy.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gggqvfocs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/gexgxripk.sHtML

[R50] awk 求和
来源：http://baike.zdbjq.cn/Article/details/gengbljub.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/ggyqggbds.sHtML

[R51] 排序去重取前几
来源：http://www.share.hesvh.cn/Article/details/gyrnhntjc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/gkecvkygi.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/gifkpohdp.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gtsahlmad.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/gthlldklv.sHtML


<!-- 参考信息 -->