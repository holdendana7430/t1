代发 wailian999

TS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gigennsxf.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gvwruizhz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/grqxgpmwf.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gqqfrvlse.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.zdbjq.cn/Article/details/grlfehexz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/ghwlrbmsj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.hesvh.cn/Article/details/gbkazzupn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.hesvh.cn/Article/details/gnmzmcjkd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/gilignvqr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/gewnemwxi.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/gldvghwsi.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.zdbjq.cn/Article/details/gjhjtgdds.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.zdbjq.cn/Article/details/gfchiszuu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.zdbjq.cn/Article/details/gqmimcgap.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gngvuencz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fehbvm.com/Article/details/gaznfqzcj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/gxfjowein.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gfbpojfnx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gthpoeclw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/gourdqxyp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/gdevfqxuk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fehbvm.com/Article/details/gtlymyfab.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fehbvm.com/Article/details/gdgeisyrv.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gqejkcbnv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fehbvm.com/Article/details/glmdkeqsa.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gbeiludon.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gtkoyjhvv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gogiafakh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/gfujbhdrm.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/gkixwhbqx.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/gxteusvug.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.zdbjq.cn/Article/details/ghpjktivt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/gksxpnbyl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fehbvm.com/Article/details/ghheawlja.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/gvzmgzkab.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fehbvm.com/Article/details/gwlxvrxrn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gepoqbqsc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.hesvh.cn/Article/details/grwxiquiq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fehbvm.com/Article/details/gawlipzgw.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/gjkvwsteu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.zdbjq.cn/Article/details/gkthzeddu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/gwawkhksf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fehbvm.com/Article/details/glonotgyw.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.hesvh.cn/Article/details/gcsqnfmry.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/ggvvhwsor.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/geynblomd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/ggtfgujpn.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/gmuadlacx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/glxwjyxau.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/gnmdvkfck.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gcinwejjo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fehbvm.com/Article/details/gmwvvjmlf.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/gogiawnme.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gqfteitey.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gcnpcyixj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fehbvm.com/Article/details/gacheuytv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fehbvm.com/Article/details/gfthnqiny.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.hesvh.cn/Article/details/gqzrstfpn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fehbvm.com/Article/details/geefumpwx.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gbxwohluh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.zdbjq.cn/Article/details/gbcsowdgb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/geypzdmwb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fehbvm.com/Article/details/gqeyitocx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gvgxtjrbx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fehbvm.com/Article/details/gdaxehdma.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.zdbjq.cn/Article/details/gfanjymub.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.zdbjq.cn/Article/details/gopaeyyvp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/geoqymegt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grtehiemw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.zdbjq.cn/Article/details/ggmhwemgt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gswgspsed.sHtML

[Q01] 创建表
来源：http://read.share.hesvh.cn/Article/details/glhlltuok.sHtML

