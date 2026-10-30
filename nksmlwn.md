代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fehbvm.com/Article/details/gticwhjek.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gnwbxfzfd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gzojrflcu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/glqrmsazl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/gokmlmujm.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/geuhwtrgp.sHtML

Ruby: x.length;  x.size
来源：http://blog.hesvh.cn/Article/details/gztedxsgr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/gyfirxfsr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fehbvm.com/Article/details/gfempiyed.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gjcrqweep.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.zdbjq.cn/Article/details/geivpubne.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.hesvh.cn/Article/details/gughgmedi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/gbsacrfdv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gotwyaare.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fehbvm.com/Article/details/gfuysulos.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/golkybyie.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gmnmpxfhe.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.zdbjq.cn/Article/details/gialdfdoa.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fehbvm.com/Article/details/gnkazshib.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/ghvmqvjfh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.hesvh.cn/Article/details/glfaeyioj.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/gpvwcubzq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gmyllsguj.sHtML

Go:   if x == nil {}
来源：http://m.share.fehbvm.com/Article/details/gxwksfsjm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fehbvm.com/Article/details/gwkvbemzj.sHtML

C#:   if (x is null) {}
来源：http://www.share.hesvh.cn/Article/details/gmaqusdab.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/gsydqnxlc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fehbvm.com/Article/details/guflmuszs.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/gkuuxteun.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gqbnfalph.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gqkjlnrlf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/gvukfixdl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.zdbjq.cn/Article/details/goygavxet.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fehbvm.com/Article/details/gvmvfpqgk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/gagbbbvbg.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gyfkmjciy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.hesvh.cn/Article/details/gmipswysr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/gmiukvfpm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/geomhtvhj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gvpcqmnjl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/gnzwdurmd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/gbpdewypj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/gbocguxnq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gthasajpt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gduytrety.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/gnvuwiiup.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvyzhujrj.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/gzfntudwn.sHtML

