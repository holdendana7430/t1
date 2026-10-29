代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.zdbjq.cn/Article/details/gsyhduhbw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fehbvm.com/Article/details/gchomxfsa.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/gxikgneuo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/gedzntxkw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/guvlrxtzq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fehbvm.com/Article/details/galzuddhb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gemjinykg.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/gpvciyknw.sHtML

CREATE TABLE users (
来源：http://wap.zdbjq.cn/Article/details/guikpxdza.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/ghyicdxyy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gognhkoli.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/gejgyersz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fehbvm.com/Article/details/gandxcufd.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/ghftykhby.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gtbgacypx.sHtML

CREATE TABLE orders (
来源：http://wap.fehbvm.com/Article/details/gvajlzkxo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/ggwhbbdep.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gnmyueeoy.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/geoqptwzc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gmpaqmfsh.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gbomlyqnn.sHtML

[Q03] 增加列
来源：http://wap.hesvh.cn/Article/details/gtbhnzaqw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fehbvm.com/Article/details/gclkhnbiw.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/gmktspnxf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/gwbfjblbk.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/gzlnuuibw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/gkalvnnog.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/ggfubvnhx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/gvlrsxkel.sHtML

[Q07] 删除表
来源：http://m.share.hesvh.cn/Article/details/gbheomvpp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/gtqrxluzr.sHtML

[Q08] 创建普通索引
来源：http://blog.hesvh.cn/Article/details/gfzdcbsgm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/ghyuimdce.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/gqjwngbjb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gclkviaus.sHtML

[Q10] 插入单行
来源：http://mobile.hesvh.cn/Article/details/gqjnyndmd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gizxwsdam.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/gglqkccih.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fehbvm.com/Article/details/ggypqleel.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.zdbjq.cn/Article/details/gitrpucym.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/gulagftzf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/ghlwtsqhd.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.hesvh.cn/Article/details/gygmvvvor.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gceepvlla.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/ghljguwbt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fehbvm.com/Article/details/guywynxzd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fehbvm.com/Article/details/gkmwbepal.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/gvijnsxlo.sHtML

SELECT * FROM users;
来源：http://blog.fehbvm.com/Article/details/gsypaxlmm.sHtML

[Q16] 查询指定列
来源：http://3g.fehbvm.com/Article/details/gacgggztw.sHtML

SELECT id, name FROM users;
来源：http://baike.hesvh.cn/Article/details/gipsxsjls.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/grllvrbib.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/govvtseym.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/gdxkbrynd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.hesvh.cn/Article/details/gbyvkofwp.sHtML

[Q19] 范围查询
来源：http://m.share.hesvh.cn/Article/details/gczcdvvlb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/gfqnefwck.sHtML

[Q20] IN 列表
来源：http://www.blog.hesvh.cn/Article/details/ggqgbytnf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/guckklupz.sHtML

[Q21] 空值判断
来源：http://blog.zdbjq.cn/Article/details/gctqbvqer.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/gjcwndjrm.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/gwgfngtas.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/gavehigcv.sHtML

[Q23] 分页
来源：http://m.share.fehbvm.com/Article/details/gxjdqlost.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/gseseljvh.sHtML

[Q24] 去重
来源：http://m.share.zdbjq.cn/Article/details/gcgylgjse.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/govasvrcx.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gmvfftzps.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.zdbjq.cn/Article/details/gwvylpdrn.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/gknormkyh.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/glvcgoeze.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/gphzsrlmz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/gonwevypv.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/gsglujjve.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gtlmecuia.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gykovuolo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gjerxilhb.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/giuwjxdvl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gixmeerle.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/gdwzqxpre.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/gvduilnkk.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/gxeojphfl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gxbsqrrkj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/gltunuoay.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/gkcnxrzco.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/gvouzxvbr.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fehbvm.com/Article/details/gbfryionq.sHtML

SELECT * FROM (
来源：http://m.share.hesvh.cn/Article/details/gdoiuwzkj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.hesvh.cn/Article/details/ghuxrhuke.sHtML

) t WHERE rn = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gulfqfvaw.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gnblstigq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gtngdayhd.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/gifqivgxt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gliynehhc.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/gzxkumsew.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fehbvm.com/Article/details/gxqzewcxy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/gxvjmdvik.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fehbvm.com/Article/details/gpinkuxoh.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fehbvm.com/Article/details/ghnqbmssh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fehbvm.com/Article/details/ggmxeonyv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.hesvh.cn/Article/details/gttnpkkxe.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/gsjixendp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/gtobywxbe.sHtML

[Q41] 多表连接
来源：http://read.share.zdbjq.cn/Article/details/ggomstdeq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/gdwajkjak.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/gapxohowa.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/gqfrqdnas.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/ggdxacyrj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/gjbrytixn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gavlozypq.sHtML

[Q43] 标量子查询
来源：http://www.blog.hesvh.cn/Article/details/glrieqwha.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.hesvh.cn/Article/details/gprkxgjsn.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/gstchflrm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fehbvm.com/Article/details/gqdokmdom.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fehbvm.com/Article/details/geejrmqym.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gudhwgfis.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fehbvm.com/Article/details/gstrmhtqz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gypunxjfq.sHtML

[Q47] 与平均值比较
来源：http://baike.fehbvm.com/Article/details/gvphrtnjh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.hesvh.cn/Article/details/gooocyvnv.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fehbvm.com/Article/details/ghzhvwggg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/gbkhciljm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/gqevqwuke.sHtML

[Q49] 更新单行
来源：http://m.share.fehbvm.com/Article/details/glnbjyjxz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gugkieice.sHtML

[Q50] 批量更新
来源：http://www.m.share.zdbjq.cn/Article/details/ghmteapgd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gzfumjeiq.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gcelffpeh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/gxgrdrhkp.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/gdavnveub.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gxtzgaear.sHtML

[Q53] 按条件删除
来源：http://blog.zdbjq.cn/Article/details/gbbnsighz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gzwumkdfm.sHtML

[Q54] 清空表
来源：http://www.m.share.hesvh.cn/Article/details/ggetnxjre.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/ghgwagcse.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/govyqqfcg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/ghdqcbbqr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/gaqovfpvb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gdaaqcqxx.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/gvibhelpf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/gbjedqqep.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/gdivdmhtr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gyknlcjmq.sHtML

[Q59] 分组内累计
来源：http://read.share.fehbvm.com/Article/details/gcyyksiew.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gmkmnjgkr.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.hesvh.cn/Article/details/gzriqhfkc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.hesvh.cn/Article/details/gagnlhalx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/gzthuadmr.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/gophzetaw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.hesvh.cn/Article/details/girjwmnoq.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/gcreaozpg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gcbamiyyq.sHtML

[Q63] 开启事务
来源：http://www.share.fehbvm.com/Article/details/gqizdndev.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fehbvm.com/Article/details/gsuerzjpi.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/gsjajmljp.sHtML

COMMIT;
来源：http://mobile.fehbvm.com/Article/details/gqduhztby.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fehbvm.com/Article/details/gqrlzvmza.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/gersholrv.sHtML

[Q66] 行锁查询
来源：http://read.share.fehbvm.com/Article/details/ggwdvooju.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.zdbjq.cn/Article/details/gtdgwmpwj.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/gsmmapkvu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fehbvm.com/Article/details/glsvszovn.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gjmgyswpy.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gktebzsht.sHtML

ROLLBACK TO sp1;
来源：http://3g.fehbvm.com/Article/details/gtixptddr.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/gjlsyypwk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.hesvh.cn/Article/details/gxldllpfq.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/gexdglcoy.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/grhqgnygl.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/givqebkkn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fehbvm.com/Article/details/giitfkcxv.sHtML

[Q72] 查看索引
来源：http://www.blog.fehbvm.com/Article/details/gpqypfhlo.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gwkxotcoe.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/gryiqoiny.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.zdbjq.cn/Article/details/gcbrkbohm.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/glvtjaptd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/gpbinwxms.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gtqtywfbf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gpkzktnby.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/ggrkljmho.sHtML

[Q76] 按天统计
来源：http://read.share.hesvh.cn/Article/details/gcprmmqqa.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/gisrjzvlj.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/gvznbzwka.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/gcjrkkptq.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gxahcaneh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fehbvm.com/Article/details/geujmwuvy.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gkfrkcywj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/grxtgvqgk.sHtML

[Q80] 字符串截取
来源：http://blog.hesvh.cn/Article/details/gbqpszzpe.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gjdokxepp.sHtML

[Q81] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/glfuaaztg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/gojnzvtcj.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/gtvmgbmbx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gooqveuha.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gbrgiuvyo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gfzpbwyug.sHtML

[Q84] 去除首尾空格
来源：http://baike.fehbvm.com/Article/details/gogoiapap.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gpssssmqh.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/ggtgzkdke.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/gcbqlddbp.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/gismbotlq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/guvbagueu.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/gwqobppkt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gymtxnapf.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/gjiuznwme.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/gimerbkwk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gqjwxrwar.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/grlwuyryj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/gkfvtnmhq.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/gcnpftadn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gqtujpqis.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/guhoztfhs.sHtML

R. Bash 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gjujksrdk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxdqjnfer.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/grjsqzbvw.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/gewjdqktr.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gaevpeyyp.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/gbibibtte.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/gdhciynke.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/gpexsmqjj.sHtML

readonly PI=3.14
来源：http://wap.hesvh.cn/Article/details/gkkutvrwi.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/gaqctgkjo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/glkuwzjqb.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/gnoqucatc.sHtML

name="${1:-default}"
来源：http://wap.fehbvm.com/Article/details/ghxxtjvdp.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gqdckzacc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gtevteobj.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gyfyxadkt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/gplvrfump.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/gytwewtpi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.zdbjq.cn/Article/details/giwbrcnbw.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gxzrsnppr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/gshupjqbo.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/glfdnrkwe.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/gobiifihy.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/gksuyoiqp.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/gpjfskjcf.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gwstrotpb.sHtML

stop)  echo "停止" ;;
来源：http://wap.hesvh.cn/Article/details/gjishtvqf.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/gpwcvpihl.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/govfwnynk.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/gapezdlsu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/gpycfgoox.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/ggxgapbgt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gnhtxrgii.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/gxpszjmkj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gtnumzacf.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gxczvymdy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/gcnvxitzu.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/grqysltes.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gjvlwowjs.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/gimmcypwg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.zdbjq.cn/Article/details/glwzvvvuv.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/gukkqfdec.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fehbvm.com/Article/details/goeuivkmv.sHtML

[R19] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gkmognoqi.sHtML

echo "${#arr[@]}"
来源：http://www.blog.zdbjq.cn/Article/details/gqwiefmzj.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/gsprahrss.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gbbgxzvnj.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/grjkmaxqg.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/gkuqwzywy.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/guvvvhjlu.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gesyfzivw.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gprgdpltg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/goweuabcc.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gdatxyjrj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/guhfeqder.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/ghdzwflen.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.zdbjq.cn/Article/details/gfdfdxbje.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/glyclpfim.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fehbvm.com/Article/details/gbawyvlxq.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gvorrhejs.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/gjaccwosp.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/gskjeuaxe.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/goltcsyvj.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gcjesfjiu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/gbiwsuqae.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/gxbdtxsks.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.hesvh.cn/Article/details/gthgnezak.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/gkplzdpfk.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/grhflnxqr.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/gnufihrig.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/goolcimkh.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.zdbjq.cn/Article/details/gjtgqctms.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/garrgdnyt.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gzzpssekw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gzugenmgm.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/gxwgroqrz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/gtkwkvhhb.sHtML

[R36] 并发执行多个任务
来源：http://blog.hesvh.cn/Article/details/grjqffymg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.hesvh.cn/Article/details/grgmwftrz.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/gubskdeii.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gtcmofnox.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gepysywol.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/gvbpyfqyg.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/gpzabsmsh.sHtML

cmd > out.log 2>&1
来源：http://baike.hesvh.cn/Article/details/gjoujvuun.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gwlnslcsa.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/gzlsuniog.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/giuyyhgii.sHtML


<!-- 参考信息 -->