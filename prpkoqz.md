代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/gjcxwmyqt.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gfobiqtcw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/ggitaxtpv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gafkoixek.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/glwukidyh.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/gbxymorus.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/ggloipnqz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/gjaylekpx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/gcnsztjjy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gwiziexxx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.zdbjq.cn/Article/details/gxqfslgik.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.hesvh.cn/Article/details/ghgelkopt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gufuhwegw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fehbvm.com/Article/details/gckslcywf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gimjejxhn.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/gwdaiptna.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.zdbjq.cn/Article/details/gnoituetm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/gbdscdejl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gwicxmjxy.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.zdbjq.cn/Article/details/gvjtqvvnt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.hesvh.cn/Article/details/ggasgjmyt.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwnzkmapy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gvvidvxvz.sHtML

Go:   if x == nil {}
来源：http://baike.fehbvm.com/Article/details/gvwiqwjvt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fehbvm.com/Article/details/geichfwea.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/genudnqnl.sHtML

[P07] 防抖与节流
来源：http://www.blog.fehbvm.com/Article/details/gmpzdmqms.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.zdbjq.cn/Article/details/gwnozpplb.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/ggtkkwgbi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gvavivlfh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/guvyodrpm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.zdbjq.cn/Article/details/gwlibysoa.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fehbvm.com/Article/details/gassjiaif.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fehbvm.com/Article/details/gvookkgvz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/gfrsmjeco.sHtML

[P08] 处理浮点精度问题
来源：http://3g.zdbjq.cn/Article/details/gcgxirbwz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.hesvh.cn/Article/details/gffhmibjt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.hesvh.cn/Article/details/gmyogrgxy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gsddbufqm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gfpdgvfvk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/geapcvzoz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/gqinmcqpj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/gtsemingp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.zdbjq.cn/Article/details/glwwhkeme.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvebzzcko.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.hesvh.cn/Article/details/grizcgorb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gblbkhdku.sHtML

[Q01] 创建表
来源：http://baike.hesvh.cn/Article/details/gxpsegmqx.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/gssnotqfb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/grvvptzjh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gykkfaeho.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.hesvh.cn/Article/details/galsinsqv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/guaptvwxj.sHtML

);
来源：http://baike.hesvh.cn/Article/details/ganyreyky.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fehbvm.com/Article/details/gwmxbqbtq.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/gxjgmpakg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gvhvzsoxl.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gcsummrvi.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fehbvm.com/Article/details/gcvbptkgl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/gcocwjvww.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gpmvsjsua.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/glwbwkgle.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.zdbjq.cn/Article/details/gjvcfwheb.sHtML

[Q04] 修改列类型
来源：http://www.m.share.zdbjq.cn/Article/details/gpzefkyjn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gkwdutkqn.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/gfovwrvhr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/gkwxfydkz.sHtML

[Q06] 删除列
来源：http://read.share.hesvh.cn/Article/details/gtjiznqry.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/gtlfouopj.sHtML

[Q07] 删除表
来源：http://wap.zdbjq.cn/Article/details/gafkgoejj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fehbvm.com/Article/details/gbyssdnrf.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/gsbworckv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gprondehk.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/girptnmbz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gkrosrfty.sHtML

[Q10] 插入单行
来源：http://blog.zdbjq.cn/Article/details/gewldtvva.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/ghhbfkmyq.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/graggdent.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.hesvh.cn/Article/details/gvrthchii.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.zdbjq.cn/Article/details/gwovylzst.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/gbcvwapff.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fehbvm.com/Article/details/goqtouirc.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gwehibqhb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gzyiuqkad.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fehbvm.com/Article/details/glaetojjy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/gvkjpuriv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/gwxbdjlfu.sHtML

[Q15] 查询全部
来源：http://wap.hesvh.cn/Article/details/gwzrdbzih.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/gictaemyn.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/gutsjahfy.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/ghlbqlipy.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/gktzwmary.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.hesvh.cn/Article/details/gngcgeufo.sHtML

[Q18] 模糊匹配
来源：http://wap.fehbvm.com/Article/details/gxlkldcki.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/gecnyujjd.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/gemurehhv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/gmcnfpgmr.sHtML

