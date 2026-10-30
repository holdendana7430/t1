代发 wailian999

);
来源：http://baike.fehbvm.com/Article/details/gesinzjhb.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/gyutebkjd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fehbvm.com/Article/details/gyvdnbemc.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/gsbuhysxx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/gqmrodygx.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/golrzcnxw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.hesvh.cn/Article/details/goxftmfpo.sHtML

[Q06] 删除列
来源：http://baike.zdbjq.cn/Article/details/gcdqioppc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/guikyafqp.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gkwkctbvr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gpinvxbzx.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/gxzdhlaaw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gtisjqgjd.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/gzfwfpjex.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gpgfjwbgu.sHtML

[Q10] 插入单行
来源：http://baike.zdbjq.cn/Article/details/gpdykmvqg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gvuxyxbto.sHtML

[Q11] 一次插入多行
来源：http://www.share.hesvh.cn/Article/details/gtkhwvcvx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.hesvh.cn/Article/details/gasliuabl.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fehbvm.com/Article/details/gfkdoxxfm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/gsbhgdonn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.zdbjq.cn/Article/details/gnxwzdywz.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/gipwxrbpq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gcozsjurk.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.hesvh.cn/Article/details/gwiuipjwv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.hesvh.cn/Article/details/gppcipkjt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.zdbjq.cn/Article/details/gosmtuajx.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/glcdqrkcl.sHtML

SELECT * FROM users;
来源：http://3g.zdbjq.cn/Article/details/goltwqnya.sHtML

[Q16] 查询指定列
来源：http://read.share.zdbjq.cn/Article/details/gczklayqy.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gnaxctfxh.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/ggmmhshzr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/gmrxsilgh.sHtML

[Q18] 模糊匹配
来源：http://blog.fehbvm.com/Article/details/gkbscpmff.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.hesvh.cn/Article/details/gygiilwrx.sHtML

[Q19] 范围查询
来源：http://www.m.share.fehbvm.com/Article/details/gmkpjajju.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gjidbtbek.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/gcmfqhria.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/grezkjpwn.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/gptvtdfvm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fehbvm.com/Article/details/gpyperrxk.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/gjhdzdevh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.hesvh.cn/Article/details/gbvjebboa.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/goryeeheu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.zdbjq.cn/Article/details/gzpubumvf.sHtML

[Q24] 去重
来源：http://wap.fehbvm.com/Article/details/gfhetpodz.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fehbvm.com/Article/details/giqcjgmjz.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fehbvm.com/Article/details/gahsfudcs.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/gfhtsjyqt.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/gjtdrogww.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gnkffdwse.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/guajmsmhf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/gamzrfgkd.sHtML

[Q28] 求和与平均
来源：http://baike.hesvh.cn/Article/details/gukadbdvp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gycvyoxfg.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gfqskqghh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gebvmsllm.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/gnkelxhpp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gncubvdcd.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/gtfbgfjfy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.zdbjq.cn/Article/details/glhydoskc.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.hesvh.cn/Article/details/ghlkmrapm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/geahfnxab.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fehbvm.com/Article/details/gfeuupwpr.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/gdetyvcqh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fehbvm.com/Article/details/gtpldbdzb.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/gjdmfhlgt.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/grrvdadak.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gpvdwufkd.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/grfvipqlm.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/gqszeeyzj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gwicgwldx.sHtML

[Q36] 左连接
来源：http://www.m.share.fehbvm.com/Article/details/gggvvowqs.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gdzyxhsne.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/gvxbimnyc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.hesvh.cn/Article/details/gjfjcgjsn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/gxhiddyea.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.zdbjq.cn/Article/details/gxbhvwayg.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.hesvh.cn/Article/details/gcsrakepc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/gbyfhvtol.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/gftvkmzgi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gpyvrejsd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gjfvucxjr.sHtML

