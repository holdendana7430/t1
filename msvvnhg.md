代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/gquhlzijc.sHtML

[Q05] 重命名列
来源：http://baike.fehbvm.com/Article/details/gobtllrvr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/gfmpictbt.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/gjquvmwtv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.hesvh.cn/Article/details/gfcuvdixm.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/gofvfvfyx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/gozsxggxy.sHtML

[Q08] 创建普通索引
来源：http://baike.hesvh.cn/Article/details/gxkopauma.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gknewszfe.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/gscpqioum.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gzineoqxo.sHtML

[Q10] 插入单行
来源：http://baike.hesvh.cn/Article/details/gplqlgxkm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gowgmgmpl.sHtML

[Q11] 一次插入多行
来源：http://wap.fehbvm.com/Article/details/grhajjebm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fehbvm.com/Article/details/gddghjage.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fehbvm.com/Article/details/gstjmbmpf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.zdbjq.cn/Article/details/guypfeijx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/gnnsrzmqy.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fehbvm.com/Article/details/gkmamnhaq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/gkvoqbuca.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gdxktjnta.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/gkdulaumd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/ghnldoali.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/gsdbgdlfz.sHtML

SELECT * FROM users;
来源：http://baike.fehbvm.com/Article/details/gnpxfqrfq.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/gbwgiwclg.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/glxkptbif.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/ggqgkeujp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fehbvm.com/Article/details/gefwsdhrq.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/glaznapox.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/gyxopjsgl.sHtML

[Q19] 范围查询
来源：http://baike.zdbjq.cn/Article/details/glqjpazcf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.zdbjq.cn/Article/details/gftisrvgb.sHtML

[Q20] IN 列表
来源：http://wap.zdbjq.cn/Article/details/gozzhkvgv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gifqjxmjl.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/gzyobkiye.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/gyzkhdqsa.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/gfgzwqdqm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fehbvm.com/Article/details/gijamcmni.sHtML

[Q23] 分页
来源：http://mobile.zdbjq.cn/Article/details/giusitlrm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gdfluzism.sHtML

[Q24] 去重
来源：http://m.share.fehbvm.com/Article/details/gnoifybmo.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gpvelyrow.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gjaqqjkyh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fehbvm.com/Article/details/gzbfqckir.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/gtikqcpkd.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fehbvm.com/Article/details/goahavpol.sHtML

[Q27] 条件计数
来源：http://www.share.fehbvm.com/Article/details/gbfljesyq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gdlejipcl.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gdfiagpyx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gvaylwdbh.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/gjlkrmlev.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gqnnzgmpg.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/gauqqgiab.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gyecopbpe.sHtML

[Q31] 分组后过滤
来源：http://m.share.hesvh.cn/Article/details/gstopxofk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.hesvh.cn/Article/details/ghwgqmedi.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gcfatiamb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gqmjrohqk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/gskpzfwjf.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/gttqgcsow.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/gagtquaac.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/gwbccvicr.sHtML

SELECT * FROM (
来源：http://www.share.zdbjq.cn/Article/details/gscepwetj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/ggbsazoxf.sHtML

) t WHERE rn = 1;
来源：http://mobile.hesvh.cn/Article/details/gvjvicnof.sHtML

[Q35] 内连接
来源：http://read.share.zdbjq.cn/Article/details/gcewsacgh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gswduuosk.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/gtxplzbfx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/geaitolhh.sHtML

[Q37] 右连接
来源：http://www.share.hesvh.cn/Article/details/gpbzqlhej.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/guemdcrww.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fehbvm.com/Article/details/gupubppmk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/gjpgwqtdf.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gvocqiwyl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/gksxbarry.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fehbvm.com/Article/details/gpuashznp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.zdbjq.cn/Article/details/gjqcmberq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fehbvm.com/Article/details/gqiwztwab.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/gmhxybfem.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/ggxfmcaca.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fehbvm.com/Article/details/gmurzxvkc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gsbewvcxj.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fehbvm.com/Article/details/gphlnlxjb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fehbvm.com/Article/details/gswdbhown.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/gnuojtvcn.sHtML

