代发 wailian999

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/gbajkgmwc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gfpvdgzqk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gcvfbmopm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/gfdsuarlt.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/gainjhlps.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gpwyyvoau.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gffoxutde.sHtML

CREATE TABLE orders (
来源：http://baike.hesvh.cn/Article/details/gnzkuyxtr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gyvvtdhuv.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gvameqzsr.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/gnttzsjgm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/gqqzokxhy.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/ggvcxozfg.sHtML

[Q03] 增加列
来源：http://blog.hesvh.cn/Article/details/gwbvlqtrw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.zdbjq.cn/Article/details/gebwglgoe.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/gjqebioej.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/glojsessj.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/gwcytgzja.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fehbvm.com/Article/details/girytuolh.sHtML

[Q06] 删除列
来源：http://mobile.fehbvm.com/Article/details/gflworpfd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/gfeyrcwhs.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/giiwjljos.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.zdbjq.cn/Article/details/gbxvujtka.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/gayrspoxp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gsfuquzsn.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/gjcewkoex.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gytemggbu.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/gxlghweip.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gpwwnegny.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/gqgesooao.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gdbmrviwv.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/getzgxmcd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fehbvm.com/Article/details/ggamniyur.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.zdbjq.cn/Article/details/gqvreirii.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fehbvm.com/Article/details/gbzihfugr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/grqofthkt.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gyenspcvj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.hesvh.cn/Article/details/gmayrziul.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/gyypldtak.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/gjbiqitck.sHtML

SELECT * FROM users;
来源：http://wap.hesvh.cn/Article/details/ggpumazhf.sHtML

[Q16] 查询指定列
来源：http://3g.fehbvm.com/Article/details/gioelnovt.sHtML

SELECT id, name FROM users;
来源：http://read.share.hesvh.cn/Article/details/gqtnukcbf.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/grtnbenao.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fehbvm.com/Article/details/geyvlpgrs.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/glwmisrgq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/gjlpeoodg.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/goiajrxvt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fehbvm.com/Article/details/gxutjtfmb.sHtML

[Q20] IN 列表
来源：http://www.blog.hesvh.cn/Article/details/gwrcpodmt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/gnjvxlvzp.sHtML

[Q21] 空值判断
来源：http://wap.zdbjq.cn/Article/details/glafkcafn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/grnycsrps.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/gvyopence.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/gcwmaogxl.sHtML

[Q23] 分页
来源：http://3g.zdbjq.cn/Article/details/gvizejvan.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gjhdxjfjj.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/gvaodtpwg.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/gluhagufg.sHtML

[Q25] 只取前 N 条
来源：http://read.share.hesvh.cn/Article/details/gqsiegprc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.zdbjq.cn/Article/details/gsovpehob.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/gayjtwlxi.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gukdfrpqa.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/gobmghyze.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/gmokomkid.sHtML

[Q28] 求和与平均
来源：http://mobile.zdbjq.cn/Article/details/gjcquairk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gjjgdvysw.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/gafzckyho.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fehbvm.com/Article/details/gusrdvlqm.sHtML

[Q30] 分组统计
来源：http://3g.hesvh.cn/Article/details/gptzgrlmq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gmxbitzwh.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/gzsseafdk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.zdbjq.cn/Article/details/gutykwmfc.sHtML

[Q32] 分组拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gdbidvgat.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gkxbimmvb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gcrtyuwtj.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gmnnrzdxm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.hesvh.cn/Article/details/gesxtnepd.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/gudwnvznm.sHtML

SELECT * FROM (
来源：http://www.m.share.zdbjq.cn/Article/details/gmibkqknp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.hesvh.cn/Article/details/gnhfkqwyj.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/grtwashoz.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/gjzozlmzj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gcoiumndn.sHtML

[Q36] 左连接
来源：http://www.blog.zdbjq.cn/Article/details/gfmgsvyrj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gjpdjiody.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/gfjvtddsj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/gclmlxojn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/gcseosysj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/ghrkibrdn.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/gosiekrha.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.zdbjq.cn/Article/details/gnnpgtkac.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.zdbjq.cn/Article/details/gaxbpyqth.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/golzvkfnv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gpxehknqq.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/gunrqofyx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/gkqkahgtx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.zdbjq.cn/Article/details/gxariddxm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gxzibgawn.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/glrntmphq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/guaumiuqw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.hesvh.cn/Article/details/gfqgxqywe.sHtML

[Q43] 标量子查询
来源：http://m.share.fehbvm.com/Article/details/gamcfewyz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.zdbjq.cn/Article/details/gjvdxglmz.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/gubvyhlso.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/gtidwxqtm.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.zdbjq.cn/Article/details/gkqchnvrs.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/guztyutpm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fehbvm.com/Article/details/gelfwyrwc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gnjaomdsp.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/gfygqypsm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.hesvh.cn/Article/details/gzjykhsjt.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.zdbjq.cn/Article/details/gcwrdytdg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/gabckzxvq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/goeojvipp.sHtML

[Q49] 更新单行
来源：http://www.m.share.zdbjq.cn/Article/details/gwanwyezk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gbgryijrv.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/glhriuake.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/gsngvutwq.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.hesvh.cn/Article/details/groyxdtww.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fehbvm.com/Article/details/gbupiomlo.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/gvnxwdfhg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gqhyktcna.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/gqzefohcc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/gmgprltjy.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/ghsdopadu.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/gaggtsmzs.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/gmeolkpyh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gufnljrla.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gihihoukj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gkfabnisa.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/ghzlvppsz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gjfycuymp.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/gczmnyrne.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gjqhyiczh.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/genlzskfm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gkkfehlxd.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.hesvh.cn/Article/details/gjdtrgrba.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.hesvh.cn/Article/details/gmepauxuv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/geivrjfwl.sHtML

[Q61] 移动平均
来源：http://wap.fehbvm.com/Article/details/ganzzcxwg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gpkqhpgfn.sHtML

[Q62] 分组占比
来源：http://www.blog.hesvh.cn/Article/details/gfazbtner.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/goggdleec.sHtML

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/gaurvafsu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/gjojzaywv.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/gyzhbkzym.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/gseaasfje.sHtML

[Q65] 回滚事务
来源：http://blog.hesvh.cn/Article/details/gfwxmmlju.sHtML

ROLLBACK;
来源：http://m.share.hesvh.cn/Article/details/gbohavzyi.sHtML

[Q66] 行锁查询
来源：http://mobile.fehbvm.com/Article/details/grgtpmkty.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/gewzhxyah.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/gdoucaxpu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/glfhqqzza.sHtML

[Q68] 保存点
来源：http://www.blog.hesvh.cn/Article/details/gdplbnloo.sHtML

SAVEPOINT sp1;
来源：http://wap.hesvh.cn/Article/details/gxqkcslcc.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/grasqxuxo.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/gzlykftty.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/gevzecfsc.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/gxzbfhyiv.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/gexiwtlao.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/ghkobgyjh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.hesvh.cn/Article/details/gscxnrlsm.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/gpnumzntq.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gdfdlameb.sHtML

[Q73] 查看表状态
来源：http://read.share.fehbvm.com/Article/details/gtjmvfskr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/gjcqbjqov.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/gzxvnejle.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/gpwlskyqr.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gcwwzobaa.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gmhjgucjy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/gltaawkyg.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/gpwnmttvo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.hesvh.cn/Article/details/gvpjcqdxs.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/geogegftm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/gpxojsjok.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/gvpfsdvxf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.zdbjq.cn/Article/details/gbolopfjr.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gkweuzzyk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/gnmegwpbe.sHtML

[Q80] 字符串截取
来源：http://blog.hesvh.cn/Article/details/grprunvok.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gubrnddtp.sHtML

[Q81] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gexjmkweg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.zdbjq.cn/Article/details/gdetercsl.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/gtabsvkij.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gktdjbkfo.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gwvhrjgxd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gxzmdlhwe.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/gfmycdcba.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gjoqizokw.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/gxipbkqno.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/gansnwylv.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gicqcgsao.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gvamlvivv.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/gsyiuznhz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fehbvm.com/Article/details/gdbxxnpfg.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gacapvyvu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/giwucxlom.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/gyvrocpgd.sHtML

[Q89] 判断表是否存在
来源：http://baike.hesvh.cn/Article/details/gsspddwij.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/gxmbkjlvh.sHtML

[Q90] 生成序号列
来源：http://3g.zdbjq.cn/Article/details/gtpxnhgjo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gmtybiqyc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/geasxtsmi.sHtML

R. Bash 专题
来源：http://3g.fehbvm.com/Article/details/ghluatkbt.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghlvhmprs.sHtML

[R01] shebang 与严格模式
来源：http://read.share.zdbjq.cn/Article/details/gcetztamj.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/gymmoecuo.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/gjmexotwy.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/gazvbhbcg.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gygfffaqa.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/gjzygfvdq.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/gqlwounwt.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/gtjiufqqz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/gezvifgfo.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/gnkkptwzl.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/gnieutzce.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/gispdrbmw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gbbhsbypk.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/gypnpxbzq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fehbvm.com/Article/details/gdozskjlq.sHtML

[R08] 数值比较
来源：http://wap.hesvh.cn/Article/details/gnxbxtkup.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.hesvh.cn/Article/details/gnlhifhjj.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gtdghlxoc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/gwbgqjtjo.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/giswbomnx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.hesvh.cn/Article/details/gucrwszje.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/gkkqvehvf.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/gwdlsajue.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/ghhidmalm.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/grudievpf.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/gljfqtrgt.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/gyiiawgmm.sHtML

[R12] for 遍历文件
来源：http://www.blog.hesvh.cn/Article/details/gfxoghopo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fehbvm.com/Article/details/gvdpzfwsz.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gvzslkbph.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/ghrfpssed.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/gghclzafy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gamteewhp.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gppxuvwwc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fehbvm.com/Article/details/gofjucdmc.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/gajysdile.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gcrqtvlqu.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/gcuuyuhpk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/gcwqravjj.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/gqwyaobof.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gcdvdosmx.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gqnmmvuen.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/gpwgetnms.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fehbvm.com/Article/details/gxrdmhtlz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fehbvm.com/Article/details/gxojlqrhx.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gjqsohgsn.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/gqaqdlzvp.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gfxityimd.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/gzeqpybye.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gvnzabuhu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/getzgcihu.sHtML

[R24] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gjeruuobz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/gzedutgbt.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/gnkgtqbxx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/gulpkkxcw.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/giupoklze.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.zdbjq.cn/Article/details/gvbicvwvi.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/guktyeopt.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/gxnhcvykf.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/gnpteraff.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.zdbjq.cn/Article/details/geuxpnzwt.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gzloxrvca.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fehbvm.com/Article/details/gkcsagjor.sHtML

[R30] 函数返回状态码
来源：http://3g.zdbjq.cn/Article/details/gnrshaktm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fehbvm.com/Article/details/goekorvdn.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/gtqhssxwi.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/ggmafgurx.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/glaquypba.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gdcwogkcf.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/guypycoip.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/ghxettgga.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/glimenlfy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gqsfqdwad.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gsohxywzo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/gkeaalsrz.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fehbvm.com/Article/details/gqwbmsqes.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/gdvkgkuxq.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/gymgvwclr.sHtML

files=$(ls -1)
来源：http://3g.hesvh.cn/Article/details/gosjbleic.sHtML

[R38] 管道串联
来源：http://3g.hesvh.cn/Article/details/gaxitmvbr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gsamcajqb.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fehbvm.com/Article/details/gglkxoubj.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gdmtithjd.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/goqmtcwoi.sHtML

echo "log" >> out.log
来源：http://wap.zdbjq.cn/Article/details/gvtjcdwlv.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/gyztffovo.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gknmqkkev.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gpgyvkcne.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gcahnbhhd.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/gcvvpqrrw.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/gfdczavgb.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/gqgobcptg.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/ggfitzpcg.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/ggqftajwy.sHtML


<!-- 参考信息 -->