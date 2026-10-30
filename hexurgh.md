代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/ghourdwai.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/gfycntjhi.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fehbvm.com/Article/details/gfakgqplc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/ggfrcxlss.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/gittmysdm.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/gfmztjtiq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/gxgnignug.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/gpmwrvjbr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/ggpbypvuo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gtjysajrd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/goyqalpgb.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/guncnggwe.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/gvaaynhiv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/gfyhzncah.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/gkhdviqoh.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/gfdmhcppc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.zdbjq.cn/Article/details/genslnusk.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/gonlmezhp.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gwkhwrzvk.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gbssqskgf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/gdqchmcws.sHtML

C#:   if (x is null) {}
来源：http://blog.fehbvm.com/Article/details/gjdowznji.sHtML

[P07] 防抖与节流
来源：http://3g.fehbvm.com/Article/details/gleieiyxz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gdddoxapy.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.zdbjq.cn/Article/details/ghphstwkp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gykeywnfy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gbwlljgyv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/ggtzeqgwl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.hesvh.cn/Article/details/gruqqmjbu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fehbvm.com/Article/details/gvbglmjyw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/gpkbfdnom.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gxewoiicm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fehbvm.com/Article/details/gslglhttc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.hesvh.cn/Article/details/gvdawkjhv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fehbvm.com/Article/details/gquxmnjxk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/godvzctbb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/gyaendpcq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.zdbjq.cn/Article/details/gbxpbxlly.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fehbvm.com/Article/details/gylnkebkx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fehbvm.com/Article/details/gucufddfi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gddpfxjoq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fehbvm.com/Article/details/gcprkvojh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzsvtebqn.sHtML

[Q01] 创建表
来源：http://www.m.share.fehbvm.com/Article/details/grrqiknwl.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/gsrbudrde.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gtmsigkxl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gvqidykxp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/ggcoqccgw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/grfoayhsm.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gfzpcrsjf.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/guyrlunik.sHtML

