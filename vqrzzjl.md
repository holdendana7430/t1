代发 wailian999

);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvhcllot.sHtML

[Q03] 增加列
来源：http://3g.fanxiaobao.xyz/Article/details/gpulllstc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fanxiaobao.xyz/Article/details/goiqwikpu.sHtML

[Q04] 修改列类型
来源：http://wap.fanxiaobao.xyz/Article/details/gofykxbam.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/gplgrvyla.sHtML

[Q05] 重命名列
来源：http://blog.fanxiaobao.xyz/Article/details/gigqxfqzu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fanxiaobao.xyz/Article/details/gkddelymx.sHtML

[Q06] 删除列
来源：http://baike.fanxiaobao.xyz/Article/details/gbqbqamvz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmqigois.sHtML

[Q07] 删除表
来源：http://m.share.fanxiaobao.xyz/Article/details/ghptvdrwf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzppfzxoc.sHtML

[Q08] 创建普通索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvuvvrlq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmyrfwis.sHtML

[Q09] 创建唯一索引
来源：http://baike.fanxiaobao.xyz/Article/details/ghsuturhl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fanxiaobao.xyz/Article/details/guwqasvjj.sHtML

[Q10] 插入单行
来源：http://www.share.fanxiaobao.xyz/Article/details/goshkasmq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gywwxovkk.sHtML

[Q11] 一次插入多行
来源：http://3g.fanxiaobao.xyz/Article/details/gueohbcrt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/gntlpjpbs.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fanxiaobao.xyz/Article/details/gxcqvnimx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fanxiaobao.xyz/Article/details/gxecrxylj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaspdbugc.sHtML

[Q13] 忽略重复插入
来源：http://wap.fanxiaobao.xyz/Article/details/giychmczu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcxlqnxb.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvaefwxi.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fanxiaobao.xyz/Article/details/gvsfrktqo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjcuyjhw.sHtML

[Q15] 查询全部
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrjcoitm.sHtML

SELECT * FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggazfmtnj.sHtML

[Q16] 查询指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzwlxysp.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnqnukge.sHtML

[Q17] 条件查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gwogunjit.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gktkkwbbk.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwxigwmy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fanxiaobao.xyz/Article/details/glfqoihhf.sHtML

[Q19] 范围查询
来源：http://baike.fanxiaobao.xyz/Article/details/gwgiwbzxo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwgwpaxk.sHtML

[Q20] IN 列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfussxqs.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyuwinku.sHtML

[Q21] 空值判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsocoiye.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fanxiaobao.xyz/Article/details/gbvvlzfae.sHtML

[Q22] 排序
来源：http://3g.fanxiaobao.xyz/Article/details/grnwsnopd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fanxiaobao.xyz/Article/details/gptyemhrk.sHtML

[Q23] 分页
来源：http://mobile.fanxiaobao.xyz/Article/details/gemypcxde.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfmuwnsw.sHtML

[Q24] 去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gnczgfadr.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/glxfcnwdr.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgtjomif.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fanxiaobao.xyz/Article/details/gaexbbnet.sHtML

[Q26] 计数
来源：http://www.share.fanxiaobao.xyz/Article/details/gsonuapru.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtvlknsb.sHtML

[Q27] 条件计数
来源：http://wap.fanxiaobao.xyz/Article/details/gwuqwahcw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gamgpzjws.sHtML

[Q28] 求和与平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsngnpiq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gqzwbapfb.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvvgwtwu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvpojpnn.sHtML

[Q30] 分组统计
来源：http://3g.fanxiaobao.xyz/Article/details/gymftlzjp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/giramzude.sHtML

[Q31] 分组后过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkuzfypr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/grjfdzntn.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/grcribprp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkrehokc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fanxiaobao.xyz/Article/details/gtzhtkkdi.sHtML

[Q33] 多列分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gointbnpx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifbzkrep.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdrnzvbo.sHtML

SELECT * FROM (
来源：http://3g.fanxiaobao.xyz/Article/details/gpirbxots.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fanxiaobao.xyz/Article/details/gvumkdvwl.sHtML

) t WHERE rn = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlepumzv.sHtML

[Q35] 内连接
来源：http://blog.fanxiaobao.xyz/Article/details/gitscrtru.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gxuzwooii.sHtML

[Q36] 左连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzolxsod.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giquaybva.sHtML

[Q37] 右连接
来源：http://wap.fanxiaobao.xyz/Article/details/gewpieutv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gjfviobgo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaakhgypx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnchukexk.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fanxiaobao.xyz/Article/details/gtqbeyvjr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fanxiaobao.xyz/Article/details/geyshsipk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gcfkkdevv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fanxiaobao.xyz/Article/details/gjngqohnc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fanxiaobao.xyz/Article/details/ghzxfvhth.sHtML

[Q41] 多表连接
来源：http://baike.fanxiaobao.xyz/Article/details/gmegfjyyt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fanxiaobao.xyz/Article/details/gvixpyfql.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fanxiaobao.xyz/Article/details/geiipfdsn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gezxjfzsy.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gshemeogu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fanxiaobao.xyz/Article/details/gegczuowg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/guixxldau.sHtML

[Q43] 标量子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gpllorzlc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpnjafcn.sHtML

[Q44] IN 子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gxawhdhhk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fanxiaobao.xyz/Article/details/geqijmoca.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkrmowzh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzrgcybu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgucllze.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcqzqgnx.sHtML

[Q47] 与平均值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyplgtkv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fanxiaobao.xyz/Article/details/gszqvkbro.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyiklxgje.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/gdsladvvv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fanxiaobao.xyz/Article/details/giipwcclp.sHtML

