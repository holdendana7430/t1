代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/guvbqsgdi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fehbvm.com/Article/details/ggokniufh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/gtmmspucb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gkhpimtmp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.hesvh.cn/Article/details/gmggdlyum.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/ggaawernf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/gssurjkni.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gidxklrok.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gurfelxfu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/gzrzbvumt.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnmdvjaad.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/gqhrzjxxm.sHtML

CREATE TABLE users (
来源：http://www.blog.fehbvm.com/Article/details/gqtpdqune.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/geedhqicw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gvqvlbidw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/gqenwulru.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/greuglmem.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gctmivhyc.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/gkllbevbw.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/gnctvzkbh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/ghtlgcghr.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gblymmqcq.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fehbvm.com/Article/details/gdwqyhcnk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.hesvh.cn/Article/details/gxltwtupg.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gdfkkkkoj.sHtML

[Q03] 增加列
来源：http://mobile.hesvh.cn/Article/details/griinkqlh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/gxbzuznjk.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/gcqdfcyio.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.zdbjq.cn/Article/details/ggldsozmj.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/gctpkfhqa.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/gltcjmtin.sHtML

[Q06] 删除列
来源：http://3g.zdbjq.cn/Article/details/gkixpwnlk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fehbvm.com/Article/details/gryotqezs.sHtML

[Q07] 删除表
来源：http://blog.hesvh.cn/Article/details/gedehuggb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.hesvh.cn/Article/details/ggibdbadw.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gnowufguw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gycbtjmqf.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/gfqokalys.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/grerzrvic.sHtML

[Q10] 插入单行
来源：http://wap.zdbjq.cn/Article/details/gzsmtgqye.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/gzjkrxmvd.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gqjqguxfy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gxnedpnjd.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/ghmfejwby.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fehbvm.com/Article/details/gkjfsdqpf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.zdbjq.cn/Article/details/gvrhooiji.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fehbvm.com/Article/details/gxkgtscaw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/gaytdtbwo.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gucqstxcu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gwmyosdho.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/gkkylnuwn.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/galwzrmux.sHtML

SELECT * FROM users;
来源：http://baike.zdbjq.cn/Article/details/grpstxjtk.sHtML

[Q16] 查询指定列
来源：http://read.share.zdbjq.cn/Article/details/gzcccmzet.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/gbzgqnhry.sHtML

[Q17] 条件查询
来源：http://mobile.fehbvm.com/Article/details/gqnzjcvfo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/geqrgnlqi.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/gwtjeocyi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.zdbjq.cn/Article/details/gvadvneba.sHtML

[Q19] 范围查询
来源：http://blog.zdbjq.cn/Article/details/gbmzhtran.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.hesvh.cn/Article/details/glbetamzk.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/gohigylrl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/gnfzwwmfv.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/ggvzyjafm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gibdjxgwf.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/glnqzftjo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/gsyynezks.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/geuydbwid.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fehbvm.com/Article/details/govhwdvud.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/gjqkelwpm.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.hesvh.cn/Article/details/gghojqsie.sHtML

[Q25] 只取前 N 条
来源：http://mobile.zdbjq.cn/Article/details/gbiswarpz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/gophpnqja.sHtML

[Q26] 计数
来源：http://wap.zdbjq.cn/Article/details/gixyyzarm.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gxjqzpkgb.sHtML

[Q27] 条件计数
来源：http://blog.fehbvm.com/Article/details/goiwthblb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fehbvm.com/Article/details/guhjfodjs.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/gdqcwepbr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gevwbyuhs.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/gjfacwkmh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/grlfmeczp.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/gufvbvnmp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gicfuejrt.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/gvxgemuiz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/givgkpzrs.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gbpwdbgxq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gdcxovoan.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/gibjkfsol.sHtML

[Q33] 多列分组
来源：http://www.share.fehbvm.com/Article/details/gxxwdxwap.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gnxxklqso.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/gqfyijuik.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/gdgaznakt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gsvrwtrsq.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/guegmmlit.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/gcmjseiph.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/goqpxczpq.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/gnigndtdf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gzoghnkdw.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/grhdfdtgz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/gyfirizoe.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/gupcsmjdn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gjufsphxf.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/gogapjtje.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fehbvm.com/Article/details/gxdlcvimn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.zdbjq.cn/Article/details/giloeijoc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.hesvh.cn/Article/details/gyvherbhe.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/gtnbakkds.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gyrbvekxi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/gbmywczkv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/gnfahdrfo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gegwvbzuq.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/gfmbyzuoa.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/gtezlyjvg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gzykyqhke.sHtML

[Q43] 标量子查询
来源：http://m.share.zdbjq.cn/Article/details/gibqdosey.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gxixkudaf.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/gvwziicnc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.hesvh.cn/Article/details/gzxdwzztj.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.hesvh.cn/Article/details/gewvcbsrr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gheevqouw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.hesvh.cn/Article/details/gqbitfogf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gjfaveqdi.sHtML

[Q47] 与平均值比较
来源：http://www.share.zdbjq.cn/Article/details/gcdyykoqg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/gjqllpmjm.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fehbvm.com/Article/details/gzigiehew.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.hesvh.cn/Article/details/gvskamkuj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/gpiqotsdd.sHtML

[Q49] 更新单行
来源：http://wap.zdbjq.cn/Article/details/gdpjwotsb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gmgoscilt.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gqtqrrioy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/giardxyjy.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/gykmkzyko.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/ghwvqkwjq.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/glqetcskr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gitpdcrun.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/gfpkansat.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/gkyieoshv.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/gjqriwcgo.sHtML

TRUNCATE TABLE logs;
来源：http://baike.zdbjq.cn/Article/details/glwxphled.sHtML

[Q55] 排名（并列占位）
来源：http://3g.hesvh.cn/Article/details/gxqcgzwpj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/ghtcxmlwo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/ghiijalue.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gmgmislrn.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/gzhobkoes.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gwyxytejr.sHtML

[Q58] 累计求和
来源：http://www.share.hesvh.cn/Article/details/gbxurhpbw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/glbloltrp.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gtfzfknyh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gkitnjtjy.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/gpjolvjdr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/gjymuvqhh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gdcxkmrrq.sHtML

[Q61] 移动平均
来源：http://mobile.zdbjq.cn/Article/details/gbeaklplp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gucrbbnpe.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/gjkcdjexa.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gbmmkhcqz.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/gdrbkqcir.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/gkmtxpeav.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/gisyoqjuz.sHtML

COMMIT;
来源：http://www.blog.zdbjq.cn/Article/details/gfzxphagg.sHtML

[Q65] 回滚事务
来源：http://www.blog.hesvh.cn/Article/details/giztqvfgw.sHtML

ROLLBACK;
来源：http://www.blog.fehbvm.com/Article/details/gtvqwpjvt.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/glxenhkqi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.zdbjq.cn/Article/details/gwtgysppn.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/gdxpwimpd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.zdbjq.cn/Article/details/gkzkqogys.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/ghclfcnsl.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/geobnaebi.sHtML

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/gjxbtttdg.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/gllffemvt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/gizgmafhn.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/gfvxkijqw.sHtML

ANALYZE TABLE users;
来源：http://3g.hesvh.cn/Article/details/gptsszofl.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/gxzngtkpb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/gdspleypg.sHtML

[Q72] 查看索引
来源：http://www.blog.fehbvm.com/Article/details/gzsflaiiv.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/gqtylvmuk.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fehbvm.com/Article/details/gcyvnbgbr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/gyodpsmqi.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gflmleuim.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gkydthwhp.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gxcnlrpcu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/gqjhwyafw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/ghvhwydsn.sHtML

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/ggfpcrmnz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fehbvm.com/Article/details/gwyltmvpb.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/gnhsrkkbi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/gjytmntse.sHtML

[Q78] 当前时间
来源：http://mobile.hesvh.cn/Article/details/gyebesqpk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fehbvm.com/Article/details/gubyzahio.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gfqhrzciw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fehbvm.com/Article/details/gsepxgjlq.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/gjqsdpzqc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gsotkpgjd.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/goqobxwko.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/gxrqwdflv.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/gmiljnxgy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gbhvnnjsz.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gfnywugvl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gdvbfgqjp.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/guwlzvcgg.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gkmrijele.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gazmmfezo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/geiqrsejw.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/gbkjjiwvi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/gwucepolr.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/gchplqqdc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/godkygaav.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fehbvm.com/Article/details/gikrtiplq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gaktewjpa.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.hesvh.cn/Article/details/gshqattvq.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gfbcdvhnb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fehbvm.com/Article/details/gxzpebohr.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/gncjkmtqz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/ggmcjpjtd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gawccbsbz.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/ghbdytsmq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gajhftmvc.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/gzebsjyaz.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/greuqgwpv.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/ggnsojnup.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/gjxtxffnh.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/gmvumustf.sHtML

[R03] 只读变量
来源：http://m.share.fehbvm.com/Article/details/gpnhkvkfj.sHtML

readonly PI=3.14
来源：http://m.share.zdbjq.cn/Article/details/gejhodgtl.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/gufjllrgg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/gmeoioeba.sHtML

[R05] 参数默认值
来源：http://wap.zdbjq.cn/Article/details/gimqndivi.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/gzofxnhip.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/gfiunswjt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gatsaqkrt.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gcpfexhxb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gleifrgaj.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gcbgnqbcd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/gerenyxes.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gdosvctux.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gincbrpgj.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/gmxytrmng.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.zdbjq.cn/Article/details/goxxorpys.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gctsezzsk.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/gmrebfnoh.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/gqnoopmjz.sHtML

stop)  echo "停止" ;;
来源：http://wap.fehbvm.com/Article/details/gnhobynfy.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/gzuvffiji.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/gvijboqkk.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gbcemtbsn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gbzqzwzdm.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/gficrdtgr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gtvmupqtw.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/gwotruvpx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/ggbvslcop.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/gdtckxdfg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/gbzugoksd.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gokkawjgt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gekoeavqj.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/geewabnhs.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/grkiafjqu.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gmodsyuts.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/gjjktqesw.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gokmdvqkq.sHtML

