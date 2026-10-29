代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://blog.fehbvm.com/Article/details/gbdqyzelw.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/ghiboacem.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gfrqypidq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.zdbjq.cn/Article/details/gnwlezfnh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/gvgikxdou.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fehbvm.com/Article/details/gojwszxpm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/gwghtwcbq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/gksndpoav.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gfrljaofj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/gzxxoyevo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gbpywfrui.sHtML

Ruby: a == b
来源：http://www.m.share.zdbjq.cn/Article/details/gwaaclljv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fehbvm.com/Article/details/gorudrkdc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/gbstziulw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/gavrcavqc.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/guqsdajez.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fehbvm.com/Article/details/grvxnzedw.sHtML

TS:   if (x == null) {}
来源：http://blog.hesvh.cn/Article/details/grdvwgqiv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gtstcsavk.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gibgleuat.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/ggghpnwvr.sHtML

C#:   if (x is null) {}
来源：http://read.share.zdbjq.cn/Article/details/gxbomkylz.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/ggituoijg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.zdbjq.cn/Article/details/gssfxvliq.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/gpazxsvgq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gvexbyliv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gajmnsgjs.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.zdbjq.cn/Article/details/gfguaprhs.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gesqfwvhz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.zdbjq.cn/Article/details/gbzbaxxto.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/gnnsjpbyq.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.hesvh.cn/Article/details/goiaqckgw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.hesvh.cn/Article/details/grttxlsrt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/gmkvpcgmp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/ghrddectu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gsjiklhqt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/ghlxwljeq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.hesvh.cn/Article/details/gmrhxspki.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.zdbjq.cn/Article/details/gfpueyzbb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fehbvm.com/Article/details/ghqotvjpv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdsknpaxb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/grdktbpkl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmzmwrnwn.sHtML

[Q01] 创建表
来源：http://www.m.share.hesvh.cn/Article/details/gfbdxobxh.sHtML

