代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.zdbjq.cn/Article/details/ghuslbeie.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/gprnpwhzp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/gqamhwcdr.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.hesvh.cn/Article/details/gjybjjgmf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.hesvh.cn/Article/details/gyovjukdy.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/gwogcglln.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gvktpsvuy.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/gpzeisply.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/gzgavzeka.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gmsqxfbyi.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/gezxjgmbf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/gtydnibgd.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/gfpaelfqc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gcwptybwe.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gjypkieze.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/gaalbjazh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.hesvh.cn/Article/details/grfamwzex.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/gedowqnbc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gogrtbilr.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/gulynelnl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gngxjlwvh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.hesvh.cn/Article/details/gfsoqlvme.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fehbvm.com/Article/details/gekskrpdd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gewyifwrd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.hesvh.cn/Article/details/gpkrigtkz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/gpghmzkfy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fehbvm.com/Article/details/ghnstrqxl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/gfasikkxk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gtsafwxae.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/ghrpyugyl.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtvelcywy.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/gdcuzhxzh.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/gcigugwdn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gexfhzjkl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gvmsschcn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/gqosmlswt.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.hesvh.cn/Article/details/gipenythw.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gauifizpy.sHtML

[Q02] 创建带外键的表
来源：http://mobile.zdbjq.cn/Article/details/gdfhdjcbt.sHtML

