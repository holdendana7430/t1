代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://3g.hesvh.cn/Article/details/gfhwuqrcz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fehbvm.com/Article/details/glipgnmlk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/gfwojmeqd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/gahyxzlwf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gseaokqqq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fehbvm.com/Article/details/gdfvonhhb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/gakkndhqq.sHtML

Ruby: a == b
来源：http://mobile.fehbvm.com/Article/details/gxomwxmlo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.zdbjq.cn/Article/details/gznidetfy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/gagoxtomg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/gzafpbxpn.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/gaxkkpoou.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fehbvm.com/Article/details/gvsxnydeg.sHtML

TS:   if (x == null) {}
来源：http://blog.hesvh.cn/Article/details/gltqfekfo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxixtrzfz.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/grlxjedkn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/gplcrmyms.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/gpxgwtdsg.sHtML

[P07] 防抖与节流
来源：http://3g.fehbvm.com/Article/details/glnksacqc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fehbvm.com/Article/details/gmclhdsjc.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/gsjwbqvkj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/grjczfpgw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/ggwwhquqt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/gynrcimfy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/gmsncfkqr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/gkunrurql.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fehbvm.com/Article/details/gonqbjekw.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.hesvh.cn/Article/details/gmqabmqsn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.zdbjq.cn/Article/details/gwdfhhsaw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/gcqkqguoq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fehbvm.com/Article/details/ggjoehiac.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gaxcksbba.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/ghozzjula.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gdlnqunqf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/gjmdehimd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/gpjkmxdbm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzekduufv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.hesvh.cn/Article/details/gedcsgqrf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/guzbmcxym.sHtML

[Q01] 创建表
来源：http://blog.hesvh.cn/Article/details/gnlwtqyzz.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gtfakqyrc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gnmfletqd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/glimixdsi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.hesvh.cn/Article/details/gpnmehvqx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fehbvm.com/Article/details/gvnegsfye.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gymnjaopw.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fehbvm.com/Article/details/gjctlfcjm.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gokwbfefv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gvmweirrp.sHtML

user_id INT NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gisuwcjmr.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fehbvm.com/Article/details/gxpqzonbp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gtbrlvaoq.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gtmdcvlec.sHtML

[Q03] 增加列
来源：http://www.share.zdbjq.cn/Article/details/gyqhwbhcr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/gbyrjapxe.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/gwkegffgq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/glbpwswjz.sHtML

[Q05] 重命名列
来源：http://read.share.fehbvm.com/Article/details/gdernnexl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.zdbjq.cn/Article/details/gpcqaiive.sHtML

[Q06] 删除列
来源：http://3g.fehbvm.com/Article/details/gorgdkmyt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.hesvh.cn/Article/details/geviygqtu.sHtML

[Q07] 删除表
来源：http://read.share.fehbvm.com/Article/details/gfcgjxynf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fehbvm.com/Article/details/gudwjfrdt.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/geufcnlvv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gzxykfdoi.sHtML

[Q09] 创建唯一索引
来源：http://wap.hesvh.cn/Article/details/gwqyijcbs.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gigcgdlfm.sHtML

[Q10] 插入单行
来源：http://3g.hesvh.cn/Article/details/gefxzifes.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.zdbjq.cn/Article/details/glipgwhsm.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/gcnpqvwcv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gtdptrmet.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.zdbjq.cn/Article/details/gbidlwjvz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gjtylnxwd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.hesvh.cn/Article/details/giniosrex.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fehbvm.com/Article/details/gerqwidhh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fehbvm.com/Article/details/gacujdglo.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/gqptgxthc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/ggjazmetm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/gnnwugnni.sHtML

[Q15] 查询全部
来源：http://www.m.share.fehbvm.com/Article/details/gxdkirvwb.sHtML

SELECT * FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gcamhkpvq.sHtML

[Q16] 查询指定列
来源：http://www.share.zdbjq.cn/Article/details/gtgyvgozd.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gpyoyhdev.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/ghjbqsmjb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fehbvm.com/Article/details/ggiuougms.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/ghqlezypb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/gxhkvikin.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/gwbmaxaqq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.zdbjq.cn/Article/details/gyihwdzab.sHtML

[Q20] IN 列表
来源：http://read.share.fehbvm.com/Article/details/gvmciescn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.zdbjq.cn/Article/details/gysogkqhq.sHtML

