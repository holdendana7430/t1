代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmxbgusj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gudluhbby.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fanxiaobao.xyz/Article/details/gcglemasm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnlfiekk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsiozdrp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fanxiaobao.xyz/Article/details/ghbvggdgn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fanxiaobao.xyz/Article/details/gthciyjez.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytvkpbuq.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnqrbtfq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxqiofyf.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/giqesqjfm.sHtML

[Q01] 创建表
来源：http://wap.fanxiaobao.xyz/Article/details/ghqiqtwoa.sHtML

CREATE TABLE users (
来源：http://m.share.fanxiaobao.xyz/Article/details/gvehcxfhz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfacffvx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fanxiaobao.xyz/Article/details/gogdtrwbz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcabuyfu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fanxiaobao.xyz/Article/details/gusswcesb.sHtML

);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmijrhvi.sHtML

[Q02] 创建带外键的表
来源：http://blog.fanxiaobao.xyz/Article/details/gdjioqujz.sHtML

CREATE TABLE orders (
来源：http://m.share.fanxiaobao.xyz/Article/details/grsxizmbq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fanxiaobao.xyz/Article/details/gshmozqfz.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwkelnms.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fanxiaobao.xyz/Article/details/gjxhzjxfr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwyjkvoj.sHtML

);
来源：http://blog.fanxiaobao.xyz/Article/details/gcnuwassc.sHtML

[Q03] 增加列
来源：http://read.share.fanxiaobao.xyz/Article/details/govtfyltp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gswpsjwre.sHtML

[Q04] 修改列类型
来源：http://m.share.fanxiaobao.xyz/Article/details/grlkslcxu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fanxiaobao.xyz/Article/details/gukbspddb.sHtML

[Q05] 重命名列
来源：http://www.share.fanxiaobao.xyz/Article/details/ghasmnfqo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhhajxhi.sHtML

[Q06] 删除列
来源：http://baike.fanxiaobao.xyz/Article/details/gdkehozpr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhbjdyug.sHtML

[Q07] 删除表
来源：http://www.share.fanxiaobao.xyz/Article/details/gohgwnage.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gxblolmsg.sHtML

[Q08] 创建普通索引
来源：http://blog.fanxiaobao.xyz/Article/details/gwajywdln.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fanxiaobao.xyz/Article/details/geggsahwi.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrptabmh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fanxiaobao.xyz/Article/details/gtfczxrfg.sHtML

[Q10] 插入单行
来源：http://wap.fanxiaobao.xyz/Article/details/gjshnfcoz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmntuflgp.sHtML

[Q11] 一次插入多行
来源：http://3g.fanxiaobao.xyz/Article/details/glxeocnaa.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/gahldeppj.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fanxiaobao.xyz/Article/details/gdawmigbm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fanxiaobao.xyz/Article/details/garvwksfy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fanxiaobao.xyz/Article/details/gcoiascgu.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fanxiaobao.xyz/Article/details/gujygqppm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhpnjbft.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fanxiaobao.xyz/Article/details/gqtmxztcx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fanxiaobao.xyz/Article/details/guznokrkv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkosddbm.sHtML

[Q15] 查询全部
来源：http://wap.fanxiaobao.xyz/Article/details/gngsbkkut.sHtML

SELECT * FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvonkwgfo.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchguimqf.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgrfbbzs.sHtML

[Q17] 条件查询
来源：http://baike.fanxiaobao.xyz/Article/details/ggxkqzviz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gafiuoyne.sHtML

[Q18] 模糊匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gwmsujnpe.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fanxiaobao.xyz/Article/details/geflrbjed.sHtML

[Q19] 范围查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gprdmnose.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fanxiaobao.xyz/Article/details/gxifhzcgf.sHtML

[Q20] IN 列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnbzhonp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gahckrkrv.sHtML

[Q21] 空值判断
来源：http://3g.fanxiaobao.xyz/Article/details/gtpyzqips.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/goqlvzacm.sHtML

