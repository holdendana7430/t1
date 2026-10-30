代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/gzypjzook.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.zdbjq.cn/Article/details/gauqvytkf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/grcouyhcg.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.zdbjq.cn/Article/details/glzwplfmv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fehbvm.com/Article/details/gqwjfyrje.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/gnykhezxe.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gcbcaihzr.sHtML

Go:   if x == nil {}
来源：http://m.share.fehbvm.com/Article/details/goeqgsrbu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fehbvm.com/Article/details/gmvplcier.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/gdjngbhse.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/gocgzpsar.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/glnvprodl.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/gkeuycdvk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gaphktlet.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gjgwefolw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.hesvh.cn/Article/details/gocjyigui.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/gqpetuxoq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/gyjfqpbuz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gefgbhikc.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/gvnwpddrh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/gawfqtteu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fehbvm.com/Article/details/gnwuvpfcq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.zdbjq.cn/Article/details/gwikbexkd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gtwisxysl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/galrembdm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.zdbjq.cn/Article/details/gqmgvtscd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/ghekzxabt.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fehbvm.com/Article/details/gyueqevbg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqwfjgwyd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gewtosulh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gslfyaktp.sHtML

[Q01] 创建表
来源：http://mobile.fehbvm.com/Article/details/grclszmcc.sHtML

