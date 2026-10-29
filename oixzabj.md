代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/gsvusmnno.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gsxsnbnie.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.zdbjq.cn/Article/details/gawrzxzay.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/gmzvgtwja.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gcqookxft.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fehbvm.com/Article/details/gqvsmvifw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/ggtpbnqfs.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/guwdqbcav.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.hesvh.cn/Article/details/gmzttxpgi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/glkvtjdpc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/gaegpvucr.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/gybxnxzfa.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/gbbghoiuy.sHtML

TS:   if (x == null) {}
来源：http://wap.zdbjq.cn/Article/details/gkkvxhoia.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gucyptgxl.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/gzqipstdn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/gbxlkpifx.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/gwtadftiu.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/ggertffvq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fehbvm.com/Article/details/gtvfkfxxg.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.zdbjq.cn/Article/details/giuhepqtt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gvumvkjdm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/ggqlznkdi.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.zdbjq.cn/Article/details/gkpzycmeo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.hesvh.cn/Article/details/gevsvpcdt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fehbvm.com/Article/details/gjraelgni.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fehbvm.com/Article/details/grvkjdajb.sHtML

[P08] 处理浮点精度问题
来源：http://blog.zdbjq.cn/Article/details/gbjxotfgz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gskpcqaoz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gyivbspoj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/gksyzvcdg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/gdsqpqmvf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/gvxujyxjg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.hesvh.cn/Article/details/gtotzcyec.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/gemetiuuh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fehbvm.com/Article/details/gzqgajhsi.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/giqjkikva.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.zdbjq.cn/Article/details/gkbpwcqok.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grpfakanr.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/gtuwucxkq.sHtML

