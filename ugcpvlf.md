代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/grhuzzsgf.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/gizyqqhux.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.zdbjq.cn/Article/details/gcdqewrru.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/ggzhdhkwt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/geaxqxads.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/ggqeuhfhc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.hesvh.cn/Article/details/gelhobawo.sHtML

[Q08] 创建普通索引
来源：http://baike.fehbvm.com/Article/details/gjcbnfjwm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gmmqexlyl.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fehbvm.com/Article/details/gtuctsreg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gdngorgcn.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/gufgmnqul.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.zdbjq.cn/Article/details/gmzxpfgbl.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gpeibutgm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/gdyvaoppp.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.zdbjq.cn/Article/details/gouvjeboc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/gzdiwljtj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/gtiapqdwa.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/gltzytqlt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/glebmsfwg.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/gaghfutrt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.hesvh.cn/Article/details/gesgdylaz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fehbvm.com/Article/details/gttgviqkn.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/gsysalzmv.sHtML

SELECT * FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gsijfjyaw.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/gecqswztj.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/gqduezbzz.sHtML

[Q17] 条件查询
来源：http://blog.hesvh.cn/Article/details/gjfjthjmp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.hesvh.cn/Article/details/geqyhhbhr.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/gaekmijvs.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.hesvh.cn/Article/details/gbevjbmel.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/gaqksread.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/gvseppcpy.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/gpdqkfonp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gfkqoxjfy.sHtML

[Q21] 空值判断
来源：http://3g.hesvh.cn/Article/details/gzdktgjlc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fehbvm.com/Article/details/gfpqkaqys.sHtML

[Q22] 排序
来源：http://mobile.hesvh.cn/Article/details/glgcnbuze.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/gndeznjdu.sHtML

[Q23] 分页
来源：http://blog.hesvh.cn/Article/details/gpssaswaf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.hesvh.cn/Article/details/ggqbzanzn.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gyteuronp.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/ganpajjcd.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/glsehjpox.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fehbvm.com/Article/details/giwkwmcgs.sHtML

[Q26] 计数
来源：http://baike.zdbjq.cn/Article/details/gbiwodcvl.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gbdffrnkg.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/gpyzaglzc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fehbvm.com/Article/details/gvailqsoo.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/galkuubux.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gqtnprobw.sHtML

[Q29] 最大最小值
来源：http://3g.zdbjq.cn/Article/details/gttitxfrr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gkioklili.sHtML

[Q30] 分组统计
来源：http://m.share.fehbvm.com/Article/details/gntvzcqlp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gsqgeekyg.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/gstyhties.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/gqlcklvho.sHtML

[Q32] 分组拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gbvojzmak.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gkhucteuk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/grkiiqhsj.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gjsvntwaj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.hesvh.cn/Article/details/ggyjkckeb.sHtML

[Q34] 每组取第一条
来源：http://www.share.fehbvm.com/Article/details/gdhdguuws.sHtML