CREATE TABLE users (
来源：http://m.share.hesvh.cn/Article/details/gsmvonmfl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gshbwkhns.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gngwclnwb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gszpjlewp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/gakyzortx.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/grazkoozd.sHtML

[Q02] 创建带外键的表
来源：http://baike.fehbvm.com/Article/details/gppstwqyk.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/gbntlburt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/ggtqnnrfy.sHtML

user_id INT NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gitzzmzzv.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/ghzbaaisu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/gighzcpsc.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gwsgwzubk.sHtML

[Q03] 增加列
来源：http://3g.hesvh.cn/Article/details/gualbrdkg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/gtysosthx.sHtML

[Q04] 修改列类型
来源：http://www.share.hesvh.cn/Article/details/gnqmdhmrj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/goacwvzlc.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/gizqqrspb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fehbvm.com/Article/details/gywevxath.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/gjrbqektn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.zdbjq.cn/Article/details/gehrxuzsw.sHtML

[Q07] 删除表
来源：http://baike.fehbvm.com/Article/details/gtzqqktfb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fehbvm.com/Article/details/glahvwdja.sHtML

[Q08] 创建普通索引
来源：http://mobile.hesvh.cn/Article/details/gfqifckhn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gspcrolrj.sHtML

[Q09] 创建唯一索引
来源：http://baike.zdbjq.cn/Article/details/gcmwzxsgr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/goodtgdna.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/guqsskemr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/gbztkmrxe.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/gpdmccclc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/grgokvnpt.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/gmdbamkph.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/gakzqvqoh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.zdbjq.cn/Article/details/gviytojjl.sHtML

[Q13] 忽略重复插入
来源：http://m.share.hesvh.cn/Article/details/gmvtdvojp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.hesvh.cn/Article/details/ghmwkkdrk.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/gxqkdiqkn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.hesvh.cn/Article/details/grdojqopx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fehbvm.com/Article/details/gwgkczeko.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/gzqgcvgvc.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gwoagiwsy.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/gehotxzfc.sHtML

SELECT id, name FROM users;
来源：http://baike.hesvh.cn/Article/details/grwpwuykk.sHtML

[Q17] 条件查询
来源：http://baike.hesvh.cn/Article/details/gvpxypddz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gmjjrrrnb.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/geadqrxru.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.zdbjq.cn/Article/details/ghfixtyrm.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gnhfgufbv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/ggydlkwgh.sHtML

[Q20] IN 列表
来源：http://3g.hesvh.cn/Article/details/gfqourzvt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/gkskcaxph.sHtML

[Q21] 空值判断
来源：http://www.blog.zdbjq.cn/Article/details/gtzuxogcr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/gxiszemvy.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/gvhinmfnq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.hesvh.cn/Article/details/gmefirrli.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/giezxwlyh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/glxjsflas.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/gficpaata.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/gackgrjag.sHtML

[Q25] 只取前 N 条
来源：http://blog.fehbvm.com/Article/details/gumsnqcmx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/gctiukkkl.sHtML

[Q26] 计数
来源：http://www.share.fehbvm.com/Article/details/giiumkddq.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.zdbjq.cn/Article/details/guqsbevti.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/gqheyrfly.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/gpgwmekmp.sHtML

[Q28] 求和与平均
来源：http://www.m.share.zdbjq.cn/Article/details/ggdvakbmt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gwcscxlqh.sHtML

[Q29] 最大最小值
来源：http://www.blog.fehbvm.com/Article/details/ghlqjnggd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/guqdbelsp.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/gxrudhlps.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gzscwkdty.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/gpwwrzscs.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.zdbjq.cn/Article/details/ggtptxqwl.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gyyrpequr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gkjlkszhr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.hesvh.cn/Article/details/gaagswzvu.sHtML

[Q33] 多列分组
来源：http://www.share.fehbvm.com/Article/details/gpgaoihwi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/guioxvofl.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/gdcxvqhnc.sHtML

SELECT * FROM (
来源：http://mobile.hesvh.cn/Article/details/gepkkojpw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/gvvvzuyiz.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gwlaptmoo.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/gpobgrcbv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/goloijkvs.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/gbflafyqu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gcphdzehw.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/gelqennql.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.zdbjq.cn/Article/details/gitcpykko.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.zdbjq.cn/Article/details/ghtismdfc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/gxnixscpg.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.hesvh.cn/Article/details/grcynelgv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/gqmbovabb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/gpszxbgpt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.zdbjq.cn/Article/details/guavwutna.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/gaybygtwq.sHtML

[Q41] 多表连接
来源：http://wap.hesvh.cn/Article/details/gqbbtifrb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fehbvm.com/Article/details/gipunukoz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/gejllmirg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/gfxmfpudp.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fehbvm.com/Article/details/gcvdeovhr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/gkjfekjya.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/gxsbdmvug.sHtML

[Q43] 标量子查询
来源：http://baike.hesvh.cn/Article/details/guoeuleuq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/gevqunapr.sHtML

[Q44] IN 子查询
来源：http://blog.hesvh.cn/Article/details/gqypfqsof.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/ghfkfqzls.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/ggofndsoo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/grkboqqum.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/gdrpgdvcf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gcxxorvio.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.zdbjq.cn/Article/details/glrxgyvxi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gexduhhks.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/gofkcyrgw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/ghtputdvo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/gibqmzbqg.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/ghscpccdi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/glboodzep.sHtML

[Q50] 批量更新
来源：http://3g.zdbjq.cn/Article/details/gxgnwkrfx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gmhmtzshk.sHtML

[Q51] 用子查询更新
来源：http://wap.hesvh.cn/Article/details/gxtbytghb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fehbvm.com/Article/details/gkmfmkspa.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/gxtsfxkep.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gjbgnfmeo.sHtML

[Q53] 按条件删除
来源：http://www.share.zdbjq.cn/Article/details/ggibexsko.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gojplhwfo.sHtML

[Q54] 清空表
来源：http://wap.fehbvm.com/Article/details/gonvkzxwz.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fehbvm.com/Article/details/geyuqjtbc.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/gpufvqrjg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gfbwrmjzk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.hesvh.cn/Article/details/ghunxbsqc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/grfegqhgw.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gjgnmmpfd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gqwxxooxm.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/goqfdukip.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/ghrsdwbqn.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/gwxmfzoxl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gymupmdrm.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/ggbazcvax.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.hesvh.cn/Article/details/grbfcosis.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gojieopmc.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/grhxcmurj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/glkqlanqq.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/ggrmgcboe.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gpmulxqch.sHtML

[Q63] 开启事务
来源：http://www.blog.hesvh.cn/Article/details/gkkaqrvft.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/grhezfift.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/gsncnibij.sHtML

COMMIT;
来源：http://wap.fehbvm.com/Article/details/gsycxafva.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/gtatbrfrz.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/glqvfwktk.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/giunnlfey.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fehbvm.com/Article/details/guqqizvoq.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.hesvh.cn/Article/details/gsqnuctko.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/gimfrvyjj.sHtML

[Q68] 保存点
来源：http://www.blog.fehbvm.com/Article/details/gkrdorwxm.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gaedwokyx.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/gtpffyozl.sHtML

[Q69] 查看执行计划
来源：http://baike.hesvh.cn/Article/details/guzvfrtbp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.zdbjq.cn/Article/details/gycfwogrc.sHtML

[Q70] 更新统计信息
来源：http://m.share.hesvh.cn/Article/details/gwzjbjbft.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/gawbykzzf.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/gnghhnkft.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.hesvh.cn/Article/details/gxbycrabs.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/gmysmdlrz.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gjjjfzcyh.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fehbvm.com/Article/details/gigfolsom.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.zdbjq.cn/Article/details/gpuahwmkw.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/gteiufylu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/gjnywwmwj.sHtML

[Q75] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gxedkhbwp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/gwpxlwbpp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/gepywxobq.sHtML

[Q76] 按天统计
来源：http://www.share.zdbjq.cn/Article/details/gcclpgbkb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.zdbjq.cn/Article/details/gsqjebxdg.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/gkfhldlgv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fehbvm.com/Article/details/gkircezyd.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/ghcovtoxz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/gpfdepaxp.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gqxgyjjvc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/gbeflniqf.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gbledvrpu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ghdpvkdjl.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gkjxqfiot.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fehbvm.com/Article/details/gjiawkbgx.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/ghpzpvosc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gfveokmub.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gagtohyqy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gcawvgmee.sHtML

[Q84] 去除首尾空格
来源：http://m.share.zdbjq.cn/Article/details/grzwwxnwm.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gehdrbjrq.sHtML

[Q85] 数值取整
来源：http://blog.fehbvm.com/Article/details/gvhxemgqj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/gmikskerv.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gvksrrnwt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/gysufbzeh.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/gfxeuchnu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.hesvh.cn/Article/details/gkrwornym.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/goxrmziik.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/gqddbvwbn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gywxhdhcm.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/goagbuaxh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/gwyytxqwx.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/gsnnsjbcv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/gqteunjvn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmpsjucfg.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gkyabfuaz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpqwyebnk.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gsubpkwks.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gzaszkjbc.sHtML

set -euo pipefail
来源：http://read.share.zdbjq.cn/Article/details/gphtjtqtu.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/guwvggraq.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fehbvm.com/Article/details/gajelltfg.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/gsjdaiywv.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/ghujoxhsy.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/gaybknbpm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/glddpddgq.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/gbjitqdzr.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gpkzfsgcg.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gjpmbafay.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gtgtfrqtn.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/gnylrkeqm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gmhgmqgrt.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gtmzqasrn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/gydfmspub.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gwxxojlcs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/gpbcqisqx.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gidfiywev.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.zdbjq.cn/Article/details/gfhhrisal.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/ggxfsolhe.sHtML

case "$1" in
来源：http://baike.fehbvm.com/Article/details/gaklnqxet.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gpbdjpfgg.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gqziojtny.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gvdhwnjtz.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gwcrybmxg.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gwxoqkxnp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gvdocdbsh.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gczrqsujd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gudzjkigk.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gkzlqpabk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gmnacffra.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gazikvoxo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/glhtanrjs.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gmtqcpdmx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gagbnvkbl.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gglnndohi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/ggukpgdqv.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/gfkufcekw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fehbvm.com/Article/details/gtocoxpbb.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/gricshppp.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/gljfivaau.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gltocuush.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/grelpfhti.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/getoojbvq.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/grxwtapjy.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gqreadbvd.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gltyydsok.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gpagndzmt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gsgzlfvcd.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gifusmjjc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/gmrmiitkl.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/gohicxhfn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/gkkraxusu.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gtmzpvrek.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.zdbjq.cn/Article/details/gmhgbzyjk.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/ganyegfjt.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.zdbjq.cn/Article/details/gyzlnozhs.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/gbhmhmybu.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/grrwypwyw.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gvjmczhre.sHtML


<!-- 参考信息 -->