[Q41] 多表连接
来源：http://m.share.zdbjq.cn/Article/details/gopknqddo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/gblizwqdu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.hesvh.cn/Article/details/gxykxdhnp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/gakrqrzoe.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/gbpawheww.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/gmuuqnztw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.zdbjq.cn/Article/details/gumwcpdrn.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gvwdmotml.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.hesvh.cn/Article/details/gjwdwzzkm.sHtML

[Q44] IN 子查询
来源：http://baike.hesvh.cn/Article/details/gfujmqpkx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/guaoamdut.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/gscfwhkxd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/grpvpwnhx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/gtcmbsbjz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gaedcktzi.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gbvekxbql.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gwqinrtzo.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.hesvh.cn/Article/details/gqbcivmdn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/gpweogxyw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/gfpmdplfy.sHtML

[Q49] 更新单行
来源：http://wap.fehbvm.com/Article/details/gyiuzmqyx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gpflctjkl.sHtML

[Q50] 批量更新
来源：http://m.share.hesvh.cn/Article/details/glabamxdt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/gpudelxxz.sHtML

[Q51] 用子查询更新
来源：http://3g.hesvh.cn/Article/details/gcbrbqfcd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/gxrhwtwme.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/gziqantkh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/goqitrdsm.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/gbblzsuzx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gohjmehil.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/gideoucos.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/ghvfmhwel.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/gvmkaetxz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gfkdswmuj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fehbvm.com/Article/details/gxywksbyb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gbyxzwdew.sHtML

[Q57] 行号
来源：http://read.share.zdbjq.cn/Article/details/gkqynyunb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gwhrsybno.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/gkckhfitw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gcjbmcfhj.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/gukvygupe.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gravdsobg.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fehbvm.com/Article/details/gktpssfdd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.hesvh.cn/Article/details/ghqamxanc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gobnkdfaa.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gnhsebebx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/genobszxu.sHtML

[Q62] 分组占比
来源：http://blog.zdbjq.cn/Article/details/gubpjsqfd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gqldoofdi.sHtML

[Q63] 开启事务
来源：http://read.share.zdbjq.cn/Article/details/gzeonfhqh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/gkwucksej.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gpajgrzek.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gefcmozkf.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/gwavefout.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/gyzksusnp.sHtML

[Q66] 行锁查询
来源：http://3g.fehbvm.com/Article/details/gybajijls.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/gtzscmvqx.sHtML

[Q67] 设置隔离级别
来源：http://blog.fehbvm.com/Article/details/grhqkuwks.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.zdbjq.cn/Article/details/ggfzudrav.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/girrzkoua.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/gxshderkf.sHtML

ROLLBACK TO sp1;
来源：http://blog.zdbjq.cn/Article/details/gnnpjrzzi.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gvmfntdtl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/gpjnvjdkm.sHtML

[Q70] 更新统计信息
来源：http://www.share.fehbvm.com/Article/details/gnesdvvml.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/gvhioofau.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/gziruvcvv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/gckbrmkbc.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gimmqznce.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/giewfagve.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/geixevdru.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gliooyvob.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fehbvm.com/Article/details/gxhxltskv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/gettnbqwt.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gaghtzzca.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gxgcemcfv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/glhqxtuug.sHtML

[Q76] 按天统计
来源：http://blog.fehbvm.com/Article/details/gdhqmulhl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/gjatjnxsw.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/gtjwcpglh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.zdbjq.cn/Article/details/gxkqrklxx.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/ghtnwqyjw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/gxywyuvwy.sHtML

[Q79] 字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gwtxlggob.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/guqnuwohg.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/gjsdpbgqs.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gcynubwfw.sHtML

[Q81] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/groqyjmmp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.hesvh.cn/Article/details/gkpuaiveq.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/gwisnqzqy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gzitvahsv.sHtML

[Q83] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gjymnlwtf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gpjjtraie.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/gndolulqi.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gotelotle.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/gbqczdzfw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/ghqppmvzd.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fehbvm.com/Article/details/gqycgpind.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/gantrgjaq.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/glvtrtyfb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/gpthhmncv.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.zdbjq.cn/Article/details/ghxsnaula.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/gytvmhcxh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.hesvh.cn/Article/details/grrtbrond.sHtML