[Q49] 更新单行
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfeitdwa.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmpfnceh.sHtML

[Q50] 批量更新
来源：http://baike.fanxiaobao.xyz/Article/details/getlmycyz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyeygxdl.sHtML

[Q51] 用子查询更新
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjeshdap.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gpnyutojy.sHtML

[Q52] 删除指定行
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkpshwgs.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgcsiosq.sHtML

[Q53] 按条件删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrnyibqz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gkjgidzar.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/gkorpzqsu.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fanxiaobao.xyz/Article/details/grjojnrwd.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrciicae.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/girzwozoy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwytnwhep.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxusobjob.sHtML

[Q57] 行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqycjluyp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowuoujci.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gaivnpehi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gbgginpvf.sHtML

[Q59] 分组内累计
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqwjdhzi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guobsuxaz.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqvvjlzr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fanxiaobao.xyz/Article/details/gawwaxavk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gsvuovefn.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/gfbeetgxn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gdtuphbxr.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrytihba.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gubbzqtpq.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpddhxgg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllogeels.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrgkyqzl.sHtML

COMMIT;
来源：http://www.share.fanxiaobao.xyz/Article/details/gavnbfgsw.sHtML

[Q65] 回滚事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gsujmmzqt.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/guvlatblv.sHtML

[Q66] 行锁查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gznjznwli.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/glqptidqb.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/gykbwahpg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyitijfea.sHtML

[Q68] 保存点
来源：http://3g.fanxiaobao.xyz/Article/details/gxdwkxmwu.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbrdzuqt.sHtML

ROLLBACK TO sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gazscgaiv.sHtML

[Q69] 查看执行计划
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfbmsuvy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gogzhsehp.sHtML

[Q70] 更新统计信息
来源：http://3g.fanxiaobao.xyz/Article/details/gstrpixpe.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/grvuctfys.sHtML

[Q71] 查看建表语句
来源：http://baike.fanxiaobao.xyz/Article/details/ginvedaqo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fanxiaobao.xyz/Article/details/grqvrrxym.sHtML

[Q72] 查看索引
来源：http://3g.fanxiaobao.xyz/Article/details/gajnobqju.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtjbhlat.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/gkveiplph.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcqbicec.sHtML

[Q74] 强制使用索引
来源：http://baike.fanxiaobao.xyz/Article/details/gnawrkumz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/garhkillq.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gxtukftef.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gxnknlmfc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/gbagnrafu.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/gnxopfywe.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrcxnwgz.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqnibczy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffjlnedw.sHtML

[Q78] 当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gglumhotf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomfqrcpy.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdesyblt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/gnngjekom.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/glodyapfa.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjofgwsvi.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gjfkgnpsb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyluduket.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxogsast.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsixeasef.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gxioxbxmt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gmnnyafug.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/ggrpspvia.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsmnyrbi.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gwawogscr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/geaqncato.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqomqrdfo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymukxday.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzlkuqrl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxuhyvti.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/ggrnfngas.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxtdouxy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrujaewa.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwaswwceh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrdvpgql.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/gssdgyyny.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslihkfde.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/glhhuqwou.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/ghgvxtxsj.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyuzfuby.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwqzwixm.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gjscshbcl.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gcnqmlqqs.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gbglsromd.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnwjrxee.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwerepvz.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxdyvwne.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/guotxmmss.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/gczyinhwe.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gnlujwncp.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/goqwuxiln.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goiznhezh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkafrntmw.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/gcolapnpj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gaazzfajs.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gakzgprby.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdprwepxi.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlgehjmi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsupwghog.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikzzyiom.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/geatvhldf.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjbaicqg.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/groukgmkx.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtahgsive.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gfcsonmep.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gesgrsnlk.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbpweuae.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/glovfunqo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gjarldhmx.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/ggeyqowik.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gljxvngot.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzyulfzb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqxdwszs.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypsskdgk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/glqzerhpy.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gwcygsqjy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/groeeycwx.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/glxrflwtq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxayezwc.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gelwarztg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gjxzbwxwe.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gnurdurxa.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrnkxtfo.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gatmjdgdd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtidkpzqn.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gftxtkhcu.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gccsltted.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfivwcop.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gshneelgl.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbhchdzf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gwwsaggzz.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/garrourxi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gabeijlkx.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gmimvfkmw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsivqsgy.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/ghafbdrtq.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gqlgyrhow.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gubuzetac.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxcownjp.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyycvnty.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/guyegmnnu.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gwtabsvzp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gthpfqnwu.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdrhkyev.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxsjiwry.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyitqhkk.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpejfmdgv.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gysuiwofe.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gffwcpfzs.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gdgdowwai.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gshdixscz.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giynuqxzx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/ghwwioalx.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqpkwyhr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcaopupo.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gitcfxssn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpescplnr.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gogpvfnpt.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijwafxpq.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/guiuevcco.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/ghycpslzt.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gvccnkpco.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhltzyfj.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gahjzwhcj.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gurxixmhk.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzuvhhee.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwhmaequ.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gysiytdkn.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gqbhgfmzr.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/guclbrxzg.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqmgjzip.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gcdxofxto.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwwmweod.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasbasuzp.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/ggpqgcldc.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqexaahr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/guaezvwss.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gecpvvesp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gvadgoryo.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gurywbiop.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucltqnns.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gaokltnpn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gifuhxrpa.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gbutjokcy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gdaquqauz.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gkauzflwn.sHtML


<!-- 参考信息 -->