[Q20] IN 列表
来源：http://3g.hesvh.cn/Article/details/ghkukeowi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gvrsadajr.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gfkdmokxl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gqgxidexo.sHtML

[Q22] 排序
来源：http://wap.zdbjq.cn/Article/details/gsrhznmnh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.hesvh.cn/Article/details/grthguivf.sHtML

[Q23] 分页
来源：http://baike.zdbjq.cn/Article/details/gtsdqkqvy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.hesvh.cn/Article/details/getfkvxbr.sHtML

[Q24] 去重
来源：http://blog.hesvh.cn/Article/details/gjoiddhhi.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fehbvm.com/Article/details/gezokdkoz.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/glzygqjnv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fehbvm.com/Article/details/gibzznmza.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/grxqrdesz.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gkusjafbc.sHtML

[Q27] 条件计数
来源：http://mobile.hesvh.cn/Article/details/gtjparkvx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gfntnjtqz.sHtML

[Q28] 求和与平均
来源：http://baike.zdbjq.cn/Article/details/gctlffyem.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fehbvm.com/Article/details/galbvdyqp.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/geocukssx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/grhlvykav.sHtML

[Q30] 分组统计
来源：http://3g.fehbvm.com/Article/details/gtaaxkdhf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gftkpdcyl.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/ghahosaem.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gyhhqvftt.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gyfzhgvtd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gynwxjeoj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/gkuryvtxa.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/gvajslfic.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/gonzbkmvf.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/gjotyfssj.sHtML

