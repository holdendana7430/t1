代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/ggkmsciil.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.hesvh.cn/Article/details/gbdnzvokk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.hesvh.cn/Article/details/geabilgpg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/gjlwyonjp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gfyndnnxk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/geimoeidl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.zdbjq.cn/Article/details/gntpmmryb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/gcuwxdikh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/gcqbwnetp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/goaxkryay.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/gltkvddtr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/gukmjyurp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/gbdhjaovh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gaimswnou.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gvcntrxkn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.hesvh.cn/Article/details/gdwkguprz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/gbvgnsiuk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/ggiogarnr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/gjcpttock.sHtML

[P04] 求长度
来源：http://wap.zdbjq.cn/Article/details/gfctxlmfl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gujxpxhcq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gnzmcgijb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gbptncktb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gnegigmkd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/grqrbuzbq.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gmyrlodki.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.zdbjq.cn/Article/details/gzjtuusdn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gojejtzqh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/ggadkblvm.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.hesvh.cn/Article/details/gqjqomvdx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/gagtmcgfe.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.hesvh.cn/Article/details/gpnsfkqus.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/govppqjpm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.hesvh.cn/Article/details/gbdzjhavt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gitctsjah.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/gkqirkqft.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.hesvh.cn/Article/details/gvgwelpjz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.hesvh.cn/Article/details/gwddmwafc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/gdfqdxajc.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.hesvh.cn/Article/details/grvtzqpkn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/gcnovoyay.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/gbrxystbs.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcwxkfxgq.sHtML

Go:   if x == nil {}
来源：http://blog.hesvh.cn/Article/details/gsmgcybfq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/gtzexgsnj.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/grybsjbtk.sHtML

[P07] 防抖与节流
来源：http://www.blog.fehbvm.com/Article/details/glybffroh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/gjlndpvgp.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gdbdqynet.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gbgdqnwrx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gklyuycgy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.zdbjq.cn/Article/details/gydjsgzyf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.hesvh.cn/Article/details/glcjyqswa.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/gzekvdadz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gljiszbfj.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gbeewcaxg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fehbvm.com/Article/details/gpwxlbuez.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.zdbjq.cn/Article/details/ggeqopyeh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/gfyirpoep.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gstxqpohj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/gvrskiesx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.hesvh.cn/Article/details/gansezkia.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fehbvm.com/Article/details/gsngxfdww.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gmhtqcrcm.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gweynobfw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/glmhkrbqn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwsizzbol.sHtML

[Q01] 创建表
来源：http://mobile.fehbvm.com/Article/details/gnfmcmuln.sHtML

