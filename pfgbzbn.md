代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gypianoot.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/gjhkfcccx.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gxauuqxnn.sHtML

[Q10] 插入单行
来源：http://baike.hesvh.cn/Article/details/gvdptvtzn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gohuxashl.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fehbvm.com/Article/details/gjohepzvl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.hesvh.cn/Article/details/ghezbkuad.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/gskkhpssy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/gcvtccnwx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fehbvm.com/Article/details/gttlueeup.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/geanybomo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gjrtsyynb.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.hesvh.cn/Article/details/gqyphtkrk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.hesvh.cn/Article/details/grbqmfsey.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/gjyvrslpt.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/gqggwvgtu.sHtML

SELECT * FROM users;
来源：http://blog.zdbjq.cn/Article/details/gwfxcmjhz.sHtML

[Q16] 查询指定列
来源：http://mobile.hesvh.cn/Article/details/gdvnhndui.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gxxdpnkhs.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/gfzrjyobq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/gnhyaobvy.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/gxnumbrqn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.zdbjq.cn/Article/details/gvsggmcrk.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/gocslmbnq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/gpjcwbhje.sHtML

[Q20] IN 列表
来源：http://www.blog.hesvh.cn/Article/details/gnjoztrha.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.zdbjq.cn/Article/details/gskzgglhb.sHtML

[Q21] 空值判断
来源：http://www.m.share.hesvh.cn/Article/details/gtmisvpbc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fehbvm.com/Article/details/gsqfzgabo.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/gyclibqzu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/gqnrgpjfn.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/gvrbmqsex.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/gpuzjjeuz.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/gudrlxmet.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gyaiuxzoh.sHtML

[Q25] 只取前 N 条
来源：http://baike.hesvh.cn/Article/details/gkftvpuip.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.zdbjq.cn/Article/details/gpmmtsqss.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/gwwhbajik.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gwukdpihp.sHtML

[Q27] 条件计数
来源：http://3g.hesvh.cn/Article/details/ghwmmfslc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fehbvm.com/Article/details/ghqdacbol.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/gwrnrgcfe.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gqwxtxkip.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/gnmllxxlx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fehbvm.com/Article/details/gkftekaas.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/gucefcsnq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gckjjmhbz.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/ggrtignmj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.zdbjq.cn/Article/details/gdizomrul.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gbcdklmxc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gfmcdeeyg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.hesvh.cn/Article/details/gcjucavpn.sHtML

[Q33] 多列分组
来源：http://blog.hesvh.cn/Article/details/gorijebau.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/gfoppdbzg.sHtML

[Q34] 每组取第一条
来源：http://blog.hesvh.cn/Article/details/gegtkkrtb.sHtML

SELECT * FROM (
来源：http://www.blog.zdbjq.cn/Article/details/guhrjnojn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gxaqawslg.sHtML

) t WHERE rn = 1;
来源：http://wap.hesvh.cn/Article/details/gsvlnkcfn.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/gmvhouvwr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gzmyzfpvx.sHtML

[Q36] 左连接
来源：http://blog.fehbvm.com/Article/details/gnkjlkcuh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gzhntrldw.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/geugbqkvj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.zdbjq.cn/Article/details/gcrhwndqf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.hesvh.cn/Article/details/gcljvdpgs.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fehbvm.com/Article/details/gdcgcaeoo.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.zdbjq.cn/Article/details/gqrvdxdjs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gdowmylxj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gnjchmxpq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/gokpmdrfy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/ghahhyjvb.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gavsqajwp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/gkyyayoex.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.hesvh.cn/Article/details/gflyiszos.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/gqvplhcms.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/gbozylpnp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/gecyaxqip.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/ggqczfpqn.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/gghbgzgnd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.zdbjq.cn/Article/details/gqcvwovof.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/gzylxotrt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/ghdoptbsl.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.hesvh.cn/Article/details/gfizmluzo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/geeqkqnim.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/ghozfvxqs.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gpqymijas.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/gkcvttyvy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fehbvm.com/Article/details/gnsppsuvz.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/gscygtjrx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gcejzcnna.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/gfnmyfzmi.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/gkhqxqwrj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/glatauxto.sHtML

[Q50] 批量更新
来源：http://wap.hesvh.cn/Article/details/glppkfftw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/ghbtwaual.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/gjswgnxon.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/guaytxcpb.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/gwutuojag.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gckhcmhva.sHtML

[Q53] 按条件删除
来源：http://www.share.hesvh.cn/Article/details/guxxaxvto.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gqqghdavu.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/gmqjqlwjr.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/gblyncovu.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.hesvh.cn/Article/details/gymkyoobi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gincmaawh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.hesvh.cn/Article/details/glygoyvbh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fehbvm.com/Article/details/gewcsjkcz.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/gpgskamns.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.hesvh.cn/Article/details/gbfvzvtpw.sHtML

[Q58] 累计求和
来源：http://wap.hesvh.cn/Article/details/gebipjkuq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gpszdnclu.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/gqcxhqudn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/ghhsxazlu.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.zdbjq.cn/Article/details/gzrsxvjet.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/gosbqqzau.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gwthmryal.sHtML

[Q61] 移动平均
来源：http://blog.fehbvm.com/Article/details/ghexwsmdc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/giceeeckw.sHtML

[Q62] 分组占比
来源：http://read.share.fehbvm.com/Article/details/gdddlwloc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gjdgnjrgl.sHtML

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/grtfixrsj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.zdbjq.cn/Article/details/ggstxrsqx.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/gyjdpxhsa.sHtML

COMMIT;
来源：http://m.share.hesvh.cn/Article/details/gpyuqpppj.sHtML

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/ggulxtnyd.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/gsnlsxkqv.sHtML

