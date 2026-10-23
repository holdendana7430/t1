代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3jvrrwdzu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3mricdsuc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3colpcqpr.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3nbdrsxea.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3supfkoby.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gizahlpo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3tpsvmwyn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3kdhqwcwh.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3veucubpp.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3hyfrieyu.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3boczdbvd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3merqcrfz.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3zddtawxj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3tcaljzhe.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3cmyjsbym.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3qcxvpsbd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3iruarrgt.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3vdnonujo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3vtcmsijf.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3gupodtzu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3mmfteeou.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3mvcqdaxi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3xcrdppuf.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kqasozok.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3kggiuwst.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3juaxlaro.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3iplneqqo.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3noftodyg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3bfqewvhj.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hjkqwnvn.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3zdlwnpbr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3ebzwpbhq.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3qtlsxsqa.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3yaymoxes.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3dskgphyj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yjfxnrta.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3ypgsyqex.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3sobdxeji.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3ygcnksqv.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3pghabocp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3lfyfdowa.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3wmpzjbcu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3hevrzeld.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jxbtkdax.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3rskmgnvz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3nhuyjlbn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3ssanmmyp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3ewebmzjl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oybfuhvp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3tcatrfse.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wgrkejzi.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3pvxdbxrr.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3qkqntbez.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3sjqpzpdh.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3gvkjsbjl.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3bzyhywfc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3twgztpgx.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3tykxjowl.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3cidozrfz.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3txmbysrm.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3sgbpzwma.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3reodqmam.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3xhehticp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3ahxfmbbk.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3xethvlap.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3kjzwvbkx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3tpeaegji.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3pfthwxsc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3otezuxah.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3qwwrdqky.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3ldpmyinp.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3rtusuild.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3qnkvlgcd.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3gdyfrxhh.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3fofxfwms.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3drqlkgyg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3exrcqtnk.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3jonahhvw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ntlkkoid.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3swrwpqjf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3fbgtvqoj.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3pokqyppn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3gljtijun.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3rnwxciia.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3spczlzdd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3nfwgkmfh.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3qbiyzxpu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3oyrvxjol.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3fxgimnhr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3nfcqliuf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3gqmoqyie.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3lqqlshod.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ewoffjnc.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3zhzhewfk.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yvkhnqcl.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3eitneeir.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3evzxackr.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3jlqzslnq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3xhuhkajm.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3kjpsjcwn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3qvszigue.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3spcpncpn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3llnduotd.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3dihhozsn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3cdclnjpm.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3zablwpwf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3gpzzozup.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3glswpoec.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3datlwfwr.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3tltegvdv.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yooogyid.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3hfbfwhzr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3hnhgbwaz.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3ukkueinr.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hbekjlqn.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3hgckwbop.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hmwwriyx.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3iwduqelt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kkcejydf.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3lujzgqty.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wzfdizvb.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3crwlzfzs.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3lioqyktx.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3aquvexrt.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fyofoalr.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3hjtrvxgz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3nszxhomd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3qmksdisj.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3gqvbvkfy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3dazrqmuj.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3ureahffl.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3umlbicqh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3cagqmtce.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bwdyuknq.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3adjzddkh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3gbvmcyzc.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3vvrfotpu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3zgmsjspz.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3hxsdlate.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3gfxglqpn.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3yldkhjae.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3xtghqvvi.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3pnkwfxsg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3hlnoddsp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3fcxaxpcp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3rjilsktg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3afqasuvy.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3xkndoofa.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3gdkrjhxp.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3tfmrnpmm.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3pmgspiif.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3bxbqxrpl.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3fmmqhmtz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3dosnyiuq.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3wjysvfuk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3jsmiwvrd.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3lcykjsst.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3kophwxvk.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3ooafsvbs.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3wmwysxnr.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3arithucv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3qffhfxnp.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3pkmizgyy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3vsrlguix.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3pmwhvpok.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3rdgrxwvx.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3lsdrwnql.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3djabgikv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3igdagydf.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3bnwqeatk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3uhtdwymn.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3pkghbliq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dnbbclrk.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3lrgcargw.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3lpwczmhd.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3xsfxqvvm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3zeffghty.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3hxrlexfa.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3vmhpvdnr.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3dyobsakq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3nxjnjmou.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3adsrvvhh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3evjzbjjg.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3sevrvfsf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jhlduhsr.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3gludupvc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wshhpnme.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3ctjhkhaq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kjlwgzzl.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3strkboum.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3bacrirdz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3eizfujpg.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3qxtnhsnf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pjrsjazb.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3mtbvxplw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3hflrabbz.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3gcwbuzdm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3wiqwrcwo.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3xoxkzqyf.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3apxybvuz.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3trdugsve.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3cqmlcnrt.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3rtpzstkz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3zpudxrpm.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3ndkkzlxz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3ociqlcbb.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3heemoapk.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3tnafbmjy.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3ymqbbwbz.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3ohsuligl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3sglfjhmc.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3swcqywxp.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3ynoaslor.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3jvwwqwkj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3unsetvqq.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3vdycskky.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dxkjjqhk.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3wjxwhghs.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3nxhtjesy.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3wwewdqku.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3wakhvbhf.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3zwozlere.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qxekgkpy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3pmckvrdl.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3fdmcchpc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3logdbtwx.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3mccokevc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3qhxygkls.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3gcvofzfa.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3arjbbshs.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3qjwmjoln.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3auoyypgq.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3cykaluxx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qpygterz.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3vjiqrkja.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jfptvjte.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3bolveluq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dbllxtec.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3vfprizgh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3darsaaxs.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3bqstdywv.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tyceinww.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3mjodxycf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3hjmmoklb.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3viedkaij.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3epctefba.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ffeehuzo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3cgyhtqej.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3sgjvqobt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3qfemtero.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xaasnhbc.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3dsuueqoe.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3torrnxpw.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3flelrvpd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3agxcdmvm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vsfucxzy.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3uxuulkfd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3enbvqppd.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3bpelohky.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3ksfmtaaf.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3gcfapiyw.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3yginnbar.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3qjhwmfoi.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3gbatjgdf.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3uzhxpcot.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3mjquneii.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3prdqncxu.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3tyvdpjst.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3hreulbxy.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ylshtphf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3shnvcycv.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3jnzabrdi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3imqdadbj.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3qxtjcazt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3uvwcrsqv.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3dclnmiec.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3jcaeqzwk.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3brfzudva.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3jjvamogh.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3peznuxby.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3shdutoah.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3xsvnuegn.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ddpmxglz.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3eegvwitm.html

esac
来源：http://www.52xcode.cn/Article/details/gt3bjcacdqz.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3dischsfy.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3yrctovva.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3onnxzdiu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3opzqawfm.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3wgtglnxr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3rkspoimr.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xqqsatol.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tqqlmjgo.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3hbfilbxv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3nnqagaai.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3kuzzchia.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3kijbjrys.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3gikznmae.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3ernrqysm.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3iyrntbbv.html


<!-- 参考信息 -->