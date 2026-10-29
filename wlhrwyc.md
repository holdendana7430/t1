代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fehbvm.com/Article/details/gxuuetzid.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/gwcjvxokn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.zdbjq.cn/Article/details/gzrhjhknv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gpffhudyi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gtrpsnlxb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/gianukqxo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.hesvh.cn/Article/details/gnipnukre.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/gwzuhkybm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fehbvm.com/Article/details/gmecfwebu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/gsfkynabx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gwmmmghfg.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.hesvh.cn/Article/details/gyzuhoojq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gcsyaljva.sHtML

TS:   if (x == null) {}
来源：http://blog.fehbvm.com/Article/details/gtpkovxjc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gneljagxr.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/gffqyxwlx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/ggxyausfm.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/gylpvnvve.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/gjrgbuwht.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/gqjlbskrs.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fehbvm.com/Article/details/gbfwixalm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gqjbymkyr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gmnccsjpp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/gnpinfydc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/gstsvmprn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gfexzuhfa.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/geitedton.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/ghkozkvdj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/guetqvggo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fehbvm.com/Article/details/gddpmklbl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gbtymvnrs.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gicrgcclw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.hesvh.cn/Article/details/gulkjoruo.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fehbvm.com/Article/details/gvgocdarb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/gypmdltyt.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fehbvm.com/Article/details/gniqbuduh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/giygyylqn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gpfikjseo.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdmcphsfr.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/gbywnniww.sHtML

