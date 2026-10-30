代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/gwlbhxknq.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gloywlmoy.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/gwijsambu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.zdbjq.cn/Article/details/gsnonunco.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.hesvh.cn/Article/details/gpnvhxhxw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/gasjvezjj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/grxjsafrb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/gwvqjozzq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gwsnrhtyx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/gafgspjbz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gvsjrdnvo.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/ggpulxmlv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fehbvm.com/Article/details/gpephibux.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.zdbjq.cn/Article/details/gcetamjcc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/gddvyaobv.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/gixitohmh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/gzhdpdqry.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/gyzxfgfyn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gkiygiflt.sHtML

Go:   if x == nil {}
来源：http://blog.hesvh.cn/Article/details/gwzgbebfk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.zdbjq.cn/Article/details/ghugqeubq.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/gbixxpgrs.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/gocjogtoo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/gxqajgcbv.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/gxlfglchn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/ghrnvyzvr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gniqkshlk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/gmlacxlfy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.hesvh.cn/Article/details/gfhvahtep.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fehbvm.com/Article/details/ghjcubvto.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fehbvm.com/Article/details/gicxndyoc.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.zdbjq.cn/Article/details/gkrakjrwk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/gxdlodmyd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.zdbjq.cn/Article/details/gwahaltba.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.zdbjq.cn/Article/details/gkzjwkaxu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gxdakpjip.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/gmiggjxip.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/gjcgzodzw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fehbvm.com/Article/details/gxddjfofo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.zdbjq.cn/Article/details/gwmquwxgf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjrjgkuwn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.hesvh.cn/Article/details/grmorgujs.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsxhjhdey.sHtML

[Q01] 创建表
来源：http://www.share.fehbvm.com/Article/details/grmbndxcq.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/gfycffgrg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/ghujgtlal.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gjenzihph.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/ghqkwzvck.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fehbvm.com/Article/details/ghbhkcmsy.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gjfwwmbmx.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/gznkqfeie.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/goegtijem.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gchsoaets.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gmezjouiw.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fehbvm.com/Article/details/ggmatqxtb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.hesvh.cn/Article/details/gyhubfjgj.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gcsbvrydj.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/gajanjjlf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fehbvm.com/Article/details/glpgcehdq.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/gbudlkqca.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/grdnvckqq.sHtML

[Q05] 重命名列
来源：http://www.share.fehbvm.com/Article/details/gndhuvwce.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/gvxqiztaj.sHtML

[Q06] 删除列
来源：http://mobile.fehbvm.com/Article/details/gcyfkufhj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gduygvwbs.sHtML

[Q07] 删除表
来源：http://blog.hesvh.cn/Article/details/gyavipfpi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/gmteszeti.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gcdelksrk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gyggppvlx.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/gyjobvxyq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gpvggfnde.sHtML

[Q10] 插入单行
来源：http://baike.hesvh.cn/Article/details/gqtaylnee.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gurwemiox.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gnqdljivo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.hesvh.cn/Article/details/gsgjgtefs.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/gsvnierwg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.zdbjq.cn/Article/details/gwwdlomur.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/gkzcjajyn.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/gwekmwtao.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/gkplhsjrz.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/gnagndtcn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/gesbtwftl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/gxnjvxhfm.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gvbfswjlq.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/gtwflkvsk.sHtML

[Q16] 查询指定列
来源：http://mobile.fehbvm.com/Article/details/gyaywydfc.sHtML

SELECT id, name FROM users;
来源：http://3g.fehbvm.com/Article/details/gztjnmpmy.sHtML

[Q17] 条件查询
来源：http://mobile.fehbvm.com/Article/details/gqksootss.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fehbvm.com/Article/details/gslufipkr.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/gtckgotir.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/gneyyodch.sHtML

[Q19] 范围查询
来源：http://mobile.hesvh.cn/Article/details/gasrpaogt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fehbvm.com/Article/details/gsljummsr.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/grpjibdvy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gmektmvyc.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/gpfacwuxf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/gyiefcysh.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/ggdqvncnw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/gmpzblqjt.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/gsjcsnhgo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.hesvh.cn/Article/details/gobpqeunu.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/ggcsdwzbn.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gsktberpi.sHtML

