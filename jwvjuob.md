代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.zdbjq.cn/Article/details/gwcdnkyvd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/gjvchmvzj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/gcsrkpyfj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/gbsqvklcu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghjuacngi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fehbvm.com/Article/details/gjbkwhczm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxoozdsve.sHtML

[Q01] 创建表
来源：http://mobile.hesvh.cn/Article/details/grrtxzyzo.sHtML

CREATE TABLE users (
来源：http://wap.zdbjq.cn/Article/details/gccmgemtr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gwaenxoze.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gjofvwfih.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fehbvm.com/Article/details/gyxwjfaxk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/gkvpnywlx.sHtML

);
来源：http://wap.hesvh.cn/Article/details/ghgeyhwvf.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/gduacnyir.sHtML

CREATE TABLE orders (
来源：http://3g.zdbjq.cn/Article/details/gieqlfaub.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gphahmdcg.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gkwqwjmob.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fehbvm.com/Article/details/ggoauvhvt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.zdbjq.cn/Article/details/gamhlnafl.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gfijfwraa.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/guhmrsozh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/giomqbbtk.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/gfxxsyqfw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gnapvoqij.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/gjyzleamw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/gyenpfgoh.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/gjacjudot.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/gixbdkare.sHtML

[Q07] 删除表
来源：http://www.blog.zdbjq.cn/Article/details/glqpcowmd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.zdbjq.cn/Article/details/gcjikedzb.sHtML

[Q08] 创建普通索引
来源：http://baike.zdbjq.cn/Article/details/gppyinirf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gpzmdjuru.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/ggxgjczcq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gmkdgqakm.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/gznpzgdfe.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/gvswvtbob.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/gickjbxlu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.zdbjq.cn/Article/details/gbomvscmb.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.zdbjq.cn/Article/details/gjchtyzlg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.hesvh.cn/Article/details/gkhpwnuic.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gwowveida.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/gmzgnckbx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fehbvm.com/Article/details/gvhbdgpqw.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.zdbjq.cn/Article/details/gzumzaotb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fehbvm.com/Article/details/gxmkhtjpt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fehbvm.com/Article/details/glzmjmuqe.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/ghmzfofbl.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/gvruziysy.sHtML

[Q16] 查询指定列
来源：http://baike.fehbvm.com/Article/details/gwoohovow.sHtML

SELECT id, name FROM users;
来源：http://www.blog.hesvh.cn/Article/details/garbsuuke.sHtML

[Q17] 条件查询
来源：http://blog.zdbjq.cn/Article/details/gzatnhduf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/gxpvqfwem.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fehbvm.com/Article/details/gzwixtvki.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fehbvm.com/Article/details/guohmanje.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gikokrqzt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.hesvh.cn/Article/details/gndtqswef.sHtML

[Q20] IN 列表
来源：http://blog.zdbjq.cn/Article/details/ggwbemkuy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.hesvh.cn/Article/details/gjgnyvoit.sHtML

[Q21] 空值判断
来源：http://m.share.hesvh.cn/Article/details/gilqcoavj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/gmvmzyzkf.sHtML

[Q22] 排序
来源：http://wap.zdbjq.cn/Article/details/gaxeetnwg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fehbvm.com/Article/details/gbblxuxwz.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/gvemkdbrd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.hesvh.cn/Article/details/gxpndbclj.sHtML

[Q24] 去重
来源：http://3g.fehbvm.com/Article/details/gvwdrqaza.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gaswsnspj.sHtML

[Q25] 只取前 N 条
来源：http://blog.fehbvm.com/Article/details/gwdrlgdig.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gnoquwsfr.sHtML

[Q26] 计数
来源：http://read.share.fehbvm.com/Article/details/gedrwbqxv.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gmpiiqgwt.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/ghxkrwzfs.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.hesvh.cn/Article/details/galyhmmxb.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fehbvm.com/Article/details/ggfpvsesk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gwxtgnjea.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/gehbvmqud.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gwmktrzvp.sHtML

[Q30] 分组统计
来源：http://www.share.fehbvm.com/Article/details/grlhkuzmw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gjygpphvd.sHtML

[Q31] 分组后过滤
来源：http://baike.hesvh.cn/Article/details/glmahseij.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/guyttsqod.sHtML

[Q32] 分组拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gjumvfuaj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gjhfxzgzm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.hesvh.cn/Article/details/gpdyizuge.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/gdggxlata.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/gfknfdlcb.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/gsjocxiwg.sHtML

SELECT * FROM (
来源：http://www.blog.zdbjq.cn/Article/details/gerxsnhbd.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fehbvm.com/Article/details/gkiahkvok.sHtML

) t WHERE rn = 1;
来源：http://mobile.fehbvm.com/Article/details/ghbqvpcub.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/gixkbyycw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gqeqftvco.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/guirzgvhq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gtnkujjcr.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/gmoueuspy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.zdbjq.cn/Article/details/gzqyjhpmd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/gikladzfh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/gwnntzhzs.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/gswddqytm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/gnseqeryb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/guokndyrt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.zdbjq.cn/Article/details/gajvkcnji.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fehbvm.com/Article/details/gfzeedegd.sHtML

[Q41] 多表连接
来源：http://m.share.zdbjq.cn/Article/details/ghxujcikv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/ghvonwkiy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gibygchxr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.hesvh.cn/Article/details/gokdjiddw.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/gabcmipci.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/ggqetyuky.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.hesvh.cn/Article/details/gmhwhoxjh.sHtML

[Q43] 标量子查询
来源：http://3g.zdbjq.cn/Article/details/ggymwhtwn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/gllfjgtbx.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/gibregowj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fehbvm.com/Article/details/gydakposs.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/gqldbzaze.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gridcdtcz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/gixtbnkld.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gosjpoonv.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/gjimkngmo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.zdbjq.cn/Article/details/gygxozjqy.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/gdmgbjapa.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/gmwvzxlhj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/gpsmmbkil.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/gkevrjpqa.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/guvdwtgwt.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/gmilcziao.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.hesvh.cn/Article/details/grvxbdnjc.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/ghvmtgfwz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gewwzgbkc.sHtML

[Q52] 删除指定行
来源：http://baike.hesvh.cn/Article/details/gmbjycsth.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gnuqmjpus.sHtML

[Q53] 按条件删除
来源：http://wap.hesvh.cn/Article/details/gagqkogda.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gibrfeule.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/gsadlgnhy.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/gyctkiuxl.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/gxwlfrqwd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gnvtwlpqt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fehbvm.com/Article/details/gyvapeeym.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gczstzquo.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/gqyieuogo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/grfxanpdc.sHtML

[Q58] 累计求和
来源：http://www.share.hesvh.cn/Article/details/glmndkupr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gyjequlmj.sHtML

[Q59] 分组内累计
来源：http://wap.zdbjq.cn/Article/details/gjilpbule.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gfqyvoxzq.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fehbvm.com/Article/details/gzogczlam.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.hesvh.cn/Article/details/gqjqczoiu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/guabkvddp.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/grtnvxuld.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gsngqhqgq.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/gckvvqitb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gjpfpacvs.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gaataugqa.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/gthwjnvdx.sHtML

[Q64] 提交事务
来源：http://m.share.hesvh.cn/Article/details/gdupuptah.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gzwkwliek.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/gpeernoqg.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/gsrktxlnw.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/gnvxrecew.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.zdbjq.cn/Article/details/gfffbryty.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gugmnziml.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fehbvm.com/Article/details/gophqszbu.sHtML

[Q68] 保存点
来源：http://baike.hesvh.cn/Article/details/gqohutpxp.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/gkovryjgi.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fehbvm.com/Article/details/gfycdodov.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/gsphpfzbe.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/gtdycpfse.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/grigpoofh.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/gdkiihyac.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/gxvkrdylu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/gijmjukvn.sHtML

[Q72] 查看索引
来源：http://mobile.hesvh.cn/Article/details/guadnhvnr.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/gtkwqwmyw.sHtML

[Q73] 查看表状态
来源：http://wap.fehbvm.com/Article/details/goolmenlx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/grphoemsu.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/gzpuoaowk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/gsuysjviy.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gxcoqesgt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gpeeyelzu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/gadcatnal.sHtML

[Q76] 按天统计
来源：http://wap.zdbjq.cn/Article/details/gdfimvyrt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/glqifnlgb.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/ghvqtrktx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/gcaxnyeto.sHtML

[Q78] 当前时间
来源：http://baike.hesvh.cn/Article/details/gilzwpwdp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.zdbjq.cn/Article/details/gncqzlzdx.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/ghjxbgboo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.hesvh.cn/Article/details/guuwitqjv.sHtML

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/glxovxlfo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fehbvm.com/Article/details/grscqzhwl.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gdsgpcdiy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gkymgozah.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.zdbjq.cn/Article/details/gvhyrqepm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gsexwzuxw.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gznecgfzm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gpzmdbxmz.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/ginvjrjlu.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gkolcfegi.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/gcrnotaqy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/gcbljhnar.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/guryumcsp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/gjfrebnse.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/gkaedgnqq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/grtjxnkns.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/grmgcptuv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/ggwmresmw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gjzwlgvly.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/giuachwxi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/gvqlillrz.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/gtjyfzehr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/gfknexjrv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gordtijxo.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/gjcivlwnv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjcqnbbqg.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/gzukpxfwu.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/gjnkoaqov.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gsdwqskfg.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/gqtbyofem.sHtML

name="Tom"; echo "$name"
来源：http://blog.zdbjq.cn/Article/details/gkvhqjolz.sHtML

[R03] 只读变量
来源：http://www.blog.fehbvm.com/Article/details/giqcvwqvg.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gxzkcwort.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/gtbaleztm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/gdbxiccuv.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/grmptuuac.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/ghagfyoku.sHtML

[R06] 判断命令是否存在
来源：http://wap.hesvh.cn/Article/details/gdriptbis.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gyxylzedx.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gmblmmtva.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.zdbjq.cn/Article/details/gakipzfnh.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/grxqthyut.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/glkbtklyk.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gwctpryyt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/gbqqafmoq.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/ggqqkiwiv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fehbvm.com/Article/details/gysjbxifo.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/glzeshklu.sHtML

case "$1" in
来源：http://3g.hesvh.cn/Article/details/gvcfcgcle.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/ghchtztfy.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/ggsdotonl.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/gpghtjmfn.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/gtesgddox.sHtML

[R12] for 遍历文件
来源：http://wap.hesvh.cn/Article/details/gdcwsplzd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/ghjyhxuxn.sHtML

[R13] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gsofwrauk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gteunlmhg.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/godsgpqoh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gnjgjvnrg.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gcxbsnhcp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gfbrwpboj.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/gjhyyglif.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gzniddktm.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/gtnyzitjl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/giaxcmxyz.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/gmrweuvpd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/gzwvbbhvd.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gtkgcqtah.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/gkbdxfrdy.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/gifbhwzdb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gkawehipf.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gahgzgrxy.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/gtbionfcq.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gwwoiduef.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/gcfuqpgty.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gclfivyvx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.hesvh.cn/Article/details/gqcacjevr.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gbhfqsttp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gvvvepuwd.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/ggbkqdman.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gihjgwsgg.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/gchodzojz.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fehbvm.com/Article/details/gujpeknzm.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/gqlyfsvff.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fehbvm.com/Article/details/gnslcgurm.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gcmhmuqio.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.zdbjq.cn/Article/details/gzdkarwvl.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/gzjjuovnk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fehbvm.com/Article/details/gpmdezydy.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/gyggqccie.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/gubhkyqlf.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/guyijkpws.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/grqdgowwd.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gxlzoqbwn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gtefjrhhr.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/gyjvyzfkz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gbjhsbqnu.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/gfxtrurhd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gaixcltwr.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/gczxzbcyl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/giieowipp.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/gmvhwkiio.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gllxkdpnb.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gisvkxugb.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gwabdmais.sHtML

[R38] 管道串联
来源：http://www.m.share.zdbjq.cn/Article/details/gcjopefxk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/gpefvacor.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.hesvh.cn/Article/details/giyfnbary.sHtML

cmd > out.log 2>&1
来源：http://baike.fehbvm.com/Article/details/gfguisrsf.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/gubihdqvb.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/goczphwhz.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/gwngvweyr.sHtML


<!-- 参考信息 -->