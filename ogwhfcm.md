代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvptxjmp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fanxiaobao.xyz/Article/details/gmoyygrbl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fanxiaobao.xyz/Article/details/gnmhwxivd.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fanxiaobao.xyz/Article/details/gobmpiyox.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fanxiaobao.xyz/Article/details/gfbbuwwnm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giurbdnoz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyauiyax.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fanxiaobao.xyz/Article/details/gpfxdmtps.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlfamqur.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrsrywsm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpsygbqk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbgbwxyx.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gubjgevvk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fanxiaobao.xyz/Article/details/gfegmfgzx.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gpblaucgg.sHtML

[Q01] 创建表
来源：http://mobile.fanxiaobao.xyz/Article/details/gwuekdecl.sHtML

CREATE TABLE users (
来源：http://blog.fanxiaobao.xyz/Article/details/ggbpwwzuv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fanxiaobao.xyz/Article/details/gvcsbydyj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuoablmv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsoyefyjk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbwbmlma.sHtML

);
来源：http://3g.fanxiaobao.xyz/Article/details/gjkirmybe.sHtML

[Q02] 创建带外键的表
来源：http://wap.fanxiaobao.xyz/Article/details/gypfmyntq.sHtML

CREATE TABLE orders (
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrtvfxcu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkaenbcv.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibeazoot.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fanxiaobao.xyz/Article/details/gaglmofkg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fanxiaobao.xyz/Article/details/gzmhzoqnq.sHtML

);
来源：http://wap.fanxiaobao.xyz/Article/details/gbtvttwgj.sHtML

[Q03] 增加列
来源：http://wap.fanxiaobao.xyz/Article/details/gmhrkgyjv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjesrxgci.sHtML

[Q04] 修改列类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpkgbqla.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxndufvp.sHtML

[Q05] 重命名列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykjvborh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvprswksx.sHtML

[Q06] 删除列
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfbbayvd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fanxiaobao.xyz/Article/details/gclvbqlmq.sHtML

[Q07] 删除表
来源：http://mobile.fanxiaobao.xyz/Article/details/glbkbybri.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gtzjqawfr.sHtML

[Q08] 创建普通索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwvpsdww.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fanxiaobao.xyz/Article/details/gzbzwqfoq.sHtML

[Q09] 创建唯一索引
来源：http://baike.fanxiaobao.xyz/Article/details/giatfecdb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fanxiaobao.xyz/Article/details/gmumhkbef.sHtML

[Q10] 插入单行
来源：http://wap.fanxiaobao.xyz/Article/details/gobvqojts.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gogxyhvoi.sHtML

[Q11] 一次插入多行
来源：http://baike.fanxiaobao.xyz/Article/details/gjfoszjrl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtxqofwu.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwgjqzgr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fanxiaobao.xyz/Article/details/gltbtaqfk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fanxiaobao.xyz/Article/details/gcljxuzrg.sHtML

[Q13] 忽略重复插入
来源：http://blog.fanxiaobao.xyz/Article/details/gdmrfvncr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdtszzrp.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fanxiaobao.xyz/Article/details/gsipiuemj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwwunpek.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsihbyyfg.sHtML

[Q15] 查询全部
来源：http://blog.fanxiaobao.xyz/Article/details/gvnlapyur.sHtML

SELECT * FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gijlyxlwm.sHtML

[Q16] 查询指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gqvwbxjbn.sHtML

SELECT id, name FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/golsnuepj.sHtML

[Q17] 条件查询
来源：http://blog.fanxiaobao.xyz/Article/details/gdqyfekuc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/georvwket.sHtML

[Q18] 模糊匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gfysnatwo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxesglpc.sHtML

[Q19] 范围查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtobfhley.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxehbubq.sHtML

[Q20] IN 列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gzaafegjl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gknnnuodw.sHtML

[Q21] 空值判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtlsqfgr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fanxiaobao.xyz/Article/details/ggjafqclb.sHtML

[Q22] 排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkahghsh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fanxiaobao.xyz/Article/details/gqfteokxi.sHtML