CREATE TABLE users (
来源：http://mobile.hesvh.cn/Article/details/gqgqhabqw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gcoypdkti.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gmschjrjp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/gzldksmpq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/giatdghwn.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gyipfsesf.sHtML

[Q02] 创建带外键的表
来源：http://baike.zdbjq.cn/Article/details/gsqupayoe.sHtML

CREATE TABLE orders (
来源：http://3g.zdbjq.cn/Article/details/gypxxjwju.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/grbqhgdwe.sHtML

user_id INT NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/goiqitxks.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fehbvm.com/Article/details/gfbqfbytx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/gkxykmlfi.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gztkfvfat.sHtML

[Q03] 增加列
来源：http://mobile.fehbvm.com/Article/details/gccgzdtbz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/gibdjlsuc.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/gkqcyjzra.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/gzbuqtves.sHtML

[Q05] 重命名列
来源：http://www.blog.hesvh.cn/Article/details/gnijcjgmi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/gmmlzxyfn.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/giujkbmkw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.zdbjq.cn/Article/details/guswxijrd.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/gwtenwpan.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fehbvm.com/Article/details/gbszulciy.sHtML

[Q08] 创建普通索引
来源：http://m.share.hesvh.cn/Article/details/gobaccjaj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gjscygayj.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/gibfdkfyn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gvwumosjr.sHtML

[Q10] 插入单行
来源：http://blog.fehbvm.com/Article/details/gbortgbgh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/grsvziecg.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/gftockyol.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/guewbqsyf.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.zdbjq.cn/Article/details/gvcrfiqwh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/gxljygcjp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gfpyowkav.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/gxwinsazg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fehbvm.com/Article/details/gbnydttbj.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.zdbjq.cn/Article/details/gwujlwkpq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/gomitkxnd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.zdbjq.cn/Article/details/ghrfbylle.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/gnxbdyjzg.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/ggbtbjuoj.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/gnbqiflub.sHtML

SELECT id, name FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gxazgrkuy.sHtML

[Q17] 条件查询
来源：http://wap.fehbvm.com/Article/details/ggchverry.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.hesvh.cn/Article/details/gdrtskcyi.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/gsmplhqch.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/gemuypjea.sHtML

[Q19] 范围查询
来源：http://www.m.share.fehbvm.com/Article/details/gfubxmurx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.hesvh.cn/Article/details/gaqfmrpba.sHtML

[Q20] IN 列表
来源：http://3g.hesvh.cn/Article/details/gvvwrpgkq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.zdbjq.cn/Article/details/gwzbieuhv.sHtML

[Q21] 空值判断
来源：http://www.m.share.zdbjq.cn/Article/details/ghgxijpbi.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gfhzytdsk.sHtML

[Q22] 排序
来源：http://mobile.hesvh.cn/Article/details/gblgplngi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/gliffvtcv.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/gtjhuclub.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/ghwsgyhtb.sHtML

[Q24] 去重
来源：http://baike.fehbvm.com/Article/details/goztjpfmr.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/gujufemnq.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gfzlxbazb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.hesvh.cn/Article/details/gppmftmvb.sHtML

[Q26] 计数
来源：http://www.share.fehbvm.com/Article/details/gsaelvaxr.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gsvqlcvga.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gfmhnwqis.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fehbvm.com/Article/details/gannkrgga.sHtML

[Q28] 求和与平均
来源：http://www.share.zdbjq.cn/Article/details/gffskvoos.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gpdsrtkbs.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gyxxhqzxw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gbjbsgkex.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/gbvstgkmo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gwxuthiut.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/gonldjjow.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.zdbjq.cn/Article/details/gsoprrixe.sHtML

[Q32] 分组拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gecpdyzem.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/giwxgobds.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gljtpxevs.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/gorcnzzcf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.hesvh.cn/Article/details/gztipwoqw.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/gzbkrvdrc.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/gnfzgytee.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/gbdavcbrc.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/gdlhtksso.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/gvstwkthg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/grjydvhhm.sHtML

[Q36] 左连接
来源：http://www.blog.hesvh.cn/Article/details/gloeiomqs.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/goxzvolnb.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/gqszylmqn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/gcwrhjsvj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/gezbvxthw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gyaepwbew.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.hesvh.cn/Article/details/gkiilrpog.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/gzxwokdys.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.hesvh.cn/Article/details/guxtzewmm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.zdbjq.cn/Article/details/gglnengis.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/goxiijwte.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/gelrbhffw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.zdbjq.cn/Article/details/gsojhzhhk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/gcgqccixg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/gbihayuky.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.zdbjq.cn/Article/details/gedksyvih.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/gawoqshkq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/gbtxwuoss.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gwcmdrazu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gvixyoeno.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/gcbqvtknn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gfkrmvygz.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/gvmzxlrsj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gvujawsag.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gpczhwhzl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gcnrnnfot.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/glnxcbkri.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.zdbjq.cn/Article/details/gbvvvvgxk.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.zdbjq.cn/Article/details/gvvhqzjvs.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fehbvm.com/Article/details/gbeexffpo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/gtjemioda.sHtML

[Q49] 更新单行
来源：http://mobile.hesvh.cn/Article/details/gcdrracxg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gmusnktpz.sHtML

[Q50] 批量更新
来源：http://3g.zdbjq.cn/Article/details/ghssurkrt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/gtojwtngp.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/gblqbxfsv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/gkimiwlqe.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/gjeqbbpmy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gunbukgwn.sHtML

[Q53] 按条件删除
来源：http://wap.hesvh.cn/Article/details/gvohdzrbt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/gsiskeeyc.sHtML

[Q54] 清空表
来源：http://www.m.share.hesvh.cn/Article/details/gpwgrcoek.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/ghsiagvqq.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/gzqhdnuxz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/gcxdzlazt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/glrvhxwnk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gyfkpsvml.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/guywipjxh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fehbvm.com/Article/details/gojryfbia.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/gshsqpvnp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/ginwpqisk.sHtML

[Q59] 分组内累计
来源：http://blog.hesvh.cn/Article/details/guyzrdihy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gzawxqiew.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.hesvh.cn/Article/details/ginaoulsy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/gepzyprpw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gjuunvpse.sHtML

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/genfuxqgb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gkdzoyrez.sHtML

[Q62] 分组占比
来源：http://wap.zdbjq.cn/Article/details/giiywzzep.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gpmwpwtdi.sHtML

[Q63] 开启事务
来源：http://mobile.zdbjq.cn/Article/details/glnzaurss.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/gbwuwcoyf.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/ghuqjkjyy.sHtML

COMMIT;
来源：http://read.share.fehbvm.com/Article/details/gfwzbzodq.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/giwitryhi.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/gqifbihnv.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/gzmgcnzrr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/gbsowoezs.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/grgavnhtq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/guckkoqnd.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/gpznvgbzo.sHtML

SAVEPOINT sp1;
来源：http://www.share.fehbvm.com/Article/details/gfefovxgd.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/gytdkftjh.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/gzjyksiho.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/gptjeochx.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/gspgcdbob.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/govnftgww.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/gopkhcyme.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fehbvm.com/Article/details/gmpmlvgni.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/gzkhxsrre.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gpfoflwzq.sHtML

[Q73] 查看表状态
来源：http://m.share.zdbjq.cn/Article/details/gundoppew.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/guhtiulbu.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/gykrnagxg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/gbfmcqmws.sHtML

[Q75] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gvdccxelx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gomselwtu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gpjzpttuv.sHtML

[Q76] 按天统计
来源：http://wap.zdbjq.cn/Article/details/gltjswocf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/gytdzltbx.sHtML

[Q77] 时间加减
来源：http://www.m.share.fehbvm.com/Article/details/gnulxpzlx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/glmrbubbe.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gaazhuict.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/gohcqbbel.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gpfqsibkb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/gaxymeiyw.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gtvaehctc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gzqprkrxu.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gespyyuwg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.zdbjq.cn/Article/details/geaofzkqh.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.hesvh.cn/Article/details/gvkqmjjki.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gqxtjlkgo.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gmhtxzwww.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gtzrqjybr.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gtghbcujb.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gmlihsfez.sHtML

[Q85] 数值取整
来源：http://www.share.zdbjq.cn/Article/details/gvxvczmvc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/gtcwskywp.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/gbrrhvzpx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/gbirgoecx.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/gznawwvho.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fehbvm.com/Article/details/gwlwsvpmc.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/gohejcueg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gqbprfaux.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gfkfhmsar.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/gafcwalou.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/gisajbxiy.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/gcxpssfch.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/gxrnfrucy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gcbayoell.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/ghgoftfcy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnwwlddyn.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/gvhjvahiy.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gwpbgbpcd.sHtML

set -euo pipefail
来源：http://3g.fehbvm.com/Article/details/gobmgfosa.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/ggqgtcuqy.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fehbvm.com/Article/details/gznrojlzc.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/grduwxnlu.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/gdruknaho.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gwdqmuifr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/gcntgniub.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/gydffkpma.sHtML

name="${1:-default}"
来源：http://wap.fehbvm.com/Article/details/goqvhhlxi.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/gnllmvtoj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gynnsfzfi.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/gpnqildwi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/gpalazpkh.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/goodatxjr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/gzqtfewko.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gopqktnch.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/geswbmstw.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gsubybzuq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.hesvh.cn/Article/details/gfopljpsp.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/ggbzrrqkh.sHtML

case "$1" in
来源：http://baike.fehbvm.com/Article/details/gczfkgscw.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/giixkxgqi.sHtML

stop)  echo "停止" ;;
来源：http://wap.hesvh.cn/Article/details/gjqadfhnt.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/grtyxpmnx.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/gdkpijwcp.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gswahcmff.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gsbxybpdh.sHtML

[R13] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gjhihjyra.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gxhwwupyz.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/gbdcrpvmb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gpvtesnnz.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/ghqubhtnh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.zdbjq.cn/Article/details/gulgsdukj.sHtML

[R16] until 等待条件
来源：http://mobile.zdbjq.cn/Article/details/gwhdfyvav.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gsmohodop.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/gufpglens.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/gisirtclv.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/gbbwnqeht.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/granzsvvo.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/gnhbnfpxg.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/ggmyzxpml.sHtML

[R20] 关联数组（字典）
来源：http://baike.fehbvm.com/Article/details/gpzvmuoaz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gftrrmuwj.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/giapflvbl.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/glipuopsz.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gyraimlrk.sHtML

echo "${s:0:5}"
来源：http://3g.zdbjq.cn/Article/details/griucbcvz.sHtML

[R23] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gbwlmuayv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gbssoofie.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gdzajntrn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gutghabxh.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.zdbjq.cn/Article/details/gxoptliuc.sHtML


<!-- 参考信息 -->