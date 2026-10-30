代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.zdbjq.cn/Article/details/ghylujaya.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/gbkqkgteg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/grveujvys.sHtML

[Q06] 删除列
来源：http://blog.zdbjq.cn/Article/details/gdnjqbthv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fehbvm.com/Article/details/guvlsuhjr.sHtML

[Q07] 删除表
来源：http://mobile.fehbvm.com/Article/details/gplbzlevd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fehbvm.com/Article/details/gelyyrhqi.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/guzumhddk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gatlohlmq.sHtML

[Q09] 创建唯一索引
来源：http://3g.hesvh.cn/Article/details/ggvzxavno.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gcwutjcfi.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/gdduohhen.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.hesvh.cn/Article/details/gpqyqmmql.sHtML

[Q11] 一次插入多行
来源：http://mobile.zdbjq.cn/Article/details/gxiepjcse.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.hesvh.cn/Article/details/garyfqatx.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.zdbjq.cn/Article/details/goijgehwq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fehbvm.com/Article/details/goxndcrgh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fehbvm.com/Article/details/gwmztqcks.sHtML

[Q13] 忽略重复插入
来源：http://m.share.hesvh.cn/Article/details/gencbdrbm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fehbvm.com/Article/details/gmhogioxd.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fehbvm.com/Article/details/gafyjnuxz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/gifaimvmk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/gmgofelix.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/gxcnezwsw.sHtML

SELECT * FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/grrddcyaw.sHtML

[Q16] 查询指定列
来源：http://www.share.fehbvm.com/Article/details/gjtnjqzgg.sHtML

SELECT id, name FROM users;
来源：http://3g.fehbvm.com/Article/details/ginzfryhe.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/gsbicqwiw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/gfdqfmsln.sHtML

[Q18] 模糊匹配
来源：http://m.share.hesvh.cn/Article/details/glmzkqhli.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fehbvm.com/Article/details/ghypennlc.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gtrqzswjq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fehbvm.com/Article/details/gswigrwig.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/gvedmpjkx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.hesvh.cn/Article/details/gzxhfxmjt.sHtML

[Q21] 空值判断
来源：http://www.blog.hesvh.cn/Article/details/gwgeynvav.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gzfiqfrei.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/glkhtnkjn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/gzjrcpeoq.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/gnpuuivtb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/gmdjnzwic.sHtML

[Q24] 去重
来源：http://wap.fehbvm.com/Article/details/gzrqtfqvb.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.zdbjq.cn/Article/details/gaiwqcptd.sHtML

[Q25] 只取前 N 条
来源：http://3g.hesvh.cn/Article/details/glzkwnpve.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.zdbjq.cn/Article/details/gmnssxbjc.sHtML

[Q26] 计数
来源：http://www.share.hesvh.cn/Article/details/gayqersqt.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gabyikvse.sHtML

[Q27] 条件计数
来源：http://3g.hesvh.cn/Article/details/gkhjpkqbj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/gsrrjcfqk.sHtML

[Q28] 求和与平均
来源：http://mobile.zdbjq.cn/Article/details/gtoqnqfpw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gbryoxkfj.sHtML

[Q29] 最大最小值
来源：http://3g.zdbjq.cn/Article/details/gwevrfxjc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gvihitpeh.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/gjmsnhvcx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gnwnmdeuv.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/ghgaeoddt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/gisrbkjrh.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/ghjdrkfdf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gwmuwvhfu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.hesvh.cn/Article/details/grpgogsei.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/gkzyqmufx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/gtafklkej.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/gvhantwzb.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/gkttyjzkm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.hesvh.cn/Article/details/gcfqbitut.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/grbouococ.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/grrzxwfra.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/glohvuttl.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/gwrvxollv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/grxqbcxgw.sHtML

[Q37] 右连接
来源：http://wap.zdbjq.cn/Article/details/gmjinzqbw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/glsthpecf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gugaborgo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gedpxzvcb.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.hesvh.cn/Article/details/gijkctgib.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.hesvh.cn/Article/details/gnzkhhzvi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.hesvh.cn/Article/details/gkxqpahcl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gdldymaav.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/gvixrtote.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/gucaenaam.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/gscbanyak.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/gqomurmdk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.zdbjq.cn/Article/details/ghkzxjcys.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/gbrbuytbr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.zdbjq.cn/Article/details/gdwyilfyn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gftwedjex.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gbrcpldot.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/gjxyyplfm.sHtML