[Q43] 标量子查询
来源：http://blog.zdbjq.cn/Article/details/gmrqpxlgi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.hesvh.cn/Article/details/guujegyog.sHtML

[Q44] IN 子查询
来源：http://blog.zdbjq.cn/Article/details/gcuqbuflt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/gchxkufhu.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/gqtsmrpzf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gjprqshgq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.hesvh.cn/Article/details/gdrfetsup.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/ghkzfiztv.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.zdbjq.cn/Article/details/giahqfmxk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/gdkopuaea.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/gfwkjaiyu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fehbvm.com/Article/details/gbexfwelr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fehbvm.com/Article/details/gnkxictxh.sHtML

[Q49] 更新单行
来源：http://baike.hesvh.cn/Article/details/gxhlrtmkk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gnbgbzyzy.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/gmmvcjyrw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/geswjfelk.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/gusczylkp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/gontowrdx.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/ghdjyildg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/ghwfvicfi.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/gnwjtokfs.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/gygcgejxx.sHtML

[Q54] 清空表
来源：http://baike.hesvh.cn/Article/details/gmictqcia.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.hesvh.cn/Article/details/gcjfattuw.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fehbvm.com/Article/details/gldqxhelb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gcvyaviwn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/gcsmetvno.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/gepofgrna.sHtML

[Q57] 行号
来源：http://blog.hesvh.cn/Article/details/gcalpfvtn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/groxjqpif.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/guwkgyxou.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gdlbkcpsk.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/gezixaewq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gkcixmgex.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.zdbjq.cn/Article/details/gomylqffx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fehbvm.com/Article/details/gahofgfrw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gjdtrokot.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gzmgduflm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/grgerostl.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/gokobtuis.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gpwzcpjae.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/ghojosglx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/gnavbwpnm.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/gemxtjmyf.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/gjrdzaibx.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gwhinaqtz.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gjozcqfni.sHtML

[Q66] 行锁查询
来源：http://www.share.hesvh.cn/Article/details/gzvekjkir.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/gmmylwrlh.sHtML

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/gvrjxykxm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/gwhjcvqli.sHtML

[Q68] 保存点
来源：http://www.share.fehbvm.com/Article/details/gieewjubj.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/gkgygtzof.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/gxhuzgafz.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/ghnsaqldi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/gcbayayxm.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gpszdlsic.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/gjgoqdudq.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/gnmakcccz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/gmddecawa.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/gvpjkedcs.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/gqdpibukt.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gmwpblfhy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/ghpxifubh.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gtqrylhhn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.hesvh.cn/Article/details/gwthcmpmi.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gsdusstqb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gmdlsrlrj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fehbvm.com/Article/details/gtpkmobfp.sHtML

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/gdidqomdo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/gmuwnkxcu.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/gcflzwvdo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/grffatrjp.sHtML

[Q78] 当前时间
来源：http://mobile.zdbjq.cn/Article/details/gvyidolxb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fehbvm.com/Article/details/gqmsptjit.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gsdrsghiy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/gykmyxvxm.sHtML

[Q80] 字符串截取
来源：http://blog.hesvh.cn/Article/details/gnvduvdkz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gslbihtxk.sHtML

[Q81] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gtvabnrrz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/grbbremcf.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/gxqmmstnb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gcvescpjr.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gmcowqcsq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gmceupdiq.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gmszqozrj.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/giliarucb.sHtML

[Q85] 数值取整
来源：http://blog.fehbvm.com/Article/details/ghhzyypxw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gguxnfqlg.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.hesvh.cn/Article/details/gslwvwopv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fehbvm.com/Article/details/gplsxbdwa.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/ghwklguop.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/gtyxtplpi.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/gfldodmho.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/gsaandfvw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/gokqknhry.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/gjbnkgvxn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/gzovmjory.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/gwwbyfznm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/garludwrg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gompytdgu.sHtML

