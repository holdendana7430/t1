代发 wailian999

CREATE TABLE users (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxiyaszi.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fanxiaobao.xyz/Article/details/gwthbuufj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fanxiaobao.xyz/Article/details/gnkhbezsm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fanxiaobao.xyz/Article/details/gxozebeeb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsikklyi.sHtML

);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsliukihh.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfvfrmyi.sHtML

CREATE TABLE orders (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshjhyhyj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fanxiaobao.xyz/Article/details/gayfoptqs.sHtML

user_id INT NOT NULL,
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsiiltsf.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrsyvvps.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fanxiaobao.xyz/Article/details/gkpgzgtnv.sHtML

);
来源：http://m.share.fanxiaobao.xyz/Article/details/gciyzpvxw.sHtML

[Q03] 增加列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkztqljdf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gwmaoukwf.sHtML

[Q04] 修改列类型
来源：http://baike.fanxiaobao.xyz/Article/details/gmljnajmv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fanxiaobao.xyz/Article/details/guwvxzmdd.sHtML

[Q05] 重命名列
来源：http://3g.fanxiaobao.xyz/Article/details/gqzytgbte.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fanxiaobao.xyz/Article/details/gzwuermfb.sHtML

[Q06] 删除列
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqhfyjcs.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fanxiaobao.xyz/Article/details/gcqhrxlwk.sHtML

[Q07] 删除表
来源：http://mobile.fanxiaobao.xyz/Article/details/gimvgobia.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gicjakavf.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmrknfja.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaiebeugm.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjsbjecm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fanxiaobao.xyz/Article/details/gchoancxw.sHtML

[Q10] 插入单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxesvboy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxndnpxh.sHtML

[Q11] 一次插入多行
来源：http://blog.fanxiaobao.xyz/Article/details/gppjiqshb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkghrvar.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhwnyeig.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwyjnxuc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fanxiaobao.xyz/Article/details/gvptmebpo.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fanxiaobao.xyz/Article/details/gngfxzxjx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/gexvnldzk.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fanxiaobao.xyz/Article/details/gsataqjni.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamivmciu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fanxiaobao.xyz/Article/details/gajyepcwk.sHtML

[Q15] 查询全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnudyduc.sHtML

SELECT * FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gijaattpn.sHtML

[Q16] 查询指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpxeonzp.sHtML

SELECT id, name FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gexhsjhzj.sHtML

[Q17] 条件查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gxttydgxb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnszdsmja.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfibcwuju.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fanxiaobao.xyz/Article/details/ggoqnwmsu.sHtML

[Q19] 范围查询
来源：http://wap.fanxiaobao.xyz/Article/details/gewmxiwer.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxatixjvt.sHtML

[Q20] IN 列表
来源：http://baike.fanxiaobao.xyz/Article/details/gillturia.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/grlvnqkuj.sHtML

[Q21] 空值判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gcggowfrx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdpwamzo.sHtML

[Q22] 排序
来源：http://blog.fanxiaobao.xyz/Article/details/gvvnpssxp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fanxiaobao.xyz/Article/details/gkfdpegxw.sHtML

[Q23] 分页
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gweekvjzo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzcqiugw.sHtML

[Q24] 去重
来源：http://www.share.fanxiaobao.xyz/Article/details/guddkcqgj.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmptgpbhn.sHtML

[Q25] 只取前 N 条
来源：http://blog.fanxiaobao.xyz/Article/details/gpmgypizd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfcslxvb.sHtML

[Q26] 计数
来源：http://blog.fanxiaobao.xyz/Article/details/geqskjgnc.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbijtpfj.sHtML

[Q27] 条件计数
来源：http://3g.fanxiaobao.xyz/Article/details/guswwrwvm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gtbylijcw.sHtML

[Q28] 求和与平均
来源：http://blog.fanxiaobao.xyz/Article/details/gwdsklkgz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/glvnnfumy.sHtML

[Q29] 最大最小值
来源：http://blog.fanxiaobao.xyz/Article/details/ghgyhytyp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gboompqub.sHtML

[Q30] 分组统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gmryptpmv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gqvkpbeod.sHtML

[Q31] 分组后过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqpgqxom.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gscfkutub.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gjyvogdcu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbddauuuw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxswdrqai.sHtML

[Q33] 多列分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjrpdzle.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fanxiaobao.xyz/Article/details/giidcewug.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfphwytj.sHtML

SELECT * FROM (
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxcirwix.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswsvyuvi.sHtML

) t WHERE rn = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gkbwbhmyh.sHtML

[Q35] 内连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gbuxhzksa.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzatbflpj.sHtML

[Q36] 左连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gyubsydsu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gysknssiz.sHtML

[Q37] 右连接
来源：http://wap.fanxiaobao.xyz/Article/details/gfnoqmrrq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gaqbcxgeo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmuazxqk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gdhohhgen.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fanxiaobao.xyz/Article/details/gprzzmrid.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fanxiaobao.xyz/Article/details/gfszmpody.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gabtmwowu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fanxiaobao.xyz/Article/details/gjaruzsqc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fanxiaobao.xyz/Article/details/gyyvnytxz.sHtML

[Q41] 多表连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqfbxlsc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fanxiaobao.xyz/Article/details/guhnmuseq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fanxiaobao.xyz/Article/details/girqxouqx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqviwedt.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczohkwsc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fanxiaobao.xyz/Article/details/gablokayt.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gyxjflnph.sHtML

[Q43] 标量子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gnipzbbco.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehbkstwu.sHtML

[Q44] IN 子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gaxuddqvy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fanxiaobao.xyz/Article/details/ggytlzent.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjofuwgz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gasgjmrkw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fanxiaobao.xyz/Article/details/ghnbjahte.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gukrgvygt.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/goixbjrer.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goigdkyrq.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gukcigxxg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxmdckcp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gswwuenoh.sHtML

