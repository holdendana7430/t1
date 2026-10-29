代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/goscewcux.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fehbvm.com/Article/details/gkfabtmlg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gaacqpkzk.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/gybimxykf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.zdbjq.cn/Article/details/ggpvcooil.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/gxtrvphie.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fehbvm.com/Article/details/gtmtianfw.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.hesvh.cn/Article/details/gdsvcxxtn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/ghbetcamk.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gjizjnljo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gnxaqftrp.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/gmumzizqz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/gdoecrxbp.sHtML

C#:   if (x is null) {}
来源：http://3g.hesvh.cn/Article/details/gwsdnqywz.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/gxqwxmxzf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fehbvm.com/Article/details/gfqblqxdj.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/geguoijxf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gpkygrblq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gdezxumzh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/goxdchxxg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/ggyudunnc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/gxwvhloxa.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.zdbjq.cn/Article/details/guawfhasn.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/gblwoqibk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.zdbjq.cn/Article/details/grejigstn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/gbbvzcqlt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fehbvm.com/Article/details/gclswwwyk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/gzkhzjljq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.hesvh.cn/Article/details/gxuizrtpp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/gjguurbnl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fehbvm.com/Article/details/gbujaurwy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.zdbjq.cn/Article/details/gottiogsr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvzagyrpc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/gfieupbqe.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqinvjhkd.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/gndxinlur.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/gmzoishjh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gqhdbqtlk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gugtmovgi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.zdbjq.cn/Article/details/gffkzqqqj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/gttibakxt.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gtaemohlb.sHtML

[Q02] 创建带外键的表
来源：http://read.share.hesvh.cn/Article/details/gpcooysab.sHtML

