代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gvgfchosm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fanxiaobao.xyz/Article/details/gfknribfj.sHtML

[P03] 生成短随机字符串
来源：http://blog.fanxiaobao.xyz/Article/details/ggbxtlvrx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fanxiaobao.xyz/Article/details/grtlzbzqv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fanxiaobao.xyz/Article/details/gkhsgbeus.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhzwajsn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsomfksde.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtknmdtc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvguwxhp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fanxiaobao.xyz/Article/details/glehvkfak.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqfakfhk.sHtML

[P04] 求长度
来源：http://blog.fanxiaobao.xyz/Article/details/gpyooinlu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvihhlnx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutqxyfjq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdhhfxuw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fanxiaobao.xyz/Article/details/gryidguxn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbioerhw.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrpwufwo.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fanxiaobao.xyz/Article/details/gojidohls.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtcpooxd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fanxiaobao.xyz/Article/details/gqhqhrfzp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fanxiaobao.xyz/Article/details/guwwnlvje.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fanxiaobao.xyz/Article/details/gtrtestwg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fanxiaobao.xyz/Article/details/gsllkxtos.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fanxiaobao.xyz/Article/details/ggnzdmjdt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtwtguvx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwwqoqon.sHtML

Ruby: a == b
来源：http://m.share.fanxiaobao.xyz/Article/details/gitmlaydu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fanxiaobao.xyz/Article/details/gqiuqhbum.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fanxiaobao.xyz/Article/details/geplczjpr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fanxiaobao.xyz/Article/details/gniawntbf.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gxjbthgku.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fanxiaobao.xyz/Article/details/gbztnewcj.sHtML

TS:   if (x == null) {}
来源：http://3g.fanxiaobao.xyz/Article/details/ghguukokn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gysyyuqxq.sHtML