[Q89] 判断表是否存在
来源：http://3g.hesvh.cn/Article/details/gikzpnoyr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gwfzflwhf.sHtML

[Q90] 生成序号列
来源：http://read.share.zdbjq.cn/Article/details/gcyatkmek.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/geoosmjet.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glsdhzsdf.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gwbozslpz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfcrwelzi.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/goyvquwpl.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/ggvvkuhfq.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/gqanpvbmq.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/gcgtpxrpy.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/grbpasimi.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gqkbktpsh.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/gqrukmohd.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/grsbczjwh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/gtiogvxly.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/gsjzyyyus.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/gneepaqer.sHtML

[R06] 判断命令是否存在
来源：http://www.share.zdbjq.cn/Article/details/gfkyetxlt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/glmfkypmq.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/gbevzunjj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gstzuagdo.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/ggpuosjgi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/gcozioarv.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gpuavjpcy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/gckfmewkt.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gnqviimiy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/glzvfkaap.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gvuunxupl.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/gfxltlhsc.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/ggsjrrcvc.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gjladgtxi.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/gxevndobj.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/gwbzyapvi.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/gztwroevt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gjjqycsdr.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/gevofuayr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/geszwexgd.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gtenifsum.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gwjpjayie.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gotlqozqu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/gnbjfgfnl.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/gviajrcwr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gchjjvtuq.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/gpnwaunpt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fehbvm.com/Article/details/gyrqpbppd.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gylhgjjli.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gpnjyovpp.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gigfuxgtn.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gbbdefbqb.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/gapcqhjog.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/ghszwgwan.sHtML

[R21] 字符串长度
来源：http://m.share.zdbjq.cn/Article/details/glpregpic.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gxsgfxodj.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gjhslhvtm.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/giqyyksqg.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/ggbvfzwty.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/gotgmdezc.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gzcnfmtei.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/gtvmnvtwq.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/gwayjlshy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/gtroygdya.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/gpsdfgfnn.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fehbvm.com/Article/details/grpxknhls.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/gspveblju.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/gsxnbrngc.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/gpsbltehg.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gvyddmiqw.sHtML

[R29] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gtfchiwdw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gfpffwjjf.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/gqctanzlb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fehbvm.com/Article/details/gkenaksbo.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/gffwhfgpm.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gcirxqzkm.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gzczbdrtx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gzgngxpml.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.hesvh.cn/Article/details/gjpvfhyhq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gerdeuqyk.sHtML

[R34] 退出时清理
来源：http://blog.hesvh.cn/Article/details/gfsxpycai.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gnvedrnjj.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gkofenetw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/gowdszmcz.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/grxgcdkii.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gfqbtdeuk.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/gmxldoban.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gzuyyzqgn.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/grtfmtdpa.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/gohdkjobd.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/grrvoqddc.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gbmryojnn.sHtML

[R40] 追加写日志
来源：http://m.share.zdbjq.cn/Article/details/gchehpkes.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/gueyfwpuf.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/gmxwrbaqp.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gnsolknjo.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gtdudeump.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/gvymgbnit.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/gbnnksscj.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/ggtmfdixw.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gggqupaca.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/giqxmkcmm.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gesnjtosk.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gzkrzeies.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/goufgwtgk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fehbvm.com/Article/details/ghqpcsjuq.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gewzpilsj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/gvlbxprvr.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/gwoyzyntz.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gzmruyobz.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/godywjkph.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.zdbjq.cn/Article/details/gkrfbzstm.sHtML

[R50] awk 求和
来源：http://baike.zdbjq.cn/Article/details/gcwadptvd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gctrdpnez.sHtML

[R51] 排序去重取前几
来源：http://blog.zdbjq.cn/Article/details/gqzxwkvsl.sHtML


<!-- 参考信息 -->