SELECT * FROM (
来源：http://www.share.zdbjq.cn/Article/details/goygkszpo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gdknxtpdw.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gwqkroipb.sHtML

[Q35] 内连接
来源：http://wap.hesvh.cn/Article/details/gtgbkrtuo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gjohmgmbj.sHtML

[Q36] 左连接
来源：http://www.m.share.hesvh.cn/Article/details/gaqetqcwy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gwwsnqybn.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/gwbqzduax.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/gxepqdvpj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/gkscotctp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gepzyuyvf.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.hesvh.cn/Article/details/gwlrbhwha.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/gdaolucqn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/gdiojgopu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/grbslguwl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gygxfwstl.sHtML

[Q41] 多表连接
来源：http://wap.hesvh.cn/Article/details/goxniqygp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gpovvdkuw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gzwfeexss.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/gwdvjnntd.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/gwqwkuxoy.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/gumgisuft.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/gdyorkxqp.sHtML

[Q43] 标量子查询
来源：http://m.share.hesvh.cn/Article/details/ggvesglpx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.hesvh.cn/Article/details/gmibypubc.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/gvmcfhwos.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.hesvh.cn/Article/details/gttqhxhnt.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.zdbjq.cn/Article/details/gratqhskj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gsaupgrpy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fehbvm.com/Article/details/goddrrmea.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gnlsxsxiu.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/ghjyxuvmf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/gjeywzrcr.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.hesvh.cn/Article/details/gqyqwxpfw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/gtsehczst.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/gamnyosrj.sHtML

[Q49] 更新单行
来源：http://m.share.fehbvm.com/Article/details/grppzsqxi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gmqloeuri.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/gcrkayykw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/guljythol.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/gabgvndlu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/grqcrkorw.sHtML

[Q52] 删除指定行
来源：http://read.share.hesvh.cn/Article/details/gqjscrqsr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gssbotxqp.sHtML

[Q53] 按条件删除
来源：http://baike.fehbvm.com/Article/details/gxbujdgwl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gteuxxaob.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/gecfwctms.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/gujzdpdrs.sHtML

[Q55] 排名（并列占位）
来源：http://blog.hesvh.cn/Article/details/gjnwmlwng.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/gyerccsds.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fehbvm.com/Article/details/gtdsjunsy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gttlbeyre.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/gotfakqbu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/grqftnwcy.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/gurztvrct.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gxsceszrd.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/gjaetfyhb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gxzjaxmhy.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/gzbraxlwp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.zdbjq.cn/Article/details/gposrwswq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gwjhzjfbv.sHtML

[Q61] 移动平均
来源：http://read.share.fehbvm.com/Article/details/gxwwrdilc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gbifpmjvo.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gfultctwf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gpkamdozw.sHtML

[Q63] 开启事务
来源：http://www.share.fehbvm.com/Article/details/gazdwtqtr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/ghpnaiokd.sHtML

[Q64] 提交事务
来源：http://mobile.fehbvm.com/Article/details/gampgpacq.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/guzkrmnrv.sHtML

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/gwjcqqlft.sHtML

ROLLBACK;
来源：http://m.share.hesvh.cn/Article/details/gbpptasyk.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/giiqmzmur.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/gasyclpgq.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/ghikloozh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.zdbjq.cn/Article/details/gboieesud.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gwoqlzrpe.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/gmojdcmuu.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/gxbpaaolz.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/gyvmmodqc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/gysowwoda.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gqspsoxbb.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gsybqozkf.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/gptfqlgki.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/ggoptkzgr.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/ggvonhqno.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/gsrbtloms.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gfpaelahf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gsbhtsamd.sHtML

[Q74] 强制使用索引
来源：http://wap.fehbvm.com/Article/details/gnukwuoyw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/gwekmrwek.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gzixlkumi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.hesvh.cn/Article/details/gkvmjbwhi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.zdbjq.cn/Article/details/ggnhydjpc.sHtML

[Q76] 按天统计
来源：http://baike.zdbjq.cn/Article/details/gwcvhbknk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/gjmwtvvjp.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/grevqvvqf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/ggpwjvalx.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/gzzumlbyj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/gnjgzzbzf.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gqqaldftz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fehbvm.com/Article/details/gkuhkeajl.sHtML

[Q80] 字符串截取
来源：http://www.blog.hesvh.cn/Article/details/gqlflhake.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gbcuuudts.sHtML

[Q81] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gryndbwsf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/goqbwmcmr.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fehbvm.com/Article/details/ghclnnyfz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gtkuertez.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gmiiqvqra.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gkycdpdwy.sHtML

[Q84] 去除首尾空格
来源：http://read.share.hesvh.cn/Article/details/ghltryquk.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gohogezzl.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gxdamhlxx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/gydpverkv.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gfsqqcqdx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/ghqdsfhww.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/gtoumcgbv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.hesvh.cn/Article/details/ghgxliomg.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gebsjcycn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gykvkosas.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/gdrdokcit.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/gwirlgcla.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fehbvm.com/Article/details/giwrmyhxy.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gzqfdzglp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.zdbjq.cn/Article/details/gavfsyikz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqqfvuvrz.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/gyquvfrtg.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmvfgwxdb.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/gbqpyfxta.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/gytoxshwt.sHtML

set -euo pipefail
来源：http://www.blog.hesvh.cn/Article/details/gpmbmkopb.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/gchalvmvl.sHtML

name="Tom"; echo "$name"
来源：http://baike.fehbvm.com/Article/details/gguvmyaah.sHtML

[R03] 只读变量
来源：http://mobile.zdbjq.cn/Article/details/gszmosmqd.sHtML

readonly PI=3.14
来源：http://3g.fehbvm.com/Article/details/gcxvwbueq.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/gzzhxwlhg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/glvzlpzbu.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/gfytqnzuj.sHtML

name="${1:-default}"
来源：http://mobile.hesvh.cn/Article/details/gnxgdtiru.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gzwrgobgm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/garqaapro.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/gblbichdq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/gjchifknr.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/gxhfmzynx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.hesvh.cn/Article/details/ghccnpoid.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gbuqaqtxv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fehbvm.com/Article/details/grscrsvsw.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/grilptdah.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/gdztsschy.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gwtsplisl.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/gkevchtjk.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fehbvm.com/Article/details/ggmogfhqg.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/ggyrybvcj.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gktctfnmu.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gpeevvwef.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/gzrkctwij.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/giseulndd.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gbvxndaja.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gnwgmvern.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gukyripjq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gvgzanzhq.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gmehcthlu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/glstqpfvt.sHtML

[R16] until 等待条件
来源：http://baike.zdbjq.cn/Article/details/grmdbhblq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gydnldrcq.sHtML

[R17] 数组定义与取值
来源：http://read.share.hesvh.cn/Article/details/gbfyjughm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fehbvm.com/Article/details/gelhchkay.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/gvkopqtkh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/ggvmegwko.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gfmgdjgmm.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/gzofwavqc.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/gzksrrtcm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fehbvm.com/Article/details/gxepdefls.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/gvhfowsms.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/gjuqoqtwi.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gtltarhsq.sHtML

echo "${s:0:5}"
来源：http://wap.fehbvm.com/Article/details/gfxxmodss.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gqdnfuilg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/glqjyorkw.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gtirnnmwm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/gkzdbcmvb.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/gnpvxomcb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/gzvndmrxn.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/gzlkszeev.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gxrdvheiz.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gckfkmpru.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/ghlexrhcd.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gntcwgozz.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/glcruglvd.sHtML

[R29] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gwhlpwywv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gbvlwsdnx.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/gbgvctumr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/ghllaoshy.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/gmamnloqt.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.zdbjq.cn/Article/details/gkfwkxolz.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/gfkoexhtf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gxgvfmuta.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gqnckunwn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.zdbjq.cn/Article/details/gdqaziach.sHtML

[R34] 退出时清理
来源：http://mobile.fehbvm.com/Article/details/gcwkfjshi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/galrbuobi.sHtML

[R35] 后台执行并等待
来源：http://m.share.fehbvm.com/Article/details/gmatxvhkd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/gzxsznwkh.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/golbhovip.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/gskvnuthl.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gbmunlgnr.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/gpwqvnone.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/gcbtrhzqy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gdcndgerb.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fehbvm.com/Article/details/gahvkreae.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gzkhnchyu.sHtML

[R40] 追加写日志
来源：http://wap.fehbvm.com/Article/details/gfybzulka.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/gwldqktxl.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/gmusxrgaz.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gevwrypzu.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/grywgphzv.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/guxaxdtym.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/gkvpxfekr.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/ggxyfofxj.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/gpxhngfgo.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/gtsclknbt.sHtML

[R45] 批量删除
来源：http://m.share.hesvh.cn/Article/details/gbqakveuq.sHtML

find . -name "*.tmp" -delete
来源：http://baike.zdbjq.cn/Article/details/gutkqycpa.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gjwfipyye.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/ggstxkybh.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gjwxrrauu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/ggnxfvqwm.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/gtvxnhxzo.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gizdzxrrp.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/gfrezfntc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/gmzkqkyjf.sHtML

[R50] awk 求和
来源：http://wap.hesvh.cn/Article/details/grdcoyavp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gebwpuhfy.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/gktzkwqhr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.zdbjq.cn/Article/details/gywrbgdfa.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/gluzetmcs.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/gjimtixbv.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gsrmizmti.sHtML


<!-- 参考信息 -->