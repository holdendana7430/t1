代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlmvlcbu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gabctrezi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fanxiaobao.xyz/Article/details/glrusekdh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fanxiaobao.xyz/Article/details/goodlhnqw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fanxiaobao.xyz/Article/details/gyayvmmsh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtcktfqp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glggyojta.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwtilylo.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gttncfmgt.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkubpopo.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gbimpaeoj.sHtML

[Q01] 创建表
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrkqbfwg.sHtML

CREATE TABLE users (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmoxdswy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fanxiaobao.xyz/Article/details/gpzueckjl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrxmeuwv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fanxiaobao.xyz/Article/details/gkiepceon.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzymtdep.sHtML

);
来源：http://wap.fanxiaobao.xyz/Article/details/gwepkszpz.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjazfqqrf.sHtML

CREATE TABLE orders (
来源：http://read.share.fanxiaobao.xyz/Article/details/goombjqib.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fanxiaobao.xyz/Article/details/guzwfztjm.sHtML

user_id INT NOT NULL,
来源：http://wap.fanxiaobao.xyz/Article/details/gaappxhxq.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fanxiaobao.xyz/Article/details/ghktsmbtz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fanxiaobao.xyz/Article/details/ghtyzbsdp.sHtML

);
来源：http://3g.fanxiaobao.xyz/Article/details/gxequalov.sHtML

[Q03] 增加列
来源：http://wap.fanxiaobao.xyz/Article/details/glqjrambx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gbrdsruti.sHtML

[Q04] 修改列类型
来源：http://3g.fanxiaobao.xyz/Article/details/gxozhuwgj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxyubvvg.sHtML

[Q05] 重命名列
来源：http://wap.fanxiaobao.xyz/Article/details/gfgfbvfjd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgwpcxwh.sHtML

[Q06] 删除列
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyszwzyf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvusbsvig.sHtML

[Q07] 删除表
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkqzldin.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fanxiaobao.xyz/Article/details/glcflzcad.sHtML

[Q08] 创建普通索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzmqjnia.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fanxiaobao.xyz/Article/details/gobuonton.sHtML

[Q09] 创建唯一索引
来源：http://baike.fanxiaobao.xyz/Article/details/giimbxofg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fanxiaobao.xyz/Article/details/guxemxdxa.sHtML

[Q10] 插入单行
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzusxpsx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gftgsvbxk.sHtML

[Q11] 一次插入多行
来源：http://baike.fanxiaobao.xyz/Article/details/guzrenwaw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpuhnpbv.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fanxiaobao.xyz/Article/details/guvzcxazh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fanxiaobao.xyz/Article/details/gftuzsuzi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlyqlmkj.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqxoajgv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlmekiiy.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkyjtuvu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fanxiaobao.xyz/Article/details/gjbcsgayr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzfvopdb.sHtML

[Q15] 查询全部
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrqktxal.sHtML

SELECT * FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/grsyequej.sHtML

[Q16] 查询指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/glnpgzjrq.sHtML

SELECT id, name FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzotqnqpj.sHtML

[Q17] 条件查询
来源：http://blog.fanxiaobao.xyz/Article/details/gspccaset.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gmynnjwlr.sHtML

[Q18] 模糊匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gsuqacpqc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fanxiaobao.xyz/Article/details/gojjeqjpn.sHtML

[Q19] 范围查询
来源：http://3g.fanxiaobao.xyz/Article/details/gkndtfgyk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswtpkdkh.sHtML

[Q20] IN 列表
来源：http://3g.fanxiaobao.xyz/Article/details/gspxlgras.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gwuzssamc.sHtML

[Q21] 空值判断
来源：http://baike.fanxiaobao.xyz/Article/details/gtxremouu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxcbcgxa.sHtML

[Q22] 排序
来源：http://blog.fanxiaobao.xyz/Article/details/gpziztzzs.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fanxiaobao.xyz/Article/details/gdlhlgaqo.sHtML