[Q25] 只取前 N 条
来源：http://blog.fehbvm.com/Article/details/grtaworld.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.zdbjq.cn/Article/details/gmhojlmgz.sHtML

[Q26] 计数
来源：http://www.blog.fehbvm.com/Article/details/gfojuanqf.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/grrxpmucu.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/gjiczujhd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/gxbrjfcet.sHtML

[Q28] 求和与平均
来源：http://read.share.zdbjq.cn/Article/details/gdvhctuqh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gpbdkvizc.sHtML

[Q29] 最大最小值
来源：http://blog.fehbvm.com/Article/details/gmbgllepo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/gxyldxqav.sHtML

[Q30] 分组统计
来源：http://www.share.fehbvm.com/Article/details/gvpdtdifd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gbyqxvogf.sHtML

[Q31] 分组后过滤
来源：http://m.share.hesvh.cn/Article/details/gdscfjuid.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/gwghorhbe.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/gmwvhgtvw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gnswktsjb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/grgswpwfn.sHtML

[Q33] 多列分组
来源：http://wap.hesvh.cn/Article/details/gpgptttce.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/gcbzaejoe.sHtML

[Q34] 每组取第一条
来源：http://blog.hesvh.cn/Article/details/gslwtmhll.sHtML

SELECT * FROM (
来源：http://3g.zdbjq.cn/Article/details/gpbbpzabj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fehbvm.com/Article/details/gjydcxbmk.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/gclkqrjqo.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/gxqyjztsf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gyiqpcxjx.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/gjncuvdxs.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gfnidtumy.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/gjosnnlan.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gwsitziul.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/gktdinipk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gbbqavrmh.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/grufsejjv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gtrmrfmzh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gqcvwwvut.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/gthydntda.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gqkrmfgcy.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/gqflbuibs.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/gyrozmjui.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/gvleoodso.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/glbfuesun.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/gubjijyok.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.hesvh.cn/Article/details/gxgcghqnf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/gejtcuisi.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/glcmbeffx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/gsdjamdse.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/gqaczxkvd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.hesvh.cn/Article/details/gefbgmozh.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.zdbjq.cn/Article/details/goxnuvgwr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/ghrgotjvl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/gpgppudpq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gxdtkxsho.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.hesvh.cn/Article/details/gsiafwesj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gtuzppuqj.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/gyolospmk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/gukckzcei.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/guwsqwljh.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gfhkspulv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gmccvvcwt.sHtML

[Q50] 批量更新
来源：http://www.m.share.zdbjq.cn/Article/details/guoldzjwr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/gsbgpkeff.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/gheloemxf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/gebowhzqi.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/gpfsrsqdw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gbdvfwgbk.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/gfsnhbthh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gnufcoxjl.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/ggjmvvnsg.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/ggicrevhp.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.zdbjq.cn/Article/details/gijladeyq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gxkisepep.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/gkucjgpcs.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/gzvdoslko.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/goxjbfmng.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ghmvrvpdb.sHtML

[Q58] 累计求和
来源：http://read.share.zdbjq.cn/Article/details/gpyuarsln.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gviswzofb.sHtML

[Q59] 分组内累计
来源：http://mobile.zdbjq.cn/Article/details/goizvzpvc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gpnduvxyj.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.hesvh.cn/Article/details/gkcufymcv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.hesvh.cn/Article/details/gqeecqimr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gmuozgvvi.sHtML

[Q61] 移动平均
来源：http://www.blog.hesvh.cn/Article/details/ggcpsorhh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gpaqabjbr.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gjfkjrpwk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gjjzuibzo.sHtML

[Q63] 开启事务
来源：http://3g.zdbjq.cn/Article/details/gnhrwecaq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/gglbhvchl.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/grapzpqay.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/gmmriesgd.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fehbvm.com/Article/details/gnlwjzykb.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/gyetclhuy.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/gicktnvus.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/gmqqhzuxq.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/gmhbkfbhe.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/goklayaoa.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/gchidvsnq.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/gryazarlw.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/ghpayreng.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/gpwywelgu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/gbhbulruy.sHtML

[Q70] 更新统计信息
来源：http://wap.fehbvm.com/Article/details/gtjxelmze.sHtML

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/gtxisbrky.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/gbsawkpaa.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.zdbjq.cn/Article/details/grjvirpgi.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/grbpqbwmn.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/gzbhguptc.sHtML

[Q73] 查看表状态
来源：http://mobile.fehbvm.com/Article/details/gumypeaut.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gidoaiiwj.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/gtlyagqkl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/gmotghwtb.sHtML

[Q75] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gtxvxssnq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.hesvh.cn/Article/details/gkubxxcav.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/guqmvdhgx.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/gjvocgpye.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/gqdfbnbxo.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/gzunhixud.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.hesvh.cn/Article/details/guulcvxdd.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gbshwuiry.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/grdfhhmaj.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gybnbnmuf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/gdemgymxb.sHtML

[Q80] 字符串截取
来源：http://baike.zdbjq.cn/Article/details/gijeeswff.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fehbvm.com/Article/details/grbmvahfa.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gzulroloo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gnivligtp.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/gyebwzuhs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gzatvwwnj.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gierivifn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/guuginaeu.sHtML

[Q84] 去除首尾空格
来源：http://3g.zdbjq.cn/Article/details/ggcvgigkd.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gyvowohod.sHtML

[Q85] 数值取整
来源：http://read.share.zdbjq.cn/Article/details/gfbpkcwiu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/gjnmitxkf.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fehbvm.com/Article/details/gfypkyzsr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/gcfstzmtj.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gchbraxvf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/ghichkjqd.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/gabaxomqi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/gkbfscjtf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/gpixldfom.sHtML

[Q89] 判断表是否存在
来源：http://baike.hesvh.cn/Article/details/gdlgomgky.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/gqjkudvqu.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/gfcstpvgo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/gtehwllhx.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxuvsealv.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/gelpwlvlu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkqwbicsx.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/gcznqupox.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/gnikckbsv.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gswceliff.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/gbvpmeopz.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/gfqypsaex.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/gbdulcfgt.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/glopxpmer.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/gsqkazjrd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gzmdfgejz.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gjosskvls.sHtML

name="${1:-default}"
来源：http://www.share.hesvh.cn/Article/details/gbxznlyym.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/gblphhldj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gpuovosqi.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/gibodewuz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gtruszvlo.sHtML

[R08] 数值比较
来源：http://m.share.hesvh.cn/Article/details/gsoqgzsax.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.zdbjq.cn/Article/details/ggyurvohb.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gyywgckkp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gxxbsmvpn.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gjfsetauu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gnddtbwya.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/grqhrakgr.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/giatkfiel.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/gwdesqksp.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/goctnkbzw.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fehbvm.com/Article/details/gxjhnrcuo.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/gcbdqkxqu.sHtML

[R12] for 遍历文件
来源：http://blog.zdbjq.cn/Article/details/gwavgonir.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/gipfbdvfa.sHtML

[R13] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gfgdcgwtt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gzurocuwb.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gwoxhrfex.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gwpbxqfoi.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gedogvzyy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.zdbjq.cn/Article/details/ggvjnuasz.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/gvinhnlpx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/glittbotr.sHtML

[R17] 数组定义与取值
来源：http://3g.fehbvm.com/Article/details/gsvqujwmx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fehbvm.com/Article/details/gnvqljfic.sHtML

[R18] 遍历数组
来源：http://3g.fehbvm.com/Article/details/ghwgtpwzf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/gcunmonol.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gnfmcgagb.sHtML

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/grviybtfd.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/ghyttdfxu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gricigfas.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/gttwbljva.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gbnfyifig.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gpbddlszk.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/ghikfimsp.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gmyfiwyhn.sHtML


<!-- 参考信息 -->