CREATE TABLE orders (
来源：http://baike.zdbjq.cn/Article/details/gxbjudnon.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gcguvjtea.sHtML

user_id INT NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gcqdmgeef.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/gslausrxc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/gcrtcrbvp.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/ghtfhrpbh.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gpsuiyqyc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.hesvh.cn/Article/details/gjqzqtmyw.sHtML

[Q04] 修改列类型
来源：http://baike.hesvh.cn/Article/details/gxlhizxup.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.zdbjq.cn/Article/details/gzpnyqulj.sHtML

[Q05] 重命名列
来源：http://www.blog.fehbvm.com/Article/details/guwwyjlso.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.zdbjq.cn/Article/details/gekdzstaf.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/gibslqmsu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fehbvm.com/Article/details/gteemimfo.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/gkrzrctqu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.zdbjq.cn/Article/details/gmyidxeeq.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/gcatozpqo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gyralezup.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/gbfjnhrfy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gktgapoje.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/gteijfbzo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/ghxlqowpu.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/gbuafeome.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gexwbjiwx.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gubtrflmo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fehbvm.com/Article/details/gavhiecrr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/guwyzhnzb.sHtML

[Q13] 忽略重复插入
来源：http://3g.zdbjq.cn/Article/details/gyaqlvwwu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gkfobttvm.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/gltnudjoy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/gxxiagbjt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.zdbjq.cn/Article/details/gwabnukpz.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/gqinjhfmx.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/gmwckqolx.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/gdlwuiyca.sHtML

SELECT id, name FROM users;
来源：http://wap.fehbvm.com/Article/details/gtegnkibr.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/gemvkolph.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/gnmecjcme.sHtML

[Q18] 模糊匹配
来源：http://baike.zdbjq.cn/Article/details/gwqzbxhxw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.hesvh.cn/Article/details/gftsvxlsk.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/gvlwtgadv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/ggbikjyoq.sHtML

[Q20] IN 列表
来源：http://read.share.fehbvm.com/Article/details/gkqnltaxz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gekvqgahz.sHtML

[Q21] 空值判断
来源：http://www.blog.zdbjq.cn/Article/details/gubpzopqs.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gwgwiswjk.sHtML

[Q22] 排序
来源：http://blog.fehbvm.com/Article/details/gamgcrxzv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/girkxkwki.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/gqqitzjtb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/gksidgrke.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/gqavnzpzm.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.hesvh.cn/Article/details/gpsikzyvv.sHtML

[Q25] 只取前 N 条
来源：http://mobile.zdbjq.cn/Article/details/ghffhtygn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/giurfrkng.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gvpcmhfbx.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.hesvh.cn/Article/details/gucotahdj.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/grkvmmcad.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/gaqcysobu.sHtML

[Q28] 求和与平均
来源：http://read.share.zdbjq.cn/Article/details/gffezrqih.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/ggprhwbgc.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/gvslurqmr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/gczepvmoo.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/ggrykbjan.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gjeyluqej.sHtML

[Q31] 分组后过滤
来源：http://m.share.hesvh.cn/Article/details/gyrogzyzu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.hesvh.cn/Article/details/gbhhhscvu.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gaoylqhnw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/goojsfuof.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.hesvh.cn/Article/details/gkzgryobf.sHtML

[Q33] 多列分组
来源：http://www.m.share.hesvh.cn/Article/details/gigvwcxic.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.zdbjq.cn/Article/details/gmkiuibnl.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/gmklecrzl.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/glenrxlek.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gbhmtblmo.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/gpxpgbgys.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/gdieihowd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gqyhnhkfh.sHtML

[Q36] 左连接
来源：http://www.blog.zdbjq.cn/Article/details/giqhmbkcw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/ggsffpgnw.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/gblnsifxr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/gtdemsgtc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.zdbjq.cn/Article/details/guqkpogyz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/gnmpykuim.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/gqwwmmhvl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/gwwhszwoe.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.zdbjq.cn/Article/details/gqikyfwzd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/gevurgiwt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/glzaqoygb.sHtML

[Q41] 多表连接
来源：http://baike.fehbvm.com/Article/details/gnkqenrye.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/gejmglxlz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fehbvm.com/Article/details/gwsjfxtbg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/gwyxhenjj.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.zdbjq.cn/Article/details/gztsmjajv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/guyrjbahq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/gzbzrsbxf.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gnpsxrjww.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/ggcjbgaqi.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/gefbrrtlc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/gglogyusa.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/geurrkuix.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/ggbbljvzo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/gjdlmvjqx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gbgiydchh.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gcizhzzez.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fehbvm.com/Article/details/gexmzfedt.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.zdbjq.cn/Article/details/ghfrjnidq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.hesvh.cn/Article/details/gzvaqlzmk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/gsebvxyll.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/gfqcvtlfj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gnygroyup.sHtML

[Q50] 批量更新
来源：http://3g.fehbvm.com/Article/details/gthgawpva.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/gcjryrjjn.sHtML

[Q51] 用子查询更新
来源：http://3g.zdbjq.cn/Article/details/gnbaxskbz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.zdbjq.cn/Article/details/gboglfukp.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/gknpvhdqs.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gbwnmlyvs.sHtML

[Q53] 按条件删除
来源：http://blog.zdbjq.cn/Article/details/gyzcxluyr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gfkzhzccw.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/gpvfehfsd.sHtML

TRUNCATE TABLE logs;
来源：http://wap.hesvh.cn/Article/details/gnztdirtz.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gtpodsqqe.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fehbvm.com/Article/details/gvlvmfjjz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/glhvbfeds.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gezfmqjjv.sHtML

[Q57] 行号
来源：http://3g.fehbvm.com/Article/details/gccdnjifr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/gijbffbmx.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/gtzdwnvvv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fehbvm.com/Article/details/gwppnngkn.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/gjrhjwozp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gftfxpxwr.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/gxeykhnov.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gyrqbvyxx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gesyeclmd.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/geytvzten.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/goyivjchg.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/gcbhiwiit.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gfijulruo.sHtML

[Q63] 开启事务
来源：http://mobile.zdbjq.cn/Article/details/gvdwhlfqe.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/gylewuszk.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/gtjkxukjz.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/gshkmninr.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gkoyizueu.sHtML

ROLLBACK;
来源：http://www.m.share.zdbjq.cn/Article/details/gidgqghey.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/geyrsazue.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/gwummgljd.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gukrwhlzk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/ggkanrkeg.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gflcamevo.sHtML

SAVEPOINT sp1;
来源：http://mobile.zdbjq.cn/Article/details/gxkwtzbrn.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/gkjswzjka.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/grnzxjvst.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/gtbwllmdo.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/gbbffhyte.sHtML

ANALYZE TABLE users;
来源：http://blog.hesvh.cn/Article/details/gvsgzjtnu.sHtML

[Q71] 查看建表语句
来源：http://m.share.fehbvm.com/Article/details/gpeokhyfu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.hesvh.cn/Article/details/gprkhpydn.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/gdhvrbtfb.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gkeuunmko.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/gxuhjmhcx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/gusiulapj.sHtML

[Q74] 强制使用索引
来源：http://baike.hesvh.cn/Article/details/gawgxdikt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/gldsyuune.sHtML

[Q75] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gdccechuq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/ggxsbumwf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/gyslzzdia.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/gohyrmbfd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fehbvm.com/Article/details/gfqfntxsz.sHtML

[Q77] 时间加减
来源：http://m.share.zdbjq.cn/Article/details/gnelbvsld.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/gmjbcjfyz.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/gpbstzarf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fehbvm.com/Article/details/gbcobvrtz.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gmjtsjkca.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.zdbjq.cn/Article/details/gczsfgyyt.sHtML

[Q80] 字符串截取
来源：http://read.share.zdbjq.cn/Article/details/giuojzzla.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gimeisobr.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gnxjokorb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/ggacmonxd.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/gkiujcjpy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gsplffbef.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gkdpanpbf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gkismarqo.sHtML

[Q84] 去除首尾空格
来源：http://m.share.zdbjq.cn/Article/details/gorxadwip.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gxdipocnw.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/guvquqzqb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/gkdklltek.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/gbnjotbsq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/gosylmxof.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gdxslqohd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.hesvh.cn/Article/details/goymvihme.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/gnysrllvi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.hesvh.cn/Article/details/gdbemdzdv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fehbvm.com/Article/details/gofbgojpf.sHtML

[Q89] 判断表是否存在
来源：http://blog.fehbvm.com/Article/details/gdsierctw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gxubgztok.sHtML

[Q90] 生成序号列
来源：http://3g.hesvh.cn/Article/details/gbfcdahhg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/gsxylsvwt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gckgwnfjk.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/ggspzkxpi.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnkkqozwl.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/gclssvkps.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/gbdvepzfx.sHtML

set -euo pipefail
来源：http://wap.fehbvm.com/Article/details/gejffecxz.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/gwlnzxfpp.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/gaorjbdnd.sHtML

[R03] 只读变量
来源：http://baike.hesvh.cn/Article/details/gtcejgbep.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/gvyxxqcqq.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/gquwwwohy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/gszhrmjkl.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gfkbztvgx.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/ghmgyplwr.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/gygjoiqkr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gghdegdzu.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/gmcbbuvnz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fehbvm.com/Article/details/gfpbbylwj.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gispprxyo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/gcyxngcva.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gnmeutitq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fehbvm.com/Article/details/gzgqaecrr.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/govjigtrk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/gozxncmqu.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/gutfokace.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gpykwoyfz.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gcisiudzu.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gxlnuxlze.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.zdbjq.cn/Article/details/gwxlxyvgh.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gzcvjzfhe.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/gyrmijfoz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/gjerkbzdp.sHtML

[R13] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/gfwczodyi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gqzecprkq.sHtML

[R14] C 风格 for
来源：http://read.share.zdbjq.cn/Article/details/gcwbrbaxr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gwjviuhua.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/gytrqlcxz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/gxgckdeta.sHtML

[R16] until 等待条件
来源：http://m.share.hesvh.cn/Article/details/ghhvnessy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gtaugfaqe.sHtML

[R17] 数组定义与取值
来源：http://www.share.zdbjq.cn/Article/details/gdrztbbkx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/gwqmhbepk.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/gnyiteswe.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fehbvm.com/Article/details/gmmeneehz.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gzfitfgcw.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gkalxmols.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gyxqwljzo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/gprghessb.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/gxjzxwtab.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/grxknuzey.sHtML

[R22] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gguvlwbwk.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gqtvghgpd.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/glpriwuqd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/gjxwxrxhp.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gvhfstwhf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/gujzozbhr.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/govriefkq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/gocevtuwj.sHtML

[R26] 命令替换
来源：http://3g.zdbjq.cn/Article/details/guqkfnuki.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fehbvm.com/Article/details/gvpqxuydh.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/gmjqospnn.sHtML


<!-- 参考信息 -->