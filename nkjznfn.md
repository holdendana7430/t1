代发 wailian999

PHP:  // 手写时间戳比较
来源：http://3g.zdbjq.cn/Article/details/gfswbtyip.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gxxxdjgvd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gruepdczx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.zdbjq.cn/Article/details/gqiwxdsra.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.zdbjq.cn/Article/details/gblhxxkex.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fehbvm.com/Article/details/gqvkcimit.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/gyycoiape.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/gtbhyczvc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/gnmfjtmrs.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fehbvm.com/Article/details/gbgmjywkg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/glwqwggmx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gtppdngns.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/gxblgbunw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.hesvh.cn/Article/details/gbnepiyyx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.zdbjq.cn/Article/details/gnrakbxuw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gyatbbuvc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gflfgorjx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.zdbjq.cn/Article/details/gpswmnjst.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfxrpdpkj.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gvejablwl.sHtML

CREATE TABLE users (
来源：http://read.share.zdbjq.cn/Article/details/gvdbfkepj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gfbuukmkn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gizhwswnh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fehbvm.com/Article/details/gyjrkulze.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/ggvzkqhfa.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gmfomfnuh.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/gixdugqmx.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/grdnswroq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gptowatiq.sHtML

user_id INT NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gwwdrbydh.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/gderhojjr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.hesvh.cn/Article/details/gcfrqggen.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gowxqtczn.sHtML

[Q03] 增加列
来源：http://wap.fehbvm.com/Article/details/guwbxvkgu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/gykyyzyhi.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/grgdbpcnz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/gimhjehlp.sHtML

[Q05] 重命名列
来源：http://www.m.share.zdbjq.cn/Article/details/gqvwnxuaj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/gmgtysvvf.sHtML

[Q06] 删除列
来源：http://wap.zdbjq.cn/Article/details/gueebngih.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.hesvh.cn/Article/details/ggynxapwx.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/gapfhqjld.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.zdbjq.cn/Article/details/gbomxfaqk.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/gfogulbbq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gwlzaxhoz.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/gzuudavre.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gruozwmui.sHtML

[Q10] 插入单行
来源：http://blog.zdbjq.cn/Article/details/gslnajxcf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/goytqblyz.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/gigghuocw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fehbvm.com/Article/details/gnnmfxdtx.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fehbvm.com/Article/details/gqkjcrbfp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/gbuwrjabr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/ghigfcbzp.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.hesvh.cn/Article/details/grcwuwibm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gcmicnwqm.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gapvztnvy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/gmchgpnhs.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fehbvm.com/Article/details/gslzpvxqh.sHtML

[Q15] 查询全部
来源：http://wap.hesvh.cn/Article/details/gpnozjnxl.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/gpyvgpsuh.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/gbsgqoxnd.sHtML

SELECT id, name FROM users;
来源：http://3g.hesvh.cn/Article/details/gzjjsykch.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/gsgbgjlyu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/gwhrxrexr.sHtML

[Q18] 模糊匹配
来源：http://www.blog.zdbjq.cn/Article/details/gxgixmrmj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/ghzfksoee.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/ggydcoaff.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.hesvh.cn/Article/details/gtsehgvyt.sHtML

[Q20] IN 列表
来源：http://mobile.fehbvm.com/Article/details/gvpylyarj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.zdbjq.cn/Article/details/guyjivjqx.sHtML

[Q21] 空值判断
来源：http://wap.hesvh.cn/Article/details/gbsnvetih.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/grzxvryvy.sHtML

[Q22] 排序
来源：http://baike.zdbjq.cn/Article/details/gaakwucxn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.hesvh.cn/Article/details/gmdtkkggl.sHtML

[Q23] 分页
来源：http://mobile.zdbjq.cn/Article/details/gjldlwcat.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.zdbjq.cn/Article/details/gtyzrjupj.sHtML

[Q24] 去重
来源：http://blog.hesvh.cn/Article/details/gszauluec.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fehbvm.com/Article/details/guftnmyqe.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/gncnxrqhy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.hesvh.cn/Article/details/goyrxnqhj.sHtML

[Q26] 计数
来源：http://wap.zdbjq.cn/Article/details/gunbtmenu.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gbklcybfv.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/guuyhtijl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gphmlvywi.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/guwpqptgu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gmmtazoyq.sHtML

[Q29] 最大最小值
来源：http://baike.hesvh.cn/Article/details/gymaqhmou.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gikcdilsv.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gpwslvubf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/giwatwwtj.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/gqfmlgesi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/gxqahpret.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gmlygohfu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gstabrxlg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/gnceapplh.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/gaeljulol.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/gxqnshcbe.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/gesgvsmqu.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gprndcybe.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.hesvh.cn/Article/details/gxmuabgsj.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/gujuzvjuy.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gvrjqazbi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gsoctioht.sHtML

[Q36] 左连接
来源：http://www.blog.zdbjq.cn/Article/details/gusoedavw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/grnqfdmze.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/glstztavn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gwrwrgjrl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/gbwfhsbvl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fehbvm.com/Article/details/gevuvzyas.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.hesvh.cn/Article/details/gykwiyzfl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/gqpcljrgv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/gokspwlan.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.hesvh.cn/Article/details/ggijlypzu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/glhtwhmzk.sHtML

[Q41] 多表连接
来源：http://www.blog.zdbjq.cn/Article/details/gjidbxnxa.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gbqbfuiuh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.hesvh.cn/Article/details/gthkoutct.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/gsvuhgqsu.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/geuhrddms.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/gzzjwxoal.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fehbvm.com/Article/details/gdfrykwum.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/gdrcyhcye.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gofegatza.sHtML

[Q44] IN 子查询
来源：http://baike.zdbjq.cn/Article/details/gnbrutwgi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/gfltaqjff.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/gftgbjeow.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gcfdjfbep.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gshkexkuw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gbynehsgg.sHtML

[Q47] 与平均值比较
来源：http://read.share.hesvh.cn/Article/details/gxlyttwbh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gxavhypyl.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.zdbjq.cn/Article/details/gldgnftoi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.hesvh.cn/Article/details/gsdzneott.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/gngsdnrqh.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/gopifxdal.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gfkcahwyp.sHtML

[Q50] 批量更新
来源：http://mobile.fehbvm.com/Article/details/gxbexggxw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gmyvncfpu.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/gpxhxzizs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gtfubcnor.sHtML

[Q52] 删除指定行
来源：http://m.share.hesvh.cn/Article/details/gjqztxong.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gopcfvgui.sHtML

[Q53] 按条件删除
来源：http://read.share.fehbvm.com/Article/details/gpzfocrop.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gfcxxlxgc.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/gigbyjclq.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gnqcvudsr.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.hesvh.cn/Article/details/gwfebdhop.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gloafuxna.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.hesvh.cn/Article/details/gayblgzpv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gipibolsr.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/gywawwcxb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/geugewozl.sHtML

[Q58] 累计求和
来源：http://blog.hesvh.cn/Article/details/gypcnnhrg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gcdhuyqwf.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/gngyzsxeo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gprigkyxp.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/gtcdxlcsg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/gbjcdwbsu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/ghbzchdzh.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/ghimsqeax.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gvroxuaal.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gxtkeelbf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gccdomspv.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/grltdvqkr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.hesvh.cn/Article/details/gloyxhesm.sHtML

[Q64] 提交事务
来源：http://m.share.hesvh.cn/Article/details/gqbcyisnj.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gjzalcepe.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gflpgbhrh.sHtML

ROLLBACK;
来源：http://3g.zdbjq.cn/Article/details/gfqcxhvgp.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/gmfznqyvd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/gnlzvmqvq.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/gguwmbcvh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/gsugdotba.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/guddluqza.sHtML

SAVEPOINT sp1;
来源：http://3g.fehbvm.com/Article/details/gmybvkpda.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gsrlsjagh.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/gtuicxcuj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gsvsygpbk.sHtML

[Q70] 更新统计信息
来源：http://wap.fehbvm.com/Article/details/gnnzbtxje.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/gvksragut.sHtML

[Q71] 查看建表语句
来源：http://3g.fehbvm.com/Article/details/gopvogrxp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/gvfgjjmad.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/gewtgcvaz.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fehbvm.com/Article/details/gvnjfthbm.sHtML

[Q73] 查看表状态
来源：http://wap.zdbjq.cn/Article/details/gwbflnoed.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gugwtoeko.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/gdnkafijg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/gxnlrvaxv.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gajfyvsle.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gwvwzmccd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/gjvgyqayr.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gaowrufpk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.zdbjq.cn/Article/details/gviiwwlbu.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/gwipkdprd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fehbvm.com/Article/details/gydrannqe.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/gehqxqibc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fehbvm.com/Article/details/gfiekdbpx.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gkugcokuk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/gydwgpwhg.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/gwezwelql.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gslifofsd.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gozlcfitm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gfvdoynfn.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.zdbjq.cn/Article/details/gxryqswzz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/ggizxzlaw.sHtML

[Q83] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gviiysltu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gxyvofmel.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.zdbjq.cn/Article/details/guactcjvk.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/ghbcongmi.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gpkkffjtq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fehbvm.com/Article/details/gbpbqusyr.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/gchdwbajv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.zdbjq.cn/Article/details/ggfqmxwyj.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.zdbjq.cn/Article/details/gvzfjnyxd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gjzmofrou.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.zdbjq.cn/Article/details/gywcygcyj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/gfbyvyioi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/gptkmphrq.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/gadnxscht.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/gqqtpkxlb.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/ggudpazqy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gnteakgep.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grjljcuob.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/gvektoxcq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqphnxywt.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/gwakvqqyo.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/grigfskjc.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/ghsfmyttq.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/gohrekhcb.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/glumueoei.sHtML

[R03] 只读变量
来源：http://read.share.hesvh.cn/Article/details/ghokqdfav.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gxomhxwkh.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/gagtzuoqe.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/guhsgcgxd.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/gwztnbqhp.sHtML

name="${1:-default}"
来源：http://wap.fehbvm.com/Article/details/gieezzucb.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/gsgzaqtft.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/ghrddhzdc.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/gmjzwterc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.hesvh.cn/Article/details/gprudnpmm.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/guzanpees.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.hesvh.cn/Article/details/gyeemmgmu.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gsmwdaujw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gqenhxvlf.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/gccjrlkee.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/ghxdpyqzj.sHtML

[R11] case 多分支
来源：http://read.share.zdbjq.cn/Article/details/gandjwwid.sHtML

case "$1" in
来源：http://blog.hesvh.cn/Article/details/gfhxzttjn.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gepxvtiom.sHtML

stop)  echo "停止" ;;
来源：http://read.share.hesvh.cn/Article/details/gvructvvv.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gegitrmum.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/geurutlzm.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/giptqjowy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gdasihvki.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/glfmqveko.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gcznlodpz.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/glvwthksv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gldugagob.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gavlvgbym.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/gpwqcwzsc.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gtkdwlozz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gwpsnuslu.sHtML