[Q49] 更新单行
来源：http://www.share.fanxiaobao.xyz/Article/details/gytncojwm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gihllizkz.sHtML

[Q50] 批量更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbfywrhc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdgurkac.sHtML

[Q51] 用子查询更新
来源：http://baike.fanxiaobao.xyz/Article/details/gjcwxeajt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gaeuxmjjb.sHtML

[Q52] 删除指定行
来源：http://read.share.fanxiaobao.xyz/Article/details/gwespodqz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvkkdvcr.sHtML

[Q53] 按条件删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gppfedjvq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrmsbjjs.sHtML

[Q54] 清空表
来源：http://wap.fanxiaobao.xyz/Article/details/gsgtzrefd.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fanxiaobao.xyz/Article/details/gagfeccvr.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghudneeps.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyimdrbh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fanxiaobao.xyz/Article/details/guklfhsds.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/guoekiezi.sHtML

[Q57] 行号
来源：http://wap.fanxiaobao.xyz/Article/details/gvodjotkd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gewundaim.sHtML

[Q58] 累计求和
来源：http://baike.fanxiaobao.xyz/Article/details/gzeubvmpv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gahyeifsz.sHtML

[Q59] 分组内累计
来源：http://baike.fanxiaobao.xyz/Article/details/gpreyavdz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gxlogrcio.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfnuetzv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpfyrrzd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gwvqivpvd.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gicxuyajf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gdlbrusfx.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gzzhqcsim.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbwiktmu.sHtML

[Q63] 开启事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghawofahl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fanxiaobao.xyz/Article/details/gyiaswalh.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/gxbbnpwtg.sHtML

COMMIT;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnnmmjeb.sHtML

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbmmwiud.sHtML

ROLLBACK;
来源：http://www.share.fanxiaobao.xyz/Article/details/glkthiqqk.sHtML

[Q66] 行锁查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqjqmmnt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fanxiaobao.xyz/Article/details/gvfdyafja.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/gufyjaeyp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtqqfasr.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/gbdgkedis.sHtML

SAVEPOINT sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gxzzavyuy.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gooxaiqde.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/grwtqtgsg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fanxiaobao.xyz/Article/details/giqxgyasa.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgwazmai.sHtML

ANALYZE TABLE users;
来源：http://3g.fanxiaobao.xyz/Article/details/gotishqph.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhxqvwkc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/ghejlnqyp.sHtML

[Q72] 查看索引
来源：http://baike.fanxiaobao.xyz/Article/details/gwgqxkyvf.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnwbqtus.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjscehuy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnadvqup.sHtML

[Q74] 强制使用索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gnymcapxf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzbgvdsl.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gzsirgcco.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gizgvjlpm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/gjmrmofgc.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/grrfxbifa.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfqixiky.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gwqihotjo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjdgqotw.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/gijcfjfjs.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhiykkhl.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gygsfbszm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/grfoomfvq.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gisybtqeg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gpcowpnus.sHtML

[Q81] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gugsfytzq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gajmppncn.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/gppgjpdie.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbghwfpax.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/giwvzopbd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gnqceizkf.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gzimnmjen.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzewnfxb.sHtML

[Q85] 数值取整
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgiqmkrq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/ghnrjpqiz.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsmkihpu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjyfjoxn.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbojeesj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyikfjauy.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/gwjsbmynj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gihrstlwj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gfdxtlzjm.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gueqchrko.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gstahfgoi.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/gymewzkbf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/guhhzuumr.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gvrxoekwj.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnplpgsk.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/geirdwlkj.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnebnpyh.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusbfmmdh.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gqqqreabj.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyokqnbft.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjfswusd.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkcpvcce.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/gwbbukqet.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gveelqgqc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsodimkn.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gdmecawgk.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmaichumc.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gniumbcma.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gsrnbwlpj.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/grtjpqfbc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gyrexsane.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gosssraie.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gyioskbyc.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/ghelgrdsd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/golroqtoe.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtvtdgrn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdsgsbdm.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcteifwju.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobqganuf.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevbmwzko.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggchebcpk.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcidcdegd.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gavjpyisb.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvypmxmai.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gcgdbdscc.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtbvhnrp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gglfwnjcu.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfvrrwjk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gffilqilt.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gpjeouktn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gujqukzor.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/ggjscvwkv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gncsfxsxa.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gquplynut.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gygupqhip.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gsbugufwa.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlvyywyi.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyjrzdpn.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvspgdefw.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqdfukpv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkmzgjwl.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gvavhhnfr.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfculnaan.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gqkggwddz.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gptkfxncm.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwtjfbhe.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gwoknagwr.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/ghmwheede.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gzpgjtxay.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlyvhpmr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gsckkdyot.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/grnrxmtao.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/glxonptdb.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmiegtbb.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gtanuhqwu.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxshpgli.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gzlufakli.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gjomtiwyb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/giwvmghot.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdmewwca.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqihuzxwt.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvlowsbv.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghiclldov.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gcwtjaeuw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxftchhny.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzgbrkjc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/guaxjvflo.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvjcsanz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gcegdgzrk.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gatorjghk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gmmaaitkk.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/ghilibmvo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrdaozzt.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnjbawpw.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/ghsfvbkef.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzrxkrsz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlqctmok.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/guicuvdid.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/geelbgtry.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gyfbdfkjc.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gyxffaxzs.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gyvljfmje.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gihcgmxkx.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gmmpruzmk.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gpnkcnbsw.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gifhhhnwg.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gcrdbnlcj.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/getkzwubn.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gjfridsns.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyurfhlg.sHtML


<!-- 参考信息 -->