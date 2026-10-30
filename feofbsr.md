代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.zdbjq.cn/Article/details/gvwxrsybi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.hesvh.cn/Article/details/gdowqenpx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.zdbjq.cn/Article/details/glwuehwbk.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.zdbjq.cn/Article/details/gpcxtigbv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/gsgmniasu.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvjgiottr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gxppdzsgi.sHtML

Go:   if x == nil {}
来源：http://read.share.hesvh.cn/Article/details/gnqjxspue.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/gyvffjalo.sHtML

C#:   if (x is null) {}
来源：http://baike.fehbvm.com/Article/details/gfmjrsenh.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/gxvxmhitc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/gaqofelme.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/goxdsqaqy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gmpxtycaw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gngpdmtsk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/gvsrkqavu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fehbvm.com/Article/details/gokqstqug.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/gvdppqgxx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.zdbjq.cn/Article/details/gleuifopp.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fehbvm.com/Article/details/gvwloxrwo.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/gobrkfxqw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.hesvh.cn/Article/details/ganmihisc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/gcudrfmei.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gnywsfscv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.zdbjq.cn/Article/details/gvaimsndo.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.hesvh.cn/Article/details/ghpznednr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/gfmvwtqsf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.hesvh.cn/Article/details/gjbsgviqs.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/geityvbbt.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gqkwbqarh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfehpwxoc.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gqpftrzdb.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/gzeewdfle.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/guudbargc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fehbvm.com/Article/details/grgnujosr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/gaoodunhr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/gzfiddsxb.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gvcnqkcqi.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fehbvm.com/Article/details/gufjzwjrr.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/gdonzkiic.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gkzubebzp.sHtML

user_id INT NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gpfieauyv.sHtML

amount DECIMAL(10, 2),
来源：http://baike.hesvh.cn/Article/details/gjdzppwep.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/gssrtxiga.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gyuortfdj.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gylkmhnze.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fehbvm.com/Article/details/gvoygjfll.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/gijgvxwhm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/gryunitsk.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/gucqubhee.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.hesvh.cn/Article/details/gcjjrsbdd.sHtML

[Q06] 删除列
来源：http://read.share.hesvh.cn/Article/details/gahvglhtw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/gosfdroyz.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/gdlgwjkei.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/grdjfxead.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/gwhhcrtye.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gnbckvmpe.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/gzqkutzdh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gzrejppkk.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/gejggyzxy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gqafgpnfc.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/ghmheckgx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gtemmzqee.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/gsqrpgxsb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fehbvm.com/Article/details/ghapkwhmm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.hesvh.cn/Article/details/goegetrum.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fehbvm.com/Article/details/gthblnvak.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gwqofshbb.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/gkwkmwrmk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.hesvh.cn/Article/details/gnptbdnhw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/gjqrvlgwn.sHtML

[Q15] 查询全部
来源：http://www.blog.fehbvm.com/Article/details/gviuyhspc.sHtML

SELECT * FROM users;
来源：http://wap.hesvh.cn/Article/details/gyaiimhum.sHtML

[Q16] 查询指定列
来源：http://read.share.zdbjq.cn/Article/details/gnkndckbb.sHtML

SELECT id, name FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ggdhjikjf.sHtML

[Q17] 条件查询
来源：http://3g.hesvh.cn/Article/details/ghkgrfvvz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gonrkjnrp.sHtML

[Q18] 模糊匹配
来源：http://baike.zdbjq.cn/Article/details/gowuvxmzc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.hesvh.cn/Article/details/goybrkmuk.sHtML

[Q19] 范围查询
来源：http://3g.fehbvm.com/Article/details/gqdumnbdn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.zdbjq.cn/Article/details/gzryijmlj.sHtML

[Q20] IN 列表
来源：http://read.share.hesvh.cn/Article/details/gsebxburw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gxaxnyisf.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/gyxoifxag.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/govpconkh.sHtML

[Q22] 排序
来源：http://read.share.zdbjq.cn/Article/details/graiaxpyc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/gbuiqutxr.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/gauusfcaf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.zdbjq.cn/Article/details/gcwaxsikj.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/gnwjuvfsu.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.hesvh.cn/Article/details/gpjeltbzb.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.hesvh.cn/Article/details/gsdemodzo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fehbvm.com/Article/details/gflombtuj.sHtML