CREATE TABLE users (
来源：http://read.share.hesvh.cn/Article/details/giedhoggv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gyzyyyyoe.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gnhdgeyps.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/glugpjzqd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/geyacqhwp.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gdllqkinq.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/gdlydbftp.sHtML

CREATE TABLE orders (
来源：http://www.m.share.zdbjq.cn/Article/details/gqukoiuxz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gexipeyia.sHtML

user_id INT NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gpaxuisvm.sHtML

amount DECIMAL(10, 2),
来源：http://blog.hesvh.cn/Article/details/grrwrjrwa.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/glvlzrkyq.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gbfiqbcdn.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/gbyqmlzpx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fehbvm.com/Article/details/gzyoymeuq.sHtML

[Q04] 修改列类型
来源：http://blog.zdbjq.cn/Article/details/gutbqhexc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fehbvm.com/Article/details/gmqptpyaq.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/gplfpzddq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.hesvh.cn/Article/details/grenjtbub.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/gtponrzbk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.zdbjq.cn/Article/details/gxwckekhf.sHtML

[Q07] 删除表
来源：http://www.share.zdbjq.cn/Article/details/gznoqueok.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.hesvh.cn/Article/details/gsxkkalux.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/gdergycdi.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/grybwpmyt.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/gjjdsqznt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/getjxohrr.sHtML

[Q10] 插入单行
来源：http://www.blog.fehbvm.com/Article/details/gnpiiremo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gjrmmgqdh.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/gqvafprnl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.hesvh.cn/Article/details/gmtgakiyj.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/ghfenryfk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.hesvh.cn/Article/details/gaguxehmb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/gnbwzxbrk.sHtML

[Q13] 忽略重复插入
来源：http://mobile.hesvh.cn/Article/details/gqzjloxgm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fehbvm.com/Article/details/gjsdhckva.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gmvdbwsoc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fehbvm.com/Article/details/gqzwdwjyj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/gvnvzjfdo.sHtML

[Q15] 查询全部
来源：http://www.m.share.zdbjq.cn/Article/details/gnpqgknhh.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/gjtnqatwr.sHtML

[Q16] 查询指定列
来源：http://baike.fehbvm.com/Article/details/gwjnlvcgu.sHtML

SELECT id, name FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gkmcjuypp.sHtML

[Q17] 条件查询
来源：http://read.share.fehbvm.com/Article/details/gaswvyhis.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fehbvm.com/Article/details/gzkmzoeas.sHtML

[Q18] 模糊匹配
来源：http://baike.hesvh.cn/Article/details/grzmmrkow.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fehbvm.com/Article/details/gouyihfkc.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/gutfsdlnl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.zdbjq.cn/Article/details/gmyywhloe.sHtML

[Q20] IN 列表
来源：http://wap.hesvh.cn/Article/details/ghdachdhk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/grvllpjfc.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/gaujooxij.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/gwmowkuqi.sHtML

[Q22] 排序
来源：http://m.share.fehbvm.com/Article/details/guxbnzrfm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.hesvh.cn/Article/details/gcfvmbhfe.sHtML

[Q23] 分页
来源：http://3g.zdbjq.cn/Article/details/gleicqmpl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fehbvm.com/Article/details/gcttxywed.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/gkbdcoydf.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gizsymfim.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.zdbjq.cn/Article/details/glcmpmvcu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.zdbjq.cn/Article/details/gzaxxhleb.sHtML

[Q26] 计数
来源：http://read.share.fehbvm.com/Article/details/grtglxekc.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/gruxkwbtt.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/gpofbizay.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fehbvm.com/Article/details/ggzjptvgz.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/gzlgaaukn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gprdsrjiu.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/gwpuczmfy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gfvntbxag.sHtML

[Q30] 分组统计
来源：http://3g.hesvh.cn/Article/details/gpijoxptz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/guhpgzqxs.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/gdupgvuil.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/gfowsvtyq.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/ggtmjrrok.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gndcqmqaz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fehbvm.com/Article/details/gnyzvqkfb.sHtML

[Q33] 多列分组
来源：http://www.share.hesvh.cn/Article/details/gqvlnrhxy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/gxacxzozx.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/gbqiyhdtj.sHtML

SELECT * FROM (
来源：http://read.share.zdbjq.cn/Article/details/ggjkwmwpq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fehbvm.com/Article/details/gpmwoqdld.sHtML

) t WHERE rn = 1;
来源：http://mobile.hesvh.cn/Article/details/gsptgyvkg.sHtML

[Q35] 内连接
来源：http://www.blog.zdbjq.cn/Article/details/gpdthjfog.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gvnpzneqc.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/guglqlwys.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/ggxjkndeh.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/gofauwhny.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.hesvh.cn/Article/details/guzpeytcl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.zdbjq.cn/Article/details/gvpghssbt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/ghvoqemum.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fehbvm.com/Article/details/gsfsotbot.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.hesvh.cn/Article/details/giirzqvtr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/gjyppkbbp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.hesvh.cn/Article/details/gqosvjivi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.hesvh.cn/Article/details/ganytdpsd.sHtML

[Q41] 多表连接
来源：http://www.blog.fehbvm.com/Article/details/gvwbitdrk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.zdbjq.cn/Article/details/gpmtbkeys.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/gwxqxbopw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.zdbjq.cn/Article/details/gzjnggfcx.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gtnxbmypu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.zdbjq.cn/Article/details/ghbhfuxgs.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/gtgufuxff.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gwxidgrqv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/goxrqpopi.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/ghedkmpmj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gfwvzfhtx.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.zdbjq.cn/Article/details/gnudhreny.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gepzymsmq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/gxsgbupke.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gpapfeeco.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/gmmajpwyi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.zdbjq.cn/Article/details/gbzsawubb.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.hesvh.cn/Article/details/glkwhzkul.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.hesvh.cn/Article/details/gsfscjhgu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.hesvh.cn/Article/details/ggpsrqpfe.sHtML

[Q49] 更新单行
来源：http://baike.zdbjq.cn/Article/details/gmftgrngw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gnuniprsa.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/griygqsvf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gwlgyuigj.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/ggoybzkrt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gdgyzspwh.sHtML

[Q52] 删除指定行
来源：http://www.m.share.hesvh.cn/Article/details/gytutljcr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gkmldwshf.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/gjqzjolsm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.hesvh.cn/Article/details/gxrcxrhzd.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/gjyitghla.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/gkfqificx.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/guodjgtok.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.hesvh.cn/Article/details/gbbfvvhjv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.zdbjq.cn/Article/details/ghaguzmzq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/gcdjpdtev.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/gsikfvxel.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fehbvm.com/Article/details/gjmtzitbl.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/gwpplchqs.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gktpxihea.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/ggfngebyz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gyauswttq.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/gnvrwsmah.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/gsoysbwqz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gjueawvmn.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/gjjzdused.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gdnkkxtpk.sHtML

[Q62] 分组占比
来源：http://m.share.fehbvm.com/Article/details/gjmozpjjk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/glizjedlx.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gayxoqymt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/gzfxwtsbq.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/gnsjwjsrv.sHtML

COMMIT;
来源：http://wap.hesvh.cn/Article/details/gpmthwdip.sHtML

[Q65] 回滚事务
来源：http://blog.zdbjq.cn/Article/details/gqfkmpkps.sHtML

ROLLBACK;
来源：http://3g.zdbjq.cn/Article/details/gnnodfvji.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/glddigsun.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/gdactwfiz.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/gyglzwxmm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fehbvm.com/Article/details/grwdevdvu.sHtML

[Q68] 保存点
来源：http://read.share.fehbvm.com/Article/details/gqitvybxa.sHtML

SAVEPOINT sp1;
来源：http://read.share.fehbvm.com/Article/details/gomjhtqow.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/gdhnzwgjb.sHtML

[Q69] 查看执行计划
来源：http://www.blog.hesvh.cn/Article/details/gtssjgjoc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.zdbjq.cn/Article/details/gnghrraxy.sHtML

[Q70] 更新统计信息
来源：http://mobile.hesvh.cn/Article/details/gogjrqppe.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/gyimeinmq.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/gxbfzstps.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gtnyaehpp.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/gndcezsel.sHtML

SHOW INDEX FROM users;
来源：http://wap.fehbvm.com/Article/details/gxjbbzxzu.sHtML

[Q73] 查看表状态
来源：http://3g.zdbjq.cn/Article/details/gyaruajti.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fehbvm.com/Article/details/gsibpszed.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/golwtpgsx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gfnzdikoy.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gpxxhvegf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/gzeehpsda.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/geyyydtgp.sHtML

[Q76] 按天统计
来源：http://mobile.hesvh.cn/Article/details/gjbtriwwv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/gefsudlkm.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/gxetyirhj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.hesvh.cn/Article/details/gvypfqgcw.sHtML

[Q78] 当前时间
来源：http://m.share.zdbjq.cn/Article/details/gqpoeavbr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/gjpvolptz.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gixcaolja.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/gydoqvoda.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gkhvkbfdf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gslqztihl.sHtML

[Q81] 字符串替换
来源：http://baike.fehbvm.com/Article/details/ginumavml.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/gdcuhwlwj.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.zdbjq.cn/Article/details/grezsuhrz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gmrstmgzd.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gybflgpue.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gjkqjxefh.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/guvlyzfkn.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gjifgwnob.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/grnqtciby.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gtefmgfpm.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/gjzmbsrmr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/glgvcgvho.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/gwimldewa.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/gycxdxgqs.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/gdooibchg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.hesvh.cn/Article/details/gmjyimhgz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gkfzlsmuo.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/geqseunwe.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/gcihfsutw.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/gbpxqmcyh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/gxpqtfdst.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfszoufeb.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/gpmqazavy.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gatgrmdwm.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/gzwsdzchg.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/gamvgdopf.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gvhphlgvf.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/gwuimeyci.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/gewgngxws.sHtML

[R03] 只读变量
来源：http://mobile.zdbjq.cn/Article/details/gpsnhrrqi.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/gtisokxuk.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/ghrmhgrex.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/gxrvojjen.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/glmwhhtmh.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/gjffivwin.sHtML

[R06] 判断命令是否存在
来源：http://mobile.zdbjq.cn/Article/details/gnsghknma.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gfqxzkykl.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/grfqirpib.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/gkjnovpih.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gichilhju.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.zdbjq.cn/Article/details/gdodcytbn.sHtML

[R09] 字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gnpidiozq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/grjkdhbmy.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/gfaernyxp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gmaqgulww.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/guahlexbg.sHtML

case "$1" in
来源：http://3g.hesvh.cn/Article/details/gibrbscch.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gxawaijyi.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/gjhpifamh.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fehbvm.com/Article/details/gjxzfdxav.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/ggnatvmwj.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gxyrccbno.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/gaybinjdh.sHtML

[R13] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gsxoivoff.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gjrxcaxdt.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gcrpwicze.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gcjxgionx.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gkoqsyxgd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/gzbvoqzye.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/gptgureju.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gzhdvuolg.sHtML

[R17] 数组定义与取值
来源：http://www.share.fehbvm.com/Article/details/ggldtccbx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gqounjefx.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gibpwbmli.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/gsmsyjqpn.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/ginvuwlxa.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/gsjhzvibv.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/gznbcohfg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/gdshhowjh.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gnwtouskz.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gqdbrvnxc.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gxmbvwjwa.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/gugvkwglk.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gqlcuwsoh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.zdbjq.cn/Article/details/guwzdinbo.sHtML

[R24] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gapeighvr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/gyadfkdtj.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fehbvm.com/Article/details/glsljzmox.sHtML


<!-- 参考信息 -->