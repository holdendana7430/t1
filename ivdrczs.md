代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/glzrujzdg.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/gbeeaxran.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/gztepcjof.sHtML

[Q08] 创建普通索引
来源：http://3g.fehbvm.com/Article/details/gualldjiu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gekngjhhf.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/ghosmzvig.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gwveuzwjr.sHtML

[Q10] 插入单行
来源：http://www.share.fehbvm.com/Article/details/gypqfddon.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gnbusmcko.sHtML

[Q11] 一次插入多行
来源：http://mobile.hesvh.cn/Article/details/gixopmbdv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.hesvh.cn/Article/details/gwiloxono.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.hesvh.cn/Article/details/grmhkqnkl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.hesvh.cn/Article/details/gseufmleg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/gctykqzmt.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gdnxuhmfr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/gimnozlwx.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/gklxommfq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/gxahcnkan.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/gzjobmbwg.sHtML

[Q15] 查询全部
来源：http://www.blog.zdbjq.cn/Article/details/gofoblemq.sHtML

SELECT * FROM users;
来源：http://baike.fehbvm.com/Article/details/gaviilsqr.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gvndmsyit.sHtML

SELECT id, name FROM users;
来源：http://m.share.fehbvm.com/Article/details/gbvelptrd.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/gumoozjkp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fehbvm.com/Article/details/gpwbqvcku.sHtML

[Q18] 模糊匹配
来源：http://mobile.fehbvm.com/Article/details/gehcuwxso.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.zdbjq.cn/Article/details/girexygnr.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/gextgxaxm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.zdbjq.cn/Article/details/gfiwdujaw.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/gaypghfon.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gysxkfzrg.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/ghekkvkew.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/gpjuabtmf.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/gvxlzsahh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/gksyfxygw.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/grkeopdeb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/guiypdebm.sHtML

[Q24] 去重
来源：http://blog.fehbvm.com/Article/details/gzgdnmcie.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.zdbjq.cn/Article/details/glcblyjjp.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/gioutgdmu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/gafjsimwq.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/gldsuzdmf.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gjehnwoys.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/giqcrmmpb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ghgmzfvgu.sHtML

[Q28] 求和与平均
来源：http://mobile.zdbjq.cn/Article/details/gyotenhjt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gcuxovkld.sHtML

[Q29] 最大最小值
来源：http://baike.zdbjq.cn/Article/details/gntixmryp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gogjccfup.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/gksjcwdml.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/grkvkzksk.sHtML

[Q31] 分组后过滤
来源：http://mobile.fehbvm.com/Article/details/gfcdmdjrc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/gleegerew.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gvixqoeab.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/guhijwjzd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gybzhatiq.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/gpftpaeeo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/gzywrzoor.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/gncmqlses.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gitchulsi.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/ggesbremt.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/ghlxuycgp.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/ghooncfdr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gtwmaqtkq.sHtML

[Q36] 左连接
来源：http://www.blog.hesvh.cn/Article/details/givtifnaa.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gylaurryc.sHtML

[Q37] 右连接
来源：http://3g.fehbvm.com/Article/details/geujokybw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gjwvjrify.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/gokapaubn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fehbvm.com/Article/details/gzkvkopwt.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/grvfzjepl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.zdbjq.cn/Article/details/gmeqatyin.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/gwoiotrlq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/guunvmebj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/gbibvarve.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/gdjtdvriz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.hesvh.cn/Article/details/gwsqhsuux.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/grnzubrms.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/gubybhwxf.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/ginbdibpv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/gwgukgbad.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fehbvm.com/Article/details/gckqywsuv.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/gcajcouod.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/gymdxinsx.sHtML

[Q44] IN 子查询
来源：http://baike.hesvh.cn/Article/details/gqtyzocje.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gmaefkkoc.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gurvhrjmk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gmuprrtcc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/gicwptrzf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gvmfvseej.sHtML

[Q47] 与平均值比较
来源：http://www.share.zdbjq.cn/Article/details/gnrhcoazf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fehbvm.com/Article/details/gbcrckeep.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/gwaogdnhd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/gxplctjgi.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.hesvh.cn/Article/details/gtfdadxih.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/gccdfpolg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gtdnrzbpt.sHtML

[Q50] 批量更新
来源：http://mobile.hesvh.cn/Article/details/gtuvmrbuh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.hesvh.cn/Article/details/giopeinij.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/gwgzysmfa.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/gqhwwvksg.sHtML

[Q52] 删除指定行
来源：http://www.m.share.zdbjq.cn/Article/details/gnvcofhxj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gerxagklz.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/gpllijwus.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fehbvm.com/Article/details/gzyrgtmdf.sHtML

[Q54] 清空表
来源：http://www.m.share.zdbjq.cn/Article/details/gdsexruzz.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/ghovhldbc.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/grfllyetc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gmxkjskyo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/gmkjzkxlq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/gyqexpkja.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/gwjqnivld.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/gqqbelckd.sHtML

[Q58] 累计求和
来源：http://blog.hesvh.cn/Article/details/gzczslmki.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fehbvm.com/Article/details/gkkejbhob.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/gpjzaqxzt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fehbvm.com/Article/details/ghwzqyjmy.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fehbvm.com/Article/details/gwflykpce.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gqtxmqgyf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/glibzddvm.sHtML

[Q61] 移动平均
来源：http://read.share.hesvh.cn/Article/details/grhwzmcom.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gifvesnwc.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/gkkmblmci.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/giljaczqa.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/grzdjfuky.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/ggmqixyno.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/gabciigyh.sHtML

COMMIT;
来源：http://baike.fehbvm.com/Article/details/gsyhkoblu.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/gsheysqnh.sHtML

