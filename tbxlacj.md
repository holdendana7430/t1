代发 wailian999

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/gpqbqfphr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grwtbrfcz.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/gpxpnjark.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxcybmxrx.sHtML

[P01] 生成 UUID
来源：http://blog.zdbjq.cn/Article/details/giwajbwtp.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fehbvm.com/Article/details/gouoipxky.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/gpqolnlqi.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gtvgmtxid.sHtML

TS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gubozpabf.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/gzjzlwykl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.hesvh.cn/Article/details/gvexrcwit.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gtjrlryle.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/gijrmkhlc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gnstcaxaw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/gexsdefrj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/gwhjvlfbj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.hesvh.cn/Article/details/gjypcvoea.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/gcbbkffmm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gkzaxiyim.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.zdbjq.cn/Article/details/gxrqcwtob.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fehbvm.com/Article/details/glsplkdsb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.hesvh.cn/Article/details/gtyaupauo.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/grxwtbefg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fehbvm.com/Article/details/gzgglsskk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.zdbjq.cn/Article/details/ghhsjklvz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gcwqjxovn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/grkeicxnw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gidovddrr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/gxrodlmbg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gaiibpwhp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/gumcijhst.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/gpnsfilzg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gykioeyve.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gaqodwryj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gmckafose.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gotaehixy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gjlmfxvfq.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gsbwpxvsp.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/gbcwnxqwc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/gsgbnjtha.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/gjwkziycd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.zdbjq.cn/Article/details/gyjpimmrm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gvgrnfqxk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/gstvwhxcn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gzxdmhiey.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gxpuwxfew.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fehbvm.com/Article/details/glqdfrbnx.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/gjebxrjit.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fehbvm.com/Article/details/gsemxtztt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gnoyjoadj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/gubeqigte.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/gowgbkqvt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/gpfwjfyrw.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/gxoasyjij.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gfsnaqziq.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/gglefimhk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/gyaarioge.sHtML

C#:   if (x is null) {}
来源：http://baike.hesvh.cn/Article/details/gyxehitgr.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/gjbdzvsmb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/gydwehobv.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/gjazjaplo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gdkzmhfla.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gcxsqfjrk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/glyeazuff.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/gqaiwaqen.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.zdbjq.cn/Article/details/genkruepk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/gjausgmnx.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fehbvm.com/Article/details/gwoidkogw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.zdbjq.cn/Article/details/gomzgmayu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fehbvm.com/Article/details/greqgqcnj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/gtnvlelzm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gulqyayel.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.hesvh.cn/Article/details/gidqkpqrv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gwifupdcx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fehbvm.com/Article/details/gjlgowyjc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/goiqiytci.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvpyhtrwn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.hesvh.cn/Article/details/genrlhkeo.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsatwhcjl.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gjtlpocle.sHtML

