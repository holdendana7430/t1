代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgpipfqk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fanxiaobao.xyz/Article/details/grmpmojiz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fanxiaobao.xyz/Article/details/gyivpyhrs.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fanxiaobao.xyz/Article/details/gngeeokmq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyvvdksf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbjnyrxa.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fanxiaobao.xyz/Article/details/ggicyqgby.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fanxiaobao.xyz/Article/details/gsjfnxawd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fanxiaobao.xyz/Article/details/gcddsmmza.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqpqfhfs.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkonudflm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fanxiaobao.xyz/Article/details/gjctdiwzk.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ghfusryns.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fanxiaobao.xyz/Article/details/giovxtwsy.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gmzezjcya.sHtML

[Q01] 创建表
来源：http://m.share.fanxiaobao.xyz/Article/details/gjztvrwai.sHtML

CREATE TABLE users (
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwjmggrl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkjfrhgk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fanxiaobao.xyz/Article/details/gglhunazy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fanxiaobao.xyz/Article/details/gkenhhmcq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fanxiaobao.xyz/Article/details/gczkaxwqi.sHtML

);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganmdmtoj.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fanxiaobao.xyz/Article/details/godhitmqn.sHtML

CREATE TABLE orders (
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxlbjxex.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmkvoqzj.sHtML

user_id INT NOT NULL,
来源：http://baike.fanxiaobao.xyz/Article/details/gmxomkpgb.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fanxiaobao.xyz/Article/details/geqdxotey.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fanxiaobao.xyz/Article/details/gqhlpvbsc.sHtML

);
来源：http://wap.fanxiaobao.xyz/Article/details/gjvytnwxu.sHtML

[Q03] 增加列
来源：http://wap.fanxiaobao.xyz/Article/details/gnpdntjvx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gvjzhvbib.sHtML

[Q04] 修改列类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgnvfsad.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexukrgji.sHtML

[Q05] 重命名列
来源：http://baike.fanxiaobao.xyz/Article/details/gsilqyczv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpdyphxp.sHtML

[Q06] 删除列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gauxrcgix.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fanxiaobao.xyz/Article/details/gompxjlae.sHtML

[Q07] 删除表
来源：http://wap.fanxiaobao.xyz/Article/details/gqknkfrxp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gukxksocs.sHtML

[Q08] 创建普通索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgkewmrn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fanxiaobao.xyz/Article/details/gxpvqpumv.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gflyffemo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghldxefau.sHtML

[Q10] 插入单行
来源：http://3g.fanxiaobao.xyz/Article/details/gtsidljzp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqlnopqi.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegyojmuh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/grwkmdtqv.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmddgvjc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fanxiaobao.xyz/Article/details/gwexfqhpf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fanxiaobao.xyz/Article/details/goirouxxk.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzklldwht.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gxhsdmova.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fanxiaobao.xyz/Article/details/gobekxrrt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fanxiaobao.xyz/Article/details/gcnxreweo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fanxiaobao.xyz/Article/details/gcqptcgaf.sHtML

[Q15] 查询全部
来源：http://wap.fanxiaobao.xyz/Article/details/gfudcaxvx.sHtML

SELECT * FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgglyiez.sHtML

[Q16] 查询指定列
来源：http://baike.fanxiaobao.xyz/Article/details/guwhiakss.sHtML

SELECT id, name FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmlfnhom.sHtML

[Q17] 条件查询
来源：http://baike.fanxiaobao.xyz/Article/details/gabwqieez.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbsoebaw.sHtML

[Q18] 模糊匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gknwiohhl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fanxiaobao.xyz/Article/details/gxfbcglvd.sHtML

[Q19] 范围查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfpwdauy.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fanxiaobao.xyz/Article/details/gopgzzvol.sHtML

[Q20] IN 列表
来源：http://baike.fanxiaobao.xyz/Article/details/gkmzybjrg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzuuwebd.sHtML

[Q21] 空值判断
来源：http://3g.fanxiaobao.xyz/Article/details/gdlvcqwuk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpizlnpu.sHtML

[Q22] 排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwdxceqv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fanxiaobao.xyz/Article/details/gscsrfipk.sHtML