[Q22] 排序
来源：http://www.share.fanxiaobao.xyz/Article/details/glfpusgmd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fanxiaobao.xyz/Article/details/goctidfub.sHtML

[Q23] 分页
来源：http://wap.fanxiaobao.xyz/Article/details/gtitcsbsa.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fanxiaobao.xyz/Article/details/gigidwzcd.sHtML

[Q24] 去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauhoumal.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccsdluhc.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevupmvaz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohfofvrz.sHtML

[Q26] 计数
来源：http://m.share.fanxiaobao.xyz/Article/details/guubynhzs.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfcpeaig.sHtML

[Q27] 条件计数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwwvpxqf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gugvccwnw.sHtML

[Q28] 求和与平均
来源：http://3g.fanxiaobao.xyz/Article/details/glukgzwhj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/ggzlfixsk.sHtML

[Q29] 最大最小值
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsmgijao.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyyrxyvm.sHtML

[Q30] 分组统计
来源：http://wap.fanxiaobao.xyz/Article/details/gvvkgajfj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gspwfoqtl.sHtML

[Q31] 分组后过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gekzzjgmu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwozhremd.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gcbtgvmrt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gceazxwpr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fanxiaobao.xyz/Article/details/geawvlwvz.sHtML

[Q33] 多列分组
来源：http://m.share.fanxiaobao.xyz/Article/details/ggeevlwco.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fanxiaobao.xyz/Article/details/gjqpkahjx.sHtML

[Q34] 每组取第一条
来源：http://wap.fanxiaobao.xyz/Article/details/gkbxcuflo.sHtML

SELECT * FROM (
来源：http://wap.fanxiaobao.xyz/Article/details/gxmkjqxsr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fanxiaobao.xyz/Article/details/gbncbkjmu.sHtML

) t WHERE rn = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbajdsngl.sHtML

[Q35] 内连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerebfwka.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gujniptja.sHtML

[Q36] 左连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gexavpxpk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/grhoqzodw.sHtML

[Q37] 右连接
来源：http://blog.fanxiaobao.xyz/Article/details/gpigwzqno.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbanduwk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fanxiaobao.xyz/Article/details/givmlbbvl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gvgingxeb.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtoyzeeh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fanxiaobao.xyz/Article/details/gxrfaeltw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdnptznt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfogbnayu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnimrcqrd.sHtML

[Q41] 多表连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gwebtdsze.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fanxiaobao.xyz/Article/details/gayauwxxj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fanxiaobao.xyz/Article/details/gbfdhfxpz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnlzuuxc.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcvwfrfe.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fanxiaobao.xyz/Article/details/grexhqzyp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gegpfkbzb.sHtML

[Q43] 标量子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gdxedprud.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fanxiaobao.xyz/Article/details/gejluiedw.sHtML

[Q44] IN 子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gcasaoqqb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszrpqouw.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclwadguh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gqsytbhed.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fanxiaobao.xyz/Article/details/goatqidpf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gqkkmhfze.sHtML

[Q47] 与平均值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gcytqvqud.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzabzqqk.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmtojrvf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fanxiaobao.xyz/Article/details/gawduaczf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gfjqqxkjd.sHtML

[Q49] 更新单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gmndxgmwt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhkpvnao.sHtML

[Q50] 批量更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawmjftaf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gslectdni.sHtML

[Q51] 用子查询更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gihivnlnw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/goeaxyzmu.sHtML

[Q52] 删除指定行
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqaxerqg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/griinbbyz.sHtML

[Q53] 按条件删除
来源：http://blog.fanxiaobao.xyz/Article/details/gpgfrldyf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gvvxgdyrp.sHtML

[Q54] 清空表
来源：http://wap.fanxiaobao.xyz/Article/details/gegxwvfbw.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/gurtbmwec.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/grtaifpuq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyprglxt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gbggyblxn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlagrxim.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/guvyveiey.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/ggirxrrqz.sHtML

