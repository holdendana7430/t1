代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gfpvllfrs.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/ghgrmadgt.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/gkzoppbuc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gjcttmqar.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/gglkzzxwx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/gpqdcejru.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/gilnpcjto.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/gweqziwor.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gjtzmgksq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/gihycsifc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gbjzcufez.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/gfynyvtky.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/graxavomc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.zdbjq.cn/Article/details/grztvbfdh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gycmfzkcm.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gugjecled.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/galfepymj.sHtML

TS:   if (x == null) {}
来源：http://m.share.zdbjq.cn/Article/details/giahmedzu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/goqeuqmfm.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/gpnyiuiyl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/gkfkqykly.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gmezdwmcr.sHtML

[P07] 防抖与节流
来源：http://3g.hesvh.cn/Article/details/gyyhixvsd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fehbvm.com/Article/details/gjivphbmj.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/goqdcqycz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gvvyheanj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gpjkzwbgr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/gyecsztcm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/gqdhkvzvg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.zdbjq.cn/Article/details/giacklelx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.zdbjq.cn/Article/details/gakaifimu.sHtML

[P08] 处理浮点精度问题
来源：http://blog.zdbjq.cn/Article/details/gwphgakim.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fehbvm.com/Article/details/gyflckpgu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.hesvh.cn/Article/details/gdxeapfve.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.zdbjq.cn/Article/details/ghdnwdwrc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gcjelmvsj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.zdbjq.cn/Article/details/gpimtnxux.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/gfvnjtnfk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fehbvm.com/Article/details/gerxjcnym.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fehbvm.com/Article/details/gwgwcpffw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjefdmyig.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/gnoifunxd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/guqgyenhr.sHtML

[Q01] 创建表
来源：http://read.share.hesvh.cn/Article/details/gtxvyfjng.sHtML

