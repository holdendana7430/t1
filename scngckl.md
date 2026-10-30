代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/gwizjgihb.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/gpliduipb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.zdbjq.cn/Article/details/gcbmgdwgz.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/glvajbnrc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gbibsentl.sHtML

[Q09] 创建唯一索引
来源：http://baike.fehbvm.com/Article/details/gozqnxuku.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gcajoynei.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/ggdjxqbye.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gksqrtwaq.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/ghkjpggzv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/gpnewyuty.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.zdbjq.cn/Article/details/gectjeimc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/gokwozkeq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.hesvh.cn/Article/details/govanscvr.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fehbvm.com/Article/details/gnjrnbvcr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gvfcwgeio.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gljqgyfmg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.zdbjq.cn/Article/details/gvxnosoor.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.zdbjq.cn/Article/details/gttaxprpm.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/gkiqciytg.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/gkyappurn.sHtML

[Q16] 查询指定列
来源：http://www.m.share.hesvh.cn/Article/details/gzvfnwrio.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/gnqftlpky.sHtML

[Q17] 条件查询
来源：http://read.share.fehbvm.com/Article/details/guwllgshn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.hesvh.cn/Article/details/gbjszrdbr.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/gdthakspb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/gddcmujpq.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/gnerbmxwg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fehbvm.com/Article/details/gyhshfxlg.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/gwhjutzag.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/gdduqrefb.sHtML

[Q21] 空值判断
来源：http://www.blog.zdbjq.cn/Article/details/gnizmzbni.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gxiwudptw.sHtML

[Q22] 排序
来源：http://mobile.hesvh.cn/Article/details/gpsqmnhhq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gntjxcwbo.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/gryzlosny.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/ghycogtuk.sHtML

[Q24] 去重
来源：http://blog.fehbvm.com/Article/details/gbcepwvyo.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gbjdplpoo.sHtML

[Q25] 只取前 N 条
来源：http://read.share.hesvh.cn/Article/details/gozpyihib.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.hesvh.cn/Article/details/gksdjnlve.sHtML

[Q26] 计数
来源：http://3g.zdbjq.cn/Article/details/gaiclbrvx.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/gkjhrmafy.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/gdsaokght.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.zdbjq.cn/Article/details/gvdqregkf.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/gbbesteyl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gdkjovjvu.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/gpjqvgyvz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/gqvggyhbi.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/ggwnxoygx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/ggrtcllen.sHtML

[Q31] 分组后过滤
来源：http://baike.hesvh.cn/Article/details/grelpvyyc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/gctmlbyji.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/gmijxulvj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gyyfcjxie.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gyqtvmtho.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/gqxxqilkn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fehbvm.com/Article/details/geguwfppz.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/gxrrqjboj.sHtML

SELECT * FROM (
来源：http://baike.hesvh.cn/Article/details/gugfqmliz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/glaqaxgsv.sHtML

) t WHERE rn = 1;
来源：http://m.share.fehbvm.com/Article/details/gwvcchfpy.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/gmxzakvbz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gqjwikpkd.sHtML

[Q36] 左连接
来源：http://mobile.zdbjq.cn/Article/details/gtzdcydgg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gdcgimdvn.sHtML

[Q37] 右连接
来源：http://3g.fehbvm.com/Article/details/gfjieunau.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gvcaclskh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/gtjxhcnuf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/gswpmonpr.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.zdbjq.cn/Article/details/gxuylqmfo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.zdbjq.cn/Article/details/gksgmzqqh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/ghxgepzld.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/gsxodolzr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.zdbjq.cn/Article/details/gkroyllyd.sHtML

[Q41] 多表连接
来源：http://baike.fehbvm.com/Article/details/gohwqkjsj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fehbvm.com/Article/details/gcdajboot.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.zdbjq.cn/Article/details/gaqcfjfjo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/gzaolgfid.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gdsvgblut.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/gumtdfigf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/gobriabqy.sHtML

[Q43] 标量子查询
来源：http://www.blog.hesvh.cn/Article/details/gpxzzetnn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.hesvh.cn/Article/details/goeiqyrem.sHtML