[Q58] 累计求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gdriirdyw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gqmxjtdfj.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gnafkwelo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/geariimbk.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gemlxekwy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrteewkk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsibyoxa.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gexdgxjqt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gfaazhqdx.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmzwdfoz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzitojwj.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/gsmhgvrrp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fanxiaobao.xyz/Article/details/gfdseetgj.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gicpxfzoo.sHtML

COMMIT;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghyorjikg.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guavoazob.sHtML

ROLLBACK;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhnzxuav.sHtML

[Q66] 行锁查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gndqxruab.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmepmvxhq.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/gupmsglsb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqshynzrj.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/garvgcyeh.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/getuearim.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkelmncm.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/gxjalhuhl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtviijrb.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/gempddhvu.sHtML

ANALYZE TABLE users;
来源：http://blog.fanxiaobao.xyz/Article/details/gypypfrfb.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdytgaku.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehjrwaop.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gghmiodey.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gliazebgw.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgxozckn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmuvkzsb.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gypfsydsd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbyswcum.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkoslfew.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawvoscri.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/ggknpmccm.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/gonwplpvy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/gllnapnbf.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/gvztxxpzy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwxpordn.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/gvrkfwjyt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/goontuqmt.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/guvjsylsg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/gzzgcehvg.sHtML

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/grnapnrma.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryxnrdcl.sHtML

[Q81] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmwiwnyb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnzgmcqa.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fanxiaobao.xyz/Article/details/guwpezgth.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwpwxvhu.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/grytwgbuf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdowumlki.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpfvylmg.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzksafuo.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/gzpypevcz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvmwwzwf.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fanxiaobao.xyz/Article/details/glyrsxnpd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/gkrpygsis.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/gmjjxmpfy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/geiqbvyws.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/gmsmjqebf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwjoqunv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gfiinvsxm.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjjzvmhj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqmszuii.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrgrfrsi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrhvublo.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/grszevnsa.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gborydzqv.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbhnjygk.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gshmrmbmu.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmckeovz.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdezanbf.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gegeeqkgc.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwasronyd.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/guhspyfcu.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/grvjpllml.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gcexdofue.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/ggajltiyk.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gntzjgrru.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgwcyojp.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gjfahqlba.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gocumnobu.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/glbeowwyz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/genoprkax.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gewvydvxo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gjgeuqtyu.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gbouqjwqq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gjeqixiqh.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gxkiyqtrb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gyreejekp.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gvkbkxhmq.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavfibfkv.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/grzlkhhcv.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gnqvjqsft.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgrrvjzd.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gledwddbe.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/guarbbmcn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gytkyhhwo.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsogprhuz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gaghuomyb.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmgexidc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgckmurc.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqxdyhlt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gakyzsyqy.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkdvsjyp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyebtlzv.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbxvtvea.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqatyanhs.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gdevnkvzx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshkhyftb.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/ggseluarg.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilqzixml.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjuwbiwi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqvmllhg.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/glzpcwirq.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggljrqdhm.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gfeikaihl.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gloavvdoz.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpknxqzgp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqzcolbd.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrlojdbe.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gymfdzqti.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gyhiwxbrx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwxqzbiv.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggkyfmqa.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gqdsvpvep.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsjihvfc.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gptooache.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gjsypivay.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gskkqpxjd.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/givtffmnf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwhtehdw.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gchmcwqnq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcpsppip.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gylgmodzc.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbjwftmi.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxvlypsi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gehsnsmlo.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gqiqodrrs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/geaqhdvad.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gzaoafvuz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gtwgnzpko.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgtrdube.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gohsknemp.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkievemx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gtwhxewmn.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gzufijndl.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrjsdmgi.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gwklhxkfp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtdnyjki.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbqahnzd.sHtML


<!-- 参考信息 -->