CREATE TABLE users (
来源：http://read.share.hesvh.cn/Article/details/gpzcxfkde.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gywzibnqn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gppwoamun.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.zdbjq.cn/Article/details/gbjzmfxim.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.hesvh.cn/Article/details/gxabrmfgy.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gijznoibv.sHtML

[Q02] 创建带外键的表
来源：http://baike.zdbjq.cn/Article/details/gthxkwqke.sHtML

CREATE TABLE orders (
来源：http://baike.zdbjq.cn/Article/details/grvqdfedh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gkiaznzww.sHtML

user_id INT NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gpyljunol.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/gkemwqmsu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fehbvm.com/Article/details/gxuqnhzgn.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gdyyemlfz.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gttqhbuep.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/gylmyydln.sHtML

[Q04] 修改列类型
来源：http://www.blog.fehbvm.com/Article/details/gvbadxmxm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.hesvh.cn/Article/details/gokozsiez.sHtML

[Q05] 重命名列
来源：http://read.share.fehbvm.com/Article/details/gaawhxiqw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/gkubxbzuj.sHtML

[Q06] 删除列
来源：http://blog.zdbjq.cn/Article/details/gplmwhirj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/gjgbpglar.sHtML

[Q07] 删除表
来源：http://www.share.zdbjq.cn/Article/details/gameerrnm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.hesvh.cn/Article/details/gaysarsxl.sHtML

[Q08] 创建普通索引
来源：http://blog.hesvh.cn/Article/details/guqfbmexk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gltdfwwxt.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/gmrviomxl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gplidtkuf.sHtML

[Q10] 插入单行
来源：http://wap.zdbjq.cn/Article/details/gukqauzcb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/gjwbxbpqf.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/giiaepedj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fehbvm.com/Article/details/gdhdhqcnj.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/grotxjfxa.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fehbvm.com/Article/details/gqdcxvqfl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.zdbjq.cn/Article/details/gzeanlbpl.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/ggoonblqd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/guautwklc.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/gjrmgjawb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/gojkfpnyi.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.hesvh.cn/Article/details/garywfthu.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/gvsvviwrj.sHtML

SELECT * FROM users;
来源：http://3g.hesvh.cn/Article/details/gfzdwkdxh.sHtML

[Q16] 查询指定列
来源：http://blog.fehbvm.com/Article/details/glnrcaixt.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gigzythmb.sHtML

[Q17] 条件查询
来源：http://m.share.fehbvm.com/Article/details/govfhmfoi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fehbvm.com/Article/details/gnmnfxjlr.sHtML

[Q18] 模糊匹配
来源：http://mobile.fehbvm.com/Article/details/gqsaducyv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/gcsmbfokm.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/goewiowyv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/gcbdvhhbs.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/grhzjewea.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/gvnvktayg.sHtML

[Q21] 空值判断
来源：http://baike.fehbvm.com/Article/details/gvjfmomxg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gxqzedccb.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/gsymdsbtw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.hesvh.cn/Article/details/gsvmdjmdn.sHtML

[Q23] 分页
来源：http://blog.hesvh.cn/Article/details/gzytecwzx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gzpxhudtu.sHtML

[Q24] 去重
来源：http://baike.hesvh.cn/Article/details/gojwxuprh.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/gvniifzww.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/gdpyznnin.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.zdbjq.cn/Article/details/glicgnmiq.sHtML

[Q26] 计数
来源：http://mobile.zdbjq.cn/Article/details/gumovtxws.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gslppmvba.sHtML

[Q27] 条件计数
来源：http://read.share.zdbjq.cn/Article/details/gyjgkoerf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.hesvh.cn/Article/details/gpketzssy.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/grpjbogya.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/guiwmieen.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/ghevaxcdw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/grrjdumra.sHtML

[Q30] 分组统计
来源：http://baike.fehbvm.com/Article/details/gcozjyqaj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gxwbhcdjy.sHtML

[Q31] 分组后过滤
来源：http://mobile.fehbvm.com/Article/details/gzngbkcfl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/gvlqasgzn.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fehbvm.com/Article/details/ggqqkkllx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gmrzouksc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/gvdbyefly.sHtML

[Q33] 多列分组
来源：http://baike.zdbjq.cn/Article/details/gjgdjosvj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.hesvh.cn/Article/details/gkfaaklld.sHtML

[Q34] 每组取第一条
来源：http://mobile.zdbjq.cn/Article/details/glogdfmqm.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/gsmubzwev.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/gkacxfdbo.sHtML

) t WHERE rn = 1;
来源：http://blog.hesvh.cn/Article/details/giydsyjdi.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gvtxupdts.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/grixcrtxr.sHtML

[Q36] 左连接
来源：http://blog.fehbvm.com/Article/details/gpauxtxbf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gohaoypkn.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gxofdwwbp.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/gvnzbfdlz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/gfsjggltc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gtjhxxgkt.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.zdbjq.cn/Article/details/gqzckconk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.zdbjq.cn/Article/details/gxevtrzfk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/gciejirjk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/grdqxoouh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.zdbjq.cn/Article/details/ggadiobry.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/glwtayuhc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/gcsbjfreo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.hesvh.cn/Article/details/glaysjjce.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/glxdvbbmj.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.zdbjq.cn/Article/details/gckotesko.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gcoxvgxse.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fehbvm.com/Article/details/gvykdmeek.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gusblsszy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fehbvm.com/Article/details/gblkegqtj.sHtML

[Q44] IN 子查询
来源：http://www.share.zdbjq.cn/Article/details/gbuwebkvz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.zdbjq.cn/Article/details/glqznhcly.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.zdbjq.cn/Article/details/geejztwey.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gdmudsats.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.hesvh.cn/Article/details/gzjljmbaa.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gztfrpytw.sHtML

[Q47] 与平均值比较
来源：http://mobile.fehbvm.com/Article/details/gqaloixkj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.hesvh.cn/Article/details/gipgjiomg.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fehbvm.com/Article/details/grrolchbx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/gqklbxjvk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/gbzbdjedo.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/gtctcgkud.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gznseiaid.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/grtaibxhe.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.hesvh.cn/Article/details/gdmyuqjyw.sHtML

[Q51] 用子查询更新
来源：http://wap.zdbjq.cn/Article/details/gteqsyefd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/gsvwqgeov.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/gqywpeqns.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/ggrvakmhz.sHtML

[Q53] 按条件删除
来源：http://3g.hesvh.cn/Article/details/gzdiedamb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gcwdrguoe.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/gfebhcowz.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/gdjdwepop.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fehbvm.com/Article/details/gsnwufnbs.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/ghtccwpov.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.zdbjq.cn/Article/details/gouyiinzv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gnglcpngy.sHtML

[Q57] 行号
来源：http://wap.hesvh.cn/Article/details/ghfrdbeyb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.zdbjq.cn/Article/details/gmoqijepy.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/gboagpkvl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gfgugbezq.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/gnculxqvo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/ghsdmajcu.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/gtpmthtlg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.hesvh.cn/Article/details/gadckxqlo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gzhavnjug.sHtML

[Q61] 移动平均
来源：http://www.blog.zdbjq.cn/Article/details/gjobhceuu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/geudvqmot.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/gssuotzel.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gdocqlpth.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/gavbhxkab.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.zdbjq.cn/Article/details/gixglzhoj.sHtML

[Q64] 提交事务
来源：http://www.share.zdbjq.cn/Article/details/gxupdvwgh.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/gudmrjouf.sHtML

[Q65] 回滚事务
来源：http://baike.hesvh.cn/Article/details/goptltdyw.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/gwveesdcr.sHtML

[Q66] 行锁查询
来源：http://baike.fehbvm.com/Article/details/glnqycbuk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.hesvh.cn/Article/details/gangsqkqb.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/gtggzuizn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/ggvpqheuv.sHtML

[Q68] 保存点
来源：http://wap.hesvh.cn/Article/details/gvcqicjcf.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gzzfyhsmr.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/ghiauxwzm.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gsqppjaja.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/giclhrctw.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/ggjrseqhl.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/gxamqmyxx.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/gbafjjvla.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fehbvm.com/Article/details/gxajylqzx.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/goujvpwfq.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gkatohbjh.sHtML

[Q73] 查看表状态
来源：http://baike.fehbvm.com/Article/details/gvspekuww.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gdhzgnlyl.sHtML

[Q74] 强制使用索引
来源：http://wap.fehbvm.com/Article/details/gqckgqkox.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/gvglpgrxh.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gfjcyxedi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gmlvvombp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/gxkxmvmsm.sHtML

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/gvoyjqywi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.zdbjq.cn/Article/details/gpyvdlime.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/goyeukjmi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/gofdpcwun.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/gtemmusyz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fehbvm.com/Article/details/gcxciyvfe.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gzlzdbyhu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/gcrtsgpyx.sHtML

[Q80] 字符串截取
来源：http://blog.hesvh.cn/Article/details/gfwilqesx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gwplksghy.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gbcrnfyfi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/gymwmdgcz.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.hesvh.cn/Article/details/gzilhrhkk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gicgarmei.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gijpjzxqa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gqpbmcqkz.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gvufgldoq.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gjzijcfgz.sHtML

[Q85] 数值取整
来源：http://www.share.zdbjq.cn/Article/details/gfpohagmg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/gurwlchmk.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gthfbtlyk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/ggjfdedpf.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/goncztpos.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gwtvyltfe.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/glvmjgtjs.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/gmoqqndtm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gnrijupeu.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/ghhllbsmj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/gkcmhgeyw.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gywtsekwk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gygewxzga.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdxonozss.sHtML

R. Bash 专题
来源：http://baike.hesvh.cn/Article/details/gswwsyvoj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxsawcswj.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/gxbwyrfrh.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/gctindijv.sHtML

set -euo pipefail
来源：http://3g.fehbvm.com/Article/details/ghtffbgxr.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/ghbmfdzxd.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/gpuewysvq.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/govtzwnbg.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/gxzqywebv.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/gzmgqcczd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/gdnclmlas.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/gykmvgshs.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/grtyqvyyn.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/giulngxjc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/genkkldch.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/gzmthgkff.sHtML


<!-- 参考信息 -->