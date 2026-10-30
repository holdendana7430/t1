代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://m.share.fehbvm.com/Article/details/ggpohxoql.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.hesvh.cn/Article/details/gdmaqgyvv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fehbvm.com/Article/details/gbyhgwyce.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gjgerqypu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gemeoarcw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/gocgyeopp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.hesvh.cn/Article/details/gklluwrep.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/gwrenoraf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.hesvh.cn/Article/details/gpgcywsml.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/gfgiaqzfw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.hesvh.cn/Article/details/gxkqukaee.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/gizvnfgpr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/gskwmzlko.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/gtudwgwph.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gtnmhlarz.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/gcqznixjq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gqltbcxgx.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/gwlwpatbc.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/gcpeerwcw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/gvhwehrai.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/gqbnzdwkm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/ggujaglzs.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gqxtxtnmb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fehbvm.com/Article/details/gqmeuzrgd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/glgpjpiaq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/gdvlddemu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gilfxooqo.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gziraihzh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fehbvm.com/Article/details/gnglattte.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gaghyinqc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fehbvm.com/Article/details/glsaumivb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/gtpldpygk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/gzgapfryn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.hesvh.cn/Article/details/gshhnrxej.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fehbvm.com/Article/details/ghblzijkn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/gwmxscyiw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqlgqcpvy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fehbvm.com/Article/details/gznkvgwtz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfbfnhobn.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/gknipqhlj.sHtML

