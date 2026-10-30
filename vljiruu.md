代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fanxiaobao.xyz/Article/details/glsfyowfw.sHtML

[Q05] 重命名列
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfbkrvfc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fanxiaobao.xyz/Article/details/ggnzngwjb.sHtML

[Q06] 删除列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwypbpjte.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqavisumc.sHtML

[Q07] 删除表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhytrhky.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gqfbbyowo.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjfhucqd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbinbwav.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gjurouldv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdpefhri.sHtML

[Q10] 插入单行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbiyalqj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/glyrqeuos.sHtML

[Q11] 一次插入多行
来源：http://3g.fanxiaobao.xyz/Article/details/gspjvdrhw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/gcapevhgz.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fanxiaobao.xyz/Article/details/goqqmjrzz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fanxiaobao.xyz/Article/details/gfvtotksp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxiildpi.sHtML

[Q13] 忽略重复插入
来源：http://baike.fanxiaobao.xyz/Article/details/gtmnerfyk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gguphatwo.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfojoioi.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fanxiaobao.xyz/Article/details/grkrulpay.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxpkjeao.sHtML

[Q15] 查询全部
来源：http://baike.fanxiaobao.xyz/Article/details/gcaxhridl.sHtML

SELECT * FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcioynyx.sHtML

[Q16] 查询指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/geddbnqdz.sHtML

SELECT id, name FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmypkmhze.sHtML

[Q17] 条件查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvcwdkvt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyihoabgz.sHtML

[Q18] 模糊匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gsptfjzvg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrubghym.sHtML

[Q19] 范围查询
来源：http://blog.fanxiaobao.xyz/Article/details/gdygskcab.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fanxiaobao.xyz/Article/details/gznzwycqg.sHtML

[Q20] IN 列表
来源：http://wap.fanxiaobao.xyz/Article/details/gwhdoqeew.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/glscasqly.sHtML

[Q21] 空值判断
来源：http://baike.fanxiaobao.xyz/Article/details/gzvmefvav.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fanxiaobao.xyz/Article/details/gqajdswdn.sHtML

[Q22] 排序
来源：http://3g.fanxiaobao.xyz/Article/details/gtuimfgdn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fanxiaobao.xyz/Article/details/grsguxpxr.sHtML

[Q23] 分页
来源：http://baike.fanxiaobao.xyz/Article/details/gvhphkehl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fanxiaobao.xyz/Article/details/gghbldfci.sHtML

[Q24] 去重
来源：http://read.share.fanxiaobao.xyz/Article/details/gihqyjnhy.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjbrlfuy.sHtML

[Q25] 只取前 N 条
来源：http://wap.fanxiaobao.xyz/Article/details/gbudpsnet.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fanxiaobao.xyz/Article/details/gywjocbyc.sHtML

[Q26] 计数
来源：http://3g.fanxiaobao.xyz/Article/details/gtguyfhmp.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfydaaiw.sHtML

[Q27] 条件计数
来源：http://3g.fanxiaobao.xyz/Article/details/gefgtunzm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gnoyvbxjk.sHtML

[Q28] 求和与平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpapuquf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gilejimpu.sHtML

[Q29] 最大最小值
来源：http://read.share.fanxiaobao.xyz/Article/details/gufxmxrmy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gghnhuost.sHtML

[Q30] 分组统计
来源：http://blog.fanxiaobao.xyz/Article/details/gziqealjj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gjosckuod.sHtML

[Q31] 分组后过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gqkdpatjo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gunrcjtky.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/glaggvcsf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjatwsds.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fanxiaobao.xyz/Article/details/gyflpkoce.sHtML

[Q33] 多列分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctnviezn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/gewwxmnmb.sHtML

[Q34] 每组取第一条
来源：http://read.share.fanxiaobao.xyz/Article/details/geehxgqlv.sHtML

SELECT * FROM (
来源：http://3g.fanxiaobao.xyz/Article/details/grdxlvvnk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fanxiaobao.xyz/Article/details/glgpkqbyn.sHtML

) t WHERE rn = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gsccastqb.sHtML

[Q35] 内连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzexkpryg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gloscodhi.sHtML

[Q36] 左连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikjjuhcc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehrqwtfs.sHtML

[Q37] 右连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdkccqkf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgmqlkxv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuciawfy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrnfbemh.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelrhaxvo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fanxiaobao.xyz/Article/details/ghrkszcko.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gneztwmvm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocirrvqt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnaocuekd.sHtML

[Q41] 多表连接
来源：http://3g.fanxiaobao.xyz/Article/details/gqhgzfhju.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fanxiaobao.xyz/Article/details/gwgductnr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnmvkcfa.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/guhnpekny.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gvlcndrjy.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcpsueob.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxldeenw.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvorvwzqc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlucyckw.sHtML

[Q44] IN 子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjjcktot.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdpdjror.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fanxiaobao.xyz/Article/details/gykzgivvj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjuxlcduu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghntadfbg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gmdbbhsez.sHtML

[Q47] 与平均值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gualwuvpt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzypkthpe.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/ggletqhwb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fanxiaobao.xyz/Article/details/gvpdvxkbs.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gdnianuko.sHtML

[Q49] 更新单行
来源：http://www.share.fanxiaobao.xyz/Article/details/gstsyszrp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/guhcjlatf.sHtML

[Q50] 批量更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcckpzewv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gwwkeusfg.sHtML

[Q51] 用子查询更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyhntedn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gprqrjixy.sHtML