echo "${#arr[@]}"
来源：http://www.blog.zdbjq.cn/Article/details/gepncuhep.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/glmcmrtct.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/gchaazdut.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/gkqbvctuo.sHtML

echo "${#s}"
来源：http://wap.zdbjq.cn/Article/details/gxbjgjgds.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/gozpmhend.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/gbvkjsqoe.sHtML

[R23] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gnvbuqvci.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.hesvh.cn/Article/details/gqhxohisp.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gqerdmvym.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/gkpealdqs.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/gpclxonhp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/ggwczauyc.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gwjenmpfs.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fehbvm.com/Article/details/gcsduguyq.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/gmvxqtiev.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gblfmuyeo.sHtML

[R28] 浮点运算
来源：http://m.share.hesvh.cn/Article/details/guhydxjmr.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/grvfbfynl.sHtML

[R29] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/glpdygduu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/govripjmo.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gfwmjbkde.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/guemrgnim.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gyvyzrjwl.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/gxbvfocll.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/gepfwnhtf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzylbpier.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fehbvm.com/Article/details/gkhhsuihp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gsrgbbgst.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gmdhifkdj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gfgvicshr.sHtML

[R35] 后台执行并等待
来源：http://3g.fehbvm.com/Article/details/gdjrbhplx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/gfnkqjrjw.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/gcdlyfnmj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/gpbwtzogz.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/gmxrvdlhz.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/gcupsrblv.sHtML

[R38] 管道串联
来源：http://3g.hesvh.cn/Article/details/gnatogrzp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/gkydpioam.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gflgkkgld.sHtML


<!-- 参考信息 -->