[Q44] IN 子查询
来源：http://read.share.fehbvm.com/Article/details/geqgroxpd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.zdbjq.cn/Article/details/gkievsgqg.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/gbfbbijkh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gjfevvzze.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.hesvh.cn/Article/details/gmkrnvfbo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gvzsxisuz.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/ghausuftu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/gffbovlyd.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/gqdgwlyjk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.hesvh.cn/Article/details/gnyjrzemu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.hesvh.cn/Article/details/gwbhgmerq.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/gykwrdpqe.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gomtsgyhr.sHtML

[Q50] 批量更新
来源：http://wap.hesvh.cn/Article/details/graqgujmi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/gzrfgbbbz.sHtML

[Q51] 用子查询更新
来源：http://3g.zdbjq.cn/Article/details/gphybhmuv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/gfkadjawi.sHtML

[Q52] 删除指定行
来源：http://www.blog.fehbvm.com/Article/details/gkrormqwz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gwimcwaph.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/gbhlpfwjq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gityvdrlt.sHtML

[Q54] 清空表
来源：http://m.share.zdbjq.cn/Article/details/gviujiivw.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/gqyojodfc.sHtML

[Q55] 排名（并列占位）
来源：http://3g.hesvh.cn/Article/details/gpozspces.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.hesvh.cn/Article/details/gkdmgnzzm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fehbvm.com/Article/details/gtergxues.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gioqkxeta.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/gvterjtmp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/gooqwgymd.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/giybnjare.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gkokzxdww.sHtML

[Q59] 分组内累计
来源：http://3g.hesvh.cn/Article/details/gttqavenx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gcoxhlzlm.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fehbvm.com/Article/details/geikriyvq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/gjmwstjol.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gufiyihvx.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gyftwdlvx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gufpniylh.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/gfhtbiglc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gulbihprv.sHtML

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/gqmjnjffq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/gqtntirjd.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/gxdypjcgu.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/gykdnzaqv.sHtML

[Q65] 回滚事务
来源：http://mobile.zdbjq.cn/Article/details/ghwgsdpkm.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/gybgapkwq.sHtML

[Q66] 行锁查询
来源：http://www.m.share.hesvh.cn/Article/details/gwfvezkzv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/gwdojedkm.sHtML

[Q67] 设置隔离级别
来源：http://m.share.zdbjq.cn/Article/details/gudgtzvpy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fehbvm.com/Article/details/glqbagnuh.sHtML

[Q68] 保存点
来源：http://blog.hesvh.cn/Article/details/gczeocfvq.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gjuggugda.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/gtcnzhkqy.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/gnscmuvkp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/gawclmjve.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/grcspiawp.sHtML

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/guyfddyrj.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gvqezsjdz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gwzweycfr.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/ggdttljvt.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gzwhpowlb.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/gwxuksrcz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.zdbjq.cn/Article/details/gptzajxge.sHtML

[Q74] 强制使用索引
来源：http://www.blog.zdbjq.cn/Article/details/grxaurfyd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fehbvm.com/Article/details/gkvkjulrw.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gfnutmzcf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gegrsemzb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/gegvkqjwz.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/ghhvnmlmj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/gkvrqzzya.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/givybrikd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gpcsmedoh.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gujteokeh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/gephovvyy.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/giucouttr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gnyvwgcwr.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/gogqcsqvj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gxxbfwiwh.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gpioopspr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/gdpuuhvru.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/gbwakjhpd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gdbnisdmg.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/goyzbmnmu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gtdfusvdg.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gbunudrtr.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gazddqdlg.sHtML

[Q85] 数值取整
来源：http://www.share.hesvh.cn/Article/details/gvftvrzkr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gsqolpivf.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/gtixxiypf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/ghhcmeiwx.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.zdbjq.cn/Article/details/gwzyjuctt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/giqmhzokp.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/gdongepgd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fehbvm.com/Article/details/gbakqlfgp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/gcwugdshq.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gwofctvhf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/gminmsxnz.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/gwbmhueox.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/gllodubqh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvikvhytd.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/gkduirqlf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gickzzjod.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/ghuizwxhv.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/gbgvswktv.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gotkgwlnh.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/gyfrlyhuf.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/gqvglukhg.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/grczycdoa.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/giwwsyvdq.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/goyhlbfer.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/gdfdorbtz.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gizlqibla.sHtML