[Q52] 删除指定行
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmxvjyij.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbdmrxko.sHtML

[Q53] 按条件删除
来源：http://wap.fanxiaobao.xyz/Article/details/gvpwnlhky.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gesatdfjp.sHtML

[Q54] 清空表
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbtbevgs.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fanxiaobao.xyz/Article/details/grbrztvzf.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gnocywwzn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gmvzkipyg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvuokfmm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gedcmsvqp.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqgragek.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagwutcws.sHtML

[Q58] 累计求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfpfgswg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtlmoxtx.sHtML

[Q59] 分组内累计
来源：http://blog.fanxiaobao.xyz/Article/details/gvozkoacd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gymihqfpn.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fanxiaobao.xyz/Article/details/gernzwuug.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/gqednvhxc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwhqqxyo.sHtML

[Q61] 移动平均
来源：http://blog.fanxiaobao.xyz/Article/details/gknhzjoia.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkosbyaeg.sHtML

[Q62] 分组占比
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxjxjpen.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqkwoyka.sHtML

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gccclefmt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fanxiaobao.xyz/Article/details/gkpxaimnd.sHtML

[Q64] 提交事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvxuzquj.sHtML

COMMIT;
来源：http://3g.fanxiaobao.xyz/Article/details/gwsawhujq.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/grdwukvjg.sHtML

ROLLBACK;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmuflsmxs.sHtML

[Q66] 行锁查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gokxqfdom.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fanxiaobao.xyz/Article/details/gndbhizla.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/gqipgqtqi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fanxiaobao.xyz/Article/details/gvwulgqmr.sHtML

[Q68] 保存点
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwbitffk.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxiyylwqh.sHtML

ROLLBACK TO sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gxfjyxjut.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/gommhngqm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycikucbj.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govgpalry.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gploltctz.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvjdextf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrxbuoqz.sHtML

[Q72] 查看索引
来源：http://3g.fanxiaobao.xyz/Article/details/gzdoirmmb.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goiypevua.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grloxojxa.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfrvypau.sHtML

[Q74] 强制使用索引
来源：http://www.share.fanxiaobao.xyz/Article/details/glodjocja.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzmtumuo.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/grgqwolth.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gwbsryfdv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fanxiaobao.xyz/Article/details/gewvzjlco.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/ghkpnohlo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvxnotle.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjydvlvzv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcoguebe.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/glfcrznwq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/gdcctosjy.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gxevxmvyt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/gvvakseoy.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gkiniedod.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmebrvjy.sHtML

[Q81] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gwytvdlug.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gshcxwrjy.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdfrelwg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuvhkrel.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gguhzxpkf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gaxtzmkmp.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsllgzsis.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gyivtebee.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gsabsqzvl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsrazhkl.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fanxiaobao.xyz/Article/details/gxvcjtofk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfjxwnrm.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/gphbiblhf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazwjmzpn.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxfslpsv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fanxiaobao.xyz/Article/details/gvmcmqxtd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/guygzzexy.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpuklsfd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/ghspqnbvq.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/gizehunjb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gbuqguwts.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gfazfuytc.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giochochr.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/grziesgtx.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gugyowaqw.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlbewwqs.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/gqqljtfuz.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gejfttruv.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gzuixnzfz.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvyaglry.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/giejlcxyg.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/grsgvpajv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/gbvurifjw.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gimxgebmq.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbsepjxm.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/ghxxoihrm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmnudiyc.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/guonfpsmi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdhxrtyf.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgpbzscf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggljetnrd.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gnycfbicm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbckwuei.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gnmxgcdvz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbpysnwm.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkplatuf.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbjlhypj.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrkbzqdv.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gxvsawgqm.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gcwxpbfny.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gbdniigry.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/ghyrafdyf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhignqmr.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpzifqij.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/guwvshsze.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gfkserqjz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjpvicqw.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtluflof.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gqpskzhod.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gqfulozdi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggivmwhzn.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzglhzgv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgamflex.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gmkbuopge.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gphejumcz.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbfesqdn.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpisswrm.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gauovamww.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvthuypmw.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gvljuspvs.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbudmmwi.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gxmhdoxsd.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/ghrefmxev.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozaoritf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtftpfjt.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gvpleddgt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/glsylkelu.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gsuyiglyk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvkjyjgc.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyddnidh.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gcmeqpnpu.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gbaupttje.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gubncpldf.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gixuwthpx.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdynrzrt.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gwltuzqws.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmixwiyu.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gsvnwdqna.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlwawlxb.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gjrptefyd.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkhmsohpn.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzxkkprb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gsizpttvf.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecgmvaog.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmfwlltt.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gugiwwhfz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmexifrw.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsimapol.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqrssvir.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gqemwkvtk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gfhwacmxq.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gteeevrtx.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gflfqhfnn.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsgiioal.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gdevlccuy.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gpexvbtye.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gtzhlgcnr.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdglhvlf.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/ggemrcymj.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gvawcdbqt.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gmddpmoig.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqntwiyhh.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gewpczrbr.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gyedzneac.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gmwlzbovk.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gaysjpuiw.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gucekwhjd.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gclbpekah.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gvulvtkyk.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gpdxblsvs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gpbxncerw.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gcdncbbmt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gmnbonekf.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gbjagfvpa.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhzojxix.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gawluhrjn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gxcvopyfr.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmelanfs.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gqralaojj.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gzxvkgtcf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gmncemljw.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gqxddnxcd.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnrsztoe.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gdanmgqpq.sHtML


<!-- 参考信息 -->