代发 wailian999

TS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gnwjlassj.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/ghfixmhre.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/gljacwfcr.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fehbvm.com/Article/details/gdtofvkbn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fehbvm.com/Article/details/gdplzbjhz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/gvidauovc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/glxqkpzxq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/gyyrplnud.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/gzgvyukhe.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/gceeafzup.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/ghzaomjcj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fehbvm.com/Article/details/grzrflddl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.zdbjq.cn/Article/details/gerxgthke.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/gbxmjlovd.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/gkgnsckdz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/gejvxulsv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gvuvatqzq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gesuwtfhp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/glrqxnocu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fehbvm.com/Article/details/gmhqgqqlp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gncyktkox.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.hesvh.cn/Article/details/gpwfdxgtw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/gjeqxuizc.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/gceywcwvj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.zdbjq.cn/Article/details/gncubvqln.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gezqfcjtv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gygwzpvtp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gaphdiinx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gjguwdnjm.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fehbvm.com/Article/details/gedbnsmpe.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/gwkvygtzf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/gswrosnpt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/gypknbyxk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gwbqhggor.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/galezjsot.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fehbvm.com/Article/details/gckyjjsnk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gjkpouiiw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/gzfwxjrya.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gswugwcyx.sHtML

Ruby: a == b
来源：http://www.share.hesvh.cn/Article/details/gvgkdyktz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/gcczwovcn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/grsgcdads.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/gryulzgig.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/gbmssmfbd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/gwvlrzzfl.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/gyvqzrzil.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gqmyfbgoi.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/gkvssguhn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fehbvm.com/Article/details/gftrosrzm.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/gluruvtnp.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/gptmlpnvo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/gpwhlvxae.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/ggnkzujmw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/ghjtucfwx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gwojooxgb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.hesvh.cn/Article/details/gpjbckyux.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/gugkrwoeq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fehbvm.com/Article/details/gxecwrawc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/gffokigvz.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/gjkxxvmrp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fehbvm.com/Article/details/glcilpvqe.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/gcayedyxg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gyngwlkcx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gyvmlhiyr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/gfyopetcs.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.hesvh.cn/Article/details/grledrajc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fehbvm.com/Article/details/gwtkhbxhb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.hesvh.cn/Article/details/grjbxvmsw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ggnpwalcw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/ghozbudby.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzghndwgy.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/gpmrfzkrz.sHtML

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/ghnwfaiyp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/guejytijr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gramnpjyk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/gstzsqdpp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/gosfaeqlo.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gzhhuwndj.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/gqphbvfbb.sHtML