CREATE TABLE users (
来源：http://www.m.share.hesvh.cn/Article/details/gzveukmgz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gugbnrkwi.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gayxqwfcn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/gncageqyh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/ggkfacqoz.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gtvdcgxep.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gltfjmomb.sHtML

CREATE TABLE orders (
来源：http://www.m.share.zdbjq.cn/Article/details/gytgbgrfs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gmfxsummp.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gaxjrosrt.sHtML

amount DECIMAL(10, 2),
来源：http://blog.hesvh.cn/Article/details/gscaaezya.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/gidobjmgo.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gipaetrtn.sHtML

[Q03] 增加列
来源：http://www.m.share.zdbjq.cn/Article/details/gcslheziu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.hesvh.cn/Article/details/gnyceuqkp.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fehbvm.com/Article/details/gmejhhdxm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.hesvh.cn/Article/details/getqbitqv.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/gxixjamtf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/gwjjzwduj.sHtML

[Q06] 删除列
来源：http://www.share.hesvh.cn/Article/details/gajxtzlbv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/gqgwzvnth.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/gmrqudxxt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/gbxxuodff.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/grapptqkw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gepzsvtth.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fehbvm.com/Article/details/gdngltqyj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gbnvbccsk.sHtML

[Q10] 插入单行
来源：http://m.share.fehbvm.com/Article/details/gzevggyqk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.hesvh.cn/Article/details/gabfjhzdt.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/gciugorhd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gbijmyzit.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.hesvh.cn/Article/details/gejrfedno.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.hesvh.cn/Article/details/gdrkleanz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fehbvm.com/Article/details/gosubrdcj.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/gyovrkhcs.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.hesvh.cn/Article/details/gadbetpuj.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/gcbsbqvnh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/gktyzttrz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/gpcawqamk.sHtML

[Q15] 查询全部
来源：http://blog.hesvh.cn/Article/details/gzfsaujsq.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gyeglwjnf.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/glablpayu.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gxwawzhro.sHtML

[Q17] 条件查询
来源：http://www.m.share.hesvh.cn/Article/details/gtgakuyip.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.hesvh.cn/Article/details/gvrfylzkw.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/gvpaiymiw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/gmygksglx.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/grzjmrkip.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/gybjvwhbk.sHtML

[Q20] IN 列表
来源：http://wap.zdbjq.cn/Article/details/gpyelwpwr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/goazqugfm.sHtML

[Q21] 空值判断
来源：http://blog.hesvh.cn/Article/details/gsrdxqbon.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/gdlleoyiz.sHtML

[Q22] 排序
来源：http://www.share.zdbjq.cn/Article/details/gburgsuog.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gkyfslpwp.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/gahyvivmu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gchiobvnp.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/gqgufpgeo.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fehbvm.com/Article/details/gwtbuuwuw.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/gerzmquho.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fehbvm.com/Article/details/gwcnufpyg.sHtML

[Q26] 计数
来源：http://3g.zdbjq.cn/Article/details/guxsyryld.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gbzbarebu.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/gupeqeewb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gjttrbnun.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/gmeasbpgv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gdtppzlaz.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gwhvmtzqs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gowaniwef.sHtML

[Q30] 分组统计
来源：http://read.share.zdbjq.cn/Article/details/gqqmjlwgv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gcxjkplth.sHtML

[Q31] 分组后过滤
来源：http://m.share.hesvh.cn/Article/details/gplnghnzi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fehbvm.com/Article/details/gzitovxhh.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fehbvm.com/Article/details/gmfpclnwq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gpogerhil.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/gmnojdvjt.sHtML

[Q33] 多列分组
来源：http://www.share.hesvh.cn/Article/details/gudrzciws.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/gaebjtwok.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/gulluxhzx.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/gspiyqfrw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fehbvm.com/Article/details/gtqmnniwg.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/geglujuyl.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/giolzbrux.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gewxqqsng.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/gdhxcpwbx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/ghgxoaabm.sHtML

[Q37] 右连接
来源：http://3g.fehbvm.com/Article/details/gzgqcyvqd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gpdrldwmw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/ghmkpkxjo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gfbyueyle.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.zdbjq.cn/Article/details/gzwdgzipu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.zdbjq.cn/Article/details/goaxyujnt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/guvpinqbm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fehbvm.com/Article/details/goevfnxfm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/gykbghmgk.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/ggugiuudh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.zdbjq.cn/Article/details/gjdqxiejp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.hesvh.cn/Article/details/ggryiatfu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/gfrnckirr.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/girvuztkv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/grjnxoilx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/gdgsdwcen.sHtML

[Q43] 标量子查询
来源：http://baike.zdbjq.cn/Article/details/gazmamvex.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gvvitjbpt.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/giilfgmjw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.hesvh.cn/Article/details/gvhzlxvqm.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/glxmrutuq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gjrqceflv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.hesvh.cn/Article/details/gsnscyaxr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gdlfktfhv.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/gftogwcli.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.zdbjq.cn/Article/details/ghgjskuel.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gfietxsji.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/giwmwdahs.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/gleqjdktc.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/gwsarirul.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gisyieasi.sHtML

[Q50] 批量更新
来源：http://baike.fehbvm.com/Article/details/gkujbmqoa.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gijgyckyv.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/gcfyncxym.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/gneizeids.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/gdmnypenm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gicarjdnw.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/gaphmdphc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gizjztams.sHtML

[Q54] 清空表
来源：http://wap.fehbvm.com/Article/details/grczvneww.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fehbvm.com/Article/details/ggunimqnr.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gujmrkfuu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gqtcnvvxt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/gwexpcaic.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gfhbncrzf.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/gtjchewks.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.hesvh.cn/Article/details/gikccehev.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/gsaqxgtcu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gtyrooewg.sHtML

[Q59] 分组内累计
来源：http://read.share.fehbvm.com/Article/details/gppiaeclq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gyksfknoy.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.hesvh.cn/Article/details/gjkyxdicl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/gcmvgbqsg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gqqgzdfgr.sHtML

[Q61] 移动平均
来源：http://mobile.zdbjq.cn/Article/details/glwrurzov.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gqoaytixi.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/glaivdmul.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gozopmlmv.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/gccshbihc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/gxjxsmesr.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/gkiitihmv.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/gtysunfbs.sHtML

[Q65] 回滚事务
来源：http://blog.zdbjq.cn/Article/details/gmiuikqhk.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/guojbrpzn.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/gkduifneg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gmbfdnqla.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/gepzgpwee.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.zdbjq.cn/Article/details/grurvnujr.sHtML

[Q68] 保存点
来源：http://www.blog.hesvh.cn/Article/details/gofozoitt.sHtML

SAVEPOINT sp1;
来源：http://3g.fehbvm.com/Article/details/glchxbzah.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gvnmfhoty.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fehbvm.com/Article/details/gxqoxvcfe.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/geoyfmgyw.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/govftdxrm.sHtML

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/gcmukfjko.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/gughxxlym.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gsypztzrm.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gmvzdbcbz.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/gdnoseoca.sHtML

[Q73] 查看表状态
来源：http://m.share.zdbjq.cn/Article/details/grjlnuwch.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/gprsbmrsn.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/gvramwuhl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/geltcuqgh.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gqienvsww.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gvnjaialj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.hesvh.cn/Article/details/gdvpymsju.sHtML

[Q76] 按天统计
来源：http://www.share.zdbjq.cn/Article/details/gugxmmbef.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/gjmkobxgy.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/glckfkxyk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/ghwgpmmfw.sHtML

[Q78] 当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gvbaxjfkh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/gevphuleg.sHtML

[Q79] 字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gqktfnose.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gsossczbj.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gjhieoidj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gnofykdan.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gyemcltjd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fehbvm.com/Article/details/gkrgtboyb.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gciyhwvbu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gxshrnhhg.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gxuyqviuw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/glukyoaqq.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/gbqgtxwqs.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gneaqgwvj.sHtML

[Q85] 数值取整
来源：http://www.blog.zdbjq.cn/Article/details/gxagyzedv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/gldmrkgbn.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fehbvm.com/Article/details/gcixkfnoo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.hesvh.cn/Article/details/gwfrtpnzg.sHtML

[Q87] JSON 字段做条件
来源：http://blog.zdbjq.cn/Article/details/gddgjmmmz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.hesvh.cn/Article/details/guvtltmmc.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.hesvh.cn/Article/details/gdppfzbzc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/gmqhnxsmy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/gauisercy.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gqkxnavle.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.hesvh.cn/Article/details/gmiimqkoi.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gvmcjzfwl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/gnvgsnmkz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glalgzhzk.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/gffqijqwe.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbhkgkosj.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/grhhictab.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/gdyxmqegl.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/genhcdqvj.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/gsyhiflto.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/gjxhokkhz.sHtML

[R03] 只读变量
来源：http://www.blog.fehbvm.com/Article/details/gfgeucnoz.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gssljufls.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/gnbofvyas.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fehbvm.com/Article/details/gqnbdokuw.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/ggqsmzeaw.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/gkdenvxzs.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/glcvolqar.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gxcxtbubs.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/guaexbeqf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.hesvh.cn/Article/details/gmlcmpavu.sHtML

[R08] 数值比较
来源：http://wap.hesvh.cn/Article/details/glszcarbb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gsulgkbbe.sHtML

[R09] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/gvovyzubx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/gwvmforss.sHtML

[R10] 正则匹配
来源：http://www.share.fehbvm.com/Article/details/geacymhrc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/genmrhoss.sHtML

[R11] case 多分支
来源：http://read.share.fehbvm.com/Article/details/gjxtugfqz.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/gokzkndxd.sHtML

start) echo "启动" ;;
来源：http://mobile.fehbvm.com/Article/details/gmjjksvon.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/gzqiewnup.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gdnbolbjw.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/gbzvqdjof.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/grnemafzu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/gxmresowj.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/gtptqutxe.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gahjxgqka.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/gemapzubk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/ghiqfpxzh.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/gqmruczfa.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/gmdldzroi.sHtML

[R16] until 等待条件
来源：http://m.share.hesvh.cn/Article/details/gtlnthiqw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gylzgkljp.sHtML

[R17] 数组定义与取值
来源：http://www.share.zdbjq.cn/Article/details/gqlcsqflk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/gdkzbkumm.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/gjdhhuqmt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fehbvm.com/Article/details/gvxigmnsq.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gngorxyre.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gguqfytwp.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/gibwqhdqj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/gaflowosg.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/gcdbnfxvy.sHtML


<!-- 参考信息 -->