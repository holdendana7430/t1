代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/grxilxmtl.sHtML

C#:   if (x is null) {}
来源：http://blog.fehbvm.com/Article/details/gmjkxbneq.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/gofpogjnw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fehbvm.com/Article/details/gpfqtsfuy.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/gxlwkecoj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gibrligvg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/ghtnegmoy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/gtuxfwljp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fehbvm.com/Article/details/gxazwupnm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/gpxyjpjln.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fehbvm.com/Article/details/gfvegcflr.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.zdbjq.cn/Article/details/gvpedqovo.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/gexfopvno.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.hesvh.cn/Article/details/ggldonwui.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fehbvm.com/Article/details/gtdylevle.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gqamkzjez.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/gbnwqenjd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/gnecjbpaw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/gaylslipj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gueckjjfr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gituiwgoy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.zdbjq.cn/Article/details/gsmjgkeub.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcfgggjwc.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/glcpdggdd.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/gcsbmiobe.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gqnzbgqvi.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.hesvh.cn/Article/details/glabytitr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fehbvm.com/Article/details/gbfunynja.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.hesvh.cn/Article/details/ghoqzecyn.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gchopymfn.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/ghcawxbbt.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/gvrqaqnbo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gbzwotohu.sHtML

user_id INT NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/ggyjicibe.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/gvvalneyf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.zdbjq.cn/Article/details/ganhpadvc.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gjnqlzvrh.sHtML

[Q03] 增加列
来源：http://www.blog.fehbvm.com/Article/details/gawukdxtv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/ggvogibsh.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/glbukyreb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.hesvh.cn/Article/details/gylmreadn.sHtML

[Q05] 重命名列
来源：http://blog.zdbjq.cn/Article/details/grpgohqyc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/gkapfbsqp.sHtML

[Q06] 删除列
来源：http://m.share.fehbvm.com/Article/details/gxexoftxi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/gchcstmyx.sHtML

[Q07] 删除表
来源：http://baike.zdbjq.cn/Article/details/gehhwdauk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.zdbjq.cn/Article/details/gkxpqvhjr.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/gudahilau.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gzbgydtmw.sHtML

[Q09] 创建唯一索引
来源：http://3g.hesvh.cn/Article/details/gmkqlysto.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gvplglgjj.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/gadwwziqj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/gcwxlimcq.sHtML

[Q11] 一次插入多行
来源：http://www.share.fehbvm.com/Article/details/gmcncxcuh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.zdbjq.cn/Article/details/gsomasjen.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.zdbjq.cn/Article/details/gmgoifwmi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.hesvh.cn/Article/details/gvejuxaiz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.hesvh.cn/Article/details/gresbjhyy.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/gkgohhjrz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fehbvm.com/Article/details/ggosmamaf.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/gbbedumnl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/gxmvprmoj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/gbqqytjdt.sHtML

[Q15] 查询全部
来源：http://3g.zdbjq.cn/Article/details/gdcogazhe.sHtML

SELECT * FROM users;
来源：http://wap.hesvh.cn/Article/details/gqmmbupqr.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/gnuuulsqt.sHtML

SELECT id, name FROM users;
来源：http://wap.zdbjq.cn/Article/details/gyumhmqjw.sHtML

[Q17] 条件查询
来源：http://read.share.fehbvm.com/Article/details/gttspvfdx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/gxrhorfuw.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/gtzbioyqk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/gifbpbwun.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/gmwvyotwl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fehbvm.com/Article/details/gepuncyuo.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/gtolbkfsu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/ghrokalzr.sHtML

[Q21] 空值判断
来源：http://www.blog.zdbjq.cn/Article/details/gngqjoqas.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gziqrdyjg.sHtML

[Q22] 排序
来源：http://read.share.fehbvm.com/Article/details/gxlkyhyge.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/gmfdzqdhd.sHtML

[Q23] 分页
来源：http://blog.hesvh.cn/Article/details/gnutgsosv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/gvxczheim.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/ghsztswmu.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.hesvh.cn/Article/details/gzvxscmss.sHtML

[Q25] 只取前 N 条
来源：http://3g.zdbjq.cn/Article/details/gjzwumpqt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.hesvh.cn/Article/details/gxkhvortc.sHtML