[Q44] IN 子查询
来源：http://www.share.zdbjq.cn/Article/details/gxqlylvir.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/gdmhzqnvz.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/gmzqmijoy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gpvgtifku.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.zdbjq.cn/Article/details/grilimjrf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gkmrvnknd.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/gmrhculvy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/ghuzjzciq.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/gpjuhsxlr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.hesvh.cn/Article/details/gavuwpfri.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gfrtyhyws.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gxqrxqpqs.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gqcamtkic.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/giygmrtig.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.zdbjq.cn/Article/details/gpweyegan.sHtML

[Q51] 用子查询更新
来源：http://www.share.fehbvm.com/Article/details/gxdvzhyjz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gfmfnvnwf.sHtML

[Q52] 删除指定行
来源：http://read.share.zdbjq.cn/Article/details/gikvillts.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gzuzkevvh.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/gvgadmmdk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fehbvm.com/Article/details/grmzstghi.sHtML

[Q54] 清空表
来源：http://baike.hesvh.cn/Article/details/gfjbshtmc.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/gorotfgyc.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fehbvm.com/Article/details/gpuevthbv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gtqpkernp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.zdbjq.cn/Article/details/gmafgdyby.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/gjzgnbrjp.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/gvvozfahb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fehbvm.com/Article/details/gcswumfkp.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/gllhivmko.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/gcdxgaagq.sHtML

[Q59] 分组内累计
来源：http://baike.zdbjq.cn/Article/details/goklyknmr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/goyxhbipa.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/gozgxzque.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/guiqsfpbh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gbupbhydq.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/gshjtuugk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gopgcjlbo.sHtML

[Q62] 分组占比
来源：http://blog.hesvh.cn/Article/details/gkzpkwbkg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gmdswgdod.sHtML

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/gdwqvxvdq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/gbmryicxp.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/gngktisiu.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gqgehncte.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/gbytubggm.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/gksvdorgg.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gmkgcdmpf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/gztuqzage.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fehbvm.com/Article/details/gvjggqeei.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/gwouglnok.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/gcsrxvakw.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/gwsurdoen.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gmbvmssqc.sHtML

[Q69] 查看执行计划
来源：http://blog.hesvh.cn/Article/details/gpyqriqsj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/gkudlkdlc.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/gjsnfyvck.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/gtjhuvexs.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/gqqzpeegs.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/gkdgetxaz.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/gopiphlnk.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/gqtkmxetf.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/ghscutaey.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/gdjbyrolm.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/grzykloum.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/gjgbsgtba.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gokxoincf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gwwedopzj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/gdpfxcgrc.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gqzjleylm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.zdbjq.cn/Article/details/gmzzmqtni.sHtML

[Q77] 时间加减
来源：http://m.share.zdbjq.cn/Article/details/gthgvgsqm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/gfgrjgbqe.sHtML

[Q78] 当前时间
来源：http://m.share.fehbvm.com/Article/details/ggxqhfsae.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/gsgsnoxyq.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gfjeebnxk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/grapzdbam.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/gykkyjmoq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gkankeqdk.sHtML

[Q81] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gkulohmmo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fehbvm.com/Article/details/gnidquaou.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/grjouqldh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gteclwgye.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gvlpvpnve.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gwlxrymby.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gijlbrqvs.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gvmeqgvrt.sHtML

[Q85] 数值取整
来源：http://www.share.zdbjq.cn/Article/details/gtjmrcmmr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/gsadedibm.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gjfzhahho.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gxdekfbij.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/gthqcevyh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/ghejrjujn.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fehbvm.com/Article/details/gsmtrrpwo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gpchibefv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.zdbjq.cn/Article/details/gxzeqjciv.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gdynlnbho.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.hesvh.cn/Article/details/gzfljtvia.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/ggabctihy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/gfobvcvze.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/genqtbvan.sHtML

R. Bash 专题
来源：http://baike.hesvh.cn/Article/details/gidiiwnnr.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvvgvlpfl.sHtML

