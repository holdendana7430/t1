代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/goawqmnxv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/gskqoydur.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fehbvm.com/Article/details/gthlrzbxr.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gcghfgfkn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/gsueubxxz.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gsymsuixk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/ghaxinyaq.sHtML

Go:   if x == nil {}
来源：http://www.blog.zdbjq.cn/Article/details/gxgwhclmj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fehbvm.com/Article/details/gdbgqiwmr.sHtML

C#:   if (x is null) {}
来源：http://baike.hesvh.cn/Article/details/gvmsvxllt.sHtML

[P07] 防抖与节流
来源：http://m.share.hesvh.cn/Article/details/gqpcwzujq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/glslunhvd.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fehbvm.com/Article/details/gfqejcmfi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gffrokkva.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gyynmrxds.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gwfgrkjou.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.zdbjq.cn/Article/details/glsygcifq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/gjehylbdi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/ggsduoims.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/gpudolahd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.hesvh.cn/Article/details/ghlsbharl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.zdbjq.cn/Article/details/gjdjkbydb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gskxvgjmp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/guyhynuan.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/gjcqjjvwk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.hesvh.cn/Article/details/gbrwuuxxa.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/gohpxvqci.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.zdbjq.cn/Article/details/gjjsrxafu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gyudnzvei.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/ggjbxqpuf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gudzpxcbu.sHtML

[Q01] 创建表
来源：http://www.share.fehbvm.com/Article/details/gxrahoodw.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/gqarcrgps.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gdgqstzmn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gvbyyrytx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.hesvh.cn/Article/details/gfznambnh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.hesvh.cn/Article/details/gbesytjuw.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gnjqlpwqg.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fehbvm.com/Article/details/ggrdasqaa.sHtML

