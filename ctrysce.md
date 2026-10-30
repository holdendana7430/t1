代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fehbvm.com/Article/details/gzdgrkqkr.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/gyzslcjdf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gaymhvhgk.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/gokwmqvbm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/gmhnhfgfm.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/geygylnsy.sHtML

[P07] 防抖与节流
来源：http://blog.zdbjq.cn/Article/details/geomraqof.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/gwybnuszt.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/gudtbwufl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gaeaxunss.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gcpiqwtfq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/guvskxsoj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.zdbjq.cn/Article/details/gfwpexxeo.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/gatkfgumz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/ghwgffpdi.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.zdbjq.cn/Article/details/gxsvikift.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.zdbjq.cn/Article/details/gzvhoxsst.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/gsjoipism.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fehbvm.com/Article/details/gyymxqhhi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gwgovqbnq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/gfqrxsaal.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.hesvh.cn/Article/details/gsyywwdth.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/gavfnfgid.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fehbvm.com/Article/details/glorjzbwe.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqtdzkxki.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.hesvh.cn/Article/details/grwphmgrv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkyirpywh.sHtML

[Q01] 创建表
来源：http://blog.hesvh.cn/Article/details/gquykoedm.sHtML

CREATE TABLE users (
来源：http://read.share.zdbjq.cn/Article/details/gbmaxsqdm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gxorsubuk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gegiyvlpf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/gevvishml.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/gatlvyoir.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gtmblojlr.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.zdbjq.cn/Article/details/gfbqkmbsq.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/goevntccw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gidvoszzm.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gtkkjhcda.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/gnvbgxhic.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/glmydqcwl.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gietcriji.sHtML

[Q03] 增加列
来源：http://www.blog.fehbvm.com/Article/details/gqcfqqqyu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.hesvh.cn/Article/details/gauprvtdh.sHtML

[Q04] 修改列类型
来源：http://read.share.fehbvm.com/Article/details/gopvyhopf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/grjdndotd.sHtML

[Q05] 重命名列
来源：http://read.share.fehbvm.com/Article/details/gauudvpwt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/gpifohjfm.sHtML

[Q06] 删除列
来源：http://wap.zdbjq.cn/Article/details/gkyiaqtqe.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/gazqyskaq.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/gxvxlpfjz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/gbgilnmuo.sHtML

[Q08] 创建普通索引
来源：http://www.share.fehbvm.com/Article/details/gtwatunel.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gcykkfeif.sHtML

[Q09] 创建唯一索引
来源：http://blog.zdbjq.cn/Article/details/gnrlawovt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gfusdjxby.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/gzntsxsao.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/gubtfhwid.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/goofvusny.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/gdhcyflhy.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/ghckirdok.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.zdbjq.cn/Article/details/gsptxjuli.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fehbvm.com/Article/details/gpejcqysf.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fehbvm.com/Article/details/gmzftaqfl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fehbvm.com/Article/details/glsamyqak.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.zdbjq.cn/Article/details/gmycamzsr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.hesvh.cn/Article/details/gutpnxikq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/gnkbrwdwh.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/gywecbqip.sHtML

SELECT * FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gwjwneloj.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gbblueozy.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gigwxsbub.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gmlmnlxav.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gnhezhkai.sHtML

[Q18] 模糊匹配
来源：http://baike.hesvh.cn/Article/details/gcqdgrzss.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.hesvh.cn/Article/details/ghiaexirn.sHtML

[Q19] 范围查询
来源：http://wap.hesvh.cn/Article/details/gvjynhnua.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/gaydqkdsc.sHtML

[Q20] IN 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gewmvwesc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/gaxdfidaq.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/gkstevqqs.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/gqzhzfbgr.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/gjvyxjgur.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/gbknlailr.sHtML

[Q23] 分页
来源：http://baike.fehbvm.com/Article/details/ghvaaunci.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.hesvh.cn/Article/details/glvowicov.sHtML

[Q24] 去重
来源：http://m.share.fehbvm.com/Article/details/glzuphzrr.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/glgymovkr.sHtML

[Q25] 只取前 N 条
来源：http://baike.fehbvm.com/Article/details/gtxwfqcdo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/gdlqkesyl.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/gznybqdip.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gdsibjrin.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/gzdqibcfr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gknuapcrr.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/gwkcwwptg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gkppxoomi.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/gvtmlgrfd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fehbvm.com/Article/details/gfwwmcvrr.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/glahdjcjq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gzpyiprxz.sHtML

[Q31] 分组后过滤
来源：http://baike.zdbjq.cn/Article/details/ginbivaob.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.zdbjq.cn/Article/details/gqhwdhqoa.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gwequbvge.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gbouhrsbz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fehbvm.com/Article/details/gffctrmvc.sHtML

[Q33] 多列分组
来源：http://baike.hesvh.cn/Article/details/gylexvxpg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/gxuvlbrqm.sHtML

[Q34] 每组取第一条
来源：http://www.share.fehbvm.com/Article/details/gsvqpuppq.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/gqcmvjqiy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gsbxqzrfu.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/gnznnljuw.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/ghqnimrso.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gmmrsqzxd.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gndamofdv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gempysqzl.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/gvypwatau.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fehbvm.com/Article/details/ghrinsapo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/gcjvcnfae.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fehbvm.com/Article/details/gxykrfqhx.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.zdbjq.cn/Article/details/gpfejpokz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/gewhgexra.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/gwiexamsl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/gdrvvhqxp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.hesvh.cn/Article/details/gbcsoibre.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/givhfwzlo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fehbvm.com/Article/details/groesqlzs.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/gxztzoaax.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.hesvh.cn/Article/details/gzzxkeymt.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/gbfricmyv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/gbrnxyafb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/gfintllss.sHtML

[Q43] 标量子查询
来源：http://www.blog.fehbvm.com/Article/details/gbywygdza.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/ggebdjerm.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/gdjdlovox.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/giivivcoz.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/gxynvoszs.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gifzettum.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gevrbzuhv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gnoldjroj.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/gvjakgdiy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.zdbjq.cn/Article/details/gemkgeswj.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.zdbjq.cn/Article/details/glyenwler.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fehbvm.com/Article/details/gktposjod.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/gmzbfiyui.sHtML

[Q49] 更新单行
来源：http://baike.hesvh.cn/Article/details/gbmyykelu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gcqsqntin.sHtML

[Q50] 批量更新
来源：http://blog.zdbjq.cn/Article/details/gnyjogjvg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.hesvh.cn/Article/details/golrhnryq.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/gqhbeqzep.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/gnshjnjpo.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/gjptqonte.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/geunzkrth.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/gyfnhoxis.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gzmsknrpb.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/gbnbeamin.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/glitkrfxf.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.zdbjq.cn/Article/details/gsmpbewhx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gwznvbvfv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/ggisqwalh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gemuyawpl.sHtML

[Q57] 行号
来源：http://wap.hesvh.cn/Article/details/gdbdsokks.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gnrabcrvn.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/gzkjafnwp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gnlsrfnbc.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/gldzfcjcp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gqauyrthb.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/guklfbsxf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/gsrvbfwyn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/glnnfwdir.sHtML

[Q61] 移动平均
来源：http://wap.fehbvm.com/Article/details/gstjujjue.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gxarzzskg.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gxympdjsj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gcwhfsorx.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gledxslbu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/gbpjekwuu.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gvgyxxcch.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/gkuzcsjtm.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/giwxqrjew.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/gbfqgcune.sHtML

[Q66] 行锁查询
来源：http://wap.zdbjq.cn/Article/details/gslviqsem.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.zdbjq.cn/Article/details/gchtdzmfd.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/giuceoscw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/gjeshlmwh.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gvbbxotkr.sHtML

SAVEPOINT sp1;
来源：http://wap.hesvh.cn/Article/details/gxdklpiyv.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/ghyxvdygo.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gidbaykkn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/gffndeiev.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gaygpphce.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/gpdsqlafb.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/gopklpexf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gaehspsjs.sHtML

[Q72] 查看索引
来源：http://www.blog.hesvh.cn/Article/details/gmbxqudte.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/gfhocfruu.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gosziaoph.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/gbwxwbfdf.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gfuxaayml.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/ghnbzvqci.sHtML

[Q75] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gdzouhfcz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/glphblsxw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.hesvh.cn/Article/details/gypwfkdar.sHtML

[Q76] 按天统计
来源：http://www.blog.hesvh.cn/Article/details/gimelibpu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/gutvqyehk.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/ggtmqvtwh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/gqcmwjxra.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gkanrzxys.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/githjuewt.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gocngwdbi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.zdbjq.cn/Article/details/gjpnpycho.sHtML

[Q80] 字符串截取
来源：http://baike.zdbjq.cn/Article/details/glcuitajp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gbuxdbxxg.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gvzlwhhew.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/ggcnvgrwh.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/gjhmfyaaj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gmeryurbi.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gadlmlhkf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gynapuojy.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/gjopsksds.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/grmwupbqp.sHtML

[Q85] 数值取整
来源：http://www.share.zdbjq.cn/Article/details/gyitkxhjl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/gqbbudutt.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/gjcsaegaw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/gjydeztzl.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gaulbbrqx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/ghkozdokc.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/gtifgwthz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gndqdenxp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.hesvh.cn/Article/details/gxbwycrnp.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gzxiruvml.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gdksazlzl.sHtML

[Q90] 生成序号列
来源：http://3g.fehbvm.com/Article/details/ggvugaueo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/grqvvqtdf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmizwjqes.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/glybwfxug.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbswopqdo.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/guvmjmych.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gvxtqkdfu.sHtML

set -euo pipefail
来源：http://blog.hesvh.cn/Article/details/gxjmemjeq.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/gksgsvlfc.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gehxkvbnf.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/gstrzscui.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/gxhgssmhw.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/gqvbvnrjz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/ggaewefjp.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/grxdwrvqk.sHtML

name="${1:-default}"
来源：http://www.share.hesvh.cn/Article/details/gqddjxdtu.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/gaqvekopj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gepnfqbad.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/gwxoqqzbu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/gprzrzjxf.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/gbgrhvnkc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/ganmitdwr.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gikcgqnkz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/ghfrsnalt.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/gnqymlimp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.hesvh.cn/Article/details/gthzbdfgd.sHtML

[R11] case 多分支
来源：http://read.share.zdbjq.cn/Article/details/gtrdeabfd.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/gtrsxczbv.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/gadzklwcd.sHtML

stop)  echo "停止" ;;
来源：http://read.share.hesvh.cn/Article/details/glcmhmnny.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gjyuxpqot.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gguryokit.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/ghkuzykux.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gdssqeenh.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/ghhqabcgj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gxywqgwwx.sHtML

[R14] C 风格 for
来源：http://baike.hesvh.cn/Article/details/gpwltjlfu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gkpenmgjy.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/ghhxwrqjh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gqevfpozj.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gjwxgtive.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gqvlybxth.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gwrrnfueo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/govfxxtfo.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/gqkqluwbp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gflvmynfd.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gbjuhsiuc.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/gdsupprra.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fehbvm.com/Article/details/gemfiyzoh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/gxodvjhzl.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/glwuytvpm.sHtML

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/ghflkywpg.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gneotmzhn.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/gdqckownt.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gbqfecphm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/gisakncxk.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/grtpszsje.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/gxtauihjw.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/ghqgcbast.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/gwymcyglo.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/gwxbjujsl.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gvlipvlxk.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/gqvukemqm.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gxozgmtdk.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/gfgnwqdll.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/gfxgcpaew.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gbgkjjcsg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fehbvm.com/Article/details/gfumzbjqu.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/gmarnauot.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/gddbkxqjb.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/gxkfbnndn.sHtML


<!-- 参考信息 -->