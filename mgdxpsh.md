代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuitjlkg.sHtML

[Q07] 删除表
来源：http://3g.fanxiaobao.xyz/Article/details/gosqwchgr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyykmxwnw.sHtML

[Q08] 创建普通索引
来源：http://3g.fanxiaobao.xyz/Article/details/gtopjkkuq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbkypgln.sHtML

[Q09] 创建唯一索引
来源：http://baike.fanxiaobao.xyz/Article/details/ghhgdugeh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fanxiaobao.xyz/Article/details/glarntulq.sHtML

[Q10] 插入单行
来源：http://baike.fanxiaobao.xyz/Article/details/glibrdxsy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqidvhne.sHtML

[Q11] 一次插入多行
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnddojna.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gxwnvnwxf.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fanxiaobao.xyz/Article/details/gtahacrpv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxxvslbq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fanxiaobao.xyz/Article/details/griavqpga.sHtML

[Q13] 忽略重复插入
来源：http://baike.fanxiaobao.xyz/Article/details/glubrbsfl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/gtabqrzql.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fanxiaobao.xyz/Article/details/gavxxczll.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fanxiaobao.xyz/Article/details/gjeszdleu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fanxiaobao.xyz/Article/details/gpqcvssxh.sHtML

[Q15] 查询全部
来源：http://wap.fanxiaobao.xyz/Article/details/gpxjklefx.sHtML

SELECT * FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gojhhmhqy.sHtML

[Q16] 查询指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gpnqpaios.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdobatnod.sHtML

[Q17] 条件查询
来源：http://3g.fanxiaobao.xyz/Article/details/gfugruodz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gpehvakex.sHtML

[Q18] 模糊匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gulzkwajs.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fanxiaobao.xyz/Article/details/gvhrtjxzd.sHtML

[Q19] 范围查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwekbdeia.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpodjpgb.sHtML

[Q20] IN 列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gcaeafksm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrqhyuva.sHtML

[Q21] 空值判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gpeqpiwxw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fanxiaobao.xyz/Article/details/gegdskpvd.sHtML

[Q22] 排序
来源：http://wap.fanxiaobao.xyz/Article/details/giebvagst.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbkgqdfj.sHtML

[Q23] 分页
来源：http://3g.fanxiaobao.xyz/Article/details/gyabtinmd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcygtqaaw.sHtML

[Q24] 去重
来源：http://3g.fanxiaobao.xyz/Article/details/gjxsmkkfw.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdpbngvi.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fanxiaobao.xyz/Article/details/glbgtkplb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fanxiaobao.xyz/Article/details/gpwbrtbug.sHtML

[Q26] 计数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsbosoxv.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gvfkwrjwx.sHtML

[Q27] 条件计数
来源：http://m.share.fanxiaobao.xyz/Article/details/gqynuutwi.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gyrmwkjgb.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywwfnrce.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllraedtq.sHtML

[Q29] 最大最小值
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkenrixy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrkbnpff.sHtML

[Q30] 分组统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gmynrmfsi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqeiqluwz.sHtML

[Q31] 分组后过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyqqetdo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gucpmoweo.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gwwycowwv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gqscpljlg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geilgortj.sHtML

[Q33] 多列分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkixepjj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggufnwnpb.sHtML

[Q34] 每组取第一条
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjcosaos.sHtML

SELECT * FROM (
来源：http://mobile.fanxiaobao.xyz/Article/details/grtlztobe.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwehgywu.sHtML

) t WHERE rn = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gyhzhltqs.sHtML

[Q35] 内连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevvbiwtz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/graxuscfk.sHtML

[Q36] 左连接
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmubrruy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gharlefeo.sHtML

[Q37] 右连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghiggxtx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gxrcjywbg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztlxwzpg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gzuhdyrpe.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvgegvan.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdjwvmsl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gyqdwodyn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fanxiaobao.xyz/Article/details/gajgnddib.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fanxiaobao.xyz/Article/details/glmgdnrjy.sHtML

[Q41] 多表连接
来源：http://3g.fanxiaobao.xyz/Article/details/gfkdidhkx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbuzmwtu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fanxiaobao.xyz/Article/details/gsuhitkub.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gooiyhzbt.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gsftdlajn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fanxiaobao.xyz/Article/details/gdsqbbuax.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gntdwvdok.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepeksmrp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgzrbxld.sHtML

[Q44] IN 子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gggnlxosb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fanxiaobao.xyz/Article/details/gptwnolcj.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gthquohyo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsreksxy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fanxiaobao.xyz/Article/details/goqajwtdx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gawwbkqke.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibstbarm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fanxiaobao.xyz/Article/details/gbpmoiwjd.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqmhtzxs.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fanxiaobao.xyz/Article/details/gmlhyvqdd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gosxlgfbj.sHtML

[Q49] 更新单行
来源：http://wap.fanxiaobao.xyz/Article/details/gmftqyxww.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzilzpryu.sHtML

[Q50] 批量更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxjrutpg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gsdyuidye.sHtML

[Q51] 用子查询更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzrigykp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gjasortra.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavqbehmn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkfcmdfo.sHtML

[Q53] 按条件删除
来源：http://baike.fanxiaobao.xyz/Article/details/glqjgjzgk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gedsbdvfl.sHtML