ROLLBACK;
来源：http://3g.fehbvm.com/Article/details/gwedkhhlp.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gutzhkvbt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/gkbrmlskq.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/golwcyqfi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/gmwtbxqzx.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/gbfwpyipu.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fehbvm.com/Article/details/gdrihhtkz.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/gcmffqqvr.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/glkdyjltq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/gqozqyvea.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/gxydejagm.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/gzmemwems.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/gybsdzomx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/glzokwzce.sHtML

[Q72] 查看索引
来源：http://mobile.hesvh.cn/Article/details/goymmwlga.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gywqtddek.sHtML

[Q73] 查看表状态
来源：http://read.share.fehbvm.com/Article/details/gfogiuqgc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/gkfgmscps.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/goqezapnv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/gtbruekox.sHtML

[Q75] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/ghgkdzmlg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gqkuxefsn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/gjfusjjdk.sHtML

[Q76] 按天统计
来源：http://www.share.fehbvm.com/Article/details/gkrxybeqo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.zdbjq.cn/Article/details/gmbcmeizr.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gdxxvoobg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/gtyyuyunm.sHtML

[Q78] 当前时间
来源：http://mobile.hesvh.cn/Article/details/gqcrucvvy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.zdbjq.cn/Article/details/gksodoymu.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/gzshhiqbv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gyitjjtyd.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/goangbbll.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gyhvjraej.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gizuxazio.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/gugozpzbf.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.zdbjq.cn/Article/details/gvtwwhfdi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gohpavbto.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gebtrufuc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gwoxorwiv.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/grmfpgbzs.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gfbpsoqnt.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/gmikpyxng.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.hesvh.cn/Article/details/gckojmhaa.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.hesvh.cn/Article/details/gqrdgjxpq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/gmnqrvitb.sHtML

[Q87] JSON 字段做条件
来源：http://3g.hesvh.cn/Article/details/gdjesbheo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/gjvocrmyd.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/gmkdoquuh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.hesvh.cn/Article/details/gsfoudnyg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gbyxmovjw.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/ggcwilhvd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/gbikuntef.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/gzvkovbei.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/ghpfrfmtp.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcawufiqt.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/gdjkocsht.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gscqvotwz.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/gcczjfoog.sHtML

#!/usr/bin/env bash
来源：http://baike.zdbjq.cn/Article/details/gftsidumf.sHtML

set -euo pipefail
来源：http://read.share.zdbjq.cn/Article/details/ggirrnvxf.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gojyyfhvk.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/gesmzccke.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/gzaqdiiep.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/gtgfviuhh.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/gvntujfon.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gcfebscik.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gwitgurvo.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/gkcnniwjp.sHtML

[R06] 判断命令是否存在
来源：http://wap.hesvh.cn/Article/details/gekwruoav.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/griibfojh.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/gjcttjtvn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fehbvm.com/Article/details/gwsphpomz.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/ggodmfgji.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gervjmplx.sHtML

[R09] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/gnyoyhbho.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/getdpsjth.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/gogkyrizi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gkzvbhjbw.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gzjotxzgd.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/gsqlewbpf.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/gaafzrgct.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/gsiirwahq.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fehbvm.com/Article/details/gbfpkmcqm.sHtML

esac
来源：http://wap.fehbvm.com/Article/details/gblmlhvyf.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/giuafxrhc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/gkhvdssjf.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/ghtlcicoh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gbpxqwucz.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/gsphunebe.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gcyuhukio.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gzhlustfk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/gawkajhon.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gmtxhaypb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gqvzrqfts.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gubmjzkci.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/ghjpsxhwd.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/gikeupcqt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gswbrjhpk.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gfiysmkvf.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/gpgctvolo.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/gwiakpdax.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/gjttzbkum.sHtML

[R21] 字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gnwttlzek.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/gkycgevbv.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gpfgmsufo.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gjugehyjb.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/grafyrlrr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gnuvrbylo.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gvjtlnpsa.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/gqjiayvjw.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fehbvm.com/Article/details/gowejiagf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/geitwzuxy.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/gtzwtehit.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/gnchriidc.sHtML

[R27] 算术展开
来源：http://m.share.zdbjq.cn/Article/details/gprlarhhb.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/guvzyetgl.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/gqvvmzqqy.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/gxhulqdqq.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/golfkzfyp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/gpzitnamg.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gqnfhidvn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/gidmjuczi.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/goxksrirm.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/glrjhgtsg.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/gzvcdwwre.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/ghkmspaop.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/ghqzwoqhs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gnsqhnlvb.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gdmegafeq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gbkmdzroq.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/goklqcrvz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/giccnaohw.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/gqzbatryt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/gunqsvqgh.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gtreriscd.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gfmkoekdf.sHtML

[R38] 管道串联
来源：http://3g.hesvh.cn/Article/details/gldfkbieh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/ggefqulag.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.hesvh.cn/Article/details/gnftrvxhi.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/ggnorpyoc.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gfwgbclnp.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/goublvere.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/gbqocqgxp.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gnzhmpztc.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gzkyabjda.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/guzzlrpym.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/gqbokudjc.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gcizavucf.sHtML

[R44] 按修改时间查找
来源：http://read.share.zdbjq.cn/Article/details/gpmwxeoge.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/gczmeenjr.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gjofgugtq.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gmboouclf.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/gzvrvcval.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/gxljvjjgm.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/galbtxbmc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/gwyyexknl.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gqzfvyaqv.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gmbiregic.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/ghyeuzunm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/gqiiuzwtb.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gdusncvlp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/gjauwjyel.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gqubhksew.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/gleyefggp.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/gbdyciyvh.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/ghzmqcegc.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.hesvh.cn/Article/details/ggrcbroln.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gffjnzbiy.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gdgrgowpr.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/gmysbsrnt.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gbtxyqtza.sHtML


<!-- 参考信息 -->