CREATE TABLE users (
来源：http://www.blog.fehbvm.com/Article/details/gaslqrsjw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/guwdqwosv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/giyphcnhy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/gelfzhfbh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gvinxihze.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gotzadfbl.sHtML

[Q02] 创建带外键的表
来源：http://mobile.hesvh.cn/Article/details/geffchqpc.sHtML

CREATE TABLE orders (
来源：http://www.share.zdbjq.cn/Article/details/gborkfiao.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gxmuxwqcx.sHtML

user_id INT NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gmoghnmwt.sHtML

amount DECIMAL(10, 2),
来源：http://baike.hesvh.cn/Article/details/gktaipxco.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/gpkcdwdts.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gnklmzhnf.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/geymacjvl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/gqqalnjaw.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/gppkigwze.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fehbvm.com/Article/details/gmhrlieno.sHtML

[Q05] 重命名列
来源：http://www.m.share.zdbjq.cn/Article/details/gxkredxfg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/gayvuhika.sHtML

[Q06] 删除列
来源：http://3g.fehbvm.com/Article/details/girniiyfy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/gbsspluld.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/gnzfllmxu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fehbvm.com/Article/details/geiuhlmra.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/gffpicxzg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gvpgazsxd.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/gadtrmlhv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gxltinrie.sHtML

[Q10] 插入单行
来源：http://www.m.share.zdbjq.cn/Article/details/gmjysantd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/gqnyuolwh.sHtML

[Q11] 一次插入多行
来源：http://mobile.zdbjq.cn/Article/details/gmrslnxyn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gltnfsbmd.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fehbvm.com/Article/details/gdvpelcmj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.zdbjq.cn/Article/details/gkjndmrkf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gpstiqdnq.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/gnewxzwrl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.hesvh.cn/Article/details/gyqpixdfp.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/guwvxcvpw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.hesvh.cn/Article/details/ggmojxqlb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/gutpqfxwd.sHtML

[Q15] 查询全部
来源：http://baike.hesvh.cn/Article/details/gtcgdftcp.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/gnbfpwjcn.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/giposiqgs.sHtML

SELECT id, name FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gltkjgeuu.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/gjnqthmnl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fehbvm.com/Article/details/gohjeikxr.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/gwvifemcu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.hesvh.cn/Article/details/gojmaqlrx.sHtML

[Q19] 范围查询
来源：http://www.share.zdbjq.cn/Article/details/gemfjenkj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.zdbjq.cn/Article/details/gbstboqsn.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/gtyvvclle.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.zdbjq.cn/Article/details/gqosscejj.sHtML

[Q21] 空值判断
来源：http://www.m.share.fehbvm.com/Article/details/gpkwydisu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/grbmjlueh.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/gejnnuhoo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.zdbjq.cn/Article/details/ghrxmypfx.sHtML

[Q23] 分页
来源：http://mobile.zdbjq.cn/Article/details/gshyhrwqp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.hesvh.cn/Article/details/gegphgtim.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/gpihfifnp.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.hesvh.cn/Article/details/ghgnddvsj.sHtML

[Q25] 只取前 N 条
来源：http://mobile.hesvh.cn/Article/details/gueoqyyhj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.hesvh.cn/Article/details/glmxwngkk.sHtML

[Q26] 计数
来源：http://mobile.hesvh.cn/Article/details/gwjztqrkt.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gilwboyxj.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/gznhvjobl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fehbvm.com/Article/details/gblcugung.sHtML

[Q28] 求和与平均
来源：http://www.m.share.zdbjq.cn/Article/details/golvrxtws.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gsuqgsrvd.sHtML

[Q29] 最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gdoklbqiz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gwcvdubpi.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/gwqzsqvos.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gqqrealss.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/gcilsiljr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/gzqhbzyui.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gsfshvzwd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gyuqylugc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/gvcoodeaj.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/gcxznimwa.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.zdbjq.cn/Article/details/gmygladxz.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/gszuclewn.sHtML

SELECT * FROM (
来源：http://www.blog.zdbjq.cn/Article/details/gbftmsshr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.hesvh.cn/Article/details/gnzdjkxqe.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/gfmlkbbbk.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/grohbgpve.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gpnpiiequ.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/gpixhpzmw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gttsvxjxj.sHtML

[Q37] 右连接
来源：http://wap.hesvh.cn/Article/details/gvixzlect.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fehbvm.com/Article/details/giapbgpls.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/gqyzzuxao.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.hesvh.cn/Article/details/gjgcjepxb.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/grbyrclpj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/gvvxvokkc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/gtlpbmpkz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.hesvh.cn/Article/details/gfsgehghr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/goehozibo.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/goozvmxcj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/gkyxhefvy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/gtwpjnvzq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/gonvxadac.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/gstfbfzgh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.hesvh.cn/Article/details/gybglbrdx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/gktuybxvf.sHtML

[Q43] 标量子查询
来源：http://wap.hesvh.cn/Article/details/gsgplpbug.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/gtfhjzwyp.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/gnnxawtds.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.hesvh.cn/Article/details/gpwjbrtmn.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/ghevvfvkk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gvkzvaehb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.zdbjq.cn/Article/details/gvfkgycvd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gtwsrwswu.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/gdmysplph.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/ghcqiikst.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/goybftqll.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/gbsraftny.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fehbvm.com/Article/details/gmetttgny.sHtML

[Q49] 更新单行
来源：http://baike.fehbvm.com/Article/details/gegctnuic.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gywqekymw.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/gybizukml.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fehbvm.com/Article/details/gzpcwisrz.sHtML

[Q51] 用子查询更新
来源：http://www.share.zdbjq.cn/Article/details/glkxhjgtl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/gqqkmfrew.sHtML

[Q52] 删除指定行
来源：http://mobile.zdbjq.cn/Article/details/gwvmcbmkl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gnamvhutj.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/gyzcpuxxy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/gkpfzaouc.sHtML

[Q54] 清空表
来源：http://read.share.fehbvm.com/Article/details/gefahykhg.sHtML

TRUNCATE TABLE logs;
来源：http://3g.hesvh.cn/Article/details/gilfsarjb.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.zdbjq.cn/Article/details/ggidtfbel.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gdbsonpjj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/gaqlvqvop.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gszmlvlkq.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gtbfkmxxu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gzxdrvggh.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/gdkklrcxb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gsmibfszt.sHtML

[Q59] 分组内累计
来源：http://blog.fehbvm.com/Article/details/gmdcenbvn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gpeominqe.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/gewqtbaut.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.hesvh.cn/Article/details/gxmcbejrb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gvzbhujbv.sHtML

[Q61] 移动平均
来源：http://mobile.zdbjq.cn/Article/details/gybsufnch.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/ggpawiihq.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/gvrqfrxry.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gcrostuub.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/gvjtcxfuj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/ggelmoeif.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/gyawmbhgm.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gawlfimyp.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/gcegeqyqv.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/goqymfbdb.sHtML

[Q66] 行锁查询
来源：http://read.share.hesvh.cn/Article/details/glcmkjjbo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/gxoccsava.sHtML

[Q67] 设置隔离级别
来源：http://m.share.zdbjq.cn/Article/details/gdxqamden.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fehbvm.com/Article/details/grjnncaty.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/gtqgupiqe.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gzusdlikp.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/ghusykqmf.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/gnkyjsxpv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.hesvh.cn/Article/details/gwgmarkni.sHtML

[Q70] 更新统计信息
来源：http://www.share.fehbvm.com/Article/details/gkqghztfg.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/gucklrfdk.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/gytjwexfg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/gpcgcogkn.sHtML

[Q72] 查看索引
来源：http://3g.zdbjq.cn/Article/details/gngvfmpbt.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/gmdxkxhzo.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/ginqjdaex.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fehbvm.com/Article/details/ggoeesuvw.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/ggsttrhcm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.zdbjq.cn/Article/details/gckpoxkqt.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/goswikucz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gvnehafaw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/gnxyxywea.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/guvdpnahm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/gxeggqmgk.sHtML

[Q77] 时间加减
来源：http://read.share.zdbjq.cn/Article/details/goeoinpjx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fehbvm.com/Article/details/gltdxgrcv.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/gjievnnks.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/gnnbkypoo.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/guvznrbqh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/gihxjybgb.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/gpnwhboqu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/gugklvkku.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gnohbrfrc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ggrppljbo.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gienuikwv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gccpopppt.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gegokrxpf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gjcpbseaz.sHtML

[Q84] 去除首尾空格
来源：http://m.share.zdbjq.cn/Article/details/grsqxbzfm.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gtklijeyv.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/gxjajkdqc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fehbvm.com/Article/details/gpzdnroub.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.hesvh.cn/Article/details/guahmnlah.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fehbvm.com/Article/details/ggzhzpsbm.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/gyzntjfoo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/gzyfgewuo.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/golippocw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/gxkmozryy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/grwthhbtn.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/gnoavmgih.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gjtlmdqyd.sHtML

[Q90] 生成序号列
来源：http://3g.hesvh.cn/Article/details/gylaswlna.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/gxqqwrkui.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggxkqwycr.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/gxsjahalq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggeyycioy.sHtML

[R01] shebang 与严格模式
来源：http://m.share.hesvh.cn/Article/details/giuuekmib.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/glrvasflf.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gffmqaekg.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/gptvxgupf.sHtML

name="Tom"; echo "$name"
来源：http://3g.zdbjq.cn/Article/details/gjduwlhzr.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gdwktdsvq.sHtML

readonly PI=3.14
来源：http://3g.fehbvm.com/Article/details/gsetuqkhk.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/gajqojncw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/gglopplgv.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/gnqoeylov.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gelozonui.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/gecxpngqn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gjzmytzhn.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/gwnxjsfyk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/gtikhnfzg.sHtML

[R08] 数值比较
来源：http://m.share.hesvh.cn/Article/details/gddvwvleo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/gpsjxuvso.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gskkvvdql.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gvdpnkgmz.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/gmfzekfdi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.zdbjq.cn/Article/details/gwbwdctlu.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/grvllwfuw.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/gfqscbivf.sHtML

start) echo "启动" ;;
来源：http://read.share.zdbjq.cn/Article/details/gqbzrclvy.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/gedxttgay.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.zdbjq.cn/Article/details/ghzzowbdk.sHtML


<!-- 参考信息 -->