CREATE TABLE orders (
来源：http://www.share.fehbvm.com/Article/details/ghcucwtav.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gslmnhttq.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gnrqzduls.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fehbvm.com/Article/details/gfbqkdezc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/gvkbutffr.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gjjebznhj.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/gdqjbqgvr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fehbvm.com/Article/details/gnemotxvx.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/gfdpyncuk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.hesvh.cn/Article/details/gmgukvumr.sHtML

[Q05] 重命名列
来源：http://wap.hesvh.cn/Article/details/ggqpcalsh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/ggdvkqzfl.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/gqwbxkahf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fehbvm.com/Article/details/gsryzewkv.sHtML

[Q07] 删除表
来源：http://blog.hesvh.cn/Article/details/grqaniciz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.hesvh.cn/Article/details/gkscszbsl.sHtML

[Q08] 创建普通索引
来源：http://www.share.fehbvm.com/Article/details/gaswmjzas.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gyudpgons.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.zdbjq.cn/Article/details/gudcbhlzd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gzzemowpv.sHtML

[Q10] 插入单行
来源：http://baike.hesvh.cn/Article/details/giyytkbar.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/guiwwtoeg.sHtML

[Q11] 一次插入多行
来源：http://mobile.hesvh.cn/Article/details/gxilgtgpa.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.hesvh.cn/Article/details/ggsniudqj.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.zdbjq.cn/Article/details/ggnwqerzh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/ggskkgooq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/givtujgvu.sHtML

[Q13] 忽略重复插入
来源：http://wap.zdbjq.cn/Article/details/grpucehgz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gptrrzpjd.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/gjiuuxozv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fehbvm.com/Article/details/glddimrbc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fehbvm.com/Article/details/grtkirzrw.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gebmncvov.sHtML

SELECT * FROM users;
来源：http://wap.hesvh.cn/Article/details/gkpuiyowi.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/gjnjlialk.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/gigkjytob.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/gacdvwovo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fehbvm.com/Article/details/gjlimkxwx.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/gaszqhskh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/gqtyiumvs.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/gcelnyvgy.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/gmsxjlzrj.sHtML

[Q20] IN 列表
来源：http://m.share.fehbvm.com/Article/details/gvudycujc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/glgbopqwy.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gywnipvjn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gzazjjojm.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/gnyjantlt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/gworiqxfe.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/gleiubosd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/ghppkhfye.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/gwdzxmrhz.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/gjfifoctr.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.hesvh.cn/Article/details/gnejeogdx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.hesvh.cn/Article/details/gjzvdkqso.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/geddtjyfw.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gjbxcyslz.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/gqmrkxqxj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/gvmjfbcdd.sHtML

[Q28] 求和与平均
来源：http://blog.fehbvm.com/Article/details/guhbiwcnb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/geemyfppy.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/geebsnguk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gyjexhnpr.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/gnjkrjwgb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/ghahnejnz.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/gforfvepk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.hesvh.cn/Article/details/gkospxhlt.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gcwdscwbk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gagrtkwlx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.hesvh.cn/Article/details/gxmuvlymo.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/ggrtqqoar.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/glkyqnpwd.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/gahjajmzy.sHtML

SELECT * FROM (
来源：http://m.share.fehbvm.com/Article/details/gjdqbzpfz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fehbvm.com/Article/details/gnpqvbrlf.sHtML

) t WHERE rn = 1;
来源：http://baike.zdbjq.cn/Article/details/gnkqjieyv.sHtML

[Q35] 内连接
来源：http://www.m.share.hesvh.cn/Article/details/gfncrbgfh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gpsyyhxaj.sHtML

[Q36] 左连接
来源：http://blog.zdbjq.cn/Article/details/gvwrthgnk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gksyolfyk.sHtML

[Q37] 右连接
来源：http://www.m.share.fehbvm.com/Article/details/geshelzcb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/ggcjfimln.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/gizmwndmx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gezuecmae.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fehbvm.com/Article/details/gqcokwxxs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.zdbjq.cn/Article/details/glzzyhnpt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/gcbhubyrt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.hesvh.cn/Article/details/gwzjovuwl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gurhnnfby.sHtML

[Q41] 多表连接
来源：http://wap.hesvh.cn/Article/details/gwgbhckru.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/giqavcxdm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/gfgxgozqd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/gpdpljcyx.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.zdbjq.cn/Article/details/gyczvruva.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gxpcocnna.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/gvzmphxhd.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/gugftwqfx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/guhngcwny.sHtML

[Q44] IN 子查询
来源：http://www.blog.zdbjq.cn/Article/details/gktthkihg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.zdbjq.cn/Article/details/gjsgciyrg.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/gfojxqkzy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gwjeujzux.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gvqwgttlx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gnzfvldcb.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/gtavmjzjl.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.hesvh.cn/Article/details/gpysgojmd.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.zdbjq.cn/Article/details/gfvclcjmv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/gvhyoluyw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.hesvh.cn/Article/details/gxspxquwr.sHtML

[Q49] 更新单行
来源：http://baike.zdbjq.cn/Article/details/gkalyanvs.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/guyqscyow.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/gksnimbmc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/genbupzvs.sHtML

[Q51] 用子查询更新
来源：http://3g.hesvh.cn/Article/details/gqzplifvs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gfzlnbrfz.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/gboinlryt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/glyritoyj.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/gvcdrutnq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fehbvm.com/Article/details/gmjbzfcym.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/gnrwdpdap.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/gwqgotdas.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gfzzgedww.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gawtlidkb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.hesvh.cn/Article/details/gbspoukyp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fehbvm.com/Article/details/gtwtkvgth.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/gsynkitrw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.zdbjq.cn/Article/details/gvtqpzfrg.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/gkkcgiagx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/ghlozracg.sHtML

[Q59] 分组内累计
来源：http://baike.zdbjq.cn/Article/details/gtypveznp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fehbvm.com/Article/details/giuzrmhxw.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/gxljqczyw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/gqmpdfujx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gjnwjstak.sHtML

[Q61] 移动平均
来源：http://mobile.zdbjq.cn/Article/details/gaijkcdzw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gjdfpbwwu.sHtML

[Q62] 分组占比
来源：http://blog.zdbjq.cn/Article/details/gpstlcpzx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gwfiyfczy.sHtML

[Q63] 开启事务
来源：http://www.share.fehbvm.com/Article/details/gxoznhvvc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/gzubometu.sHtML

[Q64] 提交事务
来源：http://www.blog.hesvh.cn/Article/details/gfhugjnsp.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gbadmtvgx.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gvestaflf.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gaphceoyz.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/gawwpabiu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/gcwbebvxl.sHtML

[Q67] 设置隔离级别
来源：http://3g.hesvh.cn/Article/details/ggdnuoecr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.zdbjq.cn/Article/details/gkrchxria.sHtML

[Q68] 保存点
来源：http://blog.fehbvm.com/Article/details/gttipivdp.sHtML

SAVEPOINT sp1;
来源：http://read.share.zdbjq.cn/Article/details/gijvigqrv.sHtML

ROLLBACK TO sp1;
来源：http://read.share.hesvh.cn/Article/details/gvsrgovwq.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/gkpshulln.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/gvmyevmju.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/gkkiwbrza.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/gopcphinl.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/geyfdhxud.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/gliwinkzh.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/gtoelilrk.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/gyqchtzmz.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gqnuzboll.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gpmpaeyct.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fehbvm.com/Article/details/gfsxiskhg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/gelavykqa.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/griuzzyqo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/ghdwelgaq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fehbvm.com/Article/details/glpajntek.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/ginzvkcvw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fehbvm.com/Article/details/goyzyrwoz.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/gadpfbaom.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.zdbjq.cn/Article/details/gyuvqjdgw.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/gcegrpdbm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.zdbjq.cn/Article/details/gmakpvodw.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gqecuvoij.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/glzhfewxb.sHtML

[Q80] 字符串截取
来源：http://baike.zdbjq.cn/Article/details/gxgmmavqc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gluceokmb.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gaahrvgzr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/gslitfrmv.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/gnayimraa.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gchkxjpfd.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/ggvvvqboj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gejgmnukm.sHtML

[Q84] 去除首尾空格
来源：http://baike.zdbjq.cn/Article/details/gnynakuxc.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gjedccegj.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/grtwxuafw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.zdbjq.cn/Article/details/gjwdgrhqa.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/gpnuxbeuu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/gctonvora.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/gswgdzudo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/gnmbxbqtc.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.zdbjq.cn/Article/details/gjclykqdo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gphahfotu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/gfsrnffkx.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/gtlmjsfny.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/gjpdayuuz.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/gulmctorf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/grcpvgenz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gideymvyq.sHtML

R. Bash 专题
来源：http://baike.hesvh.cn/Article/details/genkwmmur.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpbflqkcm.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/gzfssltzr.sHtML

#!/usr/bin/env bash
来源：http://baike.hesvh.cn/Article/details/gzjohtbvw.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/gangbdpki.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gtmoiuvdd.sHtML

name="Tom"; echo "$name"
来源：http://m.share.zdbjq.cn/Article/details/gmehbcvbq.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/gbpfxkmxv.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/gtqrsxzbv.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/gzdfvfggy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/gmdboetag.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gkondajwh.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gcnklofqw.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/gvgvkmvoj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gozeruujt.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/gjhpusqfn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/gnpfgozrk.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/gyivycuuj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/gqmnsqkyf.sHtML

[R09] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gcnhkayox.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/gyzlxtuzo.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/grnqedoyg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/ghwrsllrs.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/ggzoauzro.sHtML


<!-- 参考信息 -->