name="${1:-default}"
来源：http://www.m.share.hesvh.cn/Article/details/gfxtzdriv.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/gvpfzauge.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gbfiethir.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/grtxqhcwd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/gmqslbgtc.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gzulojomx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.hesvh.cn/Article/details/gjrzfoydl.sHtML

[R09] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/ggzkdglvw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/gvkfazxyc.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/gkinwuvrc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/gdfbyuneu.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gugbtogcz.sHtML

case "$1" in
来源：http://read.share.fehbvm.com/Article/details/gvgrackvb.sHtML

start) echo "启动" ;;
来源：http://mobile.hesvh.cn/Article/details/gbbnimson.sHtML

stop)  echo "停止" ;;
来源：http://wap.hesvh.cn/Article/details/gkeviqxcb.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/goxtqpkjc.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/gsabbjmjm.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/gxaoypfuk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.zdbjq.cn/Article/details/gruetvnde.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gdnlohlmf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gtftkbqgb.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/gruapmywy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/ggubswzjn.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gnclddxpt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fehbvm.com/Article/details/gpeiarjtt.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/glkqafqzg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gpebvvhms.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gqwwsindr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/gjbygvavu.sHtML

[R18] 遍历数组
来源：http://www.m.share.zdbjq.cn/Article/details/gvtbxqzoj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gjgnlueim.sHtML

[R19] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gxcbhdmjo.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/gtaqrexhl.sHtML

[R20] 关联数组（字典）
来源：http://read.share.hesvh.cn/Article/details/gnadvtejp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/guqegtmbx.sHtML

[R21] 字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gnosnqptj.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/giszluakh.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/geyjagroa.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/gkftykfko.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/ggpvozucp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/gyqwfxaix.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gisrghnyp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/giauxxdzt.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/geoaunzjh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/gahykqrxd.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gqbnyoedf.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/gakjijfwg.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gqwasgtei.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/gdtmcdnpu.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gygdxyise.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/gevdpmjxn.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/grmzkxcqg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/gvfpdatqk.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/gtbsubbwu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/gqzzbaddu.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/gdvppomrv.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/gazdkwixn.sHtML

[R32] 参数个数校验
来源：http://wap.zdbjq.cn/Article/details/gxnhbaacf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/goevywslp.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/gzmvplkjf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/gnaoeezal.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gmmrjnlvv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gvqedryyd.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/gdujrzcvl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/gacuksjls.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/gqbghytip.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.zdbjq.cn/Article/details/gjwyzhfda.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.hesvh.cn/Article/details/gbotfahsn.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/gkbzkfznl.sHtML

[R38] 管道串联
来源：http://3g.hesvh.cn/Article/details/giwcwhdid.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.hesvh.cn/Article/details/giwnhdqdg.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gedqghjyw.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/gkhthaays.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/glptwmysj.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/gxeuevrmk.sHtML

[R41] 丢弃输出
来源：http://www.m.share.hesvh.cn/Article/details/gumqjatso.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fehbvm.com/Article/details/gslvspbbs.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/gzjiohvnk.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/guczpklpp.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/gswlnegxf.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/gsvikkyhk.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/ghrfrsezl.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/gktivijpq.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/gcbmouosg.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/gnhwnqeoq.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/gnramjgea.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.hesvh.cn/Article/details/gjxzlrtkg.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/guaichkbo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gvdcmcaan.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/gfkvzfkmd.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/gwbkxhdin.sHtML

[R49] awk 带条件
来源：http://www.blog.zdbjq.cn/Article/details/gzxskgncw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gybbctwbz.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/gwvzrejhj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/ghmnoyyqv.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/gtytdryyh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gucxlcmeo.sHtML

[R52] 统计行数
来源：http://read.share.hesvh.cn/Article/details/gvgqojcbc.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/gxpdfcujr.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/gjvqosjsg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gmzcvuxha.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/gkfjfeplu.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/gqqyfoydc.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gzmajrryb.sHtML


<!-- 参考信息 -->