[Q23] 分页
来源：http://baike.fanxiaobao.xyz/Article/details/gxmbiaslp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fanxiaobao.xyz/Article/details/gekecxebh.sHtML

[Q24] 去重
来源：http://mobile.fanxiaobao.xyz/Article/details/gkinueumz.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gdirlqxet.sHtML

[Q25] 只取前 N 条
来源：http://baike.fanxiaobao.xyz/Article/details/gkfmwwkxn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fanxiaobao.xyz/Article/details/gywbjlyjq.sHtML

[Q26] 计数
来源：http://read.share.fanxiaobao.xyz/Article/details/gsljauqcf.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrmwgxyw.sHtML

[Q27] 条件计数
来源：http://read.share.fanxiaobao.xyz/Article/details/glvrxbiqk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gulryjrlm.sHtML

[Q28] 求和与平均
来源：http://read.share.fanxiaobao.xyz/Article/details/girtazngr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpiqwffvi.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmctubxc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxhtwfbk.sHtML

[Q30] 分组统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaahelwkt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjefyghcg.sHtML

[Q31] 分组后过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gdqmfnkig.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gqudldzsf.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/guyiyjxge.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/guxjvfrlh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhyacaes.sHtML

[Q33] 多列分组
来源：http://3g.fanxiaobao.xyz/Article/details/gftbgregq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fanxiaobao.xyz/Article/details/gpcoedxea.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylokekni.sHtML

SELECT * FROM (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntriggel.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fanxiaobao.xyz/Article/details/gaylbshkq.sHtML

) t WHERE rn = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/girevelpz.sHtML

[Q35] 内连接
来源：http://blog.fanxiaobao.xyz/Article/details/gqwljafsl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/goybysdyj.sHtML

[Q36] 左连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gpthxbuyh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktnsyumn.sHtML

[Q37] 右连接
来源：http://3g.fanxiaobao.xyz/Article/details/gmrunpukt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmadhwau.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fanxiaobao.xyz/Article/details/ghkynlazv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnedwbpgi.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fanxiaobao.xyz/Article/details/gueswzdee.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcjmdejd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/govszfkfe.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggisufano.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fanxiaobao.xyz/Article/details/gilowvdbl.sHtML

[Q41] 多表连接
来源：http://baike.fanxiaobao.xyz/Article/details/gqseavear.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvlzbxiy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fanxiaobao.xyz/Article/details/gyftthkmy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gzlnddxrv.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbwwylrg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fanxiaobao.xyz/Article/details/gdiziyojv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gfqcvgrju.sHtML

[Q43] 标量子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/geypkodty.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fanxiaobao.xyz/Article/details/glbojxqle.sHtML

[Q44] IN 子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gcgqiwppo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fanxiaobao.xyz/Article/details/gpehfxmmt.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fanxiaobao.xyz/Article/details/gasyrsoxx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gipqmczbf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fanxiaobao.xyz/Article/details/gcuafeuod.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhvsprjp.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gcaluxknk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fanxiaobao.xyz/Article/details/gtjmxmpzl.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gsuwwwebl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdvegajw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkfcxhwn.sHtML

[Q49] 更新单行
来源：http://blog.fanxiaobao.xyz/Article/details/gytzxhqsy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfqmbrbn.sHtML

[Q50] 批量更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsxxqwdi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gdtuxtvda.sHtML

[Q51] 用子查询更新
来源：http://baike.fanxiaobao.xyz/Article/details/gqyocnkmq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/griwiadvu.sHtML

[Q52] 删除指定行
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxwsadrz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gymzsbzna.sHtML

[Q53] 按条件删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gtueuzwkt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/geuypgdka.sHtML

[Q54] 清空表
来源：http://baike.fanxiaobao.xyz/Article/details/gfqdyrxnj.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fanxiaobao.xyz/Article/details/gcjarntdl.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvdkudyn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggonmmhsb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gocsjnwsf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gudkfylxb.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gszxdmrcw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gruhwpdnj.sHtML

[Q58] 累计求和
来源：http://baike.fanxiaobao.xyz/Article/details/gvshatzqh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkyauaaz.sHtML