CREATE TABLE orders (
来源：http://wap.zdbjq.cn/Article/details/gezcqonxx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gsiobhdvw.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/ggrbsrcov.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fehbvm.com/Article/details/gokjqncac.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/gxbdzrsio.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gzeyvspwy.sHtML

[Q03] 增加列
来源：http://mobile.fehbvm.com/Article/details/gxydriggo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/gytkeupoy.sHtML

[Q04] 修改列类型
来源：http://mobile.fehbvm.com/Article/details/gtdpjwkws.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/gllyjgygn.sHtML

[Q05] 重命名列
来源：http://www.blog.zdbjq.cn/Article/details/ghllolhmc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fehbvm.com/Article/details/gkxgbcqfs.sHtML

[Q06] 删除列
来源：http://www.share.hesvh.cn/Article/details/gwuijgrxv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/gsfppvzzw.sHtML

[Q07] 删除表
来源：http://wap.zdbjq.cn/Article/details/gkrilfudh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gubuuniuc.sHtML

[Q08] 创建普通索引
来源：http://3g.zdbjq.cn/Article/details/ggfetbbpi.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gulgqgsdd.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/goibjfegj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gytbgtfna.sHtML

[Q10] 插入单行
来源：http://www.blog.zdbjq.cn/Article/details/gfwmispun.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/gtctdjdjj.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/ggaaqsezg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gmevpoutn.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/gboksiimf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.hesvh.cn/Article/details/gakxizuqv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.hesvh.cn/Article/details/gmbvnpmfq.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fehbvm.com/Article/details/gijktiukx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gmpxntvew.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/gsaxpfohw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.zdbjq.cn/Article/details/gmvtmevdj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.hesvh.cn/Article/details/gidpaxxpm.sHtML

[Q15] 查询全部
来源：http://m.share.fehbvm.com/Article/details/ggyikvxcf.sHtML

SELECT * FROM users;
来源：http://3g.zdbjq.cn/Article/details/gztykwicz.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/gpgzywbyl.sHtML

SELECT id, name FROM users;
来源：http://m.share.fehbvm.com/Article/details/ggwmrtcxi.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/gulfawfgp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.hesvh.cn/Article/details/gtwcfbaff.sHtML

[Q18] 模糊匹配
来源：http://wap.fehbvm.com/Article/details/gshjqebko.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/guxapzjbz.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/gessncmdj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fehbvm.com/Article/details/ghbxjwxlo.sHtML

[Q20] IN 列表
来源：http://www.share.hesvh.cn/Article/details/gouarawbi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/ghhttmsuu.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/gxqwzbfuk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fehbvm.com/Article/details/gxjjqgclv.sHtML

[Q22] 排序
来源：http://www.m.share.fehbvm.com/Article/details/gzmmsfwfc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/gogmbehmp.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/gshmwuses.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/glonmteon.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/gtodwpjml.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/gefpptppg.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/gnonvlwrm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/gkeopzrez.sHtML

[Q26] 计数
来源：http://mobile.fehbvm.com/Article/details/ghciynbfw.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/gogcfgvdg.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/grzvjsngz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gcadquauw.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/gvqufzrtb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gckodppus.sHtML

[Q29] 最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gpghfxhrr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/guthdbfbw.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/gzhtflibg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gkmdfpsjk.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/gttohrzee.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.zdbjq.cn/Article/details/gzyfadpez.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gutudioto.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/grrpmujhj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/gspghohsq.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gibxuvyao.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.hesvh.cn/Article/details/gflhfktgx.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/gvoacefzt.sHtML

SELECT * FROM (
来源：http://baike.fehbvm.com/Article/details/gebygjokc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.zdbjq.cn/Article/details/glbnfncaf.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/gubqvxwca.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/gugppxruh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gbugkzsnn.sHtML

[Q36] 左连接
来源：http://read.share.fehbvm.com/Article/details/gdzcfopok.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gwoendzap.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/gvpjhbziu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gzdddetmq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fehbvm.com/Article/details/gfvgynhzj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gphdmmuho.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.hesvh.cn/Article/details/ghrbuinax.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fehbvm.com/Article/details/gptugmpgt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fehbvm.com/Article/details/gnwizklmh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/gwhsqmpxa.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/gkqfmqmpv.sHtML

[Q41] 多表连接
来源：http://baike.fehbvm.com/Article/details/gcppxwhvn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fehbvm.com/Article/details/ghnltnian.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fehbvm.com/Article/details/gojiuclzf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/gogrnwuuk.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.hesvh.cn/Article/details/gyfvekrsz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.zdbjq.cn/Article/details/gpzfxoemd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/gawmmbuwy.sHtML

[Q43] 标量子查询
来源：http://blog.zdbjq.cn/Article/details/gsyqpjuaj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/gdrjlnykv.sHtML

[Q44] IN 子查询
来源：http://blog.hesvh.cn/Article/details/gvhivdgck.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.zdbjq.cn/Article/details/genfpwnoq.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.zdbjq.cn/Article/details/gyzniirpp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gefsvpuxq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.hesvh.cn/Article/details/gilruvthq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gszvozpnv.sHtML

[Q47] 与平均值比较
来源：http://read.share.zdbjq.cn/Article/details/ghjqsjakd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.hesvh.cn/Article/details/glfyzpyxu.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/gyjgmtypw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.hesvh.cn/Article/details/gbegehieg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.hesvh.cn/Article/details/gxjlamvjs.sHtML

[Q49] 更新单行
来源：http://mobile.hesvh.cn/Article/details/glelbdrpw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gbrgcmbca.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/gfbzkdlvo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gofiyfmza.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/ghpviubpf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/gedezufon.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/gelvgmgvg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gzhgeumjl.sHtML

[Q53] 按条件删除
来源：http://baike.fehbvm.com/Article/details/gowxlstms.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gasxwotcr.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/gydchdpmk.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/giaqkzszj.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/ghgfcyryo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gfvksuyar.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.zdbjq.cn/Article/details/gfppvtehn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gdseysubr.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/giohblixu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.hesvh.cn/Article/details/gpfyhaukf.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/gbvwdgvvd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gltpfyhya.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/gewvqjpbt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gkkzfeisr.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/gomcecznk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.hesvh.cn/Article/details/gjsgyxlsj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gkesfdptv.sHtML

[Q61] 移动平均
来源：http://baike.hesvh.cn/Article/details/ggkuhwacm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gotzxemkn.sHtML

[Q62] 分组占比
来源：http://read.share.fehbvm.com/Article/details/gsfsmlhxd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/galvdhvou.sHtML

[Q63] 开启事务
来源：http://mobile.zdbjq.cn/Article/details/gdrzpwoad.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.zdbjq.cn/Article/details/gsuakxqea.sHtML

[Q64] 提交事务
来源：http://www.blog.zdbjq.cn/Article/details/gxclnxebc.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/gudvgfgsw.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/gpapssaqm.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gndupslyf.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/gwivttrfm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/gnvwlnrep.sHtML

[Q67] 设置隔离级别
来源：http://read.share.zdbjq.cn/Article/details/gczwqfryl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.zdbjq.cn/Article/details/gqqxmyyxt.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gcfzgvzyh.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/gkgrgwwcs.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/gjppkwujo.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/gmrmwkeub.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.zdbjq.cn/Article/details/gaoxsudoq.sHtML

[Q70] 更新统计信息
来源：http://read.share.fehbvm.com/Article/details/guadgwhag.sHtML

ANALYZE TABLE users;
来源：http://www.blog.hesvh.cn/Article/details/ghgxhsquu.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/gxayapkdr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/gudfwzqgi.sHtML

[Q72] 查看索引
来源：http://blog.hesvh.cn/Article/details/gfimpxzii.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gwveqqjrt.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/gsidxwgbm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.zdbjq.cn/Article/details/gayekqbli.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.zdbjq.cn/Article/details/gpzotnkes.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/ggcnsqlpb.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gkqytsbhs.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.zdbjq.cn/Article/details/giebydigz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/gjucntcal.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/gywxgclru.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/gjylnawmy.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/gjkbjfbjg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/gpyclnplq.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gfuyfnynu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fehbvm.com/Article/details/gywwwyecl.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gslhbbuon.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/glurhyhwb.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/gnqtepsoz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gpzvzxuqv.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gjcvtvimf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/ggqkrexgh.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fehbvm.com/Article/details/gllkmnayy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gkwkyuahd.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gbbpzceym.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gfzctrbav.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/gogszfuov.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gnbzalevp.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/gmdpqbwew.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fehbvm.com/Article/details/gaqeknpvw.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fehbvm.com/Article/details/gkthayeax.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fehbvm.com/Article/details/gwvjdxgqm.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/gqzlrmxng.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.hesvh.cn/Article/details/gceyrqrll.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/gwxmqobks.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/gudejjmqo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/gzevexirt.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/gybwtuiek.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.hesvh.cn/Article/details/gxnogmfop.sHtML

[Q90] 生成序号列
来源：http://3g.zdbjq.cn/Article/details/gymivhqdh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.zdbjq.cn/Article/details/gstgcwewd.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gghggqepu.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/goncwuhcw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkhfxrpla.sHtML

[R01] shebang 与严格模式
来源：http://baike.zdbjq.cn/Article/details/gbufczopu.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.hesvh.cn/Article/details/glizmwlyr.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gmigydfrw.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/gcentpzfh.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gjwvlaznv.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/gdfzlutqz.sHtML

readonly PI=3.14
来源：http://wap.zdbjq.cn/Article/details/gbzwmyqbx.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gohieqegt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/goxboufwb.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/ghuhyvlrn.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/ghfafvhaf.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/gwegetpvb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gpumlgzut.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gkzlsviom.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/gnstriizj.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/gymhpuwpq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/gdcjlwvwr.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/ghptywnky.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gvqdyryxx.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gtwbpapgr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gclfucpof.sHtML

[R11] case 多分支
来源：http://www.blog.fehbvm.com/Article/details/gfdhfhcry.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/godhvgdys.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/gtpkhcqjs.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/gsulzkcly.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/gbnpayqms.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/grylfogof.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/gmzmprmog.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fehbvm.com/Article/details/gifitckga.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/goalanbos.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gedxkqjyg.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/gvwgefjfw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gojsukkbm.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/gekdovenw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/gcqszzsca.sHtML

[R16] until 等待条件
来源：http://3g.hesvh.cn/Article/details/glkvhmboo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gianvatxc.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/geqmjxpbl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.hesvh.cn/Article/details/gjmplqejo.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/gekwfocbu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/gaisuscqq.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gxviysjis.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/ghpyhwrmz.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/ggytfkiwl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/glzupacbh.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/gpneeusdy.sHtML

echo "${#s}"
来源：http://www.m.share.zdbjq.cn/Article/details/gepadejzt.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/ghsiflbyb.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/gxjcyikjm.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gikotlnvu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.hesvh.cn/Article/details/gnwnoxuda.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gldyacryj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/gsepagbdf.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/gmpvvggby.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/gllqtbcue.sHtML

[R26] 命令替换
来源：http://read.share.fehbvm.com/Article/details/ghskhclbb.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gqfvjoeyo.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/gsbpmqblb.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/gdiiowjjc.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gjwraixle.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gegypekxz.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/gtyexqaun.sHtML


<!-- 参考信息 -->