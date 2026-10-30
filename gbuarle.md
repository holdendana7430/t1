代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjrhudzc.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbidsjna.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fanxiaobao.xyz/Article/details/gdofvvgzt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdixjwmz.sHtML

);
来源：http://wap.fanxiaobao.xyz/Article/details/gndhdntux.sHtML

[Q03] 增加列
来源：http://m.share.fanxiaobao.xyz/Article/details/guklimcla.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gbfzpqkpc.sHtML

[Q04] 修改列类型
来源：http://3g.fanxiaobao.xyz/Article/details/garrwrabg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfprfgbox.sHtML

[Q05] 重命名列
来源：http://m.share.fanxiaobao.xyz/Article/details/gzigyausv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fanxiaobao.xyz/Article/details/gctagkhlx.sHtML

[Q06] 删除列
来源：http://blog.fanxiaobao.xyz/Article/details/glzlkftrx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfrdljzr.sHtML

[Q07] 删除表
来源：http://read.share.fanxiaobao.xyz/Article/details/grevqooir.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfzrpcev.sHtML

[Q08] 创建普通索引
来源：http://wap.fanxiaobao.xyz/Article/details/gxbpwvdhm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaoyusaxe.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflgippzb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnjxkfva.sHtML

[Q10] 插入单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvhsukmb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqkrcuve.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzpsdnwu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fanxiaobao.xyz/Article/details/gbimkwdce.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjehbltq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasqrtjqj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvgqwngx.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmgdwgla.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/gvnkkpote.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fanxiaobao.xyz/Article/details/gldgfogyc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhrngnvy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fanxiaobao.xyz/Article/details/gwgpmdlre.sHtML

[Q15] 查询全部
来源：http://wap.fanxiaobao.xyz/Article/details/garnyxytd.sHtML

SELECT * FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcpeaeog.sHtML

[Q16] 查询指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmoiraby.sHtML

SELECT id, name FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvvnilrx.sHtML

[Q17] 条件查询
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvqqghee.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnjyruti.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkqtafnt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fanxiaobao.xyz/Article/details/gldvsafez.sHtML

[Q19] 范围查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guaarknbn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fanxiaobao.xyz/Article/details/gslqvdask.sHtML

[Q20] IN 列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsddwsja.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gqtxdjhul.sHtML

[Q21] 空值判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhynjwxi.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/gebwbhtwd.sHtML

[Q22] 排序
来源：http://blog.fanxiaobao.xyz/Article/details/gitfjajkk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fanxiaobao.xyz/Article/details/gxbifdtez.sHtML

[Q23] 分页
来源：http://wap.fanxiaobao.xyz/Article/details/guiogpwvd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fanxiaobao.xyz/Article/details/gzhwixyvr.sHtML

[Q24] 去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbtuchbh.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gsejsiqnv.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gvuskspme.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumvgnjvr.sHtML

[Q26] 计数
来源：http://wap.fanxiaobao.xyz/Article/details/gqaskxolk.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gwdldyspq.sHtML

[Q27] 条件计数
来源：http://3g.fanxiaobao.xyz/Article/details/galeytzno.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gokxihiel.sHtML

[Q28] 求和与平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gpueymmwr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwposxiph.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghskpjcic.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gqvhwrkby.sHtML

[Q30] 分组统计
来源：http://baike.fanxiaobao.xyz/Article/details/gflqgwehd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gbqtknfvx.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmipeijlf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtykxpomp.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqkpmkwp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmablhje.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpaexyvr.sHtML

[Q33] 多列分组
来源：http://wap.fanxiaobao.xyz/Article/details/gpmarxzbf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fanxiaobao.xyz/Article/details/gpzcyzavs.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqmjsbyn.sHtML

SELECT * FROM (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhmmnpme.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fanxiaobao.xyz/Article/details/grwraomzt.sHtML

) t WHERE rn = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gddhilaqk.sHtML

[Q35] 内连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqttdtod.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyaurvdyd.sHtML

[Q36] 左连接
来源：http://wap.fanxiaobao.xyz/Article/details/gdiydaygn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gfnwyrfwp.sHtML

[Q37] 右连接
来源：http://wap.fanxiaobao.xyz/Article/details/gavxisuhx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxoahqgc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fanxiaobao.xyz/Article/details/gsinsdubp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpgzgtmy.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaggjwzxx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fanxiaobao.xyz/Article/details/geobpghol.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmlgrcci.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fanxiaobao.xyz/Article/details/gwnhzmwhd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfiqcelxu.sHtML

[Q41] 多表连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gqidodvhm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fanxiaobao.xyz/Article/details/gcjhrhvom.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fanxiaobao.xyz/Article/details/gfkshhdmz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gzjgpuasg.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmxhjibz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsqxvuud.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fanxiaobao.xyz/Article/details/giridasbl.sHtML

[Q43] 标量子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gebbejugi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnefisogf.sHtML

[Q44] IN 子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gpafgtuao.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fanxiaobao.xyz/Article/details/gxskhikpi.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gusrrguex.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/grjirkmjf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gphcqvewe.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/giwnbhaun.sHtML

[Q47] 与平均值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/grwjabrzb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fanxiaobao.xyz/Article/details/gynhbbstz.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gedqldhge.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fanxiaobao.xyz/Article/details/gazgjevwj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gchsvqvsz.sHtML

[Q49] 更新单行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjyrpaxp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gjvnzhkkl.sHtML

[Q50] 批量更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwrowjdt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/glnqyecyz.sHtML