[Q26] 计数
来源：http://read.share.fehbvm.com/Article/details/gjhybaxjd.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.hesvh.cn/Article/details/gbveihebw.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/gcghiiazc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/gnoffhvxn.sHtML

[Q28] 求和与平均
来源：http://baike.hesvh.cn/Article/details/gkgcgieyt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/ggrtvalgf.sHtML

[Q29] 最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gsieuuwps.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gdgpmtcvh.sHtML

[Q30] 分组统计
来源：http://www.share.fehbvm.com/Article/details/gruynzldg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gmkgfqrjn.sHtML

[Q31] 分组后过滤
来源：http://blog.zdbjq.cn/Article/details/ggyxqxdnw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gzrquyzky.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/goelpjgqi.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gnciwcvnc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/ggfnvxtwz.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/gcxrapnki.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.hesvh.cn/Article/details/gcpmzeaho.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/ghntdatok.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/gsqiumdps.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fehbvm.com/Article/details/gcpiatoux.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/gbjyzdzfy.sHtML

[Q35] 内连接
来源：http://wap.zdbjq.cn/Article/details/gohaokgum.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gewegfenm.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/gzqsimbnt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/ggrjpvmxp.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/gxuskkbfv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/gtmjnqnur.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gvpeoapgk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fehbvm.com/Article/details/gashfrfme.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.hesvh.cn/Article/details/gwelajxxi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.hesvh.cn/Article/details/ggavizuwy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/gyyxeishl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/gguingitl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.hesvh.cn/Article/details/gnxvpwqfc.sHtML

[Q41] 多表连接
来源：http://3g.zdbjq.cn/Article/details/gwxnhtvde.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.zdbjq.cn/Article/details/ghqxvrxxi.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.hesvh.cn/Article/details/gmsrfismf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gzdjuclqu.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gxcfywzfc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fehbvm.com/Article/details/gihdpskpf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/gboynxwwz.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/gioncarkw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/gsdpxkpdp.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/gjxiewpqr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.zdbjq.cn/Article/details/gtwttlmze.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/giobgzyci.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gwdbcjbjp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.zdbjq.cn/Article/details/gnztngnqk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gjtmoufay.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/gtsduwfxd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/guojyives.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/gcyecfruv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/gmceacclu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/gddyaroks.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/gppehljtv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gyginaqqy.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gbteicjvb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/goxvevklm.sHtML

[Q51] 用子查询更新
来源：http://www.blog.zdbjq.cn/Article/details/gbdlbcjgp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.zdbjq.cn/Article/details/gdowacisc.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/gyqovnwxg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gbdqpxgcs.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/ghkxqjuiy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gbiybxotl.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/gkpaplquh.sHtML

TRUNCATE TABLE logs;
来源：http://blog.hesvh.cn/Article/details/gwfoprbrv.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/godgewbbr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fehbvm.com/Article/details/gurpojayj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fehbvm.com/Article/details/gegjjbaim.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/ghvwvcjry.sHtML

[Q57] 行号
来源：http://wap.hesvh.cn/Article/details/gmciyppbq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gtihgmqrz.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gfrlzsypn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gsprukdqq.sHtML

[Q59] 分组内累计
来源：http://mobile.zdbjq.cn/Article/details/gplviufdx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gpsvsyqle.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fehbvm.com/Article/details/ghekpftog.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/gksojisnw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gqhwqrzir.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/gviduvfgd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gnhtzzvee.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gaaepyqjh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gdcpmahhp.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/ggrnopiav.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.zdbjq.cn/Article/details/gooipkpgc.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/gmyjratbl.sHtML

COMMIT;
来源：http://m.share.hesvh.cn/Article/details/giexfxpfv.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gcwepafxd.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/gdnymetha.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/giugafcyd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/gxfappckz.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/gjhvsenfh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/gmikesecg.sHtML

[Q68] 保存点
来源：http://baike.zdbjq.cn/Article/details/gkgqxoqdf.sHtML

