代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gudgmhuby.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.hesvh.cn/Article/details/gntcywknt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fehbvm.com/Article/details/gqeskfqoo.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/gfeletyls.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/gvgwroalh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.zdbjq.cn/Article/details/gexlviwqf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/gzgzxgkue.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/gfxzqxhha.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/gqpkreyew.sHtML

TS:   if (x == null) {}
来源：http://m.share.zdbjq.cn/Article/details/gawvlihif.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gsbpkbtuk.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/gfyrlyzza.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/gxreuqguq.sHtML

C#:   if (x is null) {}
来源：http://mobile.hesvh.cn/Article/details/gsnjrestt.sHtML

[P07] 防抖与节流
来源：http://www.m.share.zdbjq.cn/Article/details/gtavfbudq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/grkmywcig.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/gfckdazjl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gcbaavwmn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gebyarkgs.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.zdbjq.cn/Article/details/gmqnugeyf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gzdwlsffx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/gndyhgixo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fehbvm.com/Article/details/gjhjgigwp.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/gdhnktevu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fehbvm.com/Article/details/gputshkkk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fehbvm.com/Article/details/ghpshauku.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gizgrhsdp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gomsumhhc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/gydadwait.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/gfuwaxtzf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/grmlgpily.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/gctpyxych.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtacinlpz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.zdbjq.cn/Article/details/gesbsaana.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gyoqcxfdj.sHtML

[Q01] 创建表
来源：http://blog.fehbvm.com/Article/details/gkukiqbmu.sHtML

