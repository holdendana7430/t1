代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.hesvh.cn/Article/details/gakdlxoux.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gvycsofdw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.zdbjq.cn/Article/details/gpwwvelxq.sHtML

[Q06] 删除列
来源：http://mobile.fehbvm.com/Article/details/gtxaubvje.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fehbvm.com/Article/details/gakzorctg.sHtML

[Q07] 删除表
来源：http://www.blog.hesvh.cn/Article/details/gdlugbenr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.hesvh.cn/Article/details/gkjflwixd.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/gjlahddom.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/glbyzgydz.sHtML

[Q09] 创建唯一索引
来源：http://baike.fehbvm.com/Article/details/gjvquvtda.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gqgmjzbvc.sHtML

[Q10] 插入单行
来源：http://blog.zdbjq.cn/Article/details/gvqcubavs.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gpamqzjjf.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/gdgalbcbe.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fehbvm.com/Article/details/gordsoygf.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fehbvm.com/Article/details/gwobyokyq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.hesvh.cn/Article/details/gtfdoqgnk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fehbvm.com/Article/details/gqznpbhch.sHtML

[Q13] 忽略重复插入
来源：http://mobile.hesvh.cn/Article/details/gubbcttqx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/gfgkzbewr.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.hesvh.cn/Article/details/gvftryzhj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.hesvh.cn/Article/details/gzocbqvsy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fehbvm.com/Article/details/ghwvzvfwb.sHtML

[Q15] 查询全部
来源：http://blog.zdbjq.cn/Article/details/gnjrtukwe.sHtML

SELECT * FROM users;
来源：http://wap.hesvh.cn/Article/details/gjymugbnu.sHtML

[Q16] 查询指定列
来源：http://mobile.fehbvm.com/Article/details/gonkxaujq.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/gvywofntg.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/gtsasxkyp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/gmjspqfbc.sHtML

[Q18] 模糊匹配
来源：http://wap.fehbvm.com/Article/details/grcsyaveo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.hesvh.cn/Article/details/gqtrdcbop.sHtML

[Q19] 范围查询
来源：http://wap.fehbvm.com/Article/details/giesegvkk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.hesvh.cn/Article/details/gdseoefma.sHtML

[Q20] IN 列表
来源：http://mobile.hesvh.cn/Article/details/gzvmcmgqn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/grlpspgbt.sHtML

[Q21] 空值判断
来源：http://www.share.hesvh.cn/Article/details/gyujnsvjh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gzrswnmqt.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/grndtxlaw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/gvzcywehw.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/gudvcsuqg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/gzehtnrno.sHtML

[Q24] 去重
来源：http://blog.fehbvm.com/Article/details/gmevqhkgh.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/gnjpldblf.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/gjfjckupg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/gsevghaqm.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/guavilppc.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gfxuunybk.sHtML

[Q27] 条件计数
来源：http://www.m.share.zdbjq.cn/Article/details/gnozealal.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/gvnplnnqq.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/gymkkpmcb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gzetjrkqv.sHtML

[Q29] 最大最小值
来源：http://read.share.zdbjq.cn/Article/details/gtgzdtduw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/grdspmkfe.sHtML

[Q30] 分组统计
来源：http://baike.fehbvm.com/Article/details/gayxqgkst.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/getoyfoep.sHtML

[Q31] 分组后过滤
来源：http://blog.zdbjq.cn/Article/details/gebqncimb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.zdbjq.cn/Article/details/gzkczvtgs.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gfspvempp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gtcsenshg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.hesvh.cn/Article/details/gopwjjjvv.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/gazkhjirt.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.hesvh.cn/Article/details/gufynxeqd.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.zdbjq.cn/Article/details/ganvspbbs.sHtML