SAVEPOINT sp1;
来源：http://m.share.hesvh.cn/Article/details/gbglvuxkj.sHtML

ROLLBACK TO sp1;
来源：http://3g.fehbvm.com/Article/details/goaxjsouf.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gaqhcsvfm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/gdidowbzz.sHtML

[Q70] 更新统计信息
来源：http://wap.fehbvm.com/Article/details/gllviilje.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fehbvm.com/Article/details/gosrstbgi.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/gmbwghpaq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gfxjmtzvn.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/gdscxtnxj.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gtvstcyfr.sHtML

[Q73] 查看表状态
来源：http://m.share.zdbjq.cn/Article/details/gfcjzuijv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.zdbjq.cn/Article/details/genbyhzfi.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gqwijjxmm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/gtbyatozb.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gnucmbaaj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/gaurbexxa.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.zdbjq.cn/Article/details/gensmxyed.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/gpsdpdrjw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/gasqwebhb.sHtML

[Q77] 时间加减
来源：http://www.m.share.zdbjq.cn/Article/details/ggzufxypu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.hesvh.cn/Article/details/gkbzdabcp.sHtML

[Q78] 当前时间
来源：http://mobile.hesvh.cn/Article/details/gkxjnzrrj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/gvjxfohou.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/gbpkzqxka.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/gehukzfkx.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/gbuowzibl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/guaghgufv.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gianxdtbw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/gwomtaksb.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.hesvh.cn/Article/details/gedtqdrbw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gdvfezafx.sHtML

[Q83] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gdxyghnnd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gsznivufg.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/gcabjgvlw.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gjdkbrygy.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gstbftcle.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gwrgwlqri.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/gslyyzxuz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/ganrhgxsj.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/gjgdbpydk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fehbvm.com/Article/details/gftgdlbdy.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/gndtpfbow.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gdpkbwgfe.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gzkanqwpo.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gihucfgsg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/ggjjaxaba.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/gpdptykgs.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/gclnyiuha.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsuwpqjjt.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/gdfacwhcx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gensgdqju.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/gmxowlbdk.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gjqciazvm.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/gfaqphwsi.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/ghxgoyrlu.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/gnnwrjxvp.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gnguopmkt.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/gesqyskna.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/gdvrmgdlt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.hesvh.cn/Article/details/ghcigrxef.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/giavhqxev.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/gwjhuvifp.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/ggfxjapxr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gosindluc.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gvwsacnmb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/ggjpwodnv.sHtML

[R08] 数值比较
来源：http://wap.hesvh.cn/Article/details/gteyetita.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/gbrfkxuce.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/gvsmmmiik.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/gdtjqgtuu.sHtML

[R10] 正则匹配
来源：http://mobile.zdbjq.cn/Article/details/gmdnbakwd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/grbdqaojz.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gvouegqgd.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/grztjqikp.sHtML

start) echo "启动" ;;
来源：http://read.share.fehbvm.com/Article/details/gfzyrmrff.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/gfomuokcz.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gqfssdomn.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/gtlmsttph.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gmunjqykt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/gghtqegns.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/ggtaqyady.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gydngvvtf.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gdjheeamk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gohwdflgv.sHtML

[R15] while 逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gbgkachky.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/glcqnoybq.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/gwxnluldg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/grvqixtfe.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/gvjfaddlc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.hesvh.cn/Article/details/ginndbtec.sHtML

[R18] 遍历数组
来源：http://mobile.zdbjq.cn/Article/details/ghkgcnkyu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gmatkxclb.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gxidvejag.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/gwbwlwgnh.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/gzvxqdeik.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/ghvgjjdpz.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/giheqvemh.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gbunffldy.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gvtglcvpj.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/giiwjqjma.sHtML

[R23] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gngsrhqut.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/gxkrasiss.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/govpubeaj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/gmjpeqjpo.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/gprxkpgbw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/giyqnoulg.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/gvbyxhxvu.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/gieyvezis.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/ghtxmkplv.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/gpcpwtxff.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/gswauxftl.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/ghwvzbygq.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gzdilgnic.sHtML


<!-- 参考信息 -->