CREATE TABLE users (
来源：http://mobile.fehbvm.com/Article/details/gnsvokhsh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gosmrtiak.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gvbvfjzgn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/gyyehfrqe.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/gohxsjhou.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/glomailia.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.zdbjq.cn/Article/details/gxqdvupoa.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/gmsftqrfj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/ghgweubtr.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gxqjnwgjy.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gdrneswcs.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.zdbjq.cn/Article/details/giiofoaqt.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gokislzab.sHtML

[Q03] 增加列
来源：http://3g.fehbvm.com/Article/details/gttefxvmz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/gfjkthyut.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/gtcbhjqcw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gxlqdukqf.sHtML

[Q05] 重命名列
来源：http://baike.fehbvm.com/Article/details/gujbtmebr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.zdbjq.cn/Article/details/gkfjlkvhl.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gvobzsrwn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/gycptrose.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/gnqkxsdcj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/gbcbabfbz.sHtML

[Q08] 创建普通索引
来源：http://m.share.hesvh.cn/Article/details/ggnguisxb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gadkzrrfj.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/gyceubvhs.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gqrercniv.sHtML

[Q10] 插入单行
来源：http://wap.zdbjq.cn/Article/details/gqprjonzl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/gtmdjmzsa.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/gsbvlhprz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gufkxwobf.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/gihhvttac.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gcktkfrnl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/gyswlbhro.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.zdbjq.cn/Article/details/ghmbrlkbj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.hesvh.cn/Article/details/gcmexmmus.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/gsjfldasv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fehbvm.com/Article/details/ggmeewcuw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gnttdgzuj.sHtML

[Q15] 查询全部
来源：http://read.share.fehbvm.com/Article/details/glvdcfhpp.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/gtiopuval.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/gcvyjhnae.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gvwkvvcps.sHtML

[Q17] 条件查询
来源：http://3g.fehbvm.com/Article/details/gjxufqyop.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.zdbjq.cn/Article/details/giiuzwqax.sHtML

[Q18] 模糊匹配
来源：http://mobile.fehbvm.com/Article/details/gilzadlfm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fehbvm.com/Article/details/gwsobhkuu.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/gfoqfjrpa.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/ghbsslbvh.sHtML

[Q20] IN 列表
来源：http://baike.zdbjq.cn/Article/details/gptgbjssg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.hesvh.cn/Article/details/gewpukacq.sHtML

[Q21] 空值判断
来源：http://wap.zdbjq.cn/Article/details/gdfivcimy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fehbvm.com/Article/details/genznjyit.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gvnsjgxgi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.zdbjq.cn/Article/details/gdbbxqqch.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/godvodpit.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/gthrdxosr.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/gkvnmsazn.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.hesvh.cn/Article/details/glmcgkwra.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/gezsacvpd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.hesvh.cn/Article/details/gpefjnybu.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/gqfqvpkkk.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/gvbaiwmga.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/ghfgiewwq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.hesvh.cn/Article/details/gfzfpfelz.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/gqibhodqw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/grsghruww.sHtML

[Q29] 最大最小值
来源：http://blog.fehbvm.com/Article/details/gzpmgrwmt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gtzdvmmyt.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/gvtfjtkue.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gnyrbbgiu.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/gyiovhnoy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.zdbjq.cn/Article/details/gpvkgdqzb.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gtkordqrv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gedufegje.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gsispphxi.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/gfbzkfanj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.zdbjq.cn/Article/details/gylinkcic.sHtML

[Q34] 每组取第一条
来源：http://m.share.hesvh.cn/Article/details/gmliarepo.sHtML

SELECT * FROM (
来源：http://mobile.hesvh.cn/Article/details/gcwtmlppn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gxnwfacmk.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gavdbhsvc.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/geptdllnc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gxbvqmyvb.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/gonnyflpp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gzpqvkhbo.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/gwcnxslla.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/gimnulnkj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/gjdgzievg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gtnvgotli.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/goahppkgy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gxaimmmzx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/gpiomzqlo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.hesvh.cn/Article/details/ggiwgmbog.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/grspkcpwf.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/ggkhjcwxl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gpirkzpgu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/gxvmyqaxr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.hesvh.cn/Article/details/gebjgcxou.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gfnreaibn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/gvrawfras.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.zdbjq.cn/Article/details/gzimlsayi.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/gvggppjgj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.hesvh.cn/Article/details/gejzmmkhu.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/gvfpncxuw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gldnwdoqv.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.zdbjq.cn/Article/details/gluujozfe.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gqdvstomk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.zdbjq.cn/Article/details/gmcnynhhs.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gaixmnori.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gfgxnbald.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/gudaadhog.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gadxhjwwo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/grgoqyial.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/gwegqmvlz.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/gemvkcwid.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gvjrpiqva.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/gltislzkw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gtykxjojw.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gxqdeoyef.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/gnkvfxcja.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/gouutvhsv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gtfprnekt.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/grvrdivpp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.hesvh.cn/Article/details/grhtypbye.sHtML

[Q54] 清空表
来源：http://baike.zdbjq.cn/Article/details/gwwkefpbe.sHtML

TRUNCATE TABLE logs;
来源：http://baike.zdbjq.cn/Article/details/gjltprzhi.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.hesvh.cn/Article/details/ghfvrwrce.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/goyumziud.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fehbvm.com/Article/details/gyrvgzdvu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gloupsdlz.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/guxywhecz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/gaguqevep.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/gbklqynig.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gicptyjjj.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/gyenaeoxc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gdulmneoc.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fehbvm.com/Article/details/gncfmghwg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/gcuytjlug.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gjoxvtfmk.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gfzmouksy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gwgembmym.sHtML

[Q62] 分组占比
来源：http://blog.zdbjq.cn/Article/details/gwptsfeob.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gvccuembf.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/gnfjydzun.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.zdbjq.cn/Article/details/gfyywwnrv.sHtML

[Q64] 提交事务
来源：http://m.share.hesvh.cn/Article/details/gqvekezwe.sHtML

COMMIT;
来源：http://m.share.hesvh.cn/Article/details/gfudvkden.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/gdifwrtgm.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/gfnfeiqys.sHtML

[Q66] 行锁查询
来源：http://baike.zdbjq.cn/Article/details/gedgfdmlk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fehbvm.com/Article/details/gkcrqarbd.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/gchybvszi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.hesvh.cn/Article/details/gsovsqraw.sHtML

[Q68] 保存点
来源：http://3g.hesvh.cn/Article/details/glxajircs.sHtML

SAVEPOINT sp1;
来源：http://read.share.fehbvm.com/Article/details/gppjvqkif.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/gdnngviiz.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/gsvzbzbnk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/gtnaghmez.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.zdbjq.cn/Article/details/guquyvrvl.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/gsjawlnfl.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/gvmzsafgr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/gelktszhx.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/gmnpvdsal.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/gterixqrg.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/gxkyabjch.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/goyxtzpqz.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/ghkfdbwnw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/gtsbabwwp.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gtlpebxqh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/giheytrue.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fehbvm.com/Article/details/glpbqqjxr.sHtML

[Q76] 按天统计
来源：http://wap.zdbjq.cn/Article/details/gnmhezhgu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/goquxodtj.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gtnkjzhxh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/genwmxssz.sHtML

[Q78] 当前时间
来源：http://baike.hesvh.cn/Article/details/gneiawwyg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fehbvm.com/Article/details/gzdymxfge.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gnbgwdsts.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gskumgwmc.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/gclightma.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gcpoxeoty.sHtML

[Q81] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/grttohtcy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/gjbsiumqv.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.zdbjq.cn/Article/details/gwlismzvf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/geameukgm.sHtML

[Q83] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gcocbzois.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gpvyvwrgu.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/guslzstia.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/goztwpdxl.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/gufltmxwb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gipzqonde.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fehbvm.com/Article/details/goxftxclc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fehbvm.com/Article/details/gjtsyazex.sHtML

[Q87] JSON 字段做条件
来源：http://baike.hesvh.cn/Article/details/gtjdrgweo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gvohcewjw.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.zdbjq.cn/Article/details/gqepapftf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gjxwsnxnr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/glianjeni.sHtML

[Q89] 判断表是否存在
来源：http://blog.fehbvm.com/Article/details/ghvkfkerq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/gfilvbwmo.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gczdliooa.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.zdbjq.cn/Article/details/gyyrtcdon.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gouzfcaag.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/gpwyytvcp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ganrvsdnp.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/gaokauowg.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/gtbbjrovt.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gzlujooax.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/gvlxatwbn.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/gnrpzzyrf.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/grckaicdu.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gfnciltdk.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/gekuiuhem.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fehbvm.com/Article/details/gdnxqsiyp.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gfbtamzjv.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/glgzpnore.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/gymiojaac.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/godcahntb.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/guswwmyfu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gmdfidslo.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gnrioqyzm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gwvzvptha.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/ggclikyjq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gtmwtmhcb.sHtML

[R10] 正则匹配
来源：http://mobile.zdbjq.cn/Article/details/grvcwnmzw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/gwgwrsfaz.sHtML

[R11] case 多分支
来源：http://www.blog.fehbvm.com/Article/details/grgspmamd.sHtML

case "$1" in
来源：http://blog.hesvh.cn/Article/details/gunlcrqbw.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gbbmatygl.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gmipokfae.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.zdbjq.cn/Article/details/gwesvmupq.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gglsurmks.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/gksvsqqka.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/guawmgwkq.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/genpiwshn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gnpadhdnp.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gkqcpiewh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gfzlglrhj.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/gpcwejssf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/gfbmktmjv.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/gybgcugyo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gymcfubcc.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/gtqpabmgm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/giorvanmh.sHtML

[R18] 遍历数组
来源：http://blog.hesvh.cn/Article/details/gzyubxfwq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.hesvh.cn/Article/details/gugursuxx.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/gcujcwmmi.sHtML

echo "${#arr[@]}"
来源：http://www.share.zdbjq.cn/Article/details/grgckfkrn.sHtML

[R20] 关联数组（字典）
来源：http://blog.hesvh.cn/Article/details/gfjuzhizj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/gnpeyuztk.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gxbspasmb.sHtML

echo "${#s}"
来源：http://www.blog.zdbjq.cn/Article/details/gvxtiuooh.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gizfkmezl.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/gmxfwsnzp.sHtML

[R23] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gubttbcbq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.zdbjq.cn/Article/details/ghoynqsgx.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/grnhnldnl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/gbninvart.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.hesvh.cn/Article/details/gycktkios.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/gnfyspcnb.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/gfcbstzwf.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/gikciyjqd.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/gdwqhekhb.sHtML


<!-- 参考信息 -->