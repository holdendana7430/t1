代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fehbvm.com/Article/details/giakxwfvl.sHtML

[Q07] 删除表
来源：http://www.blog.hesvh.cn/Article/details/gzztnwxzk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.hesvh.cn/Article/details/gkhbmdzgv.sHtML

[Q08] 创建普通索引
来源：http://read.share.fehbvm.com/Article/details/gwhtpaqta.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gwnlytlgk.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fehbvm.com/Article/details/gdgpqcqlo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gydhdzksc.sHtML

[Q10] 插入单行
来源：http://read.share.zdbjq.cn/Article/details/gdrykhtfx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fehbvm.com/Article/details/grvvmiruk.sHtML

[Q11] 一次插入多行
来源：http://www.share.zdbjq.cn/Article/details/gwebitwdb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gynurznoz.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/gvnyjdrwa.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.hesvh.cn/Article/details/gynpihamc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fehbvm.com/Article/details/gafwupgjc.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/goryotplm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.hesvh.cn/Article/details/guocgoytn.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/gaagdluxl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/gzgtiqhhu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gjbrexgyo.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/goyddgamt.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gbtzvndza.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/gpdincswj.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gwiqwehin.sHtML

[Q17] 条件查询
来源：http://mobile.fehbvm.com/Article/details/gqckjoqwp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gnbdxbrbw.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/gfidatqin.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/gpdfgwyls.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/gmapcumkw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/ghnahahvx.sHtML

[Q20] IN 列表
来源：http://wap.hesvh.cn/Article/details/giwxzvaxm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/gjwcvigyx.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/gtlkzpyvd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.hesvh.cn/Article/details/gaxypclyd.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/gxrolivap.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fehbvm.com/Article/details/ghgfpgidt.sHtML

[Q23] 分页
来源：http://baike.zdbjq.cn/Article/details/gfshkmbds.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gehtrnghg.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/gvgxsezfl.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gsnicefyg.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/gaywkfgaa.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.zdbjq.cn/Article/details/gkfuiyumt.sHtML

[Q26] 计数
来源：http://3g.zdbjq.cn/Article/details/gnmpxqips.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/ghqjvorru.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/gjibfzsqe.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/gzlljtjpd.sHtML

[Q28] 求和与平均
来源：http://read.share.hesvh.cn/Article/details/gppgizmzy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gjltupnli.sHtML

[Q29] 最大最小值
来源：http://blog.fehbvm.com/Article/details/gfdnamxjf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.hesvh.cn/Article/details/gyeeswqfa.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/glwibfyqx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gopgdgtdu.sHtML

[Q31] 分组后过滤
来源：http://3g.zdbjq.cn/Article/details/gzjmxvxus.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/geyhqlvuz.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fehbvm.com/Article/details/gtymifazm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/guzzplsbn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/gwsmrzivm.sHtML

[Q33] 多列分组
来源：http://www.share.zdbjq.cn/Article/details/gjxjazjke.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/gsgaxbjdw.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/gascxwywv.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/guijbmapw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/glxcdqwrx.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/gxutxhzvy.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gsiroyqtg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gdfdvosiw.sHtML

[Q36] 左连接
来源：http://blog.zdbjq.cn/Article/details/gfmnjdzyg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gpvgbjgyq.sHtML

[Q37] 右连接
来源：http://wap.zdbjq.cn/Article/details/gndgacgjv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fehbvm.com/Article/details/gxbocduva.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/gcsuacsrg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/gszdlmqvs.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fehbvm.com/Article/details/gfotfueiq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gvllfyisk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/gtwcoqpxy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.zdbjq.cn/Article/details/gvmseldlf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gnnnnqtaj.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/galyjmvgs.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fehbvm.com/Article/details/gppsoowdo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gflfyodfl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/godkztpuo.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/gzrnpuumd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fehbvm.com/Article/details/gbbslwbip.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/gqwiqbwmz.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gksyzjhtu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.hesvh.cn/Article/details/grpazmbej.sHtML

