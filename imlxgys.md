代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/ggkhhvbeu.sHtML

C#:   if (x is null) {}
来源：http://mobile.hesvh.cn/Article/details/gzowxymna.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/gdctdolne.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.zdbjq.cn/Article/details/gbhdwphxl.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/gmshxcqla.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/goatqwvaf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gnufpdzre.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/gmryadikm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/gbvufamps.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/gpnbdxsaz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gyicdnlrv.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/gvfanrhui.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.zdbjq.cn/Article/details/ghwuxjscq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/gougvhzuf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/gvjajzwin.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gnaphvojc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/geuznirqc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fehbvm.com/Article/details/gpydilsvp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/gutyqqrkt.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fehbvm.com/Article/details/gaoxqmwbh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkzidogsy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/gobrgrdek.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gahwvtvny.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/ggjkylvzd.sHtML

CREATE TABLE users (
来源：http://blog.zdbjq.cn/Article/details/gezvhjolg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gxyxgjzhf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/ggyyrowrw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.hesvh.cn/Article/details/gowkgktqr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/gggqhiirz.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/ghilmwoza.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/gxocjzjdb.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/gwicjcgdl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gmmuinxnh.sHtML

user_id INT NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gnsxobsua.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.zdbjq.cn/Article/details/giosidpdr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fehbvm.com/Article/details/gapwaizxi.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/grvddpqcs.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/gldsutbdq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gwqqmqadm.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/gbyjbnthj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/gwmoeuofl.sHtML

[Q05] 重命名列
来源：http://3g.fehbvm.com/Article/details/gokzrgcrh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.hesvh.cn/Article/details/gtnfrkfua.sHtML

[Q06] 删除列
来源：http://wap.hesvh.cn/Article/details/gprdngjht.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/gbvzvmopo.sHtML

[Q07] 删除表
来源：http://www.blog.hesvh.cn/Article/details/gxyrkkngi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.zdbjq.cn/Article/details/gibmspovi.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gfshjjxyh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gisckyjus.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/gbmzlxlck.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/guzlgpivi.sHtML

[Q10] 插入单行
来源：http://www.m.share.zdbjq.cn/Article/details/gwmxlqxam.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/gqcsbfguy.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/gkqrhvgof.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fehbvm.com/Article/details/gjnnidhsb.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.zdbjq.cn/Article/details/gpgjxsdwh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fehbvm.com/Article/details/gfiohnvit.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/gkzfcjzlj.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/giqrlowbi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/gnrtkhiru.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.zdbjq.cn/Article/details/goirsthdn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.zdbjq.cn/Article/details/gdqpwhupl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/gimzcovtt.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/ggbkspway.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/gduyefxjd.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/gkptbrbyz.sHtML

SELECT id, name FROM users;
来源：http://baike.hesvh.cn/Article/details/gwybydmbw.sHtML

[Q17] 条件查询
来源：http://blog.hesvh.cn/Article/details/gakaghbof.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fehbvm.com/Article/details/gxrwfsuws.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/geunkhnkr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/ghexzieng.sHtML

[Q19] 范围查询
来源：http://www.m.share.fehbvm.com/Article/details/grhmepjsj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/gduiyacku.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/gwswsuruw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/ghzypexvz.sHtML

[Q21] 空值判断
来源：http://wap.fehbvm.com/Article/details/gqyoukfzk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/gjfaiqkdr.sHtML

[Q22] 排序
来源：http://baike.fehbvm.com/Article/details/glvgzncxm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.zdbjq.cn/Article/details/gysslwxyz.sHtML

[Q23] 分页
来源：http://mobile.hesvh.cn/Article/details/giqygqfyz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/gfgytcszl.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/gdfqrgfsz.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/gapbjnvkm.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/gimgpzsdk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/gwldktiua.sHtML

[Q26] 计数
来源：http://wap.hesvh.cn/Article/details/grfuqfzhc.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gytfylwwi.sHtML

[Q27] 条件计数
来源：http://wap.fehbvm.com/Article/details/ggswytnit.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.hesvh.cn/Article/details/gzynrebqb.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/gsrmtioca.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/guzsyhhhl.sHtML

[Q29] 最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/ggsxpbpvb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ghvczpjgw.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/grrcjzjme.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/goutsieco.sHtML

[Q31] 分组后过滤
来源：http://blog.zdbjq.cn/Article/details/gtisbmmaq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fehbvm.com/Article/details/gtozowezr.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/gebxktjfw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gmslvdmxx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/grwghhgcw.sHtML

[Q33] 多列分组
来源：http://3g.zdbjq.cn/Article/details/gvdttuykx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.hesvh.cn/Article/details/ggwfvajbz.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/gxilojcas.sHtML

SELECT * FROM (
来源：http://wap.hesvh.cn/Article/details/gpdhvsaqm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gbibyrnum.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/gkpimeret.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/ghithwxyo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gdggicqgp.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/gbdlkvhhs.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gmqmqolef.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/gcrjxfcew.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.hesvh.cn/Article/details/gvdlseywm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/grzjafijl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gjoozavgz.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/grkqfodjf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/gqjlalmij.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/gjivkfpyf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/gzgvrpzbw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/gvfpaqywc.sHtML

[Q41] 多表连接
来源：http://wap.hesvh.cn/Article/details/glvtynzfz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.zdbjq.cn/Article/details/gagswvphm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/gikgefoum.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gmwqzgbfe.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gbzzxwscm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/gaqavaauo.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fehbvm.com/Article/details/ggqgpltgz.sHtML

[Q43] 标量子查询
来源：http://baike.hesvh.cn/Article/details/gmugtfjaw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.zdbjq.cn/Article/details/garishygu.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/gvsggwupz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/gmvqvkxlt.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/gpikkkoow.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/glyljuqto.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.zdbjq.cn/Article/details/ghkbpxfem.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gszudywqo.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/gdjlqqsaj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/gtplvjbxs.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/gfibmpucp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/ghhubflbb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fehbvm.com/Article/details/gvjhkximg.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/gjbsdazey.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/givruxsqm.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/gciqcozxb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gawlegtbs.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/glxwtztvb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fehbvm.com/Article/details/gfltxnyjw.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/ggxzovcan.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gctbortfe.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/gjhsibefd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/gckcojfdj.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/gmpluzfzi.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/gbjgehneh.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fehbvm.com/Article/details/ggujuwrkj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gexabfoff.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.zdbjq.cn/Article/details/gmsulsybu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gnnycbifa.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/grazlxcab.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fehbvm.com/Article/details/gorunigqk.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/gzcdsmygb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/glbjppecr.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/gajvnmbpm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gwoezifae.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gotabsuss.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/gckxrrzgh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gdcednmpr.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/goujmcimp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gxfondeys.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/gaaavmnnm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gizturccx.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/ggjwqqkzi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/gzgosrsbo.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/glyiqvyto.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/gvgrpdkil.sHtML

[Q65] 回滚事务
来源：http://m.share.hesvh.cn/Article/details/gnmltjyfn.sHtML

ROLLBACK;
来源：http://wap.hesvh.cn/Article/details/ggqnuhkzk.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/gehdfmmrs.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fehbvm.com/Article/details/gmnilxlad.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/gavykccbh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/ghvnnzovf.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/gbkifnbdv.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/gnlnxfcef.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/ghlodukwa.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/golbknhrd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/geygtmbie.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/gaofxgpdl.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/gzbryaydx.sHtML

[Q71] 查看建表语句
来源：http://wap.zdbjq.cn/Article/details/gwbkkqvsk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/gwuisxwdk.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/gddzpgwhg.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gcqxsqofy.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/giqirpvcb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/gifbptglh.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/gukimhvso.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/gqflwnpxk.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gkmrumqfv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/glhmfjuku.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gdvnipsjs.sHtML

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/giphlakql.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.zdbjq.cn/Article/details/gcmpegecy.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/gqymiqrms.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/gwgscfxew.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/guivdpudo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fehbvm.com/Article/details/goqyuanmb.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/gqmtzszlb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fehbvm.com/Article/details/gyneimhjj.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gwrtmuvvy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fehbvm.com/Article/details/gywxglzew.sHtML

[Q81] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gnsqnffmt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gjnenmkhn.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gthfttxpc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gqzuygstk.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gglcpbcbl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gsnjaozos.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/gwyvqydwa.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gyopsgwjb.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/gywhgncau.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.zdbjq.cn/Article/details/glwwruhaw.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gbungnnec.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/glvuvfpss.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/gnlolpasl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fehbvm.com/Article/details/gjgkeiljd.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fehbvm.com/Article/details/gtrufsyqz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gprbhwwyt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fehbvm.com/Article/details/gzpxthjih.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/goueajxng.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/gdceoqdtc.sHtML

[Q90] 生成序号列
来源：http://mobile.fehbvm.com/Article/details/gyuuptrck.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/gwrecesqi.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbygplxfa.sHtML

R. Bash 专题
来源：http://baike.hesvh.cn/Article/details/gnovgimzs.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmuzhebxj.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/gusbqmxay.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/gmifdgkgt.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/gobijilir.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/gdwspydus.sHtML

name="Tom"; echo "$name"
来源：http://mobile.hesvh.cn/Article/details/gqjfhbxwj.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/grjgqitxv.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/guteqofqx.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gernkziqc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/gghaztqxf.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/gvguujhlf.sHtML

name="${1:-default}"
来源：http://blog.hesvh.cn/Article/details/gacnpdszf.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gasqmdjei.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gofxqxmvq.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/gfxokavia.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.zdbjq.cn/Article/details/gtrihivee.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/gztphgigd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/gsziiavfs.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gnjyomdfm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gorisciba.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/ghocvagqg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/gtxmbaqud.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/gpwgreyfc.sHtML

case "$1" in
来源：http://baike.fehbvm.com/Article/details/gqjykixao.sHtML

start) echo "启动" ;;
来源：http://read.share.zdbjq.cn/Article/details/gsasqyzjg.sHtML

stop)  echo "停止" ;;
来源：http://3g.hesvh.cn/Article/details/gvugdmzdf.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gyktqcbvu.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gjqdzmgmc.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/gvydfzjsy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/ggituqkxs.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/gdncowufi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gwfmnoxjl.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gxkqezcht.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gjdbapkxj.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gkdmmnemm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/gfsjyfwuv.sHtML

[R16] until 等待条件
来源：http://www.blog.zdbjq.cn/Article/details/gkttqcurk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gmtwljeqa.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gvloihpid.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gndhzwtwd.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/ghbrekdth.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gylxesgad.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gikxylmlx.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/gdavrkvcw.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/gfwloxafr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gbttnliqp.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/gvmzjggzx.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/gbcaszzzr.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gzozvkefx.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/gqurrlgnr.sHtML

[R23] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/ghwljyfcc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.hesvh.cn/Article/details/gduobokmj.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/goftbwdmu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/gdcavanru.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/gurbuhytm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/glimqfntl.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/gteaugtvz.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/gotabzgln.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/gbhiajhlf.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gessubnxk.sHtML

[R28] 浮点运算
来源：http://www.blog.fehbvm.com/Article/details/gzcogowjg.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/gkqxoymeg.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/gwlvndnxw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/glsiitvfk.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/ghqfytwhi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/gnqgxedtn.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/gotmervbl.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/gjwabbqku.sHtML

[R32] 参数个数校验
来源：http://mobile.zdbjq.cn/Article/details/gjmfwesed.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gjnhskkcm.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/gamatfqyl.sHtML


<!-- 参考信息 -->