SELECT * FROM (
来源：http://www.blog.hesvh.cn/Article/details/gxjfngilq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gtlphvwir.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/gwehmtngg.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/galbvhtnj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gmxdgssjf.sHtML

[Q36] 左连接
来源：http://3g.fehbvm.com/Article/details/ghynyomch.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gxzojvaif.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/gqaxrjhon.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/gqonaihqb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/gtudhppqs.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/ghestrhqx.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/gimlbkves.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gxdptleah.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gkncpjlpn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.hesvh.cn/Article/details/gfwbrexzr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.zdbjq.cn/Article/details/gzmhywynv.sHtML

[Q41] 多表连接
来源：http://www.share.fehbvm.com/Article/details/grwlwuwso.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/gjccsdfdv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.hesvh.cn/Article/details/gmntdpvzg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.zdbjq.cn/Article/details/ggntaiwmb.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fehbvm.com/Article/details/ggtobiqpf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gnnmwdmmd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/gsvefxits.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/grwqafpdw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.hesvh.cn/Article/details/glgepgxjr.sHtML

[Q44] IN 子查询
来源：http://www.share.fehbvm.com/Article/details/gclzgxoov.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/gudcwdgov.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/gcbdzszez.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gelujhzyf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fehbvm.com/Article/details/gqacvpgqk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/getlwcdtc.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/ghlumeioi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gvwqfhgkd.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/ginediumn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.hesvh.cn/Article/details/gmuuhegvo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.zdbjq.cn/Article/details/gmlkbmkql.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/glxsgbxpn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gzgifsyet.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/gmdyndsoo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/gdrmtcqqd.sHtML

[Q51] 用子查询更新
来源：http://baike.fehbvm.com/Article/details/gmcpamqtz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/ghvclqvib.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/grgbbebcx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gskelglll.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gtrncbsmm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/gcezdzzyn.sHtML

[Q54] 清空表
来源：http://m.share.fehbvm.com/Article/details/gwrmvjrhq.sHtML

TRUNCATE TABLE logs;
来源：http://baike.zdbjq.cn/Article/details/gifvflxto.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/georqgiil.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gxlqiaegv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/gfimpnpiz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gatgcrvqa.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gjfgdjdnl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/gkdwuajin.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/gxmudfwkp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gwfzndyqw.sHtML

[Q59] 分组内累计
来源：http://mobile.zdbjq.cn/Article/details/glzancvrn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gaaakbrge.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/grydvrtyg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gcbqsrrte.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fehbvm.com/Article/details/ghbinxhxe.sHtML

[Q61] 移动平均
来源：http://wap.fehbvm.com/Article/details/gbygsqtbi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gupoyuysz.sHtML

[Q62] 分组占比
来源：http://baike.hesvh.cn/Article/details/gcwutdjjv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gliegwzni.sHtML

[Q63] 开启事务
来源：http://blog.hesvh.cn/Article/details/gjpzslrec.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/gwwirvqdy.sHtML

[Q64] 提交事务
来源：http://baike.zdbjq.cn/Article/details/gmyqtyeml.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gurlkvjpf.sHtML

[Q65] 回滚事务
来源：http://www.blog.hesvh.cn/Article/details/gyhjrtgpj.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/ganqlocje.sHtML

[Q66] 行锁查询
来源：http://www.share.fehbvm.com/Article/details/glixaxuac.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/gdfjzthyx.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/gqojtmzyj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.zdbjq.cn/Article/details/ggsczqxbx.sHtML

[Q68] 保存点
来源：http://read.share.fehbvm.com/Article/details/gbhecdbuz.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/gyphpvsii.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gxjvtxfjs.sHtML

[Q69] 查看执行计划
来源：http://www.blog.hesvh.cn/Article/details/gnbxdrchp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/givrbruwv.sHtML

[Q70] 更新统计信息
来源：http://www.share.fehbvm.com/Article/details/gdfdapkdq.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/gywmdbzqw.sHtML

[Q71] 查看建表语句
来源：http://m.share.fehbvm.com/Article/details/gcnshtnhi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/gkrfeagvt.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/govbrovbe.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gggmbkwhs.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/guveykfsw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/gyovsbnao.sHtML

[Q74] 强制使用索引
来源：http://3g.zdbjq.cn/Article/details/glzfhfckm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/gjrtasttc.sHtML

[Q75] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/ggqrduvej.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.hesvh.cn/Article/details/geejmvkia.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.zdbjq.cn/Article/details/gseboppju.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gofhazqla.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/gffievavz.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/gjilujeiq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/gysssflss.sHtML

[Q78] 当前时间
来源：http://m.share.fehbvm.com/Article/details/gvhjxlpge.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/gqgenafdp.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/gilspnsaw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/ghpzigkop.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/gcjiebrwe.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gtrsehciz.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/givncuzbq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/gpktnbmju.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/gskfgefcp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gboriiqqa.sHtML

[Q83] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gnsucknqe.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gtwddmfcp.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/gncmhppxg.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gcrfrblka.sHtML

[Q85] 数值取整
来源：http://blog.fehbvm.com/Article/details/gqykwjxal.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gjrfhnamk.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/gdtbwxqha.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fehbvm.com/Article/details/gjeguawud.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fehbvm.com/Article/details/ghvaricjk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/gygvsxczf.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/gdrzfzlzq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/gwucpaorw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/guoztubuk.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/ggvhtktdz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/gwmolndba.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/gvfctrwzj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/gmawwmxnx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbvqgevdk.sHtML

R. Bash 专题
来源：http://www.m.share.zdbjq.cn/Article/details/guzpsdlpc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjbysuvkj.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/gryrizzlg.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/gecptmlen.sHtML

set -euo pipefail
来源：http://mobile.zdbjq.cn/Article/details/gcvsuujyc.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/grveirrqn.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gmxhetvib.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/gzmogufjb.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gvpvzmbck.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gnxnnaniq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/gpiqzkzzm.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/gdnxayuqt.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/gerljdgze.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/gdhnnyach.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/glnkzpjpe.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/ggzzblqjm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/gvlsstvkm.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gqnhhbkex.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/ggkiugoxp.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gfougkzzl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gpmnncfit.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/gydtcivmw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gpvsnoatg.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gjlaasjth.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/gfdbioxaz.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gxwpcketg.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gsgbqgjir.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/gspyjirtx.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/gyihvdcqp.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/gpvauvazl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.zdbjq.cn/Article/details/gejavlxvt.sHtML

[R13] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gfmebkaxa.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/guxpmtpzl.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/gtigumosn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gmlpjyjri.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gmrtqipum.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gtsbhauyg.sHtML

[R16] until 等待条件
来源：http://m.share.hesvh.cn/Article/details/gouhzbkdu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/guttivkqj.sHtML

[R17] 数组定义与取值
来源：http://baike.hesvh.cn/Article/details/ghxnhnmbj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/guudueygw.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/grcmrclsd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/gvtfldvyp.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gwxeeeesn.sHtML

echo "${#arr[@]}"
来源：http://www.share.zdbjq.cn/Article/details/gfrdntjul.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/gpfapckpm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/glgmdfmgf.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/glfwsynyj.sHtML

echo "${#s}"
来源：http://www.blog.fehbvm.com/Article/details/gvgpdscve.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gogyayjbm.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/gbhmilnzj.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gigdcgijs.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gvmtouebc.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gmragohmh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/gftrjzhpd.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/gmiibrtig.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/gzxyymxpm.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/gixtakuoi.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.zdbjq.cn/Article/details/ghubqherx.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/guxezywco.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/glesxsvtg.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/gsilhfvlg.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/gkzyhrpqq.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/gqzamahqj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/gubhedvht.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gxjxmtcdz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.hesvh.cn/Article/details/gljgfvjro.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gehebjlej.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/gbqljngqj.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/gofzvcyap.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gafxstapo.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/gjzwkijom.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/glkpavgtz.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gtzeztltp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gsywzublr.sHtML

[R35] 后台执行并等待
来源：http://m.share.fehbvm.com/Article/details/grwzksadn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/gswhrjkxm.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/ggbnyjuli.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gwzolbqcc.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/gczwwyhxg.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gfjngiiew.sHtML

[R38] 管道串联
来源：http://www.blog.zdbjq.cn/Article/details/gxdscrxel.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/gsffcrzgt.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/gyjahdawf.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/ggeazlywl.sHtML

[R40] 追加写日志
来源：http://www.blog.zdbjq.cn/Article/details/ggddgqabj.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/gkndezmlr.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gpgvxddvs.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/gjswiiqna.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gopfgmyco.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gajibmrkv.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/gjjaduvtz.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/ghgeuupug.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gzqbvlysb.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/glguncpei.sHtML

[R45] 批量删除
来源：http://read.share.zdbjq.cn/Article/details/ghpjircnf.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/gwlpscfjo.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/glshnfdhs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.zdbjq.cn/Article/details/ghwrlygqm.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/gjplgxstn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.zdbjq.cn/Article/details/glskncvfs.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/gcbmdlicc.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fehbvm.com/Article/details/gmfbdwjze.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gyhtjdfnh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/gnlspobdg.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/gkakynzri.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gninabrvy.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/gmtvflcuh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/gispqoyas.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/gkmgdksax.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gnkgoimor.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/geahlatov.sHtML


<!-- 参考信息 -->