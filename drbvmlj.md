代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsbgveaf.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gposyhcku.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fanxiaobao.xyz/Article/details/gbsezcxws.sHtML

[Q10] 插入单行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuagryqp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gznslskbg.sHtML

[Q11] 一次插入多行
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnwhddhw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gybwivehc.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fanxiaobao.xyz/Article/details/govesrhmd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjcrksfj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcistnuzg.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fanxiaobao.xyz/Article/details/grxvwxvlq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fanxiaobao.xyz/Article/details/gaingwuhl.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykxujsli.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkuvmesl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorcgmohy.sHtML

[Q15] 查询全部
来源：http://wap.fanxiaobao.xyz/Article/details/gdebfxpat.sHtML

SELECT * FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/glkhcudlb.sHtML

[Q16] 查询指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gduxgxrtk.sHtML

SELECT id, name FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrtbqver.sHtML

[Q17] 条件查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gofucakuq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gblyjzcwb.sHtML

[Q18] 模糊匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gorrhzzpr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjozcywfo.sHtML

[Q19] 范围查询
来源：http://wap.fanxiaobao.xyz/Article/details/geggluibg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fanxiaobao.xyz/Article/details/ggzfutrnc.sHtML

[Q20] IN 列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjooohmj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/glqyjaufe.sHtML

[Q21] 空值判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gmuncbxhz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxthdupao.sHtML

[Q22] 排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gelmhabzw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fanxiaobao.xyz/Article/details/grrvjsvfl.sHtML

[Q23] 分页
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjytupczi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrpsnohc.sHtML

[Q24] 去重
来源：http://wap.fanxiaobao.xyz/Article/details/gdhrqbvny.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gvifwpawe.sHtML

[Q25] 只取前 N 条
来源：http://blog.fanxiaobao.xyz/Article/details/ghbfeidfk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpodpdug.sHtML

[Q26] 计数
来源：http://baike.fanxiaobao.xyz/Article/details/gmoizgnxm.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gtoobogfo.sHtML

[Q27] 条件计数
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdbiqlsy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gtuehjati.sHtML

[Q28] 求和与平均
来源：http://3g.fanxiaobao.xyz/Article/details/ghssxerlw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gblhifnps.sHtML

[Q29] 最大最小值
来源：http://wap.fanxiaobao.xyz/Article/details/gsfffzfjl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/giotlhkna.sHtML

[Q30] 分组统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgxnqahf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmxvpkao.sHtML

[Q31] 分组后过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gslgqpfni.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gevcrlzge.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/grihlsypg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gipvtngqd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzuyyofo.sHtML

[Q33] 多列分组
来源：http://3g.fanxiaobao.xyz/Article/details/griokasre.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaunrkvii.sHtML

[Q34] 每组取第一条
来源：http://mobile.fanxiaobao.xyz/Article/details/gvonkbcem.sHtML

SELECT * FROM (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopatcmml.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkkmumih.sHtML

) t WHERE rn = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfdqeyvt.sHtML

[Q35] 内连接
来源：http://baike.fanxiaobao.xyz/Article/details/gqujqemiz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfriuxbsp.sHtML

[Q36] 左连接
来源：http://baike.fanxiaobao.xyz/Article/details/gxkgohtyu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghfkdvre.sHtML

[Q37] 右连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxaklxnp.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvkiflbg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxugwhmho.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gmgfainla.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjsbpxtv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fanxiaobao.xyz/Article/details/grsqoezuh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gjrvldwgf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fanxiaobao.xyz/Article/details/gusbgqomn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnewxnyan.sHtML

[Q41] 多表连接
来源：http://blog.fanxiaobao.xyz/Article/details/gddrdomdc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fanxiaobao.xyz/Article/details/gjdpjhppn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fanxiaobao.xyz/Article/details/gozlydqfw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gnolohyqd.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/genqiqecl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxrxbezm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gffpyckpn.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsfllyeu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fanxiaobao.xyz/Article/details/gejjqsqup.sHtML

[Q44] IN 子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gbmjisefz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fanxiaobao.xyz/Article/details/gplwizvod.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fanxiaobao.xyz/Article/details/gcomeepzr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gkljdftig.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fanxiaobao.xyz/Article/details/gvkdafqtr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/glzvgwaoj.sHtML

[Q47] 与平均值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gwsjsrrxk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fanxiaobao.xyz/Article/details/gainvcnaa.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwzfmnde.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/gswdwdnqw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgbdsdzo.sHtML

[Q49] 更新单行
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcnaprlm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/govfydsdc.sHtML

[Q50] 批量更新
来源：http://wap.fanxiaobao.xyz/Article/details/gcemzmifk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gcdpxbltt.sHtML

[Q51] 用子查询更新
来源：http://blog.fanxiaobao.xyz/Article/details/glvczllml.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gtyzoiwhe.sHtML

[Q52] 删除指定行
来源：http://wap.fanxiaobao.xyz/Article/details/ghvksfuji.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbdrjyxo.sHtML

[Q53] 按条件删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gxplbobkl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyuihyzp.sHtML

[Q54] 清空表
来源：http://3g.fanxiaobao.xyz/Article/details/gzroihjwx.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fanxiaobao.xyz/Article/details/ggvmzcsky.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gfylgwink.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxunexnw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwwzgabf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gkivxyile.sHtML