CREATE TABLE users (
来源：http://m.share.fehbvm.com/Article/details/gbcwcbjko.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gdpltfywm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gkvfsthff.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/gbprxuaap.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fehbvm.com/Article/details/gnqujsflp.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gsxrstotx.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/gadbvbsqj.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/gcsnygavd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gkkcbyugl.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/giqgnaafz.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/gnpakwmlb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/gwxzfekwa.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gawgehgqi.sHtML

[Q03] 增加列
来源：http://m.share.zdbjq.cn/Article/details/gffdwhfui.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.zdbjq.cn/Article/details/gfvinniko.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/gbnwqzsfa.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.zdbjq.cn/Article/details/gwhbpjskw.sHtML

[Q05] 重命名列
来源：http://m.share.hesvh.cn/Article/details/gaympahje.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.hesvh.cn/Article/details/ggkqmyyah.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/gsiyryxev.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/gypgfskir.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/gbsgnwcjp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gfggspbcv.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gbonftarn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gjuzpqlxo.sHtML

[Q09] 创建唯一索引
来源：http://blog.zdbjq.cn/Article/details/gnisyrzxz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gzqpvqade.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/gootwqkdj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gakngbttk.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/gujenmlqu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fehbvm.com/Article/details/gudveyksd.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/gooovonqp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.hesvh.cn/Article/details/gadrsbadi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.zdbjq.cn/Article/details/gzinkotxj.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gxdeqalgl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gwezzrhxn.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/gquesgijz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.hesvh.cn/Article/details/ggkmdthrx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/gaycoogjq.sHtML

[Q15] 查询全部
来源：http://baike.hesvh.cn/Article/details/ghzyqhnat.sHtML

SELECT * FROM users;
来源：http://3g.fehbvm.com/Article/details/gwigflpqf.sHtML

[Q16] 查询指定列
来源：http://3g.hesvh.cn/Article/details/gwjihdnfv.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/gvfutookv.sHtML

[Q17] 条件查询
来源：http://blog.hesvh.cn/Article/details/gruavfboq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gnoguzaxv.sHtML

[Q18] 模糊匹配
来源：http://baike.zdbjq.cn/Article/details/gkgyczzhu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.hesvh.cn/Article/details/gdoxeikcp.sHtML

[Q19] 范围查询
来源：http://wap.hesvh.cn/Article/details/ggjdeuvqj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.hesvh.cn/Article/details/gzpahqbmq.sHtML

[Q20] IN 列表
来源：http://m.share.fehbvm.com/Article/details/gmeoxyiet.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/gipaetcpj.sHtML

[Q21] 空值判断
来源：http://www.share.fehbvm.com/Article/details/ghxxrfydj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gqcegdsup.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/gmsyyndeq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.zdbjq.cn/Article/details/gsxocogdb.sHtML

[Q23] 分页
来源：http://baike.zdbjq.cn/Article/details/gxjlostzo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gjgqhbacv.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/gwapldlaj.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gcwaqmmkl.sHtML

[Q25] 只取前 N 条
来源：http://3g.zdbjq.cn/Article/details/guxadntoa.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/gavpglqgq.sHtML

[Q26] 计数
来源：http://blog.zdbjq.cn/Article/details/gzoogggfa.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gmssbfxzs.sHtML

[Q27] 条件计数
来源：http://mobile.hesvh.cn/Article/details/gqtjzeycx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.zdbjq.cn/Article/details/gqtbtiqbv.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/gbhzztrhz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gsgimwhex.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gewbbmjfe.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fehbvm.com/Article/details/gtvraddad.sHtML

[Q30] 分组统计
来源：http://3g.zdbjq.cn/Article/details/gfjsukobn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gouvqyodv.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/ggvlgmvao.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/gdassknai.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fehbvm.com/Article/details/gxdmflihd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gzbtxiaow.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.zdbjq.cn/Article/details/gnmukwrfb.sHtML

[Q33] 多列分组
来源：http://blog.hesvh.cn/Article/details/gfgbonjck.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/givilusff.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/gevaxwfgo.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/guctwdwwr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.hesvh.cn/Article/details/gxuqmylmp.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/gbhmkjwom.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/gwcbamdtq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gwiprqonl.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/grmqdittx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gchkvnikd.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/gndaaoaos.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/gxbjecvjn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/gpvybutmh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/geoarlxdo.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gzwayqaak.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gidhlmxki.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/gnzrzkqpv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.zdbjq.cn/Article/details/guzfrycjq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gruarufwk.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/gfthtdwbx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/gejhndmle.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fehbvm.com/Article/details/glkuuphkk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/gmvhcjjct.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fehbvm.com/Article/details/gfbrnjsmm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/gnsqkrqbs.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/ghfrtalcj.sHtML

[Q43] 标量子查询
来源：http://3g.hesvh.cn/Article/details/gapdlapbz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/gmptphnxd.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/gusfwsmbr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/gjnqjldtu.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fehbvm.com/Article/details/gkatwyhic.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gydhaedqe.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.zdbjq.cn/Article/details/gtxumpcrg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gayethotz.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/gxkcutlou.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.hesvh.cn/Article/details/gtstnykwf.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.hesvh.cn/Article/details/gjdlscjyh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/gerydbhra.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/gmnrbgqib.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/gfibbmxmv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/ghdppjhiy.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gjizmzfoo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gmftiomzf.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/gkbajhips.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fehbvm.com/Article/details/gwkbkyphg.sHtML

[Q52] 删除指定行
来源：http://m.share.hesvh.cn/Article/details/gsgzypxyr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gefdmzlbh.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/gzquikpga.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.hesvh.cn/Article/details/gqbcrciyv.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/glffkxfmt.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.hesvh.cn/Article/details/gysblgrte.sHtML

[Q55] 排名（并列占位）
来源：http://blog.hesvh.cn/Article/details/gegvtgdjw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fehbvm.com/Article/details/gipkirnij.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fehbvm.com/Article/details/gkinzebow.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.hesvh.cn/Article/details/gqfeuottk.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/gxcsedpdi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/glvomkvnj.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/gufnklvkl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gbtdwxdbr.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/gxmwyebkd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gitkofqyb.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/grtxdnzsx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/gnmecaxow.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/gekoibhfu.sHtML

[Q61] 移动平均
来源：http://baike.hesvh.cn/Article/details/gfezqomam.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gktekifcq.sHtML

[Q62] 分组占比
来源：http://blog.hesvh.cn/Article/details/gfaifrcpd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gkjiwfkhq.sHtML

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/gfmzrexrx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/gzlevgytz.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/giyzhcuii.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/gdmcjzmcn.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/gnepufrtu.sHtML

ROLLBACK;
来源：http://baike.hesvh.cn/Article/details/grxalceeq.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/ggfwpejti.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/gmhdzmkqv.sHtML

[Q67] 设置隔离级别
来源：http://3g.fehbvm.com/Article/details/ggxccpzjv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.hesvh.cn/Article/details/gxaklusqo.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gwfwibtlw.sHtML

SAVEPOINT sp1;
来源：http://wap.hesvh.cn/Article/details/gpbbsrukc.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/gyfqpjbxz.sHtML

[Q69] 查看执行计划
来源：http://blog.hesvh.cn/Article/details/gxkwuwyvr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.zdbjq.cn/Article/details/ghslkiayb.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gakcynpqu.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/gzkhtsdjz.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/guoxhjkui.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.zdbjq.cn/Article/details/gtetsfidd.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/gjaeragrt.sHtML

SHOW INDEX FROM users;
来源：http://blog.zdbjq.cn/Article/details/gtkcrgofu.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/gmdtuotum.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.zdbjq.cn/Article/details/gupjtnxci.sHtML

[Q74] 强制使用索引
来源：http://baike.hesvh.cn/Article/details/gvzncikxz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fehbvm.com/Article/details/gfpfefbwy.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gvarhgxum.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/giwzrtqkx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/gedofysuh.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/geifeiupl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.zdbjq.cn/Article/details/gecdghcwr.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/gmsxficpu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/gnsbudykt.sHtML

[Q78] 当前时间
来源：http://www.share.zdbjq.cn/Article/details/gzemtrsxv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fehbvm.com/Article/details/gilcvcoco.sHtML

[Q79] 字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gwxyuyvrk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/giermpsxy.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gmiogvybj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gzqrlqgaq.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gpmlysxbp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gsndhrajx.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/glozbozvz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gvzourjgi.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gkftladad.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gtjjkdqdj.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gnsakfejs.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/glehqmwer.sHtML

[Q85] 数值取整
来源：http://www.blog.zdbjq.cn/Article/details/gykpfpovu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/ghmfhbhsw.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.hesvh.cn/Article/details/gjflnansu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/ghksmoqxb.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/ghsvujfog.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.hesvh.cn/Article/details/gayoqusdm.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/gqrdwdkur.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.zdbjq.cn/Article/details/gggvcqgic.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/gmqsrzcmn.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/geamuhyuo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/gnpefzvzz.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/gjjsrbkpl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.hesvh.cn/Article/details/gopzrxdir.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmfxagddu.sHtML

R. Bash 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gqhthafdo.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gttwzmjlx.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/gpgajoinu.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/grngonyie.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gyngjjmwu.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/gubcsenhk.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gwrmptoln.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/gqlklgimx.sHtML

readonly PI=3.14
来源：http://3g.fehbvm.com/Article/details/gvpulpykx.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/gzrcjbcbj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/gmrvoypjc.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/gaplnavvb.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/gsstclqss.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/grugxkjhv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gfgjdwvxc.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/ghefrreae.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.hesvh.cn/Article/details/gpnzktvey.sHtML

[R08] 数值比较
来源：http://mobile.hesvh.cn/Article/details/gfrngpgkd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gvyiivngu.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gwskhjtjs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/gvlichpji.sHtML

[R10] 正则匹配
来源：http://blog.fehbvm.com/Article/details/gspnrordm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/geeljgpvr.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/gjzvoswgs.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/gumewlrwm.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/ggonxdkcz.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gyczsjyba.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fehbvm.com/Article/details/goznhnpvp.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gmzhvocrx.sHtML

[R12] for 遍历文件
来源：http://blog.hesvh.cn/Article/details/gcjkddmvp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fehbvm.com/Article/details/gethkiyxd.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gqkhapjdd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gcdcaiabq.sHtML

[R14] C 风格 for
来源：http://mobile.zdbjq.cn/Article/details/gtmsgpyua.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gippvcdzh.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gawfokhju.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/gbyrtyjya.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gxpekbmfq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gmfveqitg.sHtML

[R17] 数组定义与取值
来源：http://www.share.fehbvm.com/Article/details/grcdtqyvj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fehbvm.com/Article/details/ggexaeghb.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gejuhddir.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/gnhchbpfx.sHtML

[R19] 数组长度
来源：http://3g.hesvh.cn/Article/details/gwsuigsti.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/gwskmbtoe.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/gotkpstlm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/gqsabufuz.sHtML

[R21] 字符串长度
来源：http://read.share.fehbvm.com/Article/details/gqwxcnctr.sHtML

echo "${#s}"
来源：http://www.m.share.hesvh.cn/Article/details/gbokwhxhf.sHtML

[R22] 截取子串
来源：http://baike.fehbvm.com/Article/details/gsqdwbqus.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gucvjwpql.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gdzxtylqf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.zdbjq.cn/Article/details/gpzmxjqmo.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gdalhudgf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/gvkwfbswr.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/gbexvzqqm.sHtML


<!-- 参考信息 -->