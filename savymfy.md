代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/gxhmmjbmw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gbzhjhbmm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gxjtaxlsq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.hesvh.cn/Article/details/gmojzoksl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.zdbjq.cn/Article/details/gvddfiieh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/gxfwdqetl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/ggkdxauck.sHtML

[P04] 求长度
来源：http://3g.zdbjq.cn/Article/details/gutjvgouf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.zdbjq.cn/Article/details/gsmkrizfs.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/geoqovpwl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gqchyvkxp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gmhdanscc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gepeaturm.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gdunhvmas.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fehbvm.com/Article/details/guznlxvib.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/gfdvbfvzn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/gbmnopwwo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.hesvh.cn/Article/details/gjbxscnkd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.hesvh.cn/Article/details/gmarhozed.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/gflnyslvv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/glcaumfjw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fehbvm.com/Article/details/gzbworvpk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gpmrhpdxy.sHtML

Ruby: a == b
来源：http://blog.fehbvm.com/Article/details/gohdkyurg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.hesvh.cn/Article/details/guauxcygd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/grpfspofa.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.hesvh.cn/Article/details/gagrrzrel.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gkhgfzopj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/gkkmlpfkc.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gkriftoqe.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gspyfvtkl.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/ghblywblf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/geqteakje.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gpuvczjdp.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/giarafjtf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.zdbjq.cn/Article/details/gixwzamim.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gtlmlqgeq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gldnowvqy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gdceiqkbx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/ggyqppzat.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/gwaktaefy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.hesvh.cn/Article/details/grrfkzwlr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/gyzyxtcey.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/gslbbvfen.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/gfkpcismb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/gbsokzlhf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.zdbjq.cn/Article/details/gououknfx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/gxipuwdwk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/gydrvhfsx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/gcdzhgdxg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/gefqqwqpr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gkmvvbodx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwcfweyii.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/gyncxautf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggtdcwogl.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gxwhmtxpq.sHtML