CREATE TABLE orders (
来源：http://m.share.fehbvm.com/Article/details/gbozbnlep.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gmubztajf.sHtML

user_id INT NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gpysbdmxb.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gqhvbsmxw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/geauvqzzy.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gzygeezay.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/gbyhuavct.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.hesvh.cn/Article/details/gzpxzyigh.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/gzrqlmugc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.hesvh.cn/Article/details/gcsaxctbz.sHtML

[Q05] 重命名列
来源：http://mobile.zdbjq.cn/Article/details/gwjpknfid.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/grcwxrmon.sHtML

[Q06] 删除列
来源：http://blog.zdbjq.cn/Article/details/ghjgpxfyi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/gsdztcblq.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/gtfwrdpxs.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fehbvm.com/Article/details/gyvwiqhgm.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/gvoshfign.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/ghgkdnagv.sHtML

[Q09] 创建唯一索引
来源：http://wap.hesvh.cn/Article/details/gcizjbjth.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/ggiyvnige.sHtML

[Q10] 插入单行
来源：http://www.blog.hesvh.cn/Article/details/gyjajsxbj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/gzxpmydwl.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/gusjvfnvr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/giftkkztq.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fehbvm.com/Article/details/gvltpgjbp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/gtogbupxf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/gnjaejmdp.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/giwkahdok.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gyzcoonrz.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.zdbjq.cn/Article/details/gjzjwfmzy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/gxmghgizv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/gzokczrgj.sHtML

[Q15] 查询全部
来源：http://m.share.fehbvm.com/Article/details/gdhhwugvs.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/guubzvkle.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/gvgowwxgd.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gqwfvglcv.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gyoncblxo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.hesvh.cn/Article/details/ghjbwzehs.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/ghqbctlkd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/ggsznzajg.sHtML

[Q19] 范围查询
来源：http://wap.hesvh.cn/Article/details/gncbruzwl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/gwhnfcotb.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/gmzmvsmnk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.hesvh.cn/Article/details/grbyakgsi.sHtML

[Q21] 空值判断
来源：http://www.m.share.hesvh.cn/Article/details/gfposrddg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gndmflhvp.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/gulvnkowe.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gdkcndxql.sHtML

[Q23] 分页
来源：http://3g.hesvh.cn/Article/details/ghtfpmrst.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.hesvh.cn/Article/details/gzlfhtznl.sHtML

[Q24] 去重
来源：http://blog.hesvh.cn/Article/details/gxlxkwryi.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fehbvm.com/Article/details/gacbyxekz.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/gtsehmnwd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.hesvh.cn/Article/details/gjqksxwcq.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/gorvxnasy.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gzetqmpok.sHtML

[Q27] 条件计数
来源：http://wap.fehbvm.com/Article/details/gbflcmoxs.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/goxrxppuh.sHtML

[Q28] 求和与平均
来源：http://baike.zdbjq.cn/Article/details/gqtssqwfb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gmemrfbql.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/gcxssfzrq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gpofwhgyq.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/gmzdzsplm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/ghqdioqnw.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/gfvzwvxjc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/gkuglafen.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/geuqsedjf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gwinvfgzl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/gutdnjtur.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/gbtzqvnkf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.hesvh.cn/Article/details/gzpguyuki.sHtML

[Q34] 每组取第一条
来源：http://m.share.hesvh.cn/Article/details/grwwaakuc.sHtML

SELECT * FROM (
来源：http://www.share.hesvh.cn/Article/details/gyfzupdvl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.hesvh.cn/Article/details/gffpvfspj.sHtML

) t WHERE rn = 1;
来源：http://m.share.fehbvm.com/Article/details/gevzsgugl.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/ggnqhtlhm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gevysyiom.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/gavabfzey.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gjxlfslgo.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/gkaegitxi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fehbvm.com/Article/details/gbjvlmhhm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.zdbjq.cn/Article/details/gujamjxli.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.zdbjq.cn/Article/details/gnfuukrvx.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.hesvh.cn/Article/details/gcwbqfifw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gakdepwpo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/gjyirbkhe.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/gacgsfdwr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.zdbjq.cn/Article/details/gygllkvsi.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/gdlwkoazn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/gkftsrjdz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gzszvubiz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/ggilxlnxj.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fehbvm.com/Article/details/gxwywvqab.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/gnsyvxsij.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gyltxfpos.sHtML

[Q43] 标量子查询
来源：http://3g.zdbjq.cn/Article/details/gmphzflsi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/gylozqpbi.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fehbvm.com/Article/details/ggkbldcrg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/ghvkdwpqj.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/gwivffyfw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/graipepjz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.hesvh.cn/Article/details/gvvqqsvta.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gzwabftjw.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/gqkzhnxfs.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/gdqxtqlgt.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/ghleqvozn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.hesvh.cn/Article/details/gujkeehhu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/gfulbchzo.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/gcfbsxrkp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gykjhzblz.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/gzkiqbixf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/gqpxouxox.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.hesvh.cn/Article/details/grhroajul.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fehbvm.com/Article/details/gzesfejuh.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/guhqcukzx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gyliglhss.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fehbvm.com/Article/details/gkbqwssgz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gcwmwfikr.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/gpzmhmdji.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/gruyonrzg.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.hesvh.cn/Article/details/gqbyzgquu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gnuxeldey.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/ggudlwnhz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gavljosfe.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/gbmpawuha.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gmmcbruij.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/ghmzgsbsp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gqglqtelw.sHtML

[Q59] 分组内累计
来源：http://mobile.fehbvm.com/Article/details/genpcvanp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/ggdzzkkkk.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fehbvm.com/Article/details/gcxlsualj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/gdoivqbza.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/gzbkfxalv.sHtML

[Q61] 移动平均
来源：http://baike.zdbjq.cn/Article/details/gsfflhomo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/govakzozb.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gsrzwpzez.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/geczujune.sHtML

[Q63] 开启事务
来源：http://www.m.share.hesvh.cn/Article/details/geajepeeo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/ghcouoief.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/gtozsrpye.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/ghntoqqsv.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/govwzcwwd.sHtML

ROLLBACK;
来源：http://baike.hesvh.cn/Article/details/gagzijrrs.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/gjjzvvzwj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.zdbjq.cn/Article/details/glzhpgfbn.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gxbrlblou.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/ggwyijpmx.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/gnpnnpbyf.sHtML

SAVEPOINT sp1;
来源：http://wap.hesvh.cn/Article/details/gpxqdegav.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/ginmyjxwr.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gpydlsaff.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fehbvm.com/Article/details/ggocmarpm.sHtML

[Q70] 更新统计信息
来源：http://mobile.hesvh.cn/Article/details/gmxsqqgvb.sHtML

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/gbypcpivo.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/ghywmgmfa.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gmltxhrhw.sHtML

[Q72] 查看索引
来源：http://blog.hesvh.cn/Article/details/geioryyan.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/goshnfwxs.sHtML

[Q73] 查看表状态
来源：http://3g.zdbjq.cn/Article/details/gnxzggdsm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/gskhqwmyj.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/gzgisgqjg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.hesvh.cn/Article/details/ghbaowdwr.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gtjalvqxo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gkorbcbyz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/gesrxlamm.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gdflldygb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.zdbjq.cn/Article/details/ghssbdnvb.sHtML

[Q77] 时间加减
来源：http://read.share.zdbjq.cn/Article/details/gjynakuje.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/gfmiajgou.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gjalzmjae.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fehbvm.com/Article/details/gcpdaiiha.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/gffikqrkz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/ggnqqbezn.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/ghniwtfml.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gqqpnxnww.sHtML

[Q81] 字符串替换
来源：http://blog.fehbvm.com/Article/details/grjvzapnx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ggsqubioq.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/gamorasla.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gixzeblxh.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gtknjyken.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/ghklvlssd.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gzpqdzqxf.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gewghfcph.sHtML

[Q85] 数值取整
来源：http://3g.zdbjq.cn/Article/details/ghnwjntau.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/grnldmdej.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/ghziesztp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/gebzoxstc.sHtML

[Q87] JSON 字段做条件
来源：http://baike.zdbjq.cn/Article/details/gzurtdoqg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gnzqfzamh.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/gkenpgsjo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/gczshcrjn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/gpqhwskws.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/godokcwmj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/gvoqepxwv.sHtML

[Q90] 生成序号列
来源：http://3g.hesvh.cn/Article/details/gctzbojgy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fehbvm.com/Article/details/gbfvfjvpd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gakatmpvg.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gsgqtxeze.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gskcbyzzo.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/gmwwonqte.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/gwnagymty.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gfqilmxwn.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/grbrkpttl.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/gcashebfz.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/gqmqnlxmg.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gphmhdstl.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/gukzbtuav.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.hesvh.cn/Article/details/glfxzlvht.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gqervcewr.sHtML

name="${1:-default}"
来源：http://3g.zdbjq.cn/Article/details/gppotikyz.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/gipzeyalh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/grhatwazo.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gqiahbejc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.zdbjq.cn/Article/details/glviersyq.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/gjrkpicjo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.hesvh.cn/Article/details/gdqcqzvoa.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gdliuejes.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/gkevhfqfq.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/glumrbuoj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gfjmqrtka.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/gfeeckprg.sHtML

case "$1" in
来源：http://3g.zdbjq.cn/Article/details/gzhxtysvt.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gimwzxxlr.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/goateefqd.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gxhojzxbm.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/gjoivhjuj.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/gfadnuzbp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gjabgyoeg.sHtML

[R13] for 计数循环
来源：http://baike.fehbvm.com/Article/details/gmuultssy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gkkztcqxg.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/gariqmble.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/grduwtzub.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/gkpovybld.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/gojgoywxn.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gnsjegigc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gwyfhmaar.sHtML

[R17] 数组定义与取值
来源：http://3g.fehbvm.com/Article/details/gqbpbfzfl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gsnpdyghv.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/guqrvlunv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/gptctqxzw.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gyseevpyv.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/gzfizfnqp.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gjukwqpll.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gsosyleoo.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gqtqqvria.sHtML

echo "${#s}"
来源：http://read.share.hesvh.cn/Article/details/gwiyslrfl.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/ghszknqsj.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/gzbsafnqd.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gumrvldhn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/gbhqjyqsp.sHtML

[R24] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/geztgiwyo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/grekefblk.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/gzzeexcjx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.hesvh.cn/Article/details/gwkgjvgyp.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gndwqnrhg.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/gucundjkt.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/gjxhcmund.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/gbdrbybbi.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/gdvtzxiit.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.hesvh.cn/Article/details/guajqqvpj.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/glzbxvbge.sHtML


<!-- 参考信息 -->