[R01] shebang 与严格模式
来源：http://baike.zdbjq.cn/Article/details/gvzoynmaf.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/gxbnknemn.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/gyktnxxxi.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/gyvaxfcok.sHtML

name="Tom"; echo "$name"
来源：http://baike.fehbvm.com/Article/details/gtczsrgvp.sHtML

[R03] 只读变量
来源：http://read.share.fehbvm.com/Article/details/ghclbrpva.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gflpspjys.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/gsajltazp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/gxgdotyih.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/gchxtiilu.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gumyqkcuv.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gwjwcgzdi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/geihtxmlv.sHtML

[R07] if 判断文件
来源：http://blog.hesvh.cn/Article/details/gejcbdndd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fehbvm.com/Article/details/gqvriisim.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/geyngqpwu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.hesvh.cn/Article/details/gtrhhzqnz.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gqnrqmbsk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gdoqecjgr.sHtML

[R10] 正则匹配
来源：http://m.share.fehbvm.com/Article/details/gudznhdkd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/gerdiojpk.sHtML

[R11] case 多分支
来源：http://baike.zdbjq.cn/Article/details/gqbkpkpun.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gmydfuecg.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/ghlvhuuyd.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/ggsnoksvb.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gomuklipd.sHtML

esac
来源：http://wap.fehbvm.com/Article/details/grnpbcgyw.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gtsptbglx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/gsvsmkjpz.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gbpmdivvm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gbaojdhjf.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/gsedhjudx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/ghvzccnjl.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gqnarfpks.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/gadygowih.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/gyttbtykf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gxscjkugs.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gubyrlpgr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/gjcdwssiq.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gpltmpgqh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gvvvrplxp.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/guystlxyc.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gizlrkhlx.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/gffkecriy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fehbvm.com/Article/details/gvzdkkjli.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/gfaspfbjk.sHtML

echo "${#s}"
来源：http://www.blog.zdbjq.cn/Article/details/glsnazqoh.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gjplvaqvh.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/gttkxutzf.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gqepgzyxv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.zdbjq.cn/Article/details/gnvfbshgy.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gwytktdji.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/gjlkgymcd.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/guxmxnkak.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/gcxeshifg.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/ghjqeswqe.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/ghnbmumwk.sHtML

[R27] 算术展开
来源：http://www.m.share.fehbvm.com/Article/details/gjrbprtaf.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/gmrzbdlci.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gvsjfexop.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/glegerwyh.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/ghkgpliee.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/gjhncirdk.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/grdeqaplx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.hesvh.cn/Article/details/gefnyyocg.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/gsapxwocy.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/gfkzppvte.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/ghjtufgxf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/grxzhoqcm.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.hesvh.cn/Article/details/gxebusrrf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gcgyigbiv.sHtML

[R34] 退出时清理
来源：http://www.share.hesvh.cn/Article/details/gfsnkgdky.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gflpaegno.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/ggvbunpha.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/gbxwlcwde.sHtML

[R36] 并发执行多个任务
来源：http://wap.hesvh.cn/Article/details/gymspbztr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fehbvm.com/Article/details/gxkvvkjmk.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/ghxtszzjd.sHtML

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/ggzpwkzus.sHtML

[R38] 管道串联
来源：http://www.blog.zdbjq.cn/Article/details/gjivtwern.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/gnzhgixqn.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fehbvm.com/Article/details/gpkzfbhip.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gxkhtvezn.sHtML

[R40] 追加写日志
来源：http://www.blog.zdbjq.cn/Article/details/gfcdmskyv.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/gcqikwqgj.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gcglaxoja.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gddwtdhca.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gxvepmjpg.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gslqqmegv.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.zdbjq.cn/Article/details/grhwmpdhm.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/goqfihfqu.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/gdlkscsbt.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/gbslqvzoq.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/gwmrxsuts.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gvijaxrdl.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gnfuyvahi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/ghhbcuxuu.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/gqhskgjbi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/goonxshif.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/gdquevods.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gahlsmwyl.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gtdmbuwkg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gzefuobur.sHtML

[R50] awk 求和
来源：http://wap.hesvh.cn/Article/details/gzqfvfynp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gcmsrzlya.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gtmtmyjqa.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gqnidiyul.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/ggqvudvsi.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/glysiqsbt.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gvchgaihn.sHtML


<!-- 参考信息 -->