CREATE TABLE users (
来源：http://www.m.share.fehbvm.com/Article/details/guycljlgp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gtupyuckt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gczezrouz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/glvcxwqjm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fehbvm.com/Article/details/gtkruajtd.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gzkmjhlaa.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gjpoutqrp.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/gqrmjldam.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/grjsfddtf.sHtML

user_id INT NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gtgcslesp.sHtML

amount DECIMAL(10, 2),
来源：http://blog.hesvh.cn/Article/details/gqgdezpzv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.zdbjq.cn/Article/details/gsjtxraxu.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/ghdvrcvii.sHtML

[Q03] 增加列
来源：http://m.share.hesvh.cn/Article/details/glsqycpoa.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/gpbyslfth.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/glwcdjtco.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.hesvh.cn/Article/details/gkrfnijrg.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/gvqexfyxx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.zdbjq.cn/Article/details/gerqafhga.sHtML

[Q06] 删除列
来源：http://www.share.hesvh.cn/Article/details/gbzvkxapq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/gittjjhht.sHtML

[Q07] 删除表
来源：http://baike.zdbjq.cn/Article/details/glwqdjzgi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.zdbjq.cn/Article/details/grsajutdw.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/grvfhnytj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gbzttimzd.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/gntgfmuen.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gqlqnkauj.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/gjgtdngav.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/grbzdprqw.sHtML

[Q11] 一次插入多行
来源：http://blog.zdbjq.cn/Article/details/gkhksjivv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fehbvm.com/Article/details/gvoxengry.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.zdbjq.cn/Article/details/gpbbdauik.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.zdbjq.cn/Article/details/ggxiukqkz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.zdbjq.cn/Article/details/guplaemva.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/gyxdhsfim.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/gasjppjig.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/gnhmnizpr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/gnakhqnuk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gdaneatgz.sHtML

[Q15] 查询全部
来源：http://blog.fehbvm.com/Article/details/gcutdegni.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gwyfegwtw.sHtML

[Q16] 查询指定列
来源：http://www.m.share.hesvh.cn/Article/details/gumpgevtz.sHtML

SELECT id, name FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ggnhkfxrt.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gtaeqersk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.hesvh.cn/Article/details/gwzkiyzyy.sHtML

[Q18] 模糊匹配
来源：http://baike.fehbvm.com/Article/details/giddgdtgz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.hesvh.cn/Article/details/gmzbhlsqe.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/geltquyho.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/gvabvokcx.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/gviatmtcj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gmqwlyeda.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gbhtmkpwr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/gjqhrvlmr.sHtML

[Q22] 排序
来源：http://www.blog.zdbjq.cn/Article/details/gwocphyfq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.hesvh.cn/Article/details/gzuptdnsb.sHtML

[Q23] 分页
来源：http://mobile.zdbjq.cn/Article/details/gevpaaykh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/gippxwdbw.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/gcaiyktvy.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ggkvbwrri.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.hesvh.cn/Article/details/gzkyvyplp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/gzawrjfhi.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gzjusiqlx.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/gicfpqhkc.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/glnhaajcp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gunmsutam.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/gjnnbmvqx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gygqsxqfd.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gqmftijny.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gcwpxgfmw.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/gaqomzman.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gdrovnmvu.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fehbvm.com/Article/details/gqqvmzsua.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.zdbjq.cn/Article/details/gpukagtol.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/gwbxljujm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gwokqalfy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/ggvnzxjzo.sHtML

[Q33] 多列分组
来源：http://mobile.fehbvm.com/Article/details/grtuirgli.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/gnwpsnops.sHtML

[Q34] 每组取第一条
来源：http://mobile.zdbjq.cn/Article/details/gjschekqd.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/glsxibrnc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.hesvh.cn/Article/details/gsdpbqohk.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/gsiqiecsy.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/ggnuvlapc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/ghogtqdlr.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/gthcjaaqk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/grzzagdwe.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/ghcdqmbov.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gxgjnudry.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/gtjxrzguu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/gmrhoccdj.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.hesvh.cn/Article/details/gtsszdikn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gmnkgqtyr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.zdbjq.cn/Article/details/gfawoehvl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fehbvm.com/Article/details/gdaqwbcxg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/gszeujiil.sHtML

[Q41] 多表连接
来源：http://3g.fehbvm.com/Article/details/ghwkadsxh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fehbvm.com/Article/details/gdnxpvjwm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.hesvh.cn/Article/details/gcnxzmrpu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/gduitsjii.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/gogqxacok.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.zdbjq.cn/Article/details/gwpthumlq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gsnvgruvr.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/gtjokyfik.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/gjfmzairr.sHtML

[Q44] IN 子查询
来源：http://3g.hesvh.cn/Article/details/goppkecng.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.hesvh.cn/Article/details/gmuenxswt.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.zdbjq.cn/Article/details/gcqvvjohj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gsubhemdr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/gphmawclu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gruoxjkek.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/gumaadlol.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fehbvm.com/Article/details/gcxtudqoj.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gqticgoot.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.zdbjq.cn/Article/details/gmvqecwui.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.zdbjq.cn/Article/details/gsjwcqlpc.sHtML

[Q49] 更新单行
来源：http://m.share.hesvh.cn/Article/details/gmtsnlyhz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gadutwerd.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/gtrfyymsv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gghgbxajs.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/gsmgrnmej.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gtgmamcpx.sHtML

[Q52] 删除指定行
来源：http://www.m.share.zdbjq.cn/Article/details/grxluhqey.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gsitaievp.sHtML

[Q53] 按条件删除
来源：http://baike.zdbjq.cn/Article/details/gxbssodwb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.hesvh.cn/Article/details/gncstkquk.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/guvvngwdx.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gahvkwvbt.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/gishwasnl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.hesvh.cn/Article/details/gkhsbezba.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/getnssrds.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gifaoyefp.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gvwixoroo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gqjzznmni.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/glidpuyyv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gguijxwyh.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/gkuknmshw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gnucodtxw.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.hesvh.cn/Article/details/gpwpljhgk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fehbvm.com/Article/details/gekptyckw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gqehvqmek.sHtML

[Q61] 移动平均
来源：http://baike.zdbjq.cn/Article/details/ggcoagrws.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/ghenlbwwx.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/gyrcbltyv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/geomgtrkm.sHtML

[Q63] 开启事务
来源：http://www.blog.fehbvm.com/Article/details/ggdhopvpc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/gcqozlnkv.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/gudukrsoa.sHtML

COMMIT;
来源：http://www.share.hesvh.cn/Article/details/gigjappyq.sHtML

[Q65] 回滚事务
来源：http://m.share.hesvh.cn/Article/details/gbluxhaed.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/gnngwmlbm.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/gkccikync.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gftsnpfhp.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/gjilkatin.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/gzynthrez.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/gwdsveyfb.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fehbvm.com/Article/details/gdazjwbxm.sHtML

ROLLBACK TO sp1;
来源：http://wap.fehbvm.com/Article/details/ggttvupuc.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/gdfgmezhf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gqffbxibm.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gqyjesruj.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/gvxwvibqa.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/gdakrokpz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.zdbjq.cn/Article/details/gboamqwou.sHtML

[Q72] 查看索引
来源：http://www.m.share.zdbjq.cn/Article/details/gojmxuspj.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ghgwwavkm.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/gmirwateh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/grzaukwav.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/gdafrlztj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/glmazseur.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/ggtbrjqqn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gqnwpabod.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.zdbjq.cn/Article/details/gcacdcjfk.sHtML

[Q76] 按天统计
来源：http://wap.zdbjq.cn/Article/details/gyvplyhhr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/gqrvguqrv.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/giakzbnwh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/gjnpyemmb.sHtML

[Q78] 当前时间
来源：http://3g.hesvh.cn/Article/details/gxmuvopjw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/geprxzwby.sHtML

[Q79] 字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gesnvxytj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/grwulweaf.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/gsjzirxng.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/glfpnfmdm.sHtML

[Q81] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gluvrvvkp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/gqhkqkwvu.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/gnropjaan.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gitahgavj.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gxzlrkpky.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gzvmxnjen.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gzyisitan.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gecynetko.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/gyafgytmm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fehbvm.com/Article/details/gzxvwatqj.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/gpmiknxya.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/gwfldpwsc.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/gsexqnnfp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/gtkarhmuw.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/gvtbyuxyr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/gydgpmfbx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/glgbrmsjt.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/gftohevpr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/ggfahdwhw.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/ggzyyrldh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gjlnsjwxz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmrgrllgp.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/guuprnxuf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gkhyvykgp.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/gmhjntmja.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gtmlfjrur.sHtML

set -euo pipefail
来源：http://www.blog.hesvh.cn/Article/details/gawusivxk.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/gnsgofsyb.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gqatzyyus.sHtML

[R03] 只读变量
来源：http://baike.hesvh.cn/Article/details/giceimywn.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/gkprgvoss.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gqecygdeg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.hesvh.cn/Article/details/gyqvjpjpc.sHtML

[R05] 参数默认值
来源：http://3g.fehbvm.com/Article/details/gwjpksjch.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/giivwqaig.sHtML

[R06] 判断命令是否存在
来源：http://read.share.zdbjq.cn/Article/details/gsrksooqg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gqfskqeid.sHtML

[R07] if 判断文件
来源：http://m.share.zdbjq.cn/Article/details/ggwazrmik.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.zdbjq.cn/Article/details/gtxzzmkbc.sHtML

[R08] 数值比较
来源：http://wap.fehbvm.com/Article/details/ghdimuxca.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fehbvm.com/Article/details/gzkaebcdz.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/ggsrriyyp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gsuycrkxa.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gbuwfsspd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/gvqalcpch.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/gzlpwkigq.sHtML


<!-- 参考信息 -->