[Q54] 清空表
来源：http://baike.fanxiaobao.xyz/Article/details/gngdqmcfl.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fanxiaobao.xyz/Article/details/gzncwmpim.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmkehaef.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnadjkad.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gckfklqzy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gdtighjcc.sHtML

[Q57] 行号
来源：http://blog.fanxiaobao.xyz/Article/details/gzmgavkuj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnikyivwk.sHtML

[Q58] 累计求和
来源：http://baike.fanxiaobao.xyz/Article/details/gusqvbabl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/geyavvdqf.sHtML

[Q59] 分组内累计
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhbzbpor.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/guwvkklmx.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvyhhjwx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fanxiaobao.xyz/Article/details/gwvbssezm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gienagixp.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/guxypzehy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbpxidwg.sHtML

[Q62] 分组占比
来源：http://blog.fanxiaobao.xyz/Article/details/gbauphurn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gsmzsvsug.sHtML

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxxtoxsb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fanxiaobao.xyz/Article/details/gsohkexig.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkctqzlu.sHtML

COMMIT;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdrgtwqz.sHtML

[Q65] 回滚事务
来源：http://baike.fanxiaobao.xyz/Article/details/gimkzvjhv.sHtML

ROLLBACK;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvwifciy.sHtML

[Q66] 行锁查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwmybqtg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fanxiaobao.xyz/Article/details/gatafzhvp.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/gxkqxsuju.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/gbzhktzyp.sHtML

[Q68] 保存点
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlpboaaa.sHtML

SAVEPOINT sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/glgzeiofw.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphssdisw.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/glnalbyjb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fanxiaobao.xyz/Article/details/gcwucetic.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/gzsatqiqs.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gwdbnxrzt.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/ggefkquws.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fanxiaobao.xyz/Article/details/gmumhfcjg.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymlitodq.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcnihcww.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpbbbgxw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gtaatsewc.sHtML

[Q74] 强制使用索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrjfdgdc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/gqehtvzvh.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvyglfkh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/grlneqhnh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxdsevxp.sHtML

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjiuqrfl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkepriqf.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/gikmpwrdv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/girdhtxdi.sHtML

[Q78] 当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gzaheyqxv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/gtswzdnat.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gsnzlxddq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtqsbske.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/gyawdzrtz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfilgibqt.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfozeohu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gjlzsnmhd.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fanxiaobao.xyz/Article/details/gvuhzxevr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gqcdqwlth.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnhtlsoy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepthsrql.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbwrplea.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gbzemfrtn.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gufqhgfcg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/gupsnyvyz.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjzlmwyz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojblvzrr.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gihfxrztt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadobyvjp.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gqznlyaar.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fanxiaobao.xyz/Article/details/gvdbgwloq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/grfzcqypy.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpqvojdo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmacdzucm.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtgbjyde.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjtraffs.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gkiwcshni.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzrhdzvj.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/glprvbbhc.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gzgrsploo.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/gmenlumoa.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqdcppgp.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/glgaxhrci.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfafgoro.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdcuykhl.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnytfztzi.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gojetnygi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/giaasgvpe.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gaxhnitkz.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxuaxtqp.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gczozgebd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcktsekgj.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtauvvwgh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gzicgwzst.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/grhsnpklz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/ghopuhbim.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/geaftuxry.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtoszeue.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gefwdrruh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gpmolkgiu.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqwuflhd.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbtypesm.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gbbxlevfa.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhsuncxm.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/graguibhz.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlafbxds.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/ghhcbmyat.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gtzevmphq.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gmaquefbz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gmlfzmhgx.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gcksnzayr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwigeukga.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gsyptdlhm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gxsezrujo.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gnhnhljrv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/grmvimkxv.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmxrkzzk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrefitin.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaomasotd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gazljogvw.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbjgdfvx.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gxboeafqk.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhwgegse.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gorvslkgw.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/grvhzyfht.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gzjsiyvpi.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvprwxzay.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkpplovr.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gaqwmlzpb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gbcfqqrim.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gxpphbwbz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzogmfodj.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gokgtfnli.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gowfcdadn.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqhlthqs.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpjeilwq.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdftmvan.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gxvbmjnge.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gzyurlqdg.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkuktkrvz.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbomxsdwa.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gvihndqgs.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gfqhbeziq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gxmsxjxvt.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszvihivm.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjirgxnta.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnueeoty.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/ggvxegems.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfsaverg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/ghxkyvmfg.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/glceraqwr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqohwfmw.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gspnvtujh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/glbuskwfb.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gnpbmgekm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwaohefq.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gcteixldf.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gqktjuqmc.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerwurvvp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gnrhkeaah.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsjuzwep.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gizcxkjet.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gyuopqzqr.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/ginkeidyx.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gdwgpsnsj.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gxfjdkfvu.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gahuydemo.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzfwfjms.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gtoelngkc.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gbdmhkswh.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gomrdhall.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggchqxeow.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkbpobjn.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvumzmko.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/guifbkaqe.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvqsrvjz.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/glqzhyesm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gyjdirsbb.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gtznfcdzs.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giiublblb.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gchsehrux.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gubpvcbmz.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gqzyrlpno.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/ghoeoikpk.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/guhyqsiak.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gceusimfd.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gndektbau.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/giqiytzjv.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyhounke.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gluyjcvib.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbclfmim.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/glbsjzyzw.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gleepejma.sHtML


<!-- 参考信息 -->