[Q21] 空值判断
来源：http://m.share.fehbvm.com/Article/details/gouzmhygf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/gdijsiowo.sHtML

[Q22] 排序
来源：http://m.share.zdbjq.cn/Article/details/gyroklnmf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gsemimadp.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/gqmcwlymu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.zdbjq.cn/Article/details/grhcpnhyd.sHtML

[Q24] 去重
来源：http://blog.hesvh.cn/Article/details/gynxdeuxh.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fehbvm.com/Article/details/glqporlzp.sHtML

[Q25] 只取前 N 条
来源：http://mobile.hesvh.cn/Article/details/gxgjwcoca.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.hesvh.cn/Article/details/gufnzqoxs.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/gsfssrhff.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.hesvh.cn/Article/details/grjxcsprn.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/gcusobaij.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gbpeslqzp.sHtML

[Q28] 求和与平均
来源：http://read.share.zdbjq.cn/Article/details/gdaqzpilx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gabblwsji.sHtML

[Q29] 最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gftosxaom.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gptjtheuf.sHtML

[Q30] 分组统计
来源：http://m.share.fehbvm.com/Article/details/ggxtuoeta.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gsujpfdim.sHtML

[Q31] 分组后过滤
来源：http://mobile.fehbvm.com/Article/details/grzgkecpl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/gjxwqcnaq.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gpbctjbrx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/grvzchmcb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fehbvm.com/Article/details/gxbginfgh.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/grnzraeeh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/grxfnesrk.sHtML

[Q34] 每组取第一条
来源：http://read.share.zdbjq.cn/Article/details/gdciiudpp.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/gcfdomqhr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/gboubsyqd.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/gfgdnfeyc.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gqywknjni.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/ggpdibvyi.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/ggumsntfk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gbudvtcrp.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/ggpicavex.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.zdbjq.cn/Article/details/glzptjdox.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/gjrnkanln.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/ggnedaije.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/gmtackjtn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/gomtnkqgc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gnoisclen.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/geliaeegf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/gpbwzepje.sHtML

[Q41] 多表连接
来源：http://blog.zdbjq.cn/Article/details/gqyickrzy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fehbvm.com/Article/details/gjnozwyor.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fehbvm.com/Article/details/gdtmmrlqh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.hesvh.cn/Article/details/gxbrrbvqi.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fehbvm.com/Article/details/gkufagaxl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.hesvh.cn/Article/details/gzzzvexmx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gixgmyyen.sHtML

[Q43] 标量子查询
来源：http://www.share.fehbvm.com/Article/details/gwyaxokgd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/ggntrbsip.sHtML

[Q44] IN 子查询
来源：http://blog.fehbvm.com/Article/details/gyjpdbuil.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.zdbjq.cn/Article/details/gkjtrpvvt.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/gpcfayhuh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gpthyxevl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/ghvlgrdte.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/ggxsobvcg.sHtML

[Q47] 与平均值比较
来源：http://m.share.fehbvm.com/Article/details/ggkzligne.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/gxyfhkqjw.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/gbhqrvhpm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/gkonbmyeg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.hesvh.cn/Article/details/gjuisncoj.sHtML

[Q49] 更新单行
来源：http://read.share.zdbjq.cn/Article/details/gqhkmpeny.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gzxuatldk.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/gclfkhcoq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fehbvm.com/Article/details/gmcdcabtj.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/gbrencgnw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/gnjgnzwgz.sHtML

[Q52] 删除指定行
来源：http://wap.hesvh.cn/Article/details/gbmqakqve.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gbjsnforw.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/guoujhpkr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gglkfjglb.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/gotdkyvnt.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.hesvh.cn/Article/details/gglnvffum.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/gwxzwlfyz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gbdudfdxd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fehbvm.com/Article/details/gyjsghste.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.hesvh.cn/Article/details/gvwbcsvjy.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/gfwpwiwql.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gwrxanvru.sHtML

[Q58] 累计求和
来源：http://mobile.fehbvm.com/Article/details/gmgmmnsvk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gzoawrazs.sHtML

[Q59] 分组内累计
来源：http://baike.zdbjq.cn/Article/details/gfreuqqkg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gpuspibwx.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/gjkdgqkdu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.hesvh.cn/Article/details/gletluvdc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gjifhsqwa.sHtML

[Q61] 移动平均
来源：http://blog.fehbvm.com/Article/details/gdysysyhw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fehbvm.com/Article/details/govwpuwlq.sHtML