CREATE TABLE users (
来源：http://blog.zdbjq.cn/Article/details/ggglgxtyi.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gwseibabb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gziaxsekv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/gyknhbxuv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/gtwqtcazk.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/ghmgmaxvc.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gvpqsyumy.sHtML

CREATE TABLE orders (
来源：http://wap.fehbvm.com/Article/details/gkiccombw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gsqauecas.sHtML

user_id INT NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gddkylcly.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gpfwfxzwp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/ghgtldfqf.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gqpkmbntd.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/gwivwsjme.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/gtinjizcy.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/gghmmpeae.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/gjptulsyv.sHtML

[Q05] 重命名列
来源：http://blog.zdbjq.cn/Article/details/gnsymobvf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/grgwxypnz.sHtML

[Q06] 删除列
来源：http://www.blog.zdbjq.cn/Article/details/gijtastog.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.hesvh.cn/Article/details/gnznvzdzj.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/gcfcnhibb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/gygndnqch.sHtML

[Q08] 创建普通索引
来源：http://blog.fehbvm.com/Article/details/ghlgxdufy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gqoiowjyp.sHtML

[Q09] 创建唯一索引
来源：http://baike.hesvh.cn/Article/details/gdkqphlhb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gpwftnrzb.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/gvgtssogd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.zdbjq.cn/Article/details/gzvbhcqqn.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/grtfzjpvp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fehbvm.com/Article/details/gioqiwpup.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.hesvh.cn/Article/details/gxerophsh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.zdbjq.cn/Article/details/gpnlmjtyg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fehbvm.com/Article/details/gjyokpnjn.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/gmrmjgsco.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/ggpybmwuu.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/godguywrq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/gbztxcrfd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/gfapyrcku.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/gtvtbaosa.sHtML

SELECT * FROM users;
来源：http://blog.zdbjq.cn/Article/details/ghxltirwx.sHtML

[Q16] 查询指定列
来源：http://www.share.fehbvm.com/Article/details/gxtdpkbkv.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/grqawbmpx.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/gbxrcjbmr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/ggfvdvfuc.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/gjgmttgyc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.zdbjq.cn/Article/details/ggdcipapq.sHtML

[Q19] 范围查询
来源：http://mobile.hesvh.cn/Article/details/gndulrkeb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.hesvh.cn/Article/details/gtajimimn.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/guymnvpec.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/gjbxyofcz.sHtML

[Q21] 空值判断
来源：http://3g.hesvh.cn/Article/details/gblirtcoa.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/gljhgffft.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/gldckenuq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/gfocaljth.sHtML

[Q23] 分页
来源：http://www.share.fehbvm.com/Article/details/gckfybmzf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/gaeyeoely.sHtML

[Q24] 去重
来源：http://wap.fehbvm.com/Article/details/glfopbkpt.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ghdicsckb.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fehbvm.com/Article/details/gymoxsldr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gqfyycezp.sHtML

[Q26] 计数
来源：http://m.share.zdbjq.cn/Article/details/gqnmxkdil.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gjuqmqmaj.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/gtqlvcwoh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/gpzvbwddd.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/gnwlsgznz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gpesiatbi.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/gexwuzubz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gwhqkwehn.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/ggzvacefc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gscnnnwfl.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/ggsmxtglx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fehbvm.com/Article/details/gkkwnzjpb.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fehbvm.com/Article/details/gdzwzdldx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gumxivcqk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/glxbunjee.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/gdozsmqdy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.zdbjq.cn/Article/details/gjmegykvn.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/gsxrsadcz.sHtML

SELECT * FROM (
来源：http://www.share.zdbjq.cn/Article/details/gfyofzyus.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.zdbjq.cn/Article/details/gfhrysewt.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/gmhluntcf.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/gfrinvuxa.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gfzakgaxi.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/grheizuyg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/ggufayawm.sHtML

[Q37] 右连接
来源：http://wap.zdbjq.cn/Article/details/gghqmiztn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.hesvh.cn/Article/details/gwltxgdds.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.zdbjq.cn/Article/details/ghyuzjvzl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.zdbjq.cn/Article/details/getncixud.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/gpfkquozk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/grdzcuojk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.hesvh.cn/Article/details/gpaqhsmxp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/gwlrgjfmo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gtbtvahiu.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/gudkjqmma.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fehbvm.com/Article/details/giwftdcrl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/glrojhmje.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fehbvm.com/Article/details/gnidueqie.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/gzfrzmhyh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.hesvh.cn/Article/details/gyuutplwi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/giscjrdlv.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gnuzgzvvy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fehbvm.com/Article/details/gxxfmmunt.sHtML

[Q44] IN 子查询
来源：http://3g.hesvh.cn/Article/details/gznqvadld.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gzfpcnzpf.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/gbsfsagus.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gppthldvm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.hesvh.cn/Article/details/gkwblltds.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gmvoqfqmx.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/ghlxscylb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fehbvm.com/Article/details/gezgpoewf.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/gxzmyznqz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/gzqujqkxl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fehbvm.com/Article/details/gjfsvoqkg.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/gfajqxoud.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/geyejfjbe.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/gnsvgzeuz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/gjznrmqus.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/gwvtobpqm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/glmnebocf.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/gqnjtddhy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gwjtfopoq.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/ghmspmwhj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.hesvh.cn/Article/details/gghkweuko.sHtML

[Q54] 清空表
来源：http://read.share.fehbvm.com/Article/details/gkcbngvfs.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/gdzqbievp.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/grkvgbjvl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gaubedwwm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/gsiekfrxy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/glcuiaqvh.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gyeapsqkz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.hesvh.cn/Article/details/grznliwnq.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/gzhdzhthv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gcdkyerms.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/gtznbbkqr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/glvtfbzrc.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fehbvm.com/Article/details/gitnvkkff.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gzkoqyddo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/gwottlxla.sHtML

[Q61] 移动平均
来源：http://baike.hesvh.cn/Article/details/geawwawxq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/ghnorcfkk.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gbowrbwaq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gfqydzmlu.sHtML

[Q63] 开启事务
来源：http://blog.fehbvm.com/Article/details/gdyzmobus.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fehbvm.com/Article/details/godlwrckg.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/gdoetnnrj.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/gtwjkcibm.sHtML

[Q65] 回滚事务
来源：http://3g.zdbjq.cn/Article/details/gvkfjmlkw.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/gyysfdrrc.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/grpvascfp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/gpjrykzan.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/gcuzsoteo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/gxerwuteh.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/gndfrnscu.sHtML

SAVEPOINT sp1;
来源：http://baike.zdbjq.cn/Article/details/ggjmocdsu.sHtML

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/gheszewcx.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gjbvusiyp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.hesvh.cn/Article/details/gggygeuyt.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/geobjdggo.sHtML

ANALYZE TABLE users;
来源：http://baike.fehbvm.com/Article/details/gvhhjrklg.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/grvbnejvo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.hesvh.cn/Article/details/grxzyubnw.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/gpuhuprun.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/gtlrddzxs.sHtML

[Q73] 查看表状态
来源：http://wap.fehbvm.com/Article/details/ggvqdpizf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/gxbgsolvf.sHtML

[Q74] 强制使用索引
来源：http://blog.fehbvm.com/Article/details/grnxepetp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fehbvm.com/Article/details/gvgewstco.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gvlfgbnts.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gjqdhlgis.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.zdbjq.cn/Article/details/gbehhqanp.sHtML

[Q76] 按天统计
来源：http://www.share.hesvh.cn/Article/details/gqrgybgjc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.zdbjq.cn/Article/details/grqorfhib.sHtML

[Q77] 时间加减
来源：http://baike.fehbvm.com/Article/details/gqeadwidh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/gztssdtsf.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gptaljggf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fehbvm.com/Article/details/gtaykgpsw.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gpsbqnbbx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fehbvm.com/Article/details/genofskvo.sHtML

[Q80] 字符串截取
来源：http://www.blog.hesvh.cn/Article/details/gqrouoltg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/ggbyhmtao.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/grxwtmhvu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/gnpvennpb.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/gpcjrsksz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/giygxtkxv.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/grawpocmo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gyyiguzfz.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/grdafoeii.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gnuorzxso.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/ghioecsiw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/gmfkcimen.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.zdbjq.cn/Article/details/gnvdibdnt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gdioqazce.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/gosmmxorm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/geixpfrri.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/ghjxejpmw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/gkwnbycwd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gbovnjdml.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/givhrkulb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gkrnugruj.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/gcqrkbjlh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.zdbjq.cn/Article/details/gefwbwcmc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gnstvqxgv.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gfijhprmm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjcbdjuzk.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/glkqphzfw.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/glrcijhqr.sHtML

set -euo pipefail
来源：http://m.share.zdbjq.cn/Article/details/gycppycka.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/gnpcfvlkk.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gycfsogpu.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/gvtgkjwlq.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/gudrymliz.sHtML

[R04] 位置参数
来源：http://baike.fehbvm.com/Article/details/gngtdgayl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/gccnhcsqm.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/gblckbemj.sHtML

name="${1:-default}"
来源：http://3g.zdbjq.cn/Article/details/gfathwakc.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gohmjqjbg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gfwaphaec.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/gidrelnbx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/ggpcavgfb.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/gttstozyq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/gqywlxcwz.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gylhzdxcf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.zdbjq.cn/Article/details/gfxaiiuzd.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gundadkqr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/geabdztev.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gptkxjdqr.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/ghxybwjzr.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/gaxtdsdtk.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/gjbkfjyjr.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gjhceumva.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gdikbxoqs.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/gxjstwsgt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gsqocmhgf.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gtnnjrogi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gtwlxpnwe.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/gzausafgw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gyuxyzizk.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/gjzyqibah.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/gorwcrhvf.sHtML

[R16] until 等待条件
来源：http://3g.fehbvm.com/Article/details/glaspzugi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gymeerhvo.sHtML

[R17] 数组定义与取值
来源：http://read.share.hesvh.cn/Article/details/ggxyoebuz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/gdcwayfwi.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/gpojxnbjs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gsdhkpgqh.sHtML

[R19] 数组长度
来源：http://3g.hesvh.cn/Article/details/gsumihtgy.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/giufmnlou.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/gwhqabodc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/gzhkxajkk.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gqldvzzaz.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/goqkulhea.sHtML

[R22] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gscsxiati.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/gjrogzsdw.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gjjndrigv.sHtML


<!-- 参考信息 -->