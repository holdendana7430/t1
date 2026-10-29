代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.hesvh.cn/Article/details/gngencxcv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gyvpivkib.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/ghcgffkib.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/geelwatvo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/ggecwhcti.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.zdbjq.cn/Article/details/ggtpdcxkz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/ghstgtyql.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fehbvm.com/Article/details/gsebonsid.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glvfghaht.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fehbvm.com/Article/details/ghrilzjeq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfordromk.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gtptwnmnk.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/grtajqfdh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/givjwiwrv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gcmpeifgo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/gucbkfjmh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/gkrukxijz.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gtfotjvdg.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gzufvhnjb.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/ggncvnxau.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gvwboqxya.sHtML

user_id INT NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gfopqnavg.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fehbvm.com/Article/details/gickxqicu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fehbvm.com/Article/details/giqhxrknh.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gnhyfapsj.sHtML

[Q03] 增加列
来源：http://www.blog.fehbvm.com/Article/details/gsbelatie.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/gsukouael.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/grnqmrrud.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.hesvh.cn/Article/details/gypgvrmbv.sHtML

[Q05] 重命名列
来源：http://m.share.hesvh.cn/Article/details/gbeuxnihg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/giwxhejtc.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/gwslrynou.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.hesvh.cn/Article/details/gjequtmuq.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/gcahapswo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/ggiqwuzqn.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/gpkrpdvpt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gughcmfpq.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fehbvm.com/Article/details/gobvgozov.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gmqzrzjdn.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/gvcnewyfe.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gidqronsr.sHtML

[Q11] 一次插入多行
来源：http://www.share.zdbjq.cn/Article/details/gzpzrmeyz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.zdbjq.cn/Article/details/gwxoctqnn.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/gjcnwavas.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fehbvm.com/Article/details/gbpwsgiqt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.hesvh.cn/Article/details/gwboatjrs.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gwhldwxfq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/glccqkkxa.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gyyndqjgz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/gmvndabag.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.hesvh.cn/Article/details/givcglmus.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/ggsmrksxy.sHtML

SELECT * FROM users;
来源：http://3g.fehbvm.com/Article/details/gbwizclhb.sHtML

[Q16] 查询指定列
来源：http://www.m.share.hesvh.cn/Article/details/gkcqxeqfc.sHtML

SELECT id, name FROM users;
来源：http://3g.hesvh.cn/Article/details/gwzplefgz.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/ghsgmknnl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/gcdnnfkml.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/glpfalphh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/godssiroh.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/gugkokayz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gucixlejf.sHtML

[Q20] IN 列表
来源：http://www.share.hesvh.cn/Article/details/gnogouddl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/gbkqipraf.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/gatdujhgu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/ghyhzqzxl.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/gbmdulkxx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/gmsfkdovz.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/gqqorqzrz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/gsqeefzhu.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/gofgrdwxq.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fehbvm.com/Article/details/gqvysyles.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gxnrvoghg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.zdbjq.cn/Article/details/gdqonqugs.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/gknkpsdvp.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gddcqbekq.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/gqqzuloef.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gfwliqyvj.sHtML

[Q28] 求和与平均
来源：http://blog.fehbvm.com/Article/details/ggseszhhs.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gxjnzialp.sHtML

[Q29] 最大最小值
来源：http://baike.fehbvm.com/Article/details/gswruglme.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/ggqffrgif.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/gxpmbhrlo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gfqpmoizf.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/gsaxcdfal.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/gxqpduhmq.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gdcobtsto.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gkzphfmtd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fehbvm.com/Article/details/gqdcpnote.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/govcklprv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.hesvh.cn/Article/details/giyvlhogu.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/ggmdbfxnf.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/gwdkargde.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.hesvh.cn/Article/details/ggrxbjpon.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/ggygdthgm.sHtML

[Q35] 内连接
来源：http://mobile.zdbjq.cn/Article/details/gcdfsekdd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gbxuskbvl.sHtML

[Q36] 左连接
来源：http://blog.zdbjq.cn/Article/details/gpvdqqlqg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/ganvsqkqf.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gkjjexkvb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.zdbjq.cn/Article/details/ggvthnlar.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/gfsbtrzxg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.zdbjq.cn/Article/details/gdgirxiws.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/glepdatvd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gueutjjia.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.hesvh.cn/Article/details/gwctxehzh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/gjymjiowy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/gyjiiqbkb.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/gfropugvg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.zdbjq.cn/Article/details/gzczzoene.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gqnldzsnn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/ghdthouhb.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.zdbjq.cn/Article/details/gjfwjcoqj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fehbvm.com/Article/details/gknzdnwfi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.hesvh.cn/Article/details/gbcbshqvl.sHtML

[Q43] 标量子查询
来源：http://m.share.hesvh.cn/Article/details/gnennzlqt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.hesvh.cn/Article/details/gkphluyxa.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/grjijrrkf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.hesvh.cn/Article/details/gfvykowyh.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/gykbeldly.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/ggdsrrzjy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gibzemucu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gklzjfmup.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/gbgrxwgja.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fehbvm.com/Article/details/gsxssxqao.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gjeqwptuu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/ghjsalqab.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/gdbnrgnqf.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/gsarxvsxq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/ggfjuvcyp.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/gijnrzwcg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gacwprqwp.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/ghrjcvzlj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/gkjwkknqz.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/gtspaymxp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gexkywbzq.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/gcphqgzzp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.hesvh.cn/Article/details/gyvaqekqu.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/gybystgbc.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fehbvm.com/Article/details/gbhmmjckn.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gzmrqfsur.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gfgedzpeu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/gjrvlmnzr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gvjffrzly.sHtML