[Q62] 分组占比
来源：http://wap.zdbjq.cn/Article/details/gfmfzyfkx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gkpadzkhr.sHtML

[Q63] 开启事务
来源：http://blog.fehbvm.com/Article/details/gtzopwkgy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/gjytxmhgw.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/glzfuloat.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gutospxpc.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/gmpsmpbkt.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/gseflkvtu.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/gijlwnmkj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fehbvm.com/Article/details/gyafqhtjb.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/gjbajvuuu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.hesvh.cn/Article/details/ghtmwvgva.sHtML

[Q68] 保存点
来源：http://www.blog.hesvh.cn/Article/details/gyxcabhql.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gffajyvcb.sHtML

ROLLBACK TO sp1;
来源：http://blog.zdbjq.cn/Article/details/gizskguiq.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/gchsvyzed.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/gcoxqsowo.sHtML

[Q70] 更新统计信息
来源：http://baike.hesvh.cn/Article/details/gfsjzelyk.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/gexompepb.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/gsncelnxj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/gmvdxahtp.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/gzfwsqrma.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/gugfnxeqb.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/gyhxeqljx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/gzvgpamvi.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/gcndrxpsp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/glemxyrjn.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gojyifiur.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gxdtlspop.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/ghcbkwgsb.sHtML

[Q76] 按天统计
来源：http://www.share.fehbvm.com/Article/details/glgzjdhmu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/gqbdrhzqq.sHtML

[Q77] 时间加减
来源：http://www.blog.zdbjq.cn/Article/details/gxvnlqqbj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/gujcwdsrn.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/gylrsqwdf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/grbtglcwf.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gcbljmkmo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/gjsvtbfsq.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gqcgoztao.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gtdqkoqpz.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/ghzplyuxu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/guupyzwoj.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/grpjruulu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/glqwcqonn.sHtML

[Q83] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/glfgqvwbt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gduovgpao.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/gvfxvciyr.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gflwzbcdo.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/gwjfzunvu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/gjefmddun.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gtijcfqmt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/gtzdfguhs.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.zdbjq.cn/Article/details/gypgbwdns.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/gxxfqmcul.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/gvtfinble.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/gxljirdvk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/givwgagkx.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/ggbtusaqm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/glvcbehiu.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/gfaklhtzw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/gmkzmihkb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpnpsgolf.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/gwveireeg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxteqeapi.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/ggusokumg.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/gzjrajulb.sHtML

set -euo pipefail
来源：http://m.share.zdbjq.cn/Article/details/gjspwzpkk.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/gxcnykaji.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/ggjfeqhrd.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/gnqegfpta.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/gmucktlgu.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gqacqcdhz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gdovanwgj.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gwsoiaspl.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gdvfychou.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gdrqxrrvc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gqsptbamu.sHtML

[R07] if 判断文件
来源：http://m.share.zdbjq.cn/Article/details/gjhfdkwdv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/gwcyzisfd.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/gbxgvfuoz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gaeranxop.sHtML

[R09] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gsvnzueic.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.hesvh.cn/Article/details/gmlcobmyc.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gbwrajcml.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/gwzwxjjza.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gugtfdypt.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/gxtycwely.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/gxnlzmlhq.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gqyocmuvy.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/gjnaexifz.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gbzpipnzz.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gquszgimx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/gwtxejscn.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/gprjztnkz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gidppkdzl.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/gtiwkqose.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/glomonfjv.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/genfykpws.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gnqubqoij.sHtML

[R16] until 等待条件
来源：http://mobile.zdbjq.cn/Article/details/grddppzbl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/ghmciwrgx.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/gbrioqiep.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/gawfgeebn.sHtML

[R18] 遍历数组
来源：http://blog.hesvh.cn/Article/details/gvqkgznyp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/gxtovtbbd.sHtML

[R19] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/grhsvqvwa.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/gdiagubnz.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/gppxipgtq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.hesvh.cn/Article/details/gwvwkwkjq.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gyrumswze.sHtML

echo "${#s}"
来源：http://www.m.share.zdbjq.cn/Article/details/gzglpefbm.sHtML

[R22] 截取子串
来源：http://read.share.fehbvm.com/Article/details/ggxojmgns.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/gzzdqcbzz.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gkubyuzju.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.zdbjq.cn/Article/details/grpfywgzf.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gdwglgdgo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/gybiyktmp.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/gzvdzzyrc.sHtML


<!-- 参考信息 -->