[Q23] 分页
来源：http://m.share.fanxiaobao.xyz/Article/details/gseihmarp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdavgjsxx.sHtML

[Q24] 去重
来源：http://mobile.fanxiaobao.xyz/Article/details/gxapoptqe.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gmgsobeql.sHtML

[Q25] 只取前 N 条
来源：http://baike.fanxiaobao.xyz/Article/details/ghyhozbux.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqnfdvii.sHtML

[Q26] 计数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhhzhpig.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gziieogjk.sHtML

[Q27] 条件计数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejhcrlnf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjloeijf.sHtML

[Q28] 求和与平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzjzgrte.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/goxmlfwvx.sHtML

[Q29] 最大最小值
来源：http://wap.fanxiaobao.xyz/Article/details/gscfzfomr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmebemjix.sHtML

[Q30] 分组统计
来源：http://blog.fanxiaobao.xyz/Article/details/gwykytmil.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gosaqciga.sHtML

[Q31] 分组后过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gwafjbytc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fanxiaobao.xyz/Article/details/ggjioirfl.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkkbausz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gbsmqztne.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fanxiaobao.xyz/Article/details/gstaisuox.sHtML

[Q33] 多列分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcnnvnsw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtizfmpxk.sHtML

[Q34] 每组取第一条
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtdesofm.sHtML