[Q57] 行号
来源：http://read.share.fehbvm.com/Article/details/grkicpfyp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gnuqbdohz.sHtML

[Q58] 累计求和
来源：http://wap.hesvh.cn/Article/details/glnzconbh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/glxkduatw.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/gdhkiaawo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gklbhuglt.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/ghagoflqw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.hesvh.cn/Article/details/gordhiyug.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gcwjbcfga.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/gxdfxxfxv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gdbjnjlmu.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/goujgyhoa.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/goxejilsb.sHtML

[Q63] 开启事务
来源：http://read.share.hesvh.cn/Article/details/gsoaodgib.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gyqsujqfe.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/ghimdrztb.sHtML

COMMIT;
来源：http://wap.zdbjq.cn/Article/details/gsjcrwfgb.sHtML

[Q65] 回滚事务
来源：http://baike.fehbvm.com/Article/details/gqaoykdsf.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/gvzysvccj.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/gqtfqwrys.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/gxfjjvaxa.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/gkvxvftsp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gxpgsxpkt.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/gwoqtocxc.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/gtgstpxrh.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gkjzrbpdw.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/gswapaoeq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.hesvh.cn/Article/details/gjddvzpmp.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/glgxervrp.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/gwakressu.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/glkjsjodo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/goffkklij.sHtML

[Q72] 查看索引
来源：http://www.m.share.zdbjq.cn/Article/details/ghnmruelv.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gdvojypqg.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/gwnmomypt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/goebezita.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.zdbjq.cn/Article/details/gishhutca.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.hesvh.cn/Article/details/gavhcbedc.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gadhfclxk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/gsuqlihjf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.zdbjq.cn/Article/details/grvmlbysi.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/gyfgkavfe.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gaicicicc.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/gvvkrahgj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/gaijbhvyu.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/gmidfxzzr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/gayxyunvz.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/glnjanvrc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/gnboeakhk.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/gdbealniu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gnzutneha.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gfhildxen.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/ghlyklrac.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/gyrxbziwf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gzgmfieii.sHtML

[Q83] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gvsfoxpsf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gfaptpbuw.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gjbtmqrdl.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gnmqkvyme.sHtML

[Q85] 数值取整
来源：http://www.blog.fehbvm.com/Article/details/gyiyukgey.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/gntlsjzyx.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/gsdkwsiim.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fehbvm.com/Article/details/gcogowvjr.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/gigptmsmr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gnofbzyto.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gxbyyrglo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/gallhxolt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gaqahicmj.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/gvmlimofl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/gpvehaqsv.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/gcguowzsi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/gtfhxgeuz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gepmpsmqu.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gilwakpjr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzvzecoek.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/geiccsviw.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/ggbcmixaa.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gvxomvgsn.sHtML

[R02] 变量赋值与使用
来源：http://wap.fehbvm.com/Article/details/gnhkmckcn.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/gvjesluha.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/gesmvmuxs.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gsjdnvhwy.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/gweqpeuwq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.hesvh.cn/Article/details/gtnifzktm.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gipntfivk.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gsbcqbdhd.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gqyqruava.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gaaigqdvp.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/glqlwgclr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gxiqegjwu.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/gbsuckeeu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/goqxlubmq.sHtML

[R09] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gynqpnman.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/gofrpwmks.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/gsdsucatv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/gnrsaidke.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/gzvhhdzyn.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/gjlltcztp.sHtML

start) echo "启动" ;;
来源：http://mobile.hesvh.cn/Article/details/gaegenlxn.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/gavdlbucc.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/glprkblyl.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/gfoglrbbn.sHtML

[R12] for 遍历文件
来源：http://wap.fehbvm.com/Article/details/gchuelytl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/gmuifjngf.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gizpnqoma.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gllxxmirk.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/gcopplkow.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/ggnodjgea.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/goodpjvnm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/glurcibij.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/geiexkytd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gvgahrcmy.sHtML

[R17] 数组定义与取值
来源：http://www.share.zdbjq.cn/Article/details/gkenrkywo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/gdzyidrqp.sHtML

[R18] 遍历数组
来源：http://3g.fehbvm.com/Article/details/gzarsorpb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/gaeqjknpd.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gjuxclubb.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gsrvkndkm.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/gvrwpznrq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/giegppglv.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gzsrzsyxs.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gxjbhxwvl.sHtML

[R22] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gtwpolaai.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/gbhkzzomi.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gvcoqehgp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/gdfhrqdbv.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gfrdtceng.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/gdtbvxpid.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/gjewfejsw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/ghruyscll.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/gzzxmhzzi.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/glqmoefei.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/ggmrqjqaw.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/gmhtxcait.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/gwxcstvwe.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/gostchjky.sHtML

[R29] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/gclzvwbos.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fehbvm.com/Article/details/gilyuahqn.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/geyzwqovq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gcrlakkkw.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/grjxnlpuv.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gzntfwqxo.sHtML

[R32] 参数个数校验
来源：http://wap.zdbjq.cn/Article/details/gkjzxmtww.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gcisnmxoh.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.hesvh.cn/Article/details/gpwpdjdhn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/gmlolszoo.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/gganedupm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gbndodjoe.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gdlitntmu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gzqygqgpn.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/gcrxeyeri.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/gkfdxfrxx.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/geowoicof.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/gpjkagbbp.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/ghqdmqzqv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/gazrbwmsp.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gtgvdnrzh.sHtML


<!-- 参考信息 -->