[Q23] 分页
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyzdrksu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fanxiaobao.xyz/Article/details/gavmimnrh.sHtML

[Q24] 去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganulujsw.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/guruaozjq.sHtML

[Q25] 只取前 N 条
来源：http://wap.fanxiaobao.xyz/Article/details/gzwnevxvl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fanxiaobao.xyz/Article/details/gxcbqkkzk.sHtML

[Q26] 计数
来源：http://blog.fanxiaobao.xyz/Article/details/grvlwxfdm.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsmiqwag.sHtML

[Q27] 条件计数
来源：http://wap.fanxiaobao.xyz/Article/details/gjcytqedi.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gleyputyu.sHtML

[Q28] 求和与平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gqybdrffq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrwicnib.sHtML

[Q29] 最大最小值
来源：http://baike.fanxiaobao.xyz/Article/details/gfarxjpot.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/givlepifk.sHtML

[Q30] 分组统计
来源：http://3g.fanxiaobao.xyz/Article/details/gtoslrdld.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/grcmasqub.sHtML

[Q31] 分组后过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwchvecq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujfdwpep.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwosczid.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gracxnrph.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fanxiaobao.xyz/Article/details/gcflcujup.sHtML

[Q33] 多列分组
来源：http://m.share.fanxiaobao.xyz/Article/details/glxyxxopt.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdtojdzt.sHtML

[Q34] 每组取第一条
来源：http://mobile.fanxiaobao.xyz/Article/details/gjazvwqeh.sHtML

SELECT * FROM (
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyqjfovx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fanxiaobao.xyz/Article/details/gszhxdmkn.sHtML

) t WHERE rn = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gwlacovga.sHtML

[Q35] 内连接
来源：http://3g.fanxiaobao.xyz/Article/details/gvrvrghks.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnuvgsmg.sHtML

[Q36] 左连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgzdputm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmbffvcw.sHtML

[Q37] 右连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gzignrggd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsmizhoi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fanxiaobao.xyz/Article/details/gddvgtlmv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxgsknqj.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkgcgydp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fanxiaobao.xyz/Article/details/ggdldyqlo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gvsnlteol.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fanxiaobao.xyz/Article/details/gplhayfcr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fanxiaobao.xyz/Article/details/gcaqbysoz.sHtML

[Q41] 多表连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwiczkai.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihrkbgms.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fanxiaobao.xyz/Article/details/gqyuajrep.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghidyizca.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/grucnekqs.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fanxiaobao.xyz/Article/details/gxuptsxwa.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gogefnjya.sHtML

[Q43] 标量子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gkstspwvp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fanxiaobao.xyz/Article/details/gwfwzmntg.sHtML

[Q44] IN 子查询
来源：http://3g.fanxiaobao.xyz/Article/details/guhberzir.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgljokrx.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjooiric.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjqffidy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fanxiaobao.xyz/Article/details/glsjroruk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gaxdjnxdz.sHtML

[Q47] 与平均值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gslmaxhwv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fanxiaobao.xyz/Article/details/gggpsbcna.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gswizxfyi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkcppkcq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/giwhhpmtx.sHtML

[Q49] 更新单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gommbajfr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gdclcxsuw.sHtML

[Q50] 批量更新
来源：http://3g.fanxiaobao.xyz/Article/details/gpchblhkb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gaahisgno.sHtML

[Q51] 用子查询更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gidttjove.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzrmmsdc.sHtML

[Q52] 删除指定行
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvleezzb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gbeysxjbt.sHtML

[Q53] 按条件删除
来源：http://3g.fanxiaobao.xyz/Article/details/goflkhvai.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvakovqyu.sHtML

[Q54] 清空表
来源：http://m.share.fanxiaobao.xyz/Article/details/gfykqqwxb.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/glfbnient.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjobodwm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjbnrkhs.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozjhbhzz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjcaipni.sHtML

[Q57] 行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxoszwxup.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gsyqvkxcz.sHtML

[Q58] 累计求和
来源：http://baike.fanxiaobao.xyz/Article/details/ginvghhgc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnguexmna.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/giaimclnt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/grmzspaam.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gfytlwhlk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwppsbsl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gsbdzmdfz.sHtML