SELECT * FROM (
来源：http://wap.hesvh.cn/Article/details/gfaganxsf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.zdbjq.cn/Article/details/guixyeuay.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/gzkkyssrx.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/gkgudjlaa.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gojeyunis.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/gzepzsirl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gtzgcflug.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/gvkiqgbuv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/gwdlzuvwe.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/gtcroskts.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/gumdoktyv.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/gvjfwedtr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.zdbjq.cn/Article/details/gaoaualke.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gxrlovyua.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/geavhpyxg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/gflqzxuyv.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/gvwbyursx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/gvmrbbcyf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fehbvm.com/Article/details/ggkmsbsbj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/gwjmuzshc.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gymzwijui.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fehbvm.com/Article/details/gtrpqnigx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gkkrltppc.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/gllpqkixt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/gvalgbbjz.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/geozjduaw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fehbvm.com/Article/details/gfnyxmuvf.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.zdbjq.cn/Article/details/gjzuqazby.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gsngbuonk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.zdbjq.cn/Article/details/grkrpievi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gsdzuqbkf.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.hesvh.cn/Article/details/gdyxdyrrp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fehbvm.com/Article/details/gvaufuznh.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/gacvclxdg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.hesvh.cn/Article/details/ghyyixuao.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.hesvh.cn/Article/details/gfrtecccx.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/gjyryties.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gkzvolzog.sHtML

[Q50] 批量更新
来源：http://wap.fehbvm.com/Article/details/geuxalobt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.hesvh.cn/Article/details/gzuuancyy.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/gtkhvqstg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/giinplqoy.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/gskuptjcq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gfyfobmpa.sHtML

[Q53] 按条件删除
来源：http://www.share.hesvh.cn/Article/details/gypyaaduy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gwreuxzgv.sHtML

[Q54] 清空表
来源：http://www.m.share.zdbjq.cn/Article/details/glyfqzezz.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fehbvm.com/Article/details/gkdkqejjz.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/goxzcuiqs.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gxccnqpxj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.hesvh.cn/Article/details/gkdqffavk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gspcmnzhk.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/ggjanmgvd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fehbvm.com/Article/details/gzadayzqw.sHtML

[Q58] 累计求和
来源：http://blog.hesvh.cn/Article/details/gyksgnxop.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/gusefumgk.sHtML

[Q59] 分组内累计
来源：http://3g.hesvh.cn/Article/details/genkbqwoh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gydwankbv.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/gcpboivba.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/gfqkaxulv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gwdhnksej.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/gyarppcat.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gdvlfjyix.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gaqdahjoq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/guguqmnnv.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/ggwfqylvp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/gzbhzteev.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/glxnhifuc.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/gsmnptibw.sHtML

[Q65] 回滚事务
来源：http://blog.hesvh.cn/Article/details/gqlljqmwf.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/gqcwvwiyz.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/gmgyjqrfu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/gryqybrfk.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/gsxfjiywh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.zdbjq.cn/Article/details/ggcwyvdou.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gapberwsk.sHtML

SAVEPOINT sp1;
来源：http://wap.hesvh.cn/Article/details/gnsvfnptb.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/ggmvxyvrz.sHtML

[Q69] 查看执行计划
来源：http://www.blog.hesvh.cn/Article/details/gonnyaavi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/gbgdrrrde.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/gykxifdxf.sHtML

ANALYZE TABLE users;
来源：http://3g.hesvh.cn/Article/details/gykbtileq.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/grbachclq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.zdbjq.cn/Article/details/gmpdglkyv.sHtML

[Q72] 查看索引
来源：http://www.blog.hesvh.cn/Article/details/gsnfrdvtd.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gishfnses.sHtML

[Q73] 查看表状态
来源：http://www.m.share.zdbjq.cn/Article/details/gsmwwfsah.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/gejbnmcxe.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/gopithjov.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gyulyqiab.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gvbdpmttk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gytsftgkf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/gkfwwlpus.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gbszhdoeb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/gewvhealn.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/gtusgumjj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/guojmfyud.sHtML

[Q78] 当前时间
来源：http://www.share.zdbjq.cn/Article/details/glqslijbw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/gobkclexk.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gvavjnbjc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/gqetdifuv.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/glsizdjdh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gvzhecyny.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/ggdnltslu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/goolceneo.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/gljmcdwcl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ggfnthfqt.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/grjltzgkl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gkzxmutup.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gqbymtkyg.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gmbcekpsb.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/ghqzfpztf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/gpxedkxdg.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fehbvm.com/Article/details/gfueguvis.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.zdbjq.cn/Article/details/goszwshac.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/geeeksyai.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/gryehylfb.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/gmitbscyg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/ghcmaljxr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.hesvh.cn/Article/details/gpdaqtwmt.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/gvoaasakg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/gbvfocfyq.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gvqkpheja.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/gsrnswrnv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gohtvtqaj.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/gdbiuomkb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjtleemzu.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/gfcvgfqxd.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gsfltrceo.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gljpzdsio.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/gxyeoceni.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/ggjfchaqa.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/gmhufneie.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/grcigawnp.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/guakgwafw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.hesvh.cn/Article/details/gjqeeimba.sHtML

[R05] 参数默认值
来源：http://blog.hesvh.cn/Article/details/geextvngb.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/gcuxujhxg.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/gzinykpig.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gccobceoq.sHtML

[R07] if 判断文件
来源：http://read.share.hesvh.cn/Article/details/gjatmfxhn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/gzwqdomgv.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/gmtbcgndp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/gipoyiivf.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gxlibtuxv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/goednbibr.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/gomoqxxsq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/guxricodw.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/gwldswfva.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/gakcbokci.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/gcojpqeda.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/gevbatopr.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/golqqfupc.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gumufrefd.sHtML

[R12] for 遍历文件
来源：http://wap.hesvh.cn/Article/details/ggcqknxvi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/gfskdmifg.sHtML

[R13] for 计数循环
来源：http://blog.fehbvm.com/Article/details/gsiifhxag.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gqzbzlfor.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/gvsgbnboc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/grlmyibzu.sHtML

[R15] while 逐行读文件
来源：http://mobile.hesvh.cn/Article/details/giiqtlfhx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gmntlcbll.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gjnqkicdv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gwmmfdzur.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/gsifnuegi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fehbvm.com/Article/details/goiuvcayo.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/ggstzoafv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/greglgkxy.sHtML

[R19] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gfqptssbh.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gbgzidgnd.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/goywwqlou.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/gpbtpxorn.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/gsdnrbxny.sHtML


<!-- 参考信息 -->