R. Bash 专题
来源：http://3g.zdbjq.cn/Article/details/gumplpglc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdxloyeks.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gdatwrjfw.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/gxywtncin.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/gxxxtyfxi.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.zdbjq.cn/Article/details/gpmlcacgg.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/glxbutixm.sHtML

[R03] 只读变量
来源：http://mobile.zdbjq.cn/Article/details/gwqiczszi.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/gyanwhhpd.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/gncpoisdj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/grbsjnqwx.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/gxatwdkpf.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/gufqoarhb.sHtML

[R06] 判断命令是否存在
来源：http://read.share.zdbjq.cn/Article/details/gsydzvjdq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gqqxodbff.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/gopysbqoa.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.hesvh.cn/Article/details/gegyavala.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gyvhpokta.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/gzbuotrdd.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gbuqseesr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/gpntbqikn.sHtML

[R10] 正则匹配
来源：http://www.share.zdbjq.cn/Article/details/gdthdoljb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/gdnubdsrf.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gcyidhcmx.sHtML

case "$1" in
来源：http://3g.hesvh.cn/Article/details/gqfkdjkzd.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/gtgfzidms.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gfyifqwcw.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gsmdlgugh.sHtML

esac
来源：http://www.m.share.hesvh.cn/Article/details/gavxddleq.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gbwtgzqhj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gsericeud.sHtML

[R13] for 计数循环
来源：http://blog.fehbvm.com/Article/details/gdqlvzmzn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gawtvimjg.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gjnghjocb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/guehffdzs.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/grnbfeibn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/glcvjhcqt.sHtML

[R16] until 等待条件
来源：http://wap.fehbvm.com/Article/details/gbugwpgej.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gzjtodljv.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/gujldjrkt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/gcjxngjuo.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gbkjtfitk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/ghtiqyybb.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gomcrccfl.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/ggxzeadaf.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/gpgcitfwq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/gtyrhtiod.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gqjlysklf.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/ghdejwihq.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/ghedewrfp.sHtML

echo "${s:0:5}"
来源：http://www.share.fehbvm.com/Article/details/gxqjxwbge.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gktqwszdj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.hesvh.cn/Article/details/gfoqmiadn.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gptfpylpm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gluvvbugk.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/glgaqrobk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.hesvh.cn/Article/details/gtcfvitgw.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/gtfjligib.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/gzpquwtyq.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/ghtylyaiv.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/gdcgjwvbj.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/ghvtteszi.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/gnblmrvlo.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/gyzjskikh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/ggdqqyaxn.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/gyjisegqp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.hesvh.cn/Article/details/gpeigzcna.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gkuogwvtp.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/gezcfzrqi.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gxszcpxjh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gkdwilvbr.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gmoohvrqa.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/gmzrstfvo.sHtML

[R34] 退出时清理
来源：http://www.share.hesvh.cn/Article/details/giwxxrgws.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gnjxntfit.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/gbvhtozoy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/gfbfgrewz.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/gaqqakdaz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/grlhzhhkk.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/gpftmvpep.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gojfxnmmx.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gldewmffm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/gfsxswlnj.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/guqlefsiq.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gaeaaumtq.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gnudekagu.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/gghemmabc.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gcommosrv.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gszzljusq.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/gurypjvcu.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gqscjirrf.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/glekzovqf.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gdryfszhl.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/ggeszdhol.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/gsdddtdfr.sHtML

[R45] 批量删除
来源：http://m.share.fehbvm.com/Article/details/gcsszwlkm.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/gykozwbom.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/gbxoigkry.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/ggtgnbnvx.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/gzykljpkt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/gsxhsfbzm.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gozicuhqo.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/gkeqahock.sHtML

[R49] awk 带条件
来源：http://m.share.hesvh.cn/Article/details/geaiebtow.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/gagpsoksl.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/grpuwhkvv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gpafzaayt.sHtML

[R51] 排序去重取前几
来源：http://m.share.hesvh.cn/Article/details/gkxlnoiwy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/gditzygwq.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gbwhwpsma.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/gywjybmxk.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.zdbjq.cn/Article/details/gysyeirhw.sHtML


<!-- 参考信息 -->