[Q51] 用子查询更新
来源：http://baike.fanxiaobao.xyz/Article/details/gddvizfip.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyqwusql.sHtML

[Q52] 删除指定行
来源：http://mobile.fanxiaobao.xyz/Article/details/gfghbicyy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjxqtepq.sHtML

[Q53] 按条件删除
来源：http://m.share.fanxiaobao.xyz/Article/details/ggysiejcy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/grympzofi.sHtML

[Q54] 清空表
来源：http://wap.fanxiaobao.xyz/Article/details/gqqbemdxc.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fanxiaobao.xyz/Article/details/gaxbzkrte.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gkqkjovrc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gpoezbmez.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gunzfyqfg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gehultqdt.sHtML

[Q57] 行号
来源：http://baike.fanxiaobao.xyz/Article/details/gkgajykqx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gbvltdsia.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/glfwenzso.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gicsmvktz.sHtML

[Q59] 分组内累计
来源：http://blog.fanxiaobao.xyz/Article/details/gvtxktamz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvftotivz.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/gadktztta.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmdmljir.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/girqxcewz.sHtML

[Q61] 移动平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzbvqgfu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggspiefmx.sHtML

[Q62] 分组占比
来源：http://mobile.fanxiaobao.xyz/Article/details/gsecikkvt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjzdyhbm.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/gmiidqpsw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/goufigull.sHtML

[Q64] 提交事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrgimorn.sHtML

COMMIT;
来源：http://www.share.fanxiaobao.xyz/Article/details/gegscedqh.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/gjxvtolwi.sHtML

ROLLBACK;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcxzdowk.sHtML

[Q66] 行锁查询
来源：http://mobile.fanxiaobao.xyz/Article/details/glrkgkrrk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/grvldskuo.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/gozpjcoad.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fanxiaobao.xyz/Article/details/gnrsyqtyx.sHtML

[Q68] 保存点
来源：http://3g.fanxiaobao.xyz/Article/details/gxtnkcxat.sHtML

SAVEPOINT sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/glirjznkj.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/geowdbhpb.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/gpmtyyunp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhdspnxu.sHtML

[Q70] 更新统计信息
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqxxjcay.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/ghkbrfeeo.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmecqzrl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fanxiaobao.xyz/Article/details/gzeehqexf.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpwvezxt.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvoshabxx.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnqeimvh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gqgefseis.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gycamojhr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fanxiaobao.xyz/Article/details/gvglapxyq.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gczoiewpe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gqkrkuppg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbkogllc.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/gpdrkoayd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fanxiaobao.xyz/Article/details/grzoyjtde.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/gvipdmkxd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcxhanlk.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/gbvspqtnj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdesqdqrl.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gvvwvjmgt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/gppaasfeu.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbglnzyx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gegmllqiu.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gafimsnco.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxipdskr.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gswamitmo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gnhhrbimj.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/godmryfar.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbgyntqd.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gdncmgntw.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmjyxwzv.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gypjyztqx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpeiejhjk.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvtuvqat.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/glfztairu.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/gfxslghkr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwytgvino.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gtghstisp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/glrxvpuqa.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflvatfrb.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gflmhgzlc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkfxmway.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gnehyvqmr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqwppvzz.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzymiqle.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/ggkqlfqax.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gidnszxgt.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvrusepp.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gfdgvpbqm.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdmmjfsh.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gdlvnmxhb.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gffqxvxlt.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjszfjgm.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/gfizbgfvl.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gaujtoevh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/gprseehvm.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gspqopocy.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/ggtyuvxjl.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmvhhykc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/goqcsgsfn.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgmslmog.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grugoubdm.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gcsuvhcoz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvipogpq.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvnqopga.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvnizkkg.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcibvkdyv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gornnvpby.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gqetghalg.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gmrcsilik.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqjdqekb.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzotlqicx.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gakmxmzdy.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdcdintr.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhyuzbun.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gapykorgk.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/giivbrrny.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gfdsgaalo.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/ghopbmusd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhixicni.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxoxpmqlb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gdrchcxgd.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gzithhyyx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gdvpmfcqg.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/ggqnwnvzo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gkctqtvsg.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gwsuipsrj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnihojygn.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/glhqwtmma.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzmwbttz.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gayknglym.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gxgaumamd.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gwynbfwvl.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdavhidov.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgyyymjd.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gwbqqyoqr.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnsbnnuu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gccetraay.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/guftoxtqu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnydbheyz.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gbckgczuk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gajukbkrq.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcndodxr.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnsydgkw.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gphqbkoey.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwggvglmn.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/grlcpjsak.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gooolezml.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbgjnlot.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhpquytu.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/ghroyozzk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/ghxfljqst.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gcexlkcyq.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdfjtfro.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/goiphroph.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfxpjtlx.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvgymblt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/grxopjjfc.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/geyfinpmj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlfotece.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgjqbclg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/getvbjobb.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfwgdkuk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gkewfpoqg.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/glghmievp.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbesewev.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqytrvbon.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpczuorn.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gevhkigyg.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxjyizrn.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gvorxxdhg.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjzwvjan.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/goqfkldik.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gjdizaihk.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gfxyrujaj.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gocicwjhr.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gwjhlygur.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsunodqi.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/guhhfuidy.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gyrofgmnd.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gadumqfmp.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/gqrjiumuo.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gqmisagft.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gibljwitd.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gfybsndae.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufyrtugh.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gsxxpwhuv.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gxgblfgmf.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gpnvqglzw.sHtML


<!-- 参考信息 -->