[Q61] 移动平均
来源：http://read.share.fanxiaobao.xyz/Article/details/gafmdnihd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdaripawp.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goeeygdyk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhiqyepo.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/ggwsawluc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjsthrtg.sHtML

[Q64] 提交事务
来源：http://baike.fanxiaobao.xyz/Article/details/glwkllhvo.sHtML

COMMIT;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrlbqouh.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/gazaiqycp.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/gucybeeom.sHtML

[Q66] 行锁查询
来源：http://blog.fanxiaobao.xyz/Article/details/gnpxvvfef.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giaeeptym.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsnpunhw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fanxiaobao.xyz/Article/details/gqbmmshei.sHtML

[Q68] 保存点
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrhfzanh.sHtML

SAVEPOINT sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/guvzrzjld.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpknsomb.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/gkxhmetmh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fanxiaobao.xyz/Article/details/gsgymjmka.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/giuzimtxw.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlxjchoa.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gthugpgur.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fanxiaobao.xyz/Article/details/giwlhjjkk.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/grxjxtnky.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbddomloy.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnnrwllv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gkejfnzey.sHtML

[Q74] 强制使用索引
来源：http://baike.fanxiaobao.xyz/Article/details/gbkhqqgmt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjbwpcwo.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gdllbwfof.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gohrcwmpn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fanxiaobao.xyz/Article/details/goxpmqixb.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/giozyefzq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gifghtbnn.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/geofneukf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/goqpyusqk.sHtML

[Q78] 当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpnoyoph.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/gjwnajagp.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/garuqktui.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gnjkpvpdu.sHtML

[Q80] 字符串截取
来源：http://www.share.fanxiaobao.xyz/Article/details/grekuktvd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gztmxgesn.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gbrxelcoq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrnpoazg.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guiwomobz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gfeozotzu.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gfancvbxh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gbnggrcoq.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gxzbfovtz.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtysrqjxq.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrpxrpdb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/gygrvvjiu.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowwrpwpr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/greypuitx.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/gpdgticmy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwssfxcll.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqireqfm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/ganrkrcqs.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvlxwuyr.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gthnycwqy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gvjajougz.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnkuvmzo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gmsoiislc.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggiqoiioi.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gbiezdaoh.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gdexvkqds.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdnzlkxo.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/ggotslqtu.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/gafqptowt.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gttbeocbi.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqymalmj.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gllszlrtl.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmkkilhu.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblkanvfy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdiipvaz.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gscoceher.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/ggesvgbkv.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gkhfhdium.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grusvqmaw.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyssiatv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gsknhnprr.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gcakewqrk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnrducnw.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gsvnvxjio.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvunivdba.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gidckdbpp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvaslrkn.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/gymgfiitz.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlblkbkf.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gfrklrlcp.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gzoepkdpm.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gtfxurdjw.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gttulhjui.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbdlrjvk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/ghizlxbjf.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gofausgws.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/geaqirklk.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gipndqgok.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/guirvtjhd.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gkihwpmdo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxtfzzea.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakdylsej.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gygmszlvw.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/goqgisajh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzsimcgx.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/glepayclu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/giluwzsbc.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gebwfsfwp.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgnhjoow.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gawpktrjm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/guvrxfoom.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/guuaoordh.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gcodxuefs.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gwpeukdgr.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gwoubtvzi.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gbidwtpjo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gisgukwbq.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gcczuacjt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geaunimho.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/giqiraukf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gefngjesu.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/gmnivdkzb.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gstzzewhp.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gxssyrkgb.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gzjqpckbd.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbmbkwzb.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpwdbgjo.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsetazsb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gtixhkzpj.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/guahkgtto.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gctfluwli.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjjewepu.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhwtltbf.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gtgrhjbud.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grdusiwsw.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbyxvvtn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfvvlexl.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojravswz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/geuwiddml.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gvuzsyuqx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gaetbkdtr.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gblqqbfwt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gzryupdbe.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/guewtahnm.sHtML


<!-- 参考信息 -->