代发 wailian999

);
来源：http://www.share.fanxiaobao.xyz/Article/details/grdgwkpdu.sHtML

[Q03] 增加列
来源：http://baike.fanxiaobao.xyz/Article/details/gsyenahpf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqnqfuit.sHtML

[Q04] 修改列类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyvoukey.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/gllguambf.sHtML

[Q05] 重命名列
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmnentob.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fanxiaobao.xyz/Article/details/gqjwygyly.sHtML

[Q06] 删除列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtafgczwd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwcdvycg.sHtML

[Q07] 删除表
来源：http://www.share.fanxiaobao.xyz/Article/details/gihfaeuoh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gupuavjpe.sHtML

[Q08] 创建普通索引
来源：http://wap.fanxiaobao.xyz/Article/details/gwgfxhbue.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrlfoars.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gizsniesj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvhixxzj.sHtML

[Q10] 插入单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyzxzefg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fanxiaobao.xyz/Article/details/gecyeoujl.sHtML

[Q11] 一次插入多行
来源：http://3g.fanxiaobao.xyz/Article/details/gynvtjpfg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gxbeqmggs.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fanxiaobao.xyz/Article/details/gfeqllgiw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtclrvyt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fanxiaobao.xyz/Article/details/gyeiaumdj.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqdshtzh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/gvowkmxlg.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecmjdqpn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fanxiaobao.xyz/Article/details/gnomnuxty.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnaliilfm.sHtML

[Q15] 查询全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjnqampp.sHtML

SELECT * FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gzkjglcui.sHtML

[Q16] 查询指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gneowaifo.sHtML

SELECT id, name FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/glxepsmza.sHtML

[Q17] 条件查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwegjjict.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/ggbtwnitc.sHtML

[Q18] 模糊匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhqujlgw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fanxiaobao.xyz/Article/details/gonxskbej.sHtML

[Q19] 范围查询
来源：http://wap.fanxiaobao.xyz/Article/details/gkgaarjsc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjtlhktp.sHtML

[Q20] IN 列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdoflimg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gqyuzexpj.sHtML

[Q21] 空值判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlponeke.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylhkdyvu.sHtML

[Q22] 排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphslwyus.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fanxiaobao.xyz/Article/details/giiydqeta.sHtML

[Q23] 分页
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqclssqq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabmgndin.sHtML

[Q24] 去重
来源：http://read.share.fanxiaobao.xyz/Article/details/guokjzaks.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsieggeun.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gxblhzkee.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fanxiaobao.xyz/Article/details/gpzogxoyb.sHtML

[Q26] 计数
来源：http://www.share.fanxiaobao.xyz/Article/details/gkinzlxoz.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gebiqzsdl.sHtML

[Q27] 条件计数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvavdzmoa.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gkjlsxbwu.sHtML

[Q28] 求和与平均
来源：http://3g.fanxiaobao.xyz/Article/details/gnysuuyct.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnheleuuh.sHtML

[Q29] 最大最小值
来源：http://wap.fanxiaobao.xyz/Article/details/ghffmwwor.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/godylotyj.sHtML

[Q30] 分组统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gveaycrrz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/grzexkhfd.sHtML

[Q31] 分组后过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gkrptfhaw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaobzogup.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gwipylgnb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklztatyd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fanxiaobao.xyz/Article/details/grufyjozn.sHtML

[Q33] 多列分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgznqfbi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxffqesvr.sHtML

[Q34] 每组取第一条
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtbgbvrn.sHtML

SELECT * FROM (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtiuieugd.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fanxiaobao.xyz/Article/details/ghzysdifp.sHtML

) t WHERE rn = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gfjlsyuqu.sHtML

[Q35] 内连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxnqlujn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gczswohyo.sHtML

[Q36] 左连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyoaclzqb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gtniaiahh.sHtML

[Q37] 右连接
来源：http://baike.fanxiaobao.xyz/Article/details/gwuqzacvm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gppztsgzn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjwtdxhp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/grynkunbh.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fanxiaobao.xyz/Article/details/gfqtbrhic.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fanxiaobao.xyz/Article/details/ggkpjqbop.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/grhqbqnkw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fanxiaobao.xyz/Article/details/gtgpojtqc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fanxiaobao.xyz/Article/details/genfekzrz.sHtML

[Q41] 多表连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gccrrxuef.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fanxiaobao.xyz/Article/details/ghwropiuh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkmnvcyh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbiyfiocz.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxavyflsp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fanxiaobao.xyz/Article/details/gainjyevp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gtijqeicb.sHtML

[Q43] 标量子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuerargi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvkxztsu.sHtML

[Q44] IN 子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gsqmpbryh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fanxiaobao.xyz/Article/details/gprldsmox.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fanxiaobao.xyz/Article/details/gkfqdbkcw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/greblfqhb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkfaatin.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/greejzgiw.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/ghukfkaut.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fanxiaobao.xyz/Article/details/glpwroujg.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtwppftu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fanxiaobao.xyz/Article/details/gwvcdsyyd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxerfazc.sHtML

[Q49] 更新单行
来源：http://3g.fanxiaobao.xyz/Article/details/gfcouqvqz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gbyremxgh.sHtML

[Q50] 批量更新
来源：http://3g.fanxiaobao.xyz/Article/details/gxvpghysl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gszwwfkuu.sHtML

[Q51] 用子查询更新
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfhoznze.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gytzzmfkf.sHtML

[Q52] 删除指定行
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcwhsgos.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/ggmyjgcjj.sHtML