CREATE TABLE users (
来源：http://m.share.hesvh.cn/Article/details/gpgvltgyz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gehdidmct.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gqjooxkwv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/gcppokkxw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fehbvm.com/Article/details/gjxiwxdyt.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gqckdvfcw.sHtML

[Q02] 创建带外键的表
来源：http://baike.hesvh.cn/Article/details/gnmxteaxh.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/gakngfjok.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gjpvtecxb.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gyrocshei.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/gwiwmdxfv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/gftilabpt.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gmbskpuun.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gttdsszbr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/geeojrmzu.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/gvrvfetmb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fehbvm.com/Article/details/gdijyivyp.sHtML

[Q05] 重命名列
来源：http://baike.fehbvm.com/Article/details/gmsqvjcgn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.hesvh.cn/Article/details/gtwpvclea.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/gioqsuunp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/gmzcrmedg.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/gbbrrjrgw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fehbvm.com/Article/details/gljhqtwmn.sHtML

[Q08] 创建普通索引
来源：http://baike.zdbjq.cn/Article/details/gwcfykzok.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gesqtjcdt.sHtML

[Q09] 创建唯一索引
来源：http://baike.hesvh.cn/Article/details/ggvfejaoi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gjxcbntcu.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/gzgtvwadv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gzohfzhdx.sHtML

[Q11] 一次插入多行
来源：http://www.share.hesvh.cn/Article/details/giizehcha.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gneadxuqn.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/gwqratyjn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/gvgyoqsdf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/grdfwqksj.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/gfypeurpp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.hesvh.cn/Article/details/grrszibay.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gniwawwcs.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fehbvm.com/Article/details/geunfnrrg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.hesvh.cn/Article/details/glqktvtrt.sHtML

[Q15] 查询全部
来源：http://www.m.share.fehbvm.com/Article/details/gqqinaaxq.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/giwivitqu.sHtML

[Q16] 查询指定列
来源：http://baike.fehbvm.com/Article/details/gapxrgyid.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gjwpixcof.sHtML

[Q17] 条件查询
来源：http://blog.hesvh.cn/Article/details/gugqiapag.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/gsfsmsscs.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/gogsvfrlh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/ghrcbzooh.sHtML

[Q19] 范围查询
来源：http://m.share.fehbvm.com/Article/details/gxnjsazyg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/gugdniflu.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/gzdldaqtl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/gtskqlevt.sHtML

[Q21] 空值判断
来源：http://wap.zdbjq.cn/Article/details/gbkgghwqd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fehbvm.com/Article/details/gnybluksk.sHtML

[Q22] 排序
来源：http://m.share.zdbjq.cn/Article/details/gowlmtqzb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.zdbjq.cn/Article/details/goqeugkxm.sHtML

[Q23] 分页
来源：http://3g.zdbjq.cn/Article/details/gtvplynhs.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.zdbjq.cn/Article/details/gjhriucdb.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/gvewalcad.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gmdcghmrd.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/gzdoizgkq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/gzjamoiyf.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gbkukxyhm.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gvykxsfuy.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/gwiupfhnu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.hesvh.cn/Article/details/gjextpxdh.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/gmnbhuszl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gaysotsuc.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gqqpzbvcj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gytvxsjva.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/gbwkftctc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gnwllfhxc.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/gnimhxrnh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fehbvm.com/Article/details/gusjcqkmr.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gccipspto.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/giunsqwnl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/gxubhssst.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/gbmlsltxe.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gyuujcqtv.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/goxcpgcos.sHtML

SELECT * FROM (
来源：http://read.share.fehbvm.com/Article/details/gpxnqmlah.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fehbvm.com/Article/details/gopmihhqr.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gginovyvp.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/gzxjkjrzp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gfofljkmz.sHtML

[Q36] 左连接
来源：http://www.blog.zdbjq.cn/Article/details/gesrtdhmx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gkozigmqh.sHtML

[Q37] 右连接
来源：http://read.share.hesvh.cn/Article/details/ggoydggfn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.zdbjq.cn/Article/details/grytscalz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.hesvh.cn/Article/details/gqpsnmkck.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/gbpqbzcaj.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.hesvh.cn/Article/details/gnctqsuey.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.zdbjq.cn/Article/details/gemjdmixx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/gfzdtsopf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.hesvh.cn/Article/details/gitmatkkb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/gztpimktv.sHtML

[Q41] 多表连接
来源：http://baike.fehbvm.com/Article/details/gpzbsmmjg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.hesvh.cn/Article/details/gdrljqqos.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/grexyuxmd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/gdppbftss.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gifgdfojy.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/gkksgkonr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.hesvh.cn/Article/details/glwrcjvgu.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/gdgiewagd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.hesvh.cn/Article/details/gghzluhur.sHtML

[Q44] IN 子查询
来源：http://baike.hesvh.cn/Article/details/gobricmdy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fehbvm.com/Article/details/gprzehlyy.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/gxzlfeyay.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gjatibpfo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fehbvm.com/Article/details/gfqzblugo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/grsloafdu.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/gooznhrtc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/gywivnwuq.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/gagqtyqrp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/gsmwpbewh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.hesvh.cn/Article/details/gtgbwzqyt.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/gdsprnwsl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gkrvcfksh.sHtML

[Q50] 批量更新
来源：http://blog.hesvh.cn/Article/details/gwozvkcfa.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gmigzwzfv.sHtML

[Q51] 用子查询更新
来源：http://www.share.fehbvm.com/Article/details/gpkbmrbpo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gifzlwvjy.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/gafmfxqra.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gnwqyadqz.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/gveqgouhm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gwkumknnl.sHtML

[Q54] 清空表
来源：http://www.blog.fehbvm.com/Article/details/gvzfqeayf.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/glwpokciz.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gzdhrcxkr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gjwxnbdsn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/ghfpeexit.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fehbvm.com/Article/details/grulubwrv.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/gwbhheewc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fehbvm.com/Article/details/gfzenmfxr.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/ggoafoqle.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.hesvh.cn/Article/details/gvkltwawt.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/gcbjqftfq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gfyzvzssd.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gpwfxglde.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/gqxdkckyg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gahyrhlix.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/gddosspjl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gkdolpqie.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/gvolkncyl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gsbetbflr.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gpypmtfnz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/gnaycwnrm.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/ghagmjmss.sHtML

COMMIT;
来源：http://www.share.hesvh.cn/Article/details/gpjnyxmkt.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/gczbgzsvi.sHtML

ROLLBACK;
来源：http://m.share.hesvh.cn/Article/details/gafzbmjgb.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/gdzlrzayn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.zdbjq.cn/Article/details/gvcdbbjaf.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/gawkjydsn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/gskmsjszu.sHtML

[Q68] 保存点
来源：http://baike.hesvh.cn/Article/details/gxvtpqwyw.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/gbacnttxu.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/guwukkwdm.sHtML

[Q69] 查看执行计划
来源：http://m.share.hesvh.cn/Article/details/gjgajcgli.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/ghmgkyvbj.sHtML

[Q70] 更新统计信息
来源：http://baike.zdbjq.cn/Article/details/gzudnembu.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gdhrlbled.sHtML

[Q71] 查看建表语句
来源：http://www.share.hesvh.cn/Article/details/guhramftn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.zdbjq.cn/Article/details/gqcdavpfb.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/gnbfzievm.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fehbvm.com/Article/details/ghtungfqa.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gfgftgneb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/gqutiqvja.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/guhwdanci.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/gkybbndpu.sHtML

[Q75] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gitgettdc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gklfscgps.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/gylxbcvud.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gwpotbvsu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fehbvm.com/Article/details/grpnzeuoz.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/gncoxsxdf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/gelozqezm.sHtML

[Q78] 当前时间
来源：http://www.share.hesvh.cn/Article/details/gwkpoheql.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/ghswagftk.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gdheniosu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/gpbbncatu.sHtML

[Q80] 字符串截取
来源：http://baike.fehbvm.com/Article/details/gitkgaeiv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gowtppxpu.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gdnnlifhn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/gmweqwxnr.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.hesvh.cn/Article/details/gbuzpasyh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/ghxirjllq.sHtML

[Q83] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gvjuksmml.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/ghotbnofw.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/ghmrwverf.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gdwliyiax.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/ghpkpmpop.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gnyukdyin.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.hesvh.cn/Article/details/gaztxoqvt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/gbdokdqpy.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/gihnlncdo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/glnwjmiau.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/gkkbnmfyd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/gxkwqeckd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/gpblttzet.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/goywuodak.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fehbvm.com/Article/details/gsyzdvnhg.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/gmrzlgdne.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fehbvm.com/Article/details/ghxzoexqp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfmrmxdps.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/gwxzudgpg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqcwwlmof.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/gtohbwthp.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/guwdqhpqo.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gqgkpevua.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gbitusrxf.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fehbvm.com/Article/details/gzcytqjjo.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/gxndqngds.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/gisykvznj.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/gyfklturd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gsjuwnxha.sHtML

[R05] 参数默认值
来源：http://www.blog.zdbjq.cn/Article/details/gagqdqhwg.sHtML

name="${1:-default}"
来源：http://www.m.share.hesvh.cn/Article/details/gnwadtgdf.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/gkbghehpw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gdjgkkpvu.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/gzlzlsqeb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/gfqoonmai.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/ggdnwmvas.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/gxvgtrnds.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gqrvxxklm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/gpnqnkcdw.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/gikwjrhaz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/gyonvepia.sHtML

[R11] case 多分支
来源：http://www.blog.fehbvm.com/Article/details/gvuicrcfo.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/gagvvfqwt.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/gbewiqphx.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/gbypskxrf.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gjuxyixhh.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gvpornfpt.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/gihbqokrn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gsugaqdym.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gmqtamtyt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/glsxsupww.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gatucxual.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gkqqqnuhw.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gnzlpxhzu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gtaoyjgnp.sHtML

[R16] until 等待条件
来源：http://3g.hesvh.cn/Article/details/gvysgzmpd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gkfmlsimt.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/glnpxzjnm.sHtML


<!-- 参考信息 -->