[R17] 数组定义与取值
来源：http://3g.hesvh.cn/Article/details/gfdvzodvx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/glsvixluu.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/gfqahikok.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/glujngjys.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/gdelvboco.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gpkfxrrme.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/gmyfahwrq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/gzuicsaye.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/garhirhfw.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/gzkncnxip.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gefxnmdxk.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/gceghnfzw.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gxmsnwbto.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/gojbmsuot.sHtML

[R24] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gkwebihkp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/ghysmdmhv.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/gaygfsbbk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/gbwuylhit.sHtML

[R26] 命令替换
来源：http://m.share.hesvh.cn/Article/details/gzodbdiam.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gqrnrxzlt.sHtML

[R27] 算术展开
来源：http://m.share.zdbjq.cn/Article/details/gscfsistr.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/gacpdefyg.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gpujtxawf.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/gnutsfoxa.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gpnyaniiq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.hesvh.cn/Article/details/gawpcoetu.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/gpvbgcfon.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/gonknyxbg.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/gnxrmsibn.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/glqrcrrgz.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gzlglaxff.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gkpvqaikl.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/gkscgwpjb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fehbvm.com/Article/details/gthqfzcnh.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/gpidiyavf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gofsglorm.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/gluxoucqf.sHtML


<!-- 参考信息 -->