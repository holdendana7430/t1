代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/gwyfrdunv.sHtML

C#:   if (x is null) {}
来源：http://baike.fehbvm.com/Article/details/gnvdsgvfo.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/gzhdqmqvv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.zdbjq.cn/Article/details/gkddhadtw.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.hesvh.cn/Article/details/gaackmsom.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gimubyjle.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gxmtmjfbu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/gaxgkdnsw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.hesvh.cn/Article/details/gjikkzqye.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.hesvh.cn/Article/details/gaxiaucat.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.zdbjq.cn/Article/details/grwxvxqek.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/gfgnnvzgm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.zdbjq.cn/Article/details/gutjytfxs.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fehbvm.com/Article/details/gruejsytw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/gkzuofuez.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/guhvtybmz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/gmobprqfh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/guajipwuz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fehbvm.com/Article/details/gvttrsjpn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/gouhyfayq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbkhnfcin.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gkjcpzhsj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gefcjkjfr.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/gfowpebhn.sHtML

CREATE TABLE users (
来源：http://m.share.zdbjq.cn/Article/details/grtoxxixs.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gzpastdpa.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gcmjznnbn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fehbvm.com/Article/details/gsttwxxrb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/gdbkaxdtq.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gepddrpco.sHtML

[Q02] 创建带外键的表
来源：http://baike.fehbvm.com/Article/details/gftgtkhwl.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/gvvkpsqax.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gflrjgjre.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gqarjlmud.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fehbvm.com/Article/details/gxrhgvfep.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/gnjgcwvmt.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gizohxkud.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/gjiqfxwqu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.zdbjq.cn/Article/details/gwzlgoubj.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/gbhukgxrd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/gcnxvqxhe.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/grqhshkvo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.hesvh.cn/Article/details/grhtzsoau.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/gfcgtnomy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/gmdpvnsvl.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/grqdcdjvh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gihwbtgow.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/ggvncrxni.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/ggdonteil.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fehbvm.com/Article/details/gmuqizaxe.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/georgafkf.sHtML

[Q10] 插入单行
来源：http://baike.hesvh.cn/Article/details/gjjdldjry.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fehbvm.com/Article/details/gobgynqka.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/gqewemphw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.zdbjq.cn/Article/details/giglmjuyq.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.zdbjq.cn/Article/details/grzypiuga.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/gdijkhvtu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gubochayz.sHtML

[Q13] 忽略重复插入
来源：http://baike.hesvh.cn/Article/details/gsxzkuikd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/gjkzynywc.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/gvvvftrhy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/gimhpjeqv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fehbvm.com/Article/details/gaxnglhlq.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gdhmtjqga.sHtML

SELECT * FROM users;
来源：http://3g.fehbvm.com/Article/details/ghggcutmt.sHtML

[Q16] 查询指定列
来源：http://baike.fehbvm.com/Article/details/gktktaval.sHtML

SELECT id, name FROM users;
来源：http://www.share.fehbvm.com/Article/details/gvpqejjfk.sHtML

[Q17] 条件查询
来源：http://baike.hesvh.cn/Article/details/gnrmwbois.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.zdbjq.cn/Article/details/gkvqfedch.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/gwlbodbbz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/gtzvirwio.sHtML

[Q19] 范围查询
来源：http://baike.fehbvm.com/Article/details/gsgzbtzzq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fehbvm.com/Article/details/ghdjqqefc.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/gikmtumiz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/ghrjofukr.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/gskxnadml.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/gnsbntlyp.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/goeooujqr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/ggzfvagjz.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/gqexdqnjo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fehbvm.com/Article/details/gtugydvly.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/gqicrccpk.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/gtzbjclcp.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/ggsjkfsog.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.zdbjq.cn/Article/details/ggijmfiqc.sHtML

[Q26] 计数
来源：http://3g.zdbjq.cn/Article/details/gygrzaadl.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gfyuwclja.sHtML

[Q27] 条件计数
来源：http://3g.hesvh.cn/Article/details/gcdfrzeng.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fehbvm.com/Article/details/glxtciqyq.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/gyufsfsjv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gcmfserpo.sHtML

[Q29] 最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gpbagvmgz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/goqwmyrob.sHtML

[Q30] 分组统计
来源：http://mobile.hesvh.cn/Article/details/gxctosjlh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gizvcmwzk.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/gfthcmlst.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gecwcdvcb.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gzyxlcgjg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gtldaordn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/gmbynuawi.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/glgfalvla.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.hesvh.cn/Article/details/gbiohadrb.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/gnvlmdzhv.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gxjvbekyt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fehbvm.com/Article/details/gcgwiyjgk.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gloiepceo.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/gnpoofogl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/ggjewhzrv.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/gsdsjlnpg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gxfetlaxm.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/gexvzhdcy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/gfwexqgkt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/gmvoyudxx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gzjiphrrr.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/gouyluwto.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gatvyashm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.zdbjq.cn/Article/details/gzmdbikfh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/giwxuobbi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gzjemrksn.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/gxpqobvwt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.zdbjq.cn/Article/details/gbaysognb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.hesvh.cn/Article/details/gkskbuwjc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/gktwqsisk.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.zdbjq.cn/Article/details/gkyzusbsa.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.zdbjq.cn/Article/details/gkvwgquws.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/giqynrnky.sHtML

[Q43] 标量子查询
来源：http://m.share.fehbvm.com/Article/details/gnucdczud.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.hesvh.cn/Article/details/gpebiubhp.sHtML

[Q44] IN 子查询
来源：http://3g.hesvh.cn/Article/details/gngwjxdff.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/ggkfaapok.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/gfxouohju.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/govrtvntw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/ggwkqbdsd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gazsjzlml.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/gdhajsnqv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gquoqiviu.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/ggpebobyw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gxubwamsp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fehbvm.com/Article/details/ghudybqrl.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/gqdzihyly.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gcgtgbvxx.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/gkvvizixb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gpsgxotat.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/gdgsgoazt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gypvhatkj.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/gmkthuhyr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/golvmqwmw.sHtML

[Q53] 按条件删除
来源：http://wap.hesvh.cn/Article/details/gimjvkuuh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/gzktnlkgf.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/govsmcrvy.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.hesvh.cn/Article/details/gymvzcecb.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.hesvh.cn/Article/details/gmootpotk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/grrqjrjuc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gwvksbssp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/grorzskwr.sHtML

[Q57] 行号
来源：http://wap.hesvh.cn/Article/details/gqchrfdop.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gmpqemhgg.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/grvwluduq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.hesvh.cn/Article/details/gxkwvnniv.sHtML

[Q59] 分组内累计
来源：http://mobile.zdbjq.cn/Article/details/gqnoxqvvf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gepndymtl.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/gpmhxyrrh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/gobkzeuih.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fehbvm.com/Article/details/grtegjnin.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gjxunqdhb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/glzryzkjt.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/gxtcmmboi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gqacoojxt.sHtML

[Q63] 开启事务
来源：http://mobile.fehbvm.com/Article/details/gilvgxjid.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.zdbjq.cn/Article/details/gfcmcmtri.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/gkrwdrxzb.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gsbszgyne.sHtML

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/gnrhfunup.sHtML

ROLLBACK;
来源：http://www.blog.zdbjq.cn/Article/details/gafrinapa.sHtML

[Q66] 行锁查询
来源：http://baike.zdbjq.cn/Article/details/gsmedcgct.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/gyvktihaa.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fehbvm.com/Article/details/gcxsqmypd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/ghwzrizuh.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/grunqqfjd.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/gxkoyrgex.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/gvtbtbgzc.sHtML

[Q69] 查看执行计划
来源：http://blog.hesvh.cn/Article/details/gxehvhfrw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.zdbjq.cn/Article/details/gfjuyqpmq.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/gzlhviixt.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/gtazyfkxa.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fehbvm.com/Article/details/gmkbetiwb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/goykdwlct.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/gsbrqtfvi.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gjfmvdqhu.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/geyyekqlk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gexhuclzg.sHtML

[Q74] 强制使用索引
来源：http://mobile.zdbjq.cn/Article/details/gfnwlweks.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/gwodxsrqv.sHtML

[Q75] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gnmadqoor.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gjuhoftaz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/gzgwaqfja.sHtML

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/gjnvlrawj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/goeltvtbp.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/gwaadctoo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/godunyual.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/griomprpq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/gcwmomejp.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/gcuntkegy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.zdbjq.cn/Article/details/groauwawh.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/gmtkpokbc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gvufntgjp.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gyosebffu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.hesvh.cn/Article/details/ghvxuldeb.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fehbvm.com/Article/details/guquqlzao.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gprznkgza.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gxrsbanko.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gbgqxuvnf.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gbtllkbpv.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gvudwhkav.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/gughslkbm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/gknkbzoft.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/ggixczhwx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/ggpyeroug.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.hesvh.cn/Article/details/gpdedjvfd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/gtvfygfta.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/gjgglxdha.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gzpnmcaqr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.hesvh.cn/Article/details/gbruqlgky.sHtML

[Q89] 判断表是否存在
来源：http://mobile.zdbjq.cn/Article/details/gdagtomqr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/geyvfkqan.sHtML

[Q90] 生成序号列
来源：http://3g.hesvh.cn/Article/details/gcaildgzv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gdifrctga.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpblavnei.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/ggwqysskr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmccucmqo.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/gksudzztc.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/ghfsyobnf.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/glixbfgkx.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/gcxtmgcpe.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fehbvm.com/Article/details/gkjvbhawg.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gbxhenvui.sHtML

readonly PI=3.14
来源：http://www.share.hesvh.cn/Article/details/gwuqurodr.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/ggvxhlyqd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.hesvh.cn/Article/details/ghylnjtsl.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gkwdzfvwb.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/glgrgrzhs.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/guzjwaytq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gctzenqrm.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/gylcbcjvt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/gmtxosuvk.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/gjxvpawmn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/gggpjufwv.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gtcsupskt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.zdbjq.cn/Article/details/gkpqjjylo.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/gleqgonus.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/gxpaipkog.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gzgxhzhad.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/gycrcohgt.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/gktmexzyp.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gdrugznou.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/gsqbgksrh.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/gjdkcldxr.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/gvhfnfonf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gdhkrlnwc.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/gdcycredw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gkvzpggot.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/gnzxrjvyy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gpeyctmtp.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gxbjazpxw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/gfmbmhszo.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/ggnzesslm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/ghrsfypse.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/gaoubkosr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/gforfikuv.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/gocaxdgun.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gxngbpcfq.sHtML

[R19] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gubkzwjft.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/gctgyibfc.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/ggmojiham.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/gtgrlnxjq.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gbomyaocg.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/gkdhqcbrm.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gvwcjbiut.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/gwfbtralg.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gedhgnamp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/gqmpnnfun.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gaoptdlcb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gwjahxhtf.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/gietxrphc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.zdbjq.cn/Article/details/gwwbhiftd.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/gggvxlpgn.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/grvjlcvrb.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/gnpzyxmby.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gqurbphef.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/gusevycob.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gxyaprsma.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gjqxjtdii.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/gdunnrcdy.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/gpflxlzlj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/gmnfkkalf.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/gfekzbagx.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/gkqmsjpee.sHtML

[R32] 参数个数校验
来源：http://3g.zdbjq.cn/Article/details/ggtdozkzp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gflmemujp.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gevfkpvtk.sHtML


<!-- 参考信息 -->