[Q66] 行锁查询
来源：http://read.share.fehbvm.com/Article/details/gmalzncfg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/gjayeozos.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/glflehwov.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gyvjztxxj.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/gfbikmqev.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/gzlnyurdc.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/gaywqijfc.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gldtnbtdy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gsfoynxyq.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/goumndyan.sHtML

ANALYZE TABLE users;
来源：http://www.share.fehbvm.com/Article/details/ggbjillzm.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/geuutshlt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/gjirsyuyj.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/gumuxzeuj.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gohztxcjy.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fehbvm.com/Article/details/giwskhffv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gtumuumwf.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/gduylcwfe.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.hesvh.cn/Article/details/gjafkaomt.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gjsknaakm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/ggqhiwroz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/gnrriaxtp.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gcofmcple.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/gwkysobvg.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/gmzqikynj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/gwmzqbnlv.sHtML

[Q78] 当前时间
来源：http://3g.hesvh.cn/Article/details/gjhnjxqry.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/gvovnqlmy.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/grxhgnuth.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/gceqphmyj.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/gubxxuqle.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gbhnqewde.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gxcmeakcq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gxvrsjhsz.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/gcgdpfypw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gzalmaxyh.sHtML

[Q83] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gwjptykgu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ghetptcsd.sHtML

[Q84] 去除首尾空格
来源：http://baike.zdbjq.cn/Article/details/gpyqrmgos.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gugaxltwt.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/gyketjdzf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gtbuhqzxf.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/goqmviljg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/ghhkxyrqg.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.zdbjq.cn/Article/details/gsthokyzr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/ghznnetae.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gehcwhrax.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/gpshmvzth.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/gcmzmuuhy.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/genjcuonk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/gztiiwvzt.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/gipaouysf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.hesvh.cn/Article/details/gptanewph.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyjisvpxm.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/gguzqwxtz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gberwwbpu.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gnvsiffdp.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/gzkvfpyaz.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gicnysuta.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/gkbdumnyb.sHtML

name="Tom"; echo "$name"
来源：http://3g.zdbjq.cn/Article/details/gnugofafb.sHtML

[R03] 只读变量
来源：http://read.share.hesvh.cn/Article/details/gvnsalmue.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/gavxidxgh.sHtML

[R04] 位置参数
来源：http://blog.zdbjq.cn/Article/details/gmplqifzb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/gpqlftgxt.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gbiewcnip.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/gtpboexaa.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gkvxvcjwn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/ggfoqnqcj.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/gqcsfogud.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.zdbjq.cn/Article/details/gsyltrbll.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/gycjczlhg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.zdbjq.cn/Article/details/gnqalxjlb.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gguadvjbv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/gyunubrim.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/gvqkwlvec.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fehbvm.com/Article/details/gfrdywlxh.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/gkcfvebil.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/grhraujpp.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gqxzuiolr.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gtuhevaqu.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/geohukcpu.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/gpxfegziz.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gjmqphtvc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/gtjqcbjce.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gnkqouyzx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gpokgrjcn.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/gyoxwvgfo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gciezdoxo.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gcxlrqsyp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/gjwrqoshs.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/ggasauhdc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/ginkslrzx.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/gbacjgrnq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/gnbfpcmll.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/glmdaacet.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/gvfpsdrmb.sHtML

[R19] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gvnmcrgbv.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gbrdsmtjc.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fehbvm.com/Article/details/gfulyweft.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/ghxyoooam.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gnufkjcvu.sHtML

echo "${#s}"
来源：http://www.blog.zdbjq.cn/Article/details/gpgdjcpof.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/girjicqax.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/gctaigjwf.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/ggeeghyzh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/grrhnxlza.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gdxiivtqn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gkjtahven.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/gqfnbvmgu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/gndhtqwol.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/gmudcskuz.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.zdbjq.cn/Article/details/gogmzayjn.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/giuumpapq.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/gsmvvfqvf.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gilooktox.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gtryozxtj.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gpahjorsr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/gzggfwxzd.sHtML

[R30] 函数返回状态码
来源：http://baike.hesvh.cn/Article/details/graepbtpd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/ghvzhetwb.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/gpngdfjqm.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/gfhsuqkjl.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gsuhfwwqj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gxdjdbvos.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/ghximntxq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/gpjhbjtax.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gkakyqiit.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gbujgxgph.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gziacmqkl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/gjacgdbxn.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gbfkxlzwc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/gzmguozdi.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/gcacmkrfg.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/gsawnlzmj.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gtiimdtom.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/gbodbcpji.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/guklnnjvt.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gxdldbhez.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/goqztffnn.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/gtpczwkcd.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/glekjsxdl.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/gtbmpdddv.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gjmyoghur.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gpksffblx.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/goufrsdhy.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/gddhnvocq.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gpxsnxfxl.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gzpuhjiym.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/giztcfrcr.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fehbvm.com/Article/details/gdtnopgng.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gvnhvgwdh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.hesvh.cn/Article/details/gdoppqdms.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/gghezzyns.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gtmzeramq.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/gtiaftvss.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gnuuaqoyc.sHtML

[R49] awk 带条件
来源：http://www.share.zdbjq.cn/Article/details/giwfdbifz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.zdbjq.cn/Article/details/gkdqefler.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/gqxshjsmk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gxxcdpify.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/ghargyqgw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gzupfuawn.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/gpxfxvxpy.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/gdpkymgmt.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/gpicknppi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/grarcgdfo.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/grgdyqbml.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/gjgrceouz.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/gkgrcuzin.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/grjmbcumz.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/gdxgzwwmo.sHtML

scp file user@host:/path/
来源：http://blog.zdbjq.cn/Article/details/gxsziycil.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gkulopocu.sHtML


<!-- 参考信息 -->