[Q59] 分组内累计
来源：http://baike.fanxiaobao.xyz/Article/details/gfakltlrl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gxuywnhmk.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fanxiaobao.xyz/Article/details/gmjyagokq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/gdneftlcl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gmdzsyteb.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gfaowrbtp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgoghscz.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gdjlvfsif.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gnbefnpbu.sHtML

[Q63] 开启事务
来源：http://3g.fanxiaobao.xyz/Article/details/gbjmaxasq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fanxiaobao.xyz/Article/details/gxfhdnpxh.sHtML

[Q64] 提交事务
来源：http://3g.fanxiaobao.xyz/Article/details/geteqnqmy.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxdturcn.sHtML

[Q65] 回滚事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvoehdau.sHtML

ROLLBACK;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghoonatqa.sHtML

[Q66] 行锁查询
来源：http://m.share.fanxiaobao.xyz/Article/details/ghojirojr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fanxiaobao.xyz/Article/details/gyzupmvee.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/gzxovkhhi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fanxiaobao.xyz/Article/details/gpsqtvazn.sHtML

[Q68] 保存点
来源：http://blog.fanxiaobao.xyz/Article/details/ghqsevvov.sHtML

SAVEPOINT sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gjhedbomt.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gknepknpa.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/ggsdoybau.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fanxiaobao.xyz/Article/details/gopsbuhwl.sHtML

[Q70] 更新统计信息
来源：http://mobile.fanxiaobao.xyz/Article/details/ggctsudju.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/grfjgwydb.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/gkklrzcwk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfowmekr.sHtML

[Q72] 查看索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhfggwzi.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gyitrgojh.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/ggtzffdif.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gktninwxh.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjlnbgtw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyclojhf.sHtML

[Q75] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdamrcnon.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/ghlaxyoyv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzlwdiil.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdquhiro.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvwjwkjj.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvdoxnvz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbsnhfzv.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/gmjfntzwe.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/gvzdaoedl.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/ghzxlkpox.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqgdlxpc.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/gsjgykoyv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdpgxfpv.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmreaklc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsiyeqhd.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gskwnqhuj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhbdbroe.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gavqhjasi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnleqjevt.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gnyfjrqxo.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ggbendabw.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/gnofifrcb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqxyexiy.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gztabezic.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gxthshixj.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmstuoowb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gudgsmcjh.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/gidpiwdwg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqoqjclx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilhsgmwo.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gciozovfs.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvnpjzji.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyebrsabp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gvmysmfas.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gxqyinqcp.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gskgpljlw.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzjlammg.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/gisruqssj.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/ggwitoiec.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/gorfrengy.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gbusslldm.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/giygyrubh.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/glilalfae.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gtxnmzxbm.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/giheccgdt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gowczmwxs.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpukkncpy.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gozfbocer.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpkiqhlg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgomfqix.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/ghtaaphfi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gipnwmaxs.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gyeyjhdii.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzezlcbn.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gnedxmzym.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqzxyjvi.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsejakod.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnnrhijt.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gysltnidj.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkctgcjbt.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldqtofjd.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/geytscwvn.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlhodwyy.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtrcdtuj.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfttpbtsz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfrleuri.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/geqrpfozw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/grdlxosih.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gsanmlmsg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfdgirvr.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtheqozkz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gnukarfmx.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gskzygwfr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gpwfeeltk.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gfpadowwo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/govqfhdie.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/ghycvyetz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gjuzaljtx.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gjfbblyxr.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/griwfzaya.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/grfrhyjfc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvdeaxkm.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/grotxwdbw.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfjyrlge.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gxspqvgcu.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhikpyjz.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gqrmoiipr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasztqrlg.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gnvenpwyc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvjfiaot.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gaksspkji.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlwcprtw.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwueihdv.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gaqmisqtj.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gityzzeab.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gubncjqgd.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/gbsinbxns.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgmlutpp.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gxypczzii.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gmpripafk.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzahsayzj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gofnvvutd.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gitfumllq.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypzajeeg.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbazkmtms.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gurjadniz.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gppsnnijo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gffwykpkz.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgwgsege.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvoecxxj.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyyhaore.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwwsosmw.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gveqjhzsi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/goxtpiyrp.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gqasrrktf.sHtML


<!-- 参考信息 -->