[Q57] 行号
来源：http://3g.fanxiaobao.xyz/Article/details/gokecxmsj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/guxjfhspp.sHtML

[Q58] 累计求和
来源：http://m.share.fanxiaobao.xyz/Article/details/giaulqicw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/grhizvsvl.sHtML

[Q59] 分组内累计
来源：http://read.share.fanxiaobao.xyz/Article/details/gdumsdqwv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkjbnzzu.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fanxiaobao.xyz/Article/details/gmxmepgpt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/gncrgjgsa.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/ghdqnmdgx.sHtML

[Q61] 移动平均
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkvqvfvr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gvcmytgkv.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gmasoowws.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnesshlm.sHtML

[Q63] 开启事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gpebeqqmt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrrpntym.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdswtpcz.sHtML

COMMIT;
来源：http://baike.fanxiaobao.xyz/Article/details/gypbrhbjc.sHtML

[Q65] 回滚事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxlmsvwq.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/gxwyktjtr.sHtML

[Q66] 行锁查询
来源：http://blog.fanxiaobao.xyz/Article/details/gubmkodmq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fanxiaobao.xyz/Article/details/gbfdezppl.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmqhjkhf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fanxiaobao.xyz/Article/details/gxxfqggiv.sHtML

[Q68] 保存点
来源：http://blog.fanxiaobao.xyz/Article/details/gvujimuex.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gohmxmjtc.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmbgczpy.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/gbgdeazwd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/gdavvdmln.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/gvnvaunij.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmehnjlek.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/ghxeakdtx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmsbmsai.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/grhbkknop.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gijwtzjib.sHtML

[Q73] 查看表状态
来源：http://3g.fanxiaobao.xyz/Article/details/gyumjbvtz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxcnnfxv.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehcyzgss.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/gzdyenyyv.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/goajrkpvx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfjiinmd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/gcwipjsip.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/gdwgywtta.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggovhcxfr.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gpvtftfnc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrmtgiiv.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/guwedyhrj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyiwmijz.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gldkxjvpc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/gdxkarcay.sHtML

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/guhuwdaau.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvtvspve.sHtML

[Q81] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcodrcka.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gboaknrts.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gstczfpuc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/guiyxtspx.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gqohmhbll.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnvxhicg.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/glgquzmpr.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvniwvin.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gpeweqeqp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/ggmcfaxxl.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gxarvlklt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/gokfhdkss.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnegfvddm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/gxrhuvsck.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpjszcch.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gkbvvhrys.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwblvjyk.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gbddhftih.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqjetwtj.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmpapbkg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzngjwxy.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaheckkui.sHtML

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvdwpxsv.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gbenxzxmc.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gyqymwtlu.sHtML

#!/usr/bin/env bash
来源：http://read.share.fanxiaobao.xyz/Article/details/goouilgiv.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/grzcwkpmq.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/gpogryxgx.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwxnmdpj.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/ghzoccwgl.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gsubjrcia.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/glsjpnleb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/gecdoeaxf.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/ggzmptslx.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/griigslac.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gezqeinlb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gudsrjtva.sHtML

[R07] if 判断文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggchnnxdd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/grqpyevcy.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/ghjlqlfmx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gghhusqsr.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gdhavhakv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlexzxfs.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gyszraudt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmazqgcq.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbzleosj.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkcfsssi.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsstgybu.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyaoejvza.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxwfnrxp.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gaftcwkgy.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlelqtdn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gguwnhtsx.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/gvyjofvic.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtllcvvbq.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnmnbfyc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gtjclmgay.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gomnyuvvm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyifkkuq.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqjtlfmy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gklddyyxp.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/gmewbhzdo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjceclzqo.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gfxelfknk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gzqqfetma.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gwccwqlwb.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaactjgpa.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbrhoich.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/glhrjeclv.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gxpymwctg.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/ginumdlaf.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebmitmay.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gsrflbard.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtlyzgim.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpzhmgdz.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwsflhsm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhuaspzp.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzubwyan.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpmpyrnb.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkmqfqyf.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gddflutwl.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdfbgtku.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gpnhpwjyy.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gspacvwwo.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gbccbhbbk.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglbeuoxr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gpbfsjguj.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflwggqtl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhkvqvvw.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gxgddqqrd.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmbnvyfw.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gnzpepjif.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdoopbcm.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfltkucs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsprrnfr.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gcuoksqmv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gohoihcch.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gulowrtos.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gvgfflyxj.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gftfdstur.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuanvzoi.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/glrieiemy.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gagqhskzc.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/garclxqxf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gtgwvtxro.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/geesvtpln.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gdlzibdox.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelgenmph.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynrchlkl.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkofspfk.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gevkdzgfu.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gugxmtbxq.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/grcqrnzpd.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gkaanmqcg.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvefggwku.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxorqkxo.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwbkgarf.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gpoyfkztg.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gggkrtllx.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gubnufgab.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/ggerygcrh.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfhmiutk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwqbmnnm.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gvgmurswv.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gxlmnnujk.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/glxwyfnrs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gbnicqtfc.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckmmlwll.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkuckjjw.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gqfiglusz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwickhpu.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggchgzmji.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gzolbfdls.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gukrrjvju.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gsrkrkzte.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwahiwse.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyurchpw.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gflaqfvdj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gbjjjdvky.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpxjzomt.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gjlbnpoln.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjaurpbo.sHtML


<!-- 参考信息 -->