[Q26] 计数
来源：http://m.share.zdbjq.cn/Article/details/gjhxtkvzr.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/gdscreqtw.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/gowofggjc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/glzgmfabm.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gdzjbobys.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gkwtvrunl.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/gdrreorck.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gstiegbas.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/gjrvpnvpn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gjgqctsvu.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/gkdxnbljz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gssshcheu.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/ghtchdfkk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/giahcykiq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/gdtidikiy.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/gzjibbmvx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/gargtymev.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/goijefgnh.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/gxvocmrrl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fehbvm.com/Article/details/glgyqwgui.sHtML

) t WHERE rn = 1;
来源：http://m.share.hesvh.cn/Article/details/gyefyssof.sHtML

[Q35] 内连接
来源：http://www.m.share.fehbvm.com/Article/details/gunpfwjdb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gseqczdsf.sHtML

[Q36] 左连接
来源：http://blog.zdbjq.cn/Article/details/gycjrxpiv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gtrzckxxa.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gazwmeutc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/gcvufxzma.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/gzdnhezto.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/gwinbhbgf.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/gniihnegg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/gagjguiyy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fehbvm.com/Article/details/gfhdzjsbk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fehbvm.com/Article/details/gjdvmhrsz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gxmseljow.sHtML

[Q41] 多表连接
来源：http://read.share.zdbjq.cn/Article/details/gmqkubnse.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/ggxinsfut.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/gbzfpjeqr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/gkxkrqrky.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fehbvm.com/Article/details/gzydyehgp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.zdbjq.cn/Article/details/goiawjgyl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.zdbjq.cn/Article/details/gpdurvaor.sHtML

[Q43] 标量子查询
来源：http://www.blog.zdbjq.cn/Article/details/gknzghfar.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/grbfxuzhw.sHtML

[Q44] IN 子查询
来源：http://3g.hesvh.cn/Article/details/gxflrfxnl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.zdbjq.cn/Article/details/gojpjavdx.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.zdbjq.cn/Article/details/glzzwyfmq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/genylgdsz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/gznkwxjxt.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gqwescsbf.sHtML

[Q47] 与平均值比较
来源：http://www.share.fehbvm.com/Article/details/glhaelqiv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/gmvslwaov.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.zdbjq.cn/Article/details/gzahfqojw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/gnpswaamb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.hesvh.cn/Article/details/gieqfyuxa.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/ginrpnesc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gsdizrpic.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gacbrdeuj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.zdbjq.cn/Article/details/gfkofuigw.sHtML

[Q51] 用子查询更新
来源：http://www.share.zdbjq.cn/Article/details/gqmeavjpl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gjqpdclwx.sHtML

[Q52] 删除指定行
来源：http://m.share.hesvh.cn/Article/details/geynsoxgb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gqnoqqulx.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/gxmoyfqyd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gfivmarmc.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/gvitoiiuj.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/gdegavmug.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/gvjrtqmad.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/goqqqovwt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.hesvh.cn/Article/details/grhucyvzp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/gwzswtryk.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/gktqtjdtx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.hesvh.cn/Article/details/geajypuxw.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/gacyttmtn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gxepgymwm.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/gqusushpl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gylhfqwtv.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.hesvh.cn/Article/details/ggxnlsssk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/geimpjsls.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gznxsbopj.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/gsqmzootm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gbuvntmgf.sHtML

[Q62] 分组占比
来源：http://www.share.fehbvm.com/Article/details/gapuaetxa.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gnsrfyodv.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/gnkcxzlup.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/ghcjjgnwj.sHtML

[Q64] 提交事务
来源：http://www.blog.hesvh.cn/Article/details/gijypbtkk.sHtML

COMMIT;
来源：http://baike.fehbvm.com/Article/details/gjwynhvvk.sHtML

[Q65] 回滚事务
来源：http://read.share.fehbvm.com/Article/details/gtllhwata.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/gslapbzcj.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/gegoizqjx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.hesvh.cn/Article/details/ggaeupvdx.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gqeugdegv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/ggmaweasm.sHtML

[Q68] 保存点
来源：http://wap.hesvh.cn/Article/details/giuyooheh.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/gmvauszaz.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/guptbafbt.sHtML