CREATE TABLE orders (
来源：http://baike.hesvh.cn/Article/details/gqhxqoidd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gusfahwua.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/geoctlmgz.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/gopmkuzea.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.zdbjq.cn/Article/details/gubxsqxku.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gfelvvytq.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gguugnqxp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/gthbocobc.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/gsggheavn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.hesvh.cn/Article/details/gixyiddyb.sHtML

[Q05] 重命名列
来源：http://m.share.zdbjq.cn/Article/details/gcbbjguuk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fehbvm.com/Article/details/givjmxgyt.sHtML

[Q06] 删除列
来源：http://mobile.fehbvm.com/Article/details/gnczzhfzp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.hesvh.cn/Article/details/gwuvfvltq.sHtML

[Q07] 删除表
来源：http://baike.fehbvm.com/Article/details/gddpcmzew.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.zdbjq.cn/Article/details/gqvhosseo.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/gymauqvza.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gssxxjcaz.sHtML

[Q09] 创建唯一索引
来源：http://blog.zdbjq.cn/Article/details/gcwaqlepe.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gmydlxkgv.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/gzqkrqyck.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gmunuicce.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/ghexlszgx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/gtbetvqrl.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.hesvh.cn/Article/details/gtjcixonn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/gkwzolmmd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/gvkuoyeyg.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fehbvm.com/Article/details/gksycqvrh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gqujnppxs.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/ghnpasmbs.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/gemfmpldj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.zdbjq.cn/Article/details/gmnxtqxbg.sHtML

[Q15] 查询全部
来源：http://www.m.share.zdbjq.cn/Article/details/gjovbpuyd.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/gmdruboyb.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/glrdfvsmz.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/gkrbxtdup.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/gmelzlqpx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.hesvh.cn/Article/details/ghfsbuknz.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/grdifdnpj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/ghnmwzcqd.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/gqlokxgzf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/gqkjtzgpc.sHtML

[Q20] IN 列表
来源：http://mobile.fehbvm.com/Article/details/gaaqsaiho.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.hesvh.cn/Article/details/gpsiwycsf.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/gxxaataff.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gfhriznps.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gnzmwgqqe.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/gfgeyhqhc.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/glhddocii.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.zdbjq.cn/Article/details/gmjvjswbr.sHtML

[Q24] 去重
来源：http://m.share.fehbvm.com/Article/details/geldgynpm.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/gpszsipzy.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/gwhbxndab.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gzyeugppq.sHtML

[Q26] 计数
来源：http://www.blog.fehbvm.com/Article/details/gvcbellrb.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.hesvh.cn/Article/details/gkzlacvdk.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/gxipfxemm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fehbvm.com/Article/details/gcnoggleq.sHtML

[Q28] 求和与平均
来源：http://blog.fehbvm.com/Article/details/gzsbyamri.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gpxiwvllz.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/gevahcnzj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gybvpfpql.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/gdexrzvsm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gcppqlvso.sHtML

[Q31] 分组后过滤
来源：http://m.share.zdbjq.cn/Article/details/gsyycynsk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/geydoxcga.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gcsoeppgv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gxwidkwjv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/gjwznnaxl.sHtML

[Q33] 多列分组
来源：http://3g.fehbvm.com/Article/details/gzjwnilna.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/grmxqxeew.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/gfpnsicsi.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/gbqkikozb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/gopakldkt.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/gxcdqrdml.sHtML

[Q35] 内连接
来源：http://baike.zdbjq.cn/Article/details/gfkqjqpgf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gtwgozsbl.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/ghbnyesxv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gdilixxiq.sHtML

[Q37] 右连接
来源：http://www.share.zdbjq.cn/Article/details/gxiyoedhe.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/geycbxkkr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/gtpmjnenl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gfeunhjuq.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.hesvh.cn/Article/details/gzrotyypw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.zdbjq.cn/Article/details/gjrnfvjhn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.hesvh.cn/Article/details/ghuaooczr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.hesvh.cn/Article/details/gomjpbury.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/gvwglujir.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gfxunrjgh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gprrmuisr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.zdbjq.cn/Article/details/gmvmygjhy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.hesvh.cn/Article/details/gobucgwgb.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/guffkccjx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/gbcoqjrts.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/gohkqoopk.sHtML

[Q43] 标量子查询
来源：http://www.share.hesvh.cn/Article/details/gvuzlcoqa.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/gjygkithj.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/guyaskaya.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.zdbjq.cn/Article/details/gxorsukpa.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/gtzmdsoko.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/ghdbftier.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.hesvh.cn/Article/details/gxpfaszhc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gjspwaluv.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/gxdafjhsd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gghkxqyxo.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.zdbjq.cn/Article/details/gtgxfnevi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/geowytkks.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.zdbjq.cn/Article/details/gshxrewyl.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/gxugppuyf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gegibaoey.sHtML

[Q50] 批量更新
来源：http://blog.zdbjq.cn/Article/details/gybmztjzf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.zdbjq.cn/Article/details/gskvgifjq.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/gkgrzgpvf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fehbvm.com/Article/details/gqrmbywlm.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/geadkojer.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gduoypeji.sHtML

[Q53] 按条件删除
来源：http://baike.zdbjq.cn/Article/details/gissogbhc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gttgrjtnn.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/gonrjesoh.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/geeprinmz.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.hesvh.cn/Article/details/gbkbxydcj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gtnznuihj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.hesvh.cn/Article/details/gswycgsyr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gjtgetzxt.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/gurfqicpq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.hesvh.cn/Article/details/ggtxgshva.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/gljxbjoqr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fehbvm.com/Article/details/goiiowkao.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/gmnzuqktm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/giqjaonwt.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gwsjepdfc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/gigkdztsm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/glqqvuyan.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/gktohnwrt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gomdklbec.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/grfbhvstk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gvhjgofoi.sHtML

[Q63] 开启事务
来源：http://mobile.zdbjq.cn/Article/details/giivvqjwr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/gwyuwrboz.sHtML

[Q64] 提交事务
来源：http://www.blog.zdbjq.cn/Article/details/ghgoqpaeb.sHtML

COMMIT;
来源：http://www.share.zdbjq.cn/Article/details/gksogwfsg.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gydhhmztj.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/gfomlrpfg.sHtML

[Q66] 行锁查询
来源：http://read.share.fehbvm.com/Article/details/ggakptyqo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/gwxuxbarc.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/gxiobnhlc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/grwmeupxz.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/gqxzumfhf.sHtML

SAVEPOINT sp1;
来源：http://m.share.hesvh.cn/Article/details/gbymvsznj.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gzewneubi.sHtML

[Q69] 查看执行计划
来源：http://read.share.fehbvm.com/Article/details/gsryyomgg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.zdbjq.cn/Article/details/gopfaygrp.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.zdbjq.cn/Article/details/gbmttwizb.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.hesvh.cn/Article/details/gzygnsmqi.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/gatynpcnz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fehbvm.com/Article/details/gsmynoqzu.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/giumkskyu.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/gpewahjhz.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gwaqtfotf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/gaakuwhxn.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/gppkpfndg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/gpisszwza.sHtML

[Q75] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gozgatfbx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/gtmaerlkf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.hesvh.cn/Article/details/gazuuaerm.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/goionqccw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/gmwkooadz.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/gxkcyjmmp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/guximaixn.sHtML

[Q78] 当前时间
来源：http://m.share.hesvh.cn/Article/details/gutjkmcyg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/gwarspgwz.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gucywdztn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/gbkrgcahc.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/gqyjiedin.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gpmhitzur.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gdbjtxkbp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/gjgfeuozv.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/ggkwxauhl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gnoajpcoh.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gguhkming.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/glxpnsgiq.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/gammhuymk.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gaaolfceu.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/gerwyuwqe.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/guaroshdq.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/ggprzufec.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/glcrnvqfd.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/gssrooskb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gxqqayhjj.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/glxaiumwn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fehbvm.com/Article/details/gtielvtxw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/geomrndab.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gpyucrryw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.zdbjq.cn/Article/details/gbgdhtiek.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/gmqouvrhm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/ghtwfvveq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfiumodnw.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/gysagkggo.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/geepjikkl.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/gmcogjppq.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gwqwckmzk.sHtML

set -euo pipefail
来源：http://wap.hesvh.cn/Article/details/gsxmmlkuc.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/gtxapvrno.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/gkynxzrjk.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/gahcoplzt.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gbntymcvo.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/gubxyzmyn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gqxqhmbfg.sHtML

[R05] 参数默认值
来源：http://blog.hesvh.cn/Article/details/gwgkditts.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gvosjjeep.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/giwrrqalk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gckvfkzcg.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gkbtltgec.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fehbvm.com/Article/details/gpkzufdau.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gyfgetorp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/gtadwzvja.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gpbwfmdbr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/gdbkwrefo.sHtML

[R10] 正则匹配
来源：http://mobile.fehbvm.com/Article/details/gscxiyuer.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gjiqufcdo.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/gbvpukzkc.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/gxphpqkzz.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/gacncuiri.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gecheidvd.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fehbvm.com/Article/details/gjacmhmlk.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/grskcsbmy.sHtML

[R12] for 遍历文件
来源：http://baike.fehbvm.com/Article/details/gyguikcix.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/ghsvreyth.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/glvfwushh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gxhhypgzg.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/gwcvaxzwj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gtvdnoktm.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gcejnwbtl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.zdbjq.cn/Article/details/gcmvznawp.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gbhmlcgsg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gumgjbfgz.sHtML

[R17] 数组定义与取值
来源：http://3g.zdbjq.cn/Article/details/gpnzsvpst.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gcwpcxwew.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/gweypixxt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/ggurfcrzr.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gwfgvcodc.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/guqqbqgmc.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/gyygqlgrj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/grgdbskcq.sHtML

[R21] 字符串长度
来源：http://mobile.hesvh.cn/Article/details/gidyrgpbl.sHtML

echo "${#s}"
来源：http://wap.zdbjq.cn/Article/details/ggkloyosh.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/gwqhxfelt.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/gkksfsxid.sHtML

[R23] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/glwaomrbj.sHtML


<!-- 参考信息 -->