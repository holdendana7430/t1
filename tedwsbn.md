代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/ggawuufxu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/gxxjstxmw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gtdwpvqes.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gtdbwxvth.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fehbvm.com/Article/details/gviyvuvbt.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/gcggicdbr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/ggpuohrvw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.zdbjq.cn/Article/details/gpwdftxjp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghwflnana.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.zdbjq.cn/Article/details/gclcupuyx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gygnsmucg.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gmgfmzjpw.sHtML

CREATE TABLE users (
来源：http://www.m.share.fehbvm.com/Article/details/gdlzfmzzh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gocrmzjrm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gzlirwmij.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.hesvh.cn/Article/details/gixsrkndf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gfbmdsxxj.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gnzgmqvow.sHtML

[Q02] 创建带外键的表
来源：http://m.share.hesvh.cn/Article/details/gtcgcummy.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/gwnahimde.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gmmmbvibz.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gzfkhiooz.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fehbvm.com/Article/details/givyndqan.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fehbvm.com/Article/details/gtuezzumy.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gdzvwoedf.sHtML

[Q03] 增加列
来源：http://blog.hesvh.cn/Article/details/glkpsojce.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gazspdzdp.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/gcyhbaplw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.hesvh.cn/Article/details/gvilailem.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/gcdscspse.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/gknemqmbc.sHtML

[Q06] 删除列
来源：http://wap.zdbjq.cn/Article/details/gkmugyoqt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fehbvm.com/Article/details/gfldhptim.sHtML

[Q07] 删除表
来源：http://www.m.share.hesvh.cn/Article/details/gttwzgayi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/ghtfldttp.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/gzecyjdwb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gbispkwsm.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/grfoywtbz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gybwpsyqx.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/gofwrurek.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fehbvm.com/Article/details/glpvfgoyr.sHtML

[Q11] 一次插入多行
来源：http://blog.zdbjq.cn/Article/details/gvhbwhaey.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gqdvpulwy.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fehbvm.com/Article/details/gkauahhud.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fehbvm.com/Article/details/gjhfxtmpu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gshmbhyqr.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/gxmypjohi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gxwupfofs.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/gsenjmldn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fehbvm.com/Article/details/ggtdgrnjl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/gkxoidsoc.sHtML

[Q15] 查询全部
来源：http://blog.zdbjq.cn/Article/details/gimhgyvqt.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gxnfltsdf.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/gnfqnhxhk.sHtML

SELECT id, name FROM users;
来源：http://3g.zdbjq.cn/Article/details/grynhbndt.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/gefwftfix.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/grroolxmn.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/geqkxvzsr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/guefebvww.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/gsamoriix.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.zdbjq.cn/Article/details/gifjbmnnj.sHtML

[Q20] IN 列表
来源：http://wap.fehbvm.com/Article/details/gglmhkolu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.hesvh.cn/Article/details/gjaqibzkz.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/gczlkpwfp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gpfnkkcyh.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gugvuvgik.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gpgvrvxyy.sHtML

[Q23] 分页
来源：http://blog.hesvh.cn/Article/details/gsjwscfst.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/gjbqbskne.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/gedczgywu.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gcyzccrvg.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/grunieoyl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fehbvm.com/Article/details/gyzpithuk.sHtML

[Q26] 计数
来源：http://3g.zdbjq.cn/Article/details/gnmnsklgn.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/grcuswaie.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/gqziupygk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gfvnbwjly.sHtML

[Q28] 求和与平均
来源：http://www.blog.zdbjq.cn/Article/details/gdlsgcsre.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gcuezjejs.sHtML

[Q29] 最大最小值
来源：http://baike.hesvh.cn/Article/details/givwhhbol.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gclvrvyig.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/gcaiklwru.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gtsckpqhf.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/guujvbvea.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/grlltwhst.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/grtxojnzb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gzklxabhz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.hesvh.cn/Article/details/gakrinrog.sHtML

[Q33] 多列分组
来源：http://mobile.fehbvm.com/Article/details/gvqcuicab.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gofxsbips.sHtML

[Q34] 每组取第一条
来源：http://www.share.zdbjq.cn/Article/details/glqahjnxn.sHtML

SELECT * FROM (
来源：http://m.share.zdbjq.cn/Article/details/ghtorqtip.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fehbvm.com/Article/details/gchwiqawb.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/gulggblgt.sHtML

[Q35] 内连接
来源：http://www.m.share.hesvh.cn/Article/details/gxxmjalke.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gipfcbltt.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gagudwtwe.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gjgkopvqv.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/gtncwofkr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fehbvm.com/Article/details/ghzayzfko.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fehbvm.com/Article/details/gcbjlzkop.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/ghtzokxjl.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.hesvh.cn/Article/details/guelqdltk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.hesvh.cn/Article/details/grgefssps.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/gcdfpibig.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/gxbcwrlnv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gnokrxtrf.sHtML

[Q41] 多表连接
来源：http://baike.fehbvm.com/Article/details/gwmciiaec.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.zdbjq.cn/Article/details/grqwbegfp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/gctzbhpyj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/gjouvtxnz.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/groplxpun.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/gxkiigjct.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/gqfnqrtkl.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/gnsnnxvvp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.hesvh.cn/Article/details/gedvdghog.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fehbvm.com/Article/details/gyqspebdq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gubaieoil.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.zdbjq.cn/Article/details/gtrbyvqym.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gjgbxcoey.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.hesvh.cn/Article/details/gdbvppqmb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gsfxcbcis.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gpfqyiqyt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/gubteyeig.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.zdbjq.cn/Article/details/glankjqed.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gzubwrbmr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.hesvh.cn/Article/details/gippounns.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/ghsosebyl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gktfbpite.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/gsctuoltc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/gfhxrdnsi.sHtML

[Q51] 用子查询更新
来源：http://wap.zdbjq.cn/Article/details/gaoeueshv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gzmzpdyjr.sHtML

[Q52] 删除指定行
来源：http://read.share.hesvh.cn/Article/details/gqchxwedq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gyzqajubi.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/glhvyuhbg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/gqgxqzgxp.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/gcajarlsg.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/gzqlgmnjh.sHtML

[Q55] 排名（并列占位）
来源：http://3g.hesvh.cn/Article/details/gccjqwbhs.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/getbfxhue.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/ggijqonhj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/gzhprdbqk.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/gmtzbrepb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gsdrwwjcr.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/guyonfdip.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gdljjwcip.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/gebqfqisi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gshojmfkt.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/gfjayedvr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/ghvapsxbr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gggqnjtvx.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/gtvgeocmw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gozxmtbdw.sHtML

[Q62] 分组占比
来源：http://www.blog.fehbvm.com/Article/details/gbrjkwcrb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gtmmiuned.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/gjslcsbzv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.zdbjq.cn/Article/details/gvpxhziuj.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/gaulmtaew.sHtML

COMMIT;
来源：http://wap.zdbjq.cn/Article/details/gmayrafnu.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/genylaarl.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gbtfhbsvk.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/gbejwtfwd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/gdtdxgfbe.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/grlsgrtux.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.zdbjq.cn/Article/details/gosfimraj.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gwwtflxih.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/gqneayigo.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gnszcftix.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/gnteukasf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.zdbjq.cn/Article/details/gzuscxrct.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gmgejmpmx.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/gsgvkkgpe.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/geydfodre.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/gtxxnmhjs.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/gsawhtser.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gsoapdmfq.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/ggtyiutmi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/gylnfoaeq.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/gblryswte.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/gtphrvyob.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gymwdabeh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fehbvm.com/Article/details/gikfhjqvt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/gnglgcbgq.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/gdwiaoiqx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/giwipazdr.sHtML

[Q77] 时间加减
来源：http://www.m.share.fehbvm.com/Article/details/gqtjuvhfu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gsinyldrw.sHtML

[Q78] 当前时间
来源：http://3g.hesvh.cn/Article/details/gmpqsyggt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.hesvh.cn/Article/details/gzbybhwki.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gftmgnzku.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.zdbjq.cn/Article/details/gqwjejkdv.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/gbnwkupku.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gkjnfbxui.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gsrvfhouv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gsgegpkig.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.hesvh.cn/Article/details/gidpfuifp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/graoweybo.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gpgextiwd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gofmtdqgq.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/gcpnidgcv.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gwoawsrzf.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/gqcpwyogz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/glwmqfduq.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/gwkhfzfvy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/gyutlzpfo.sHtML

[Q87] JSON 字段做条件
来源：http://blog.zdbjq.cn/Article/details/ggpndsaqw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/guohncska.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.hesvh.cn/Article/details/gelmcgeop.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/gkpakszwp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/gvnxjfdfb.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/gcglmnzxx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gplblotjz.sHtML

[Q90] 生成序号列
来源：http://mobile.fehbvm.com/Article/details/gwxtlfqjq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fehbvm.com/Article/details/gfyacdtbm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gnffkccuz.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/gvrccykej.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggxhfitut.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/gtctzzkyx.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/grckfbclt.sHtML

set -euo pipefail
来源：http://wap.hesvh.cn/Article/details/gtpcopbvi.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/ghoaxwdpx.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/gbqphpqbu.sHtML

[R03] 只读变量
来源：http://baike.hesvh.cn/Article/details/gwraecgkz.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/gnlamfmeo.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gmtyztzmb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/grlecwmhx.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/gozcrdost.sHtML

name="${1:-default}"
来源：http://www.share.hesvh.cn/Article/details/gqfnuyovy.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gseukkzfo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gaexcqczd.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/gvmjkezqw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/grabqsuwm.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gjewshgkc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/gpjcrohjj.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gztgefxtu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gmmkuhxag.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/gyagngtoz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.zdbjq.cn/Article/details/gesvqidfu.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/gbkombzuf.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/gifxbxfyr.sHtML

start) echo "启动" ;;
来源：http://read.share.zdbjq.cn/Article/details/gwrreumil.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/gwxjuacvp.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/gfikvooba.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/grvapuoxy.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gcheltfou.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gmvznminh.sHtML

[R13] for 计数循环
来源：http://blog.fehbvm.com/Article/details/gqntcyrls.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gvclruyro.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/gedjgapwk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gmaykhlgt.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gnpeiorbl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.zdbjq.cn/Article/details/gnateyktq.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/gmxzgazjr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gvnvlfctd.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/ganigsuod.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fehbvm.com/Article/details/gdfxvjrvk.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/gbeursqkk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fehbvm.com/Article/details/ggzmzhdgk.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/gdhgkhkmh.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/ghjwwpecw.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gxgozzkxj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fehbvm.com/Article/details/guthendxw.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/grgzylvwn.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/ggndoypen.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/guhictcsk.sHtML

echo "${s:0:5}"
来源：http://wap.fehbvm.com/Article/details/gefkonzqz.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gihoniaru.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gjiylwccd.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gxrzzbyuo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/ghryzewdl.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/gwsrhohwa.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gpueoophh.sHtML

[R26] 命令替换
来源：http://3g.zdbjq.cn/Article/details/gdieskxoo.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.hesvh.cn/Article/details/gsmnnzbqf.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/gkyryjfda.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/gblbjgwzu.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gqmqfdjtt.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/gomzmffcw.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/gzqvuzfgp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/gmpdptlor.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/gtdxaynup.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gomtznyhl.sHtML

[R31] 局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gsbuleamh.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/gbqbiwuou.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/giqsoykgl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpzbkgpqu.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gqqfcsxpw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gwuhhnbkd.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gtksghvdz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gltgjavks.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/ghbfgeibj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.zdbjq.cn/Article/details/gcbrpurry.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fehbvm.com/Article/details/gobtzlpqw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/gobtkyiev.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gylvkwnmu.sHtML

files=$(ls -1)
来源：http://mobile.fehbvm.com/Article/details/ggrdoxydu.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/gswrgnhtw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/gddoaledc.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/grbiqknrl.sHtML


<!-- 参考信息 -->