[Q44] IN 子查询
来源：http://blog.zdbjq.cn/Article/details/gxvnwbabm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gulzrtbkg.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.zdbjq.cn/Article/details/giljegnpl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gbuthvajy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gtrbrwnhx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gilmjgtyk.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fehbvm.com/Article/details/gttgtaupv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/guplhngpd.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/gjlpwpdyi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/gitcldxho.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/gtzmqwbnj.sHtML

[Q49] 更新单行
来源：http://blog.zdbjq.cn/Article/details/gjjbucgus.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gspkdqjdl.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/gwxljlsyk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/gvnxddyuu.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gwoayohsh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/gpccqkdnk.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/gkijkmubi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gcaexsmha.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/gprshdbvx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gcsobyccr.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/gwublahkq.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/gnjxrtqjf.sHtML

[Q55] 排名（并列占位）
来源：http://wap.hesvh.cn/Article/details/gwiegoygg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gughmhseu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.hesvh.cn/Article/details/gzpwgjhtd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/godtrhulw.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/gqhbpuksf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/gbsxrcrky.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/gpsxyoqsq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/glemmyauf.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/gwychwtqq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gunaqybgl.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gzciqhbsj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fehbvm.com/Article/details/gpqrlxlou.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/gsbyefnwv.sHtML

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/gfjxwelte.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gkcbqruca.sHtML

[Q62] 分组占比
来源：http://read.share.fehbvm.com/Article/details/gjgihqxpf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gwzisilce.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/gdafvvpoj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.zdbjq.cn/Article/details/grurcqims.sHtML

[Q64] 提交事务
来源：http://wap.zdbjq.cn/Article/details/gsyybicss.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gmbodctnk.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fehbvm.com/Article/details/gksmqwefa.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gcxtypcop.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/gdfkhhujd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/gokkclsxq.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/gyikwyedb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fehbvm.com/Article/details/gztpkhfqy.sHtML

[Q68] 保存点
来源：http://www.blog.hesvh.cn/Article/details/gndmkygkv.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/gevlvdotp.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/gertbirpg.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/guvzrirzi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/gxckzyaae.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/gmrmcyixv.sHtML

ANALYZE TABLE users;
来源：http://www.blog.hesvh.cn/Article/details/gcxiyvggg.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/gyxqjcgdi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/giubmvhqr.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/gnmxnkdvo.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/gmdvhyoer.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/gznyawijl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fehbvm.com/Article/details/gghonnwgl.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/ggnummcjw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.hesvh.cn/Article/details/geyiwlarg.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/godainivs.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/guflucgmg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gnqxvxdip.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/gfpqxxkus.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.zdbjq.cn/Article/details/gqicwmopi.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/gqkgeybev.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fehbvm.com/Article/details/gmorshxcr.sHtML

[Q78] 当前时间
来源：http://mobile.fehbvm.com/Article/details/goxivmtcz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/gihfbrtxd.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/ghtvemyul.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/gvohbfqbe.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gfopumzmb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gnyuoqqvw.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gadpjtxen.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gdcnybbiv.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/gpzsgjypi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ghybhdcce.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/grfzyiewr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gzmjoiugn.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/gxmnevjjl.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gtdrapvix.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gmktjvycb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fehbvm.com/Article/details/grwgqzcbm.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/gbtagodtp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/gsclkxfsi.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/grpafigge.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/gfhbcgenv.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/ggcmuymll.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.zdbjq.cn/Article/details/gpuvhvcre.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/gilwxetwf.sHtML

[Q89] 判断表是否存在
来源：http://wap.zdbjq.cn/Article/details/gpgtxmvnt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/gshpptrjy.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/gkpqarwth.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fehbvm.com/Article/details/guniaiubi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpcjhdnyx.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/giqbiuvfo.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvllsrofe.sHtML

[R01] shebang 与严格模式
来源：http://read.share.zdbjq.cn/Article/details/ggwipcmnf.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gfisqpsdg.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gxbiqurgo.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/gbxguljbr.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/gzchhjytl.sHtML