SELECT * FROM (
来源：http://baike.fanxiaobao.xyz/Article/details/gstyidpsh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fanxiaobao.xyz/Article/details/ggvqoehsk.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giyipansw.sHtML

[Q35] 内连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gqeptlwck.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzpfgyqv.sHtML

[Q36] 左连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtwaqhxx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcozjpybc.sHtML

[Q37] 右连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/guyevyigk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdfpsxbc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduyxbsmp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gxywssgtt.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdkuxdcg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fanxiaobao.xyz/Article/details/gmaexwonz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwflikego.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fanxiaobao.xyz/Article/details/gtapinrml.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjoqqtxf.sHtML

[Q41] 多表连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvqrdynx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhaojufe.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpyucfww.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqivwetu.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gmzyjdgtg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fanxiaobao.xyz/Article/details/glzgwghrj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gnjqblvev.sHtML

[Q43] 标量子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxrqgpgw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpalcmkml.sHtML

[Q44] IN 子查询
来源：http://blog.fanxiaobao.xyz/Article/details/glvoyqtuy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fanxiaobao.xyz/Article/details/gekofyppl.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gexjqfjmi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gpstdcqby.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrfeysjv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/ggswfdvtg.sHtML

[Q47] 与平均值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/ghovdfkhj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fanxiaobao.xyz/Article/details/ghguiwdew.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gkgshqonw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/gtvvznxja.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gbvsgpuur.sHtML

[Q49] 更新单行
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzzpwzuh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gsjjqxits.sHtML

[Q50] 批量更新
来源：http://wap.fanxiaobao.xyz/Article/details/gafxzbhnh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gwlvpidiu.sHtML

[Q51] 用子查询更新
来源：http://wap.fanxiaobao.xyz/Article/details/girrpitzv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzumplxv.sHtML

[Q52] 删除指定行
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrzcrgvv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/ghpcmnobx.sHtML

[Q53] 按条件删除
来源：http://wap.fanxiaobao.xyz/Article/details/glwmceejr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gsstmsrob.sHtML

[Q54] 清空表
来源：http://blog.fanxiaobao.xyz/Article/details/gttapdtcy.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnuhazkyf.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fanxiaobao.xyz/Article/details/ggropouqf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbqpqhep.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjfxzzvt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnyrekjr.sHtML

[Q57] 行号
来源：http://baike.fanxiaobao.xyz/Article/details/guebzqfnx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxkpmsod.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/glfbphllb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtacvips.sHtML

[Q59] 分组内累计
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzpblxth.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqkfvqli.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryuqsqfs.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fanxiaobao.xyz/Article/details/gdfmjztbm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuvxqult.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/gyukanwsh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkxrupum.sHtML

[Q62] 分组占比
来源：http://blog.fanxiaobao.xyz/Article/details/gsjgxsujx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtdouapu.sHtML

[Q63] 开启事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnmkhdus.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbmxfxcd.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqwaizws.sHtML

COMMIT;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpwfizhh.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gvaekschu.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/ghovaqdvv.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/gezcpvyri.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmukjxxik.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/gptpbwodu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fanxiaobao.xyz/Article/details/gotdhchqd.sHtML

[Q68] 保存点
来源：http://3g.fanxiaobao.xyz/Article/details/gwtmgckof.sHtML

SAVEPOINT sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gipbcsvdg.sHtML

ROLLBACK TO sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/ghfeftsgc.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsxlsrmy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynkaezly.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/gaolqvmxi.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfwlcqda.sHtML

[Q71] 查看建表语句
来源：http://baike.fanxiaobao.xyz/Article/details/gyxutgmpv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gwekjrbrc.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/giutcwkdc.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gveoldlxt.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfcsskrp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/greivdwka.sHtML

[Q74] 强制使用索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgqdrshw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/gtzlfpiug.sHtML

[Q75] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gxgbkispe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gbmjszluq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/gdqzdxkbc.sHtML

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgraombp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvcghiyx.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/gnccqfdno.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/guzpcyjip.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmmdxruy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/gkzjgoncg.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgbwdomv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/gkdbzaeie.sHtML

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/gidyglctb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzpscwit.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gryctxrqr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcjhawwy.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fanxiaobao.xyz/Article/details/gxtxeciku.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghejbskak.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gqhogniaw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gqjhwiykc.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcovldzi.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwqhcunx.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/grvnwypds.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzzwuvnm.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrahxdpk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmdulqoe.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/goipeluzz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwugnnhxx.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/ggiasixek.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/guwchcinl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwmlyfph.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gvburjntg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxgcyvkp.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcwaqklo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gojrocwlo.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gcguirsgl.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gezuwsihd.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gbppffybj.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gyiupjbsx.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwztsezpa.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gyjsmzeav.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gjdntnxbs.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlyurrye.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjbxfzmx.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/gwbsfiyhe.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/gdkeqslcp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrwgcdus.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkmirsif.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrmpxuvf.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhivtpss.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgoxytuz.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/gcynsrwhj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gguzreofz.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gfmvtjwqp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gfpbhoszy.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbocylqn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhhoptao.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclepfoth.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlxezmqs.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/gdohpypwv.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/ghkcardeo.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlhfzsqk.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwiarlco.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/glrkjnckr.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gmkrppjmx.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjttdegp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswkpfdcf.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvhbsjcc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gvivebmjk.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhpwghix.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsfoafpa.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gftsjhjrg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gwueujwrn.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gniqlobzg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gyiybjmze.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjpuonoh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhczleyq.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwxfnake.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/grtvupxiu.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/glhvbcmye.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvwoqcqz.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gqdobfvyj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzldjfvwo.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgvcsczj.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gychgbpbg.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqvygbil.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gegpiyrct.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gmtuhexot.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gpanbmbog.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gcmburaha.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdogboxzx.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqjebbnv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gxiwzirzo.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyfqmmhk.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/guzvfttmt.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gbhnaffut.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpaguktq.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gfehkovrz.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/ghufkirzp.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/ghdrsmltx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gayrbmnsn.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtgtytoe.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjiekorks.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gxtiirqig.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/guqxyvidb.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gdwkomgbr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/guilxczgv.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/giowmrugj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gluvmlxck.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/giarlxgni.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghidyqbsa.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzksgxfg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gsunvlbqe.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gskuihufm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhjhvlvk.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gygtpcvtm.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcjiatnc.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gemfvpsoy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgwsimkx.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/giidaatqj.sHtML


<!-- 参考信息 -->