Go:   if x == nil {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gdksyfkjv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.fanxiaobao.xyz/Article/details/gstmfudga.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwpgawed.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlpaygdo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfltlwrau.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fanxiaobao.xyz/Article/details/goaupdvsy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gclaqfzlo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggscpgtub.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gyskylsfd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihfmodca.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxuocisx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fanxiaobao.xyz/Article/details/gvhuphxyl.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fanxiaobao.xyz/Article/details/gtytvufyk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fanxiaobao.xyz/Article/details/gmujkzyaa.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gfuihwzpk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkmxqfts.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqalyjzv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fanxiaobao.xyz/Article/details/gzeeyhdhx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fanxiaobao.xyz/Article/details/ghudflpbo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fanxiaobao.xyz/Article/details/gefcurjzb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqtzjvjf.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gdooglwmc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gliidyjne.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gsobjytpd.sHtML

[Q01] 创建表
来源：http://3g.fanxiaobao.xyz/Article/details/gqozynttc.sHtML

CREATE TABLE users (
来源：http://m.share.fanxiaobao.xyz/Article/details/gbigqiysn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fanxiaobao.xyz/Article/details/gqsamyhth.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjjtnimk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fanxiaobao.xyz/Article/details/gyazbwvyq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fanxiaobao.xyz/Article/details/gurdeiszg.sHtML

);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzzfsqst.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzbkzdcq.sHtML

CREATE TABLE orders (
来源：http://www.share.fanxiaobao.xyz/Article/details/gtufsleis.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fanxiaobao.xyz/Article/details/gyuwghtwa.sHtML

user_id INT NOT NULL,
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjofehpp.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fanxiaobao.xyz/Article/details/gfiiobsdw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fanxiaobao.xyz/Article/details/gvavzczvv.sHtML

);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvwkzxfj.sHtML

[Q03] 增加列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzfyqvcq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqqmjwlp.sHtML

[Q04] 修改列类型
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbusdybz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxznyppdt.sHtML

[Q05] 重命名列
来源：http://read.share.fanxiaobao.xyz/Article/details/gqktwxkez.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fanxiaobao.xyz/Article/details/gdmngnywl.sHtML

[Q06] 删除列
来源：http://3g.fanxiaobao.xyz/Article/details/gylrlrqat.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggudrcmzj.sHtML

[Q07] 删除表
来源：http://www.share.fanxiaobao.xyz/Article/details/gmclzxysn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmhpzyom.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkjngqcq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhxbqoza.sHtML

[Q09] 创建唯一索引
来源：http://3g.fanxiaobao.xyz/Article/details/gjnljpcly.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbitczknc.sHtML

[Q10] 插入单行
来源：http://3g.fanxiaobao.xyz/Article/details/gllvvashy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdkekkbe.sHtML

[Q11] 一次插入多行
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlhjaufk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrvlpclz.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fanxiaobao.xyz/Article/details/gaczvxdeq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsmqwrwq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fanxiaobao.xyz/Article/details/gprasgapo.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fanxiaobao.xyz/Article/details/gtongwxgh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gnpzuefji.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqttrapg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fanxiaobao.xyz/Article/details/gqshgklnm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fanxiaobao.xyz/Article/details/gkeaefjuw.sHtML

[Q15] 查询全部
来源：http://m.share.fanxiaobao.xyz/Article/details/gfknqrqyh.sHtML

SELECT * FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/getiwlvgv.sHtML

[Q16] 查询指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/ganmicjbe.sHtML

SELECT id, name FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gztxfqvjs.sHtML

[Q17] 条件查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbhnevde.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxxmxcno.sHtML

[Q18] 模糊匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbffelag.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpjzunip.sHtML

[Q19] 范围查询
来源：http://blog.fanxiaobao.xyz/Article/details/gkahyutdc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdeubdsb.sHtML

[Q20] IN 列表
来源：http://3g.fanxiaobao.xyz/Article/details/gjhyorcvv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gsyzkmbwh.sHtML

[Q21] 空值判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnahqeruu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fanxiaobao.xyz/Article/details/gatiyfmku.sHtML

[Q22] 排序
来源：http://baike.fanxiaobao.xyz/Article/details/gsymnqoks.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fanxiaobao.xyz/Article/details/gaictiqvy.sHtML

[Q23] 分页
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxrqcgwm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtredbvg.sHtML

[Q24] 去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvgjzupx.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gbeheuage.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcurbepl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fanxiaobao.xyz/Article/details/gleezfmkm.sHtML

[Q26] 计数
来源：http://wap.fanxiaobao.xyz/Article/details/gdjfwcfmk.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpeftwinz.sHtML

[Q27] 条件计数
来源：http://blog.fanxiaobao.xyz/Article/details/gdxioeyee.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/geqisxcrv.sHtML

[Q28] 求和与平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpeqiruhe.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvllfkblq.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmlwosop.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbezrytcx.sHtML

[Q30] 分组统计
来源：http://blog.fanxiaobao.xyz/Article/details/gyhiapblp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzdlrykg.sHtML

[Q31] 分组后过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gllwnvukv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwipcpoqf.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gbnwteexn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghouheivw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fanxiaobao.xyz/Article/details/giogcakul.sHtML

[Q33] 多列分组
来源：http://mobile.fanxiaobao.xyz/Article/details/grllcqspa.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqzurkdq.sHtML

[Q34] 每组取第一条
来源：http://www.share.fanxiaobao.xyz/Article/details/ganbgybtd.sHtML

SELECT * FROM (
来源：http://baike.fanxiaobao.xyz/Article/details/gmkqcojir.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmdfocsp.sHtML

) t WHERE rn = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gfgijbhbl.sHtML

[Q35] 内连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhjhunrv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyggdbdiq.sHtML

[Q36] 左连接
来源：http://baike.fanxiaobao.xyz/Article/details/gctoofeqk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsajchvou.sHtML

[Q37] 右连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gljfqghxd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gxowbhztj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylcbxakv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gagtjdinz.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fanxiaobao.xyz/Article/details/gydkbgtjy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcsfwlii.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gvtapouvt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpdlgjtr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpuhibzw.sHtML

[Q41] 多表连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzdfqoug.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fanxiaobao.xyz/Article/details/gtypdvupu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzlkqsap.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gqmjepisa.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gcnpjzlbs.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnndszug.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gklyojhtz.sHtML

[Q43] 标量子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpknggrd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyohyvwkt.sHtML

[Q44] IN 子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gwfhifqqo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fanxiaobao.xyz/Article/details/gzblfifzs.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkbonufw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gmonwyirp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fanxiaobao.xyz/Article/details/gavitvued.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gjhgxwtfo.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghupxjuwm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fanxiaobao.xyz/Article/details/gyubrbhqw.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbnsddqo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvcqqqlq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gqqpddabx.sHtML

[Q49] 更新单行
来源：http://m.share.fanxiaobao.xyz/Article/details/galuvqzax.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gvfbsbqzu.sHtML

[Q50] 批量更新
来源：http://blog.fanxiaobao.xyz/Article/details/gxfelhefu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gamunuetb.sHtML

[Q51] 用子查询更新
来源：http://baike.fanxiaobao.xyz/Article/details/gozozqugh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/ggeuhkuha.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guttxtexo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcigdyrmo.sHtML

[Q53] 按条件删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gboqpvame.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykzfuviu.sHtML

[Q54] 清空表
来源：http://baike.fanxiaobao.xyz/Article/details/gcgqrmrkb.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvskihtj.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrumkggf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjfbgasq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gxapigmto.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gshlbtysz.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxbfkhjo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/guxfmhuic.sHtML

[Q58] 累计求和
来源：http://wap.fanxiaobao.xyz/Article/details/grshljnkn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gieswmubp.sHtML

[Q59] 分组内累计
来源：http://wap.fanxiaobao.xyz/Article/details/gakxddpvb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gvydgkods.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmkkryrg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gwakfhdqr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gdffpouju.sHtML

[Q61] 移动平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysdunzso.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gevqbuleg.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gzdgqpzas.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gojkrhziw.sHtML

[Q63] 开启事务
来源：http://baike.fanxiaobao.xyz/Article/details/ghmzfbefg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fanxiaobao.xyz/Article/details/giwsmayfa.sHtML

[Q64] 提交事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgeeeyjd.sHtML

COMMIT;
来源：http://3g.fanxiaobao.xyz/Article/details/giivfqmfd.sHtML

[Q65] 回滚事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjyvychv.sHtML

ROLLBACK;
来源：http://read.share.fanxiaobao.xyz/Article/details/gywdgzplj.sHtML

[Q66] 行锁查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsdhvbnx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fanxiaobao.xyz/Article/details/gexfswghb.sHtML

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/grwehxdye.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fanxiaobao.xyz/Article/details/grkdyfbpp.sHtML

[Q68] 保存点
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvovsvfzc.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwqeqaej.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpbhpism.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/gcxqokarj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkijgosr.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gueqlfwcq.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/ghisjvabm.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gswmhtpbc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/gfeusseqi.sHtML

[Q72] 查看索引
来源：http://3g.fanxiaobao.xyz/Article/details/glntguoly.sHtML

SHOW INDEX FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gzusckeim.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/gudwvkwty.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcbpajyb.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxpabxhi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/gelqgiupi.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gjsucrbbm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gbpqzksgx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhdhoktd.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/gvuvdwicq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fanxiaobao.xyz/Article/details/giecxqtne.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/gregoqser.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/gezmptnhf.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/gwsldddqe.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/golttpqsq.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwtqcwtu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctrsusrb.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfkikfah.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gfitamtsd.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdlhgaqr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzcdqxqg.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gyoekqlxi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gnxfwqulc.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gjgolkjnn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gumqfztox.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/gpjnteods.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhejnbpc.sHtML

[Q85] 数值取整
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvmrpvza.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebnwkkdt.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gugmthyro.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhsjhurm.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrlkxojz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/gebbekqba.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gmgwteyad.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/grzqhrmcw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/glailjjjb.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gsjfcvlxm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gquirjodj.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlskpqlm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmonuaik.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdrqaeyo.sHtML

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsxidzjq.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkbhsuls.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/gybpsfrai.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gupaqufbg.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggyhujyue.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtuabthg.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzysztzcy.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gahewqrvt.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/glycksgud.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagbrxldb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/gqdsnhipv.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gozieehdn.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/guiazezcq.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxcqmuft.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrvcxsog.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gksendtbt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gplvujbfy.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gknuwzrss.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grztuuzmk.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gtcrtusfj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqxpyflv.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gjhzrsokp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/giuomkdsj.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/gsabhxepg.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgobmmil.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gmcnwswht.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gsiaushpo.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkosoyrby.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbwqxrpw.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gdpcmkmik.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqzabxst.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/geceqnpnu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/glvmptutc.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gjevaijbc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtexjcdd.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gsaowepmh.sHtML


<!-- 参考信息 -->