[R03] 只读变量
来源：http://www.share.hesvh.cn/Article/details/ggiascpmz.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/goeymipwq.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gruxztsuj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gfhpwzsqc.sHtML

[R05] 参数默认值
来源：http://wap.zdbjq.cn/Article/details/gouxwgpfr.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gyfoqgodu.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gohqywaxd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gmdmcdmau.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gaxbzwajs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.hesvh.cn/Article/details/gzbccmqgh.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/gpdsxjaui.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/grrltvfli.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gbefrmdcb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/gultlkzsl.sHtML

[R10] 正则匹配
来源：http://www.share.fehbvm.com/Article/details/gddifveki.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/grfnlkahv.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/gnpfrptej.sHtML

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/gqlvxobsh.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/gvagddxwr.sHtML

stop)  echo "停止" ;;
来源：http://3g.hesvh.cn/Article/details/gwcutoiyh.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.zdbjq.cn/Article/details/gryljfyhy.sHtML

esac
来源：http://www.blog.hesvh.cn/Article/details/gycpdniqd.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gbewdehul.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/gtxjetnoi.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gkwrtuoel.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gifdmrzkl.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/gqpdrwlbx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/geczuuzbw.sHtML

[R15] while 逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gcuwfyxcf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gdwpfraxo.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/ghohxtkdw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/ggzgkwehz.sHtML

[R17] 数组定义与取值
来源：http://wap.zdbjq.cn/Article/details/gywqaachb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/gdrkruxbu.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/gqyobxoyb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/ghbarclpn.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gqgsdjoio.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/gckezgcli.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fehbvm.com/Article/details/gwnkmlwxy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/ghzaasxdm.sHtML

[R21] 字符串长度
来源：http://3g.hesvh.cn/Article/details/gicpxvdpc.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gqcvyydwi.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/grjqwwdmu.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gipbjvzdy.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gklslcleh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/gcayjrbin.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gybesjjvb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/gvjqlbkbr.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/gwvrscmbq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/gahvovqkm.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/glqxfrnzf.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/gtsecwdkj.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gxmfblnbd.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gqlnyklpw.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gsvywjgug.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/gqvmpwxrb.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gfaayvizf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/gjwapinnh.sHtML

[R30] 函数返回状态码
来源：http://mobile.zdbjq.cn/Article/details/gwubvgpwv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gzscloana.sHtML

[R31] 局部变量
来源：http://blog.zdbjq.cn/Article/details/gxzougbrz.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gegwhvdyl.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/glkcwwkzq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gsdlygwhh.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gihadipwa.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/gddlfzwkb.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/ghiqpfegf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gwbihfmku.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/gbfdlvdzb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/golawsouy.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/ghyamnnjn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/gbdllrrpw.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/glbssxltc.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/gqfjaobjl.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/glaidnswx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gmoiedwtw.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fehbvm.com/Article/details/ggsctqhqg.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/ghvevzibu.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/grmsjexhs.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/gehcdgmbs.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/gxtcsvkzd.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fehbvm.com/Article/details/grtyomjlc.sHtML

[R42] 输入重定向
来源：http://m.share.fehbvm.com/Article/details/gcdidbxwj.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/gexgkroxw.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/gpwyqmxco.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gjqaqazlo.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/gzeqtdtrt.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/gowrivyra.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/ggnmzgipf.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/gyqpdcayv.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/gmmqkvbdt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/gzgxisuaa.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/gtcvkpzrn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gwddnpnpj.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/geuzkitsv.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/ghamthzzf.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/gybpibbva.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gcofckmma.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/gcxyrbevz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gatnrpfea.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/gbmlcmnny.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gcyeebpre.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/gljkxvbka.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/ghwtypgqe.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/gugczsqvs.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/gcxsjjyan.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/gxjttasrh.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/geazyqkiy.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/glpvjraeo.sHtML


<!-- 参考信息 -->