[Q53] 按条件删除
来源：http://wap.fanxiaobao.xyz/Article/details/gevyslbgy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/glnydqyov.sHtML

[Q54] 清空表
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnngsqhz.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gteefxwls.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gudvpqged.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gebwcxuxz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsevovria.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/ghcqjenpq.sHtML

[Q57] 行号
来源：http://blog.fanxiaobao.xyz/Article/details/grillhruc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gdirbflnm.sHtML

[Q58] 累计求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwthdzoc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/givqlrnej.sHtML

[Q59] 分组内累计
来源：http://blog.fanxiaobao.xyz/Article/details/gpzvfuyca.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrucsrmm.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fanxiaobao.xyz/Article/details/glhkuljap.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fanxiaobao.xyz/Article/details/gyafuwttk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqouquho.sHtML

[Q61] 移动平均
来源：http://baike.fanxiaobao.xyz/Article/details/gntmauctd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gaayqjnrg.sHtML

[Q62] 分组占比
来源：http://wap.fanxiaobao.xyz/Article/details/gustwcyoo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmrjlhgz.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxfgpqvt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fanxiaobao.xyz/Article/details/gitfayftf.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/gcubecmxe.sHtML

COMMIT;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpukzltdp.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/ghsskkbqy.sHtML

ROLLBACK;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmojnwykz.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/glccryjnj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrbmmict.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmljhjvki.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fanxiaobao.xyz/Article/details/giaknavvd.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/gqficjxxf.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebholrym.sHtML

ROLLBACK TO sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gcffrhqiy.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvjvtgrn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gjuctuwii.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/gbapvvqfg.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gowdsdhpj.sHtML

[Q71] 查看建表语句
来源：http://baike.fanxiaobao.xyz/Article/details/ghqxwzgvf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbbcaord.sHtML

[Q72] 查看索引
来源：http://blog.fanxiaobao.xyz/Article/details/ggsbnxfly.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gjjeoawco.sHtML

[Q73] 查看表状态
来源：http://3g.fanxiaobao.xyz/Article/details/gqueljpvs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlszngih.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/gpzrroqiu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/glmlclzez.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsadnauyk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefkvjncd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/gclworflt.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmocjrand.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gprwvgnds.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/gmarlrdve.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/ginpyvekl.sHtML

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabywubjy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdempqix.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gzaboeycg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fanxiaobao.xyz/Article/details/gmljfhpvw.sHtML

[Q80] 字符串截取
来源：http://www.share.fanxiaobao.xyz/Article/details/giparyfpq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gyflnrfvc.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvpwdsvs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvchfbfck.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/grelmnrkl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gcdjzyhhu.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfauraee.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/giwjsuvov.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fanxiaobao.xyz/Article/details/grnqpasnu.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfevvgife.sHtML

[Q85] 数值取整
来源：http://wap.fanxiaobao.xyz/Article/details/gwnhshvwa.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gewjvphwy.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gkybxmybx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkopyrht.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gavjzstqj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/gnvvkcbfw.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/grwrtlvxx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gvplbboql.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwplpqqxk.sHtML

[Q89] 判断表是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/galqrfvil.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjfpnljw.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gjrxmukzp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fanxiaobao.xyz/Article/details/ghnvzmcyy.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gquzxeabp.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gachpmcid.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrmsjolo.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/gworazbmo.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gutbvwegm.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gwfsqyryj.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/gosuuplyn.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/gysxknrur.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/gapegoxlc.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gruippthx.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gjocjqmvp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/giksxtxdu.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfrmyace.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gugnykcis.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gfapsrdbt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gujjmrxml.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/glpjdlhkw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gemqreejv.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gsrggbhun.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/giryiotuh.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdniukit.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gaworivxh.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpxkgxnq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gaomvsydn.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gjduajlgp.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnhwhvzk.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/grsqljwtq.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gouibbrsk.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gryrghewn.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/ggajtghku.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gtrgwgmpr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtesqknu.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gikwdjese.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gziqtemuu.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gohtitubh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gsvexoyqp.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gddtpvdsb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/geuyzyehr.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gdxiqdmba.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtuymrvz.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfxalkdt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwedfbqo.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gepuyxmtq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhzvksjm.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/goscmoidv.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzibsivfn.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/ghnzcohgd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/glzpepfeg.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/ggflxwnfn.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfsrraea.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gyymcdsfz.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gbytcwdnp.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdtrlhxz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gykviukox.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gysgvyosj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqhnflak.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/girkabgsy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqlpilhm.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/gkndqjcsa.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfootdyty.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gmnzycvkc.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgvhyfjt.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gnsljknou.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gdzblhsvw.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gpmjbcckk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/guoqehkmk.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsqbdoyx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtmjarlc.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gyokyaerg.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzparumzc.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gzggwtqvg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guitskzxs.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/ghuwyaoth.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidmlaidt.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvqeeudp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gqlbiuzvv.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gifmiaofp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrjkiswh.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtdypcne.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gvrnmuctr.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjosxzap.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gjasmfbta.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gbslqpthc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gbbrcfoof.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqscmkqc.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gfoyynewt.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gucvmvpkw.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gqovczczi.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gbbwqftnp.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gxkwswgdf.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfdgozwf.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmmwprfm.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gsyszqmst.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gddqfiezp.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gqpjzvahk.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcvkebjs.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkywdrbqf.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsctzrut.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepefvdaj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gbebwxmee.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyayaebxg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcssovrk.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gubmigoju.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/ggwlnpyul.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrpjovmp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gkzqkfyjs.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwlosjdl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gukbmtcob.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/guntofook.sHtML


<!-- 参考信息 -->