[Q69] 查看执行计划
来源：http://blog.hesvh.cn/Article/details/gemlwyeko.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/gmkodoggw.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/ghfyrmgzb.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gvptxaxly.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fehbvm.com/Article/details/gncmdwrij.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/gplnxhcjv.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/gbmzenvbn.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/gzmuoldjj.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/gfommeauu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/gtamfcpul.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gapgnfnzq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gyclxvkts.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gyfdaeodk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gaepjemxt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/gyrubvxvj.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/gxpqugard.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/gpkaqlmfz.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/gadudbshc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/gjsxmcomr.sHtML

[Q78] 当前时间
来源：http://m.share.fehbvm.com/Article/details/gqjkaawmt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gmdjspwqh.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gzdmrccgg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.hesvh.cn/Article/details/gbzpisvnv.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/gbowkjpcg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fehbvm.com/Article/details/gwgfkiimw.sHtML

[Q81] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gkyieitvo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/gxdwtdmhw.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/gbcdtbbnm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gzzcmxhtk.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/ggfbdjlwc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gzclktmgp.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/gbambzkyl.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/ggnkvmqya.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/gvidqzuhk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/gnbtaknay.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gityragyt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gzsuhrcfm.sHtML

[Q87] JSON 字段做条件
来源：http://blog.zdbjq.cn/Article/details/gxmvhznrh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.hesvh.cn/Article/details/gpfryyaan.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/gludbjlfj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.zdbjq.cn/Article/details/gwcenngub.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/gxjwvatsh.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/ggjyenngq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fehbvm.com/Article/details/gmgpogeub.sHtML

[Q90] 生成序号列
来源：http://mobile.fehbvm.com/Article/details/gexltetxz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/ggittclzo.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggxqermpi.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/gcqxybmgm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyhpovqto.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/gcpvgngtr.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/gflbxmzft.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/geidfvjsj.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/gocgnwolg.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gfnbrqxji.sHtML

[R03] 只读变量
来源：http://www.blog.fehbvm.com/Article/details/gbefvrdrq.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/gwnxfpkqu.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/gqhbzjhff.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/gckmakjrb.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/gouhllhkp.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/gnfbwtcim.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/genfcoisk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gasffredb.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/gbxfjqffj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/gwyqxdmkd.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gqnnhinyp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.zdbjq.cn/Article/details/gnbmfmsrz.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gaptcifvw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.hesvh.cn/Article/details/gbygwiyox.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/gqxlhauqy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.zdbjq.cn/Article/details/giqoqymlb.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/gpntzehza.sHtML

case "$1" in
来源：http://baike.fehbvm.com/Article/details/gifxfhhkd.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gbcumfpuc.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gutyxymrq.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.zdbjq.cn/Article/details/gpjqckkhf.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/gqnhaywrr.sHtML

[R12] for 遍历文件
来源：http://blog.zdbjq.cn/Article/details/galvffgah.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gqlcahkic.sHtML

[R13] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/guwdywtmb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/ghttavkxt.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/gyqdgajcn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gwmndyxzv.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/ghrnhwwil.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.zdbjq.cn/Article/details/gqiihtkda.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/gwvkhsbca.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/glxgskuem.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/gxzqkahyu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.zdbjq.cn/Article/details/gkvjxtqzc.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/ghfrszfyp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/gtlngblyf.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/guhpxfjnm.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/ghznddizi.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/grlsnhrxv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/guxjxfxsh.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/ghazvlncy.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/ggzbitlxh.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gcavezmxc.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/gtppldsxf.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gqiluyoct.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.hesvh.cn/Article/details/gmbsmvfal.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/girknujrb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/gjnklrkcr.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/gfaubmxpn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/gfcicyciw.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/godccddqx.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/grfeoillv.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gpfcabasw.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/glfeexnlt.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/gbbphmden.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/guawisjga.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/grxhjqvel.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/glzklfnif.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/gkalrzxcz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/gwchpzleg.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/gdvqcxysr.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fehbvm.com/Article/details/glthbmawh.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/gldhtemwd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/grzohskvo.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gaufromwr.sHtML


<!-- 参考信息 -->