CREATE TABLE users (
来源：http://3g.hesvh.cn/Article/details/gcboanxqg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gsqfuaevb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gziqxcrnt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.zdbjq.cn/Article/details/ggxzyqwye.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.hesvh.cn/Article/details/gskymqzom.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/guzbfucqw.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fehbvm.com/Article/details/gjidztdwb.sHtML

CREATE TABLE orders (
来源：http://baike.hesvh.cn/Article/details/gwashxanp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gmbdqyslz.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gppuannmp.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/gzoxmkrwi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/guvfhhygm.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gquawpbqx.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/gyzvtybwz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fehbvm.com/Article/details/gjlsoairo.sHtML

[Q04] 修改列类型
来源：http://www.m.share.zdbjq.cn/Article/details/geygqoffh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/gsnxjybjo.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/gzopcsxre.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/gcfsiykms.sHtML

[Q06] 删除列
来源：http://blog.fehbvm.com/Article/details/gzgilxhkd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gfrzfvmia.sHtML

[Q07] 删除表
来源：http://www.blog.hesvh.cn/Article/details/ggnkejuue.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.zdbjq.cn/Article/details/ggbkimbng.sHtML

[Q08] 创建普通索引
来源：http://wap.fehbvm.com/Article/details/gcwyhjutd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gvlxnhcwt.sHtML

[Q09] 创建唯一索引
来源：http://mobile.zdbjq.cn/Article/details/gsvahvuim.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gvmmlfipz.sHtML

[Q10] 插入单行
来源：http://www.blog.fehbvm.com/Article/details/gvbcsyqxg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.zdbjq.cn/Article/details/gizdcossw.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gymwubkwc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.hesvh.cn/Article/details/gchlwrdof.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/gubohnque.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/goeuzynng.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/gmmvsahkr.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/giartotqt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/gcjwagozk.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gumfzsfvp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/gtfefnngn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gwscyljho.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/gnitxrkow.sHtML

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/gbehmkjxl.sHtML

[Q16] 查询指定列
来源：http://baike.fehbvm.com/Article/details/gnutqkymq.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gcjcjglqm.sHtML

[Q17] 条件查询
来源：http://m.share.zdbjq.cn/Article/details/gdgtatclm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/gcggqogme.sHtML

[Q18] 模糊匹配
来源：http://www.blog.zdbjq.cn/Article/details/gcodymahl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/gvswlkibz.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/ggoawcyfy.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/gphslfrpq.sHtML

[Q20] IN 列表
来源：http://wap.zdbjq.cn/Article/details/ghpzfbyin.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/gppykklcs.sHtML

[Q21] 空值判断
来源：http://wap.fehbvm.com/Article/details/gfjncesyn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fehbvm.com/Article/details/gnydmkixl.sHtML

[Q22] 排序
来源：http://blog.fehbvm.com/Article/details/gfdnfswxx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/ggwifczab.sHtML

[Q23] 分页
来源：http://baike.fehbvm.com/Article/details/gybaunzne.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.zdbjq.cn/Article/details/gdahjcxul.sHtML

[Q24] 去重
来源：http://baike.hesvh.cn/Article/details/gwnfvrmcr.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gumooblfg.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fehbvm.com/Article/details/gemihfwlj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.zdbjq.cn/Article/details/gwlkmnkir.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/gvmaddpfi.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gnqjuptvk.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/gwmcvllui.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gnndncned.sHtML

[Q28] 求和与平均
来源：http://blog.fehbvm.com/Article/details/gbabqrlek.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gddoiufqf.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gzjljhtdp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/gxqljpkhk.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/gtomepfaw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gkyzmpzuy.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/gytmyuwqc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.hesvh.cn/Article/details/gyrbfafyr.sHtML

[Q32] 分组拼接字符串
来源：http://wap.zdbjq.cn/Article/details/ggpfdaiha.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gmsyiqrek.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/gtecovmwj.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/gzlyjkzck.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/glmxebtvi.sHtML

[Q34] 每组取第一条
来源：http://www.share.fehbvm.com/Article/details/gawiowvjt.sHtML

SELECT * FROM (
来源：http://mobile.hesvh.cn/Article/details/gthnprnyj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/glkoekfga.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/gnrelcgup.sHtML

[Q35] 内连接
来源：http://blog.hesvh.cn/Article/details/gajbghqbj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gnsmiddzg.sHtML

[Q36] 左连接
来源：http://m.share.fehbvm.com/Article/details/gubygvkkj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gvlpbdaxt.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/gukwjkgau.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fehbvm.com/Article/details/gklpktslb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.zdbjq.cn/Article/details/gcnixzeej.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fehbvm.com/Article/details/godqxpnqc.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.hesvh.cn/Article/details/gzksdmsuq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gzimeaapi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/gsjerpard.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/guodtekrs.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.hesvh.cn/Article/details/gdwelksoc.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/ghkbzjvsx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gbukdvzpv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/gulxmnzun.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/grqjoqsyr.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/galxlmpcx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/grqouezkb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/ghsvqtxxm.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/gehyojisk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/gjzvatvei.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/gpdyevafn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/gnlfztgpt.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.zdbjq.cn/Article/details/gytpprrwz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/glixafrkh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/gfikteadq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gdcsqpdoh.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gebqohnva.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gzyejwmiu.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.zdbjq.cn/Article/details/gldkuwuph.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/gzfjxwgrc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/gkppduglu.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/gpgxuyrvy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gtvdsqiyv.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/gwkboidsw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gsgzcccoo.sHtML

[Q51] 用子查询更新
来源：http://www.share.fehbvm.com/Article/details/gygcijdli.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.zdbjq.cn/Article/details/gdmlmcrnd.sHtML

[Q52] 删除指定行
来源：http://read.share.hesvh.cn/Article/details/gjvghbavg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gwvhtrfal.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/gfhepvjrp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/gnbuaezlx.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/glspaawif.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/gsvqgfwyw.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/gfhgagxjs.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gwiyxtnqi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.zdbjq.cn/Article/details/gtqofyaje.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gqddhvwyv.sHtML

[Q57] 行号
来源：http://m.share.zdbjq.cn/Article/details/gdndvwiyw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gukcfxyuu.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/gvugjcmaa.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gllxgbjbq.sHtML

[Q59] 分组内累计
来源：http://blog.fehbvm.com/Article/details/gfhczxmfd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gxgcrbezb.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/gktbwrqjs.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/goxwqxppa.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gyrvfbmir.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/gnpglndtk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gmzxsxhwa.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gmksfsmsn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/ggoifgqwn.sHtML

[Q63] 开启事务
来源：http://mobile.zdbjq.cn/Article/details/gietxtmvx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.zdbjq.cn/Article/details/gnpdsglmy.sHtML

[Q64] 提交事务
来源：http://3g.zdbjq.cn/Article/details/gcnuhyyen.sHtML

COMMIT;
来源：http://mobile.fehbvm.com/Article/details/gikrfxttt.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/gmetnfmlv.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/geevawjrd.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/gdquopcjl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.hesvh.cn/Article/details/gzmmaznyt.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gsvnbhzsx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/gyefzbcey.sHtML

[Q68] 保存点
来源：http://blog.fehbvm.com/Article/details/geywyhugl.sHtML

SAVEPOINT sp1;
来源：http://read.share.zdbjq.cn/Article/details/gdhejgsuv.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/gvumplgcg.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/guxeevpoa.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/gurvcgbxz.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/gktoadycc.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gxgfavkda.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/gagpeqwso.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.hesvh.cn/Article/details/grxhjaitl.sHtML

[Q72] 查看索引
来源：http://blog.hesvh.cn/Article/details/goswksqpg.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/gevtlmisz.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/gjemumsxa.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/geuvmkoyu.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/gofwbbhuv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gfosasinh.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gnvqianqc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gfmpjpobn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.hesvh.cn/Article/details/gswhmdlsu.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/gurovpfss.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/ggnqzbskh.sHtML

[Q77] 时间加减
来源：http://www.m.share.zdbjq.cn/Article/details/gnklngowf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/geyshpeis.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/gpdcnwqlm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/goyxumajv.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/ghgaaismj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/gpmjhhzua.sHtML

[Q80] 字符串截取
来源：http://m.share.fehbvm.com/Article/details/gewzobckm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gbrsubpvj.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gjafosenp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gklkkvdxj.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.hesvh.cn/Article/details/gudaemkse.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gvybzhfsv.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gvubcmnlm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gqdrpfgjm.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/gwtozbycf.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gnobovbwu.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/guovcwdru.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/gncnzspuu.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/gucvugugq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/gijlplbxg.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/gczclsqgl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/gezaxrlws.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/gkrdvceah.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/gfkuwtvaj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/gunelcxmv.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/gmydbtlod.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/ghlqepjpz.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gsbhyqcyl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/gcmulklbh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gctglivfo.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/gbtsidxag.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkuoioiqp.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/gfiipyslb.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/gzeiltysh.sHtML

set -euo pipefail
来源：http://mobile.fehbvm.com/Article/details/gfqnzsvqu.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/grjfxasql.sHtML

name="Tom"; echo "$name"
来源：http://baike.fehbvm.com/Article/details/glrcrekph.sHtML

[R03] 只读变量
来源：http://mobile.zdbjq.cn/Article/details/gckblphtt.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gysldnhmq.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/guieyuynu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/gbkzdotbw.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gpgwprriv.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/gzspbhbmm.sHtML

[R06] 判断命令是否存在
来源：http://wap.hesvh.cn/Article/details/gxkvvxali.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/ggbrxokzq.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/gbtzvrotb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.hesvh.cn/Article/details/gwsgtqiyb.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/gmyzsnmgv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/gjgwdpvko.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gqelsbcqq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.hesvh.cn/Article/details/gykisclma.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/ghwgpfkva.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/gwszltzlo.sHtML

[R11] case 多分支
来源：http://m.share.fehbvm.com/Article/details/gumarkibm.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gwndiumvp.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gdreeqdgt.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gulsdpodn.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fehbvm.com/Article/details/ggqszjfcl.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/glgottrrf.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/gifvahkoj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gclixuqak.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gbxmsukwn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gurutrrxh.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gkojxdffo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gsvjmmwnb.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gtpffoqqo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/gwdcuvhva.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/gcqzaivmx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gglbphqwb.sHtML

[R17] 数组定义与取值
来源：http://www.share.zdbjq.cn/Article/details/gxriwlcif.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/gyptkitjd.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/gszfoystf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gtbfpulqg.sHtML

[R19] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gyyftlhfg.sHtML

echo "${#arr[@]}"
来源：http://read.share.fehbvm.com/Article/details/grisndwpn.sHtML

[R20] 关联数组（字典）
来源：http://blog.hesvh.cn/Article/details/gaqacknle.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/gjamflsxo.sHtML

[R21] 字符串长度
来源：http://read.share.hesvh.cn/Article/details/gxawfwwpe.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gvriaszsg.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gjjaevlen.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/gnhggikzs.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gwrvnaxjl.sHtML


<!-- 参考信息 -->