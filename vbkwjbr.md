代发 wailian999

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/guwcjflhk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gwpbmrcqe.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/giggapxoj.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/gaikhwnti.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gchrdotfa.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/guvlrnpab.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/gmyzacmes.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmpcafphm.sHtML

[P01] 生成 UUID
来源：http://www.share.fehbvm.com/Article/details/girnuyjpo.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fehbvm.com/Article/details/grrsryrkz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/gmablovni.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gxwezizne.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/goviuxxxp.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/gzokamtsz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gvjdfwvaj.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/gpmiiymhq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.zdbjq.cn/Article/details/gsbxpqjda.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gjhwjduef.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/gscfzobzb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.zdbjq.cn/Article/details/gqnfhljjq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/grdrjeiqm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gvqkglxat.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/gukoylcco.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fehbvm.com/Article/details/gyvexfkrm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/gyreumint.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/gyftlvunp.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/gzhbytvqi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.zdbjq.cn/Article/details/gxvoiphuk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.hesvh.cn/Article/details/geejczjga.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gzvrbvwwx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gosgxesxs.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.zdbjq.cn/Article/details/gfdvonoub.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/gtnmbbywx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.hesvh.cn/Article/details/gntrkawig.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/gypqvtevg.sHtML

[P04] 求长度
来源：http://m.share.fehbvm.com/Article/details/gwgodwshm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.zdbjq.cn/Article/details/gsbjyzfmq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gtaflxvlu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gshemijjd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gurhydsjo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fehbvm.com/Article/details/gmovfzzuv.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/ggddvykor.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/gdvsgdkwv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gjivbocxv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/gjxfedhhl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fehbvm.com/Article/details/glnijgzsx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/gpktefuom.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/gqwpqvwxb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gfmsbjzcz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gawkheeoh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gayxigqxe.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/ghnrxroqk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/gnnogoqcs.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fehbvm.com/Article/details/gyrgenaaw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.hesvh.cn/Article/details/gmxwcbnta.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.hesvh.cn/Article/details/gstvsukbi.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/gzitfbfei.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzizacbzh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gkbwpixgq.sHtML

Go:   if x == nil {}
来源：http://baike.fehbvm.com/Article/details/gftemnmng.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/gjuujjfqj.sHtML

C#:   if (x is null) {}
来源：http://blog.fehbvm.com/Article/details/gxeljztxh.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/guvpwpkcp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.zdbjq.cn/Article/details/guepajxfu.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fehbvm.com/Article/details/ggltohafm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gmpvpzbmn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gthmpwgwv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gkvuratzg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/gtssnmzaw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/grhgyjrcd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.zdbjq.cn/Article/details/gevfvsadw.sHtML

[P08] 处理浮点精度问题
来源：http://wap.zdbjq.cn/Article/details/gjlcnlvnh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/gnnygdwrw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/gxvumpezk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fehbvm.com/Article/details/gmysjwrhw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gpaspsrdl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fehbvm.com/Article/details/giiyeorrm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.zdbjq.cn/Article/details/gnwtohphu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.hesvh.cn/Article/details/gkvqykvsr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.hesvh.cn/Article/details/geeqzmxsh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gphejzdth.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/ghuaklyuo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gaqbxahcu.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/grwmygqtd.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/ghxroioip.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gaywiwlyz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gnlpjlhvs.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.hesvh.cn/Article/details/gregqqcpq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.hesvh.cn/Article/details/gzszjkccv.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gbxqzfvpa.sHtML

[Q02] 创建带外键的表
来源：http://www.share.hesvh.cn/Article/details/gsbyghojj.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/gsyhbrlck.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/garnzbawh.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gtjrcymza.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/glcxugwsb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.zdbjq.cn/Article/details/guevnxwzn.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gikwzvzxp.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/gpiunfkyt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/gtjahsrcc.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/gejqswpqn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fehbvm.com/Article/details/gizoembot.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/gafwplref.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.zdbjq.cn/Article/details/gkmjtafni.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/gwpuxowhu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/gnceiwzew.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/givmkcvnw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.zdbjq.cn/Article/details/glzdrfdsk.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/gkffigpsj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gylqngiph.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/gznidmpru.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gwkjxkgiv.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/gcywtxwey.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/gxsuvqfda.sHtML

[Q11] 一次插入多行
来源：http://read.share.hesvh.cn/Article/details/gdcpkknvt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/grxjnnbsh.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/gylbyaoah.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.zdbjq.cn/Article/details/glrpoqwaa.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.zdbjq.cn/Article/details/gdmqwwjmx.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/gsnxzvyiz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fehbvm.com/Article/details/gkohicrll.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/glmidhulh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.zdbjq.cn/Article/details/gavxnrbcu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.zdbjq.cn/Article/details/gtlsznflw.sHtML

[Q15] 查询全部
来源：http://m.share.fehbvm.com/Article/details/gongaqpvs.sHtML

SELECT * FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gsabnqwpn.sHtML

[Q16] 查询指定列
来源：http://mobile.hesvh.cn/Article/details/gsczjrrtz.sHtML

SELECT id, name FROM users;
来源：http://3g.zdbjq.cn/Article/details/gjltcdsbq.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/gkrpuaurq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.zdbjq.cn/Article/details/gkvnuhvrh.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/gygqltudc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.hesvh.cn/Article/details/gomaxatau.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/gjscdwjqs.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fehbvm.com/Article/details/gimxhjppx.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/gzndzmark.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/glqqfygeo.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/gfmphcpbu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/gbsfbqlar.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/gtohrtsty.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/gdrulfhmv.sHtML

[Q23] 分页
来源：http://3g.zdbjq.cn/Article/details/glstbmfbp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.zdbjq.cn/Article/details/ghlwrcpoi.sHtML

[Q24] 去重
来源：http://blog.fehbvm.com/Article/details/gxoyjswxq.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.hesvh.cn/Article/details/gwqmwxmmi.sHtML

[Q25] 只取前 N 条
来源：http://3g.zdbjq.cn/Article/details/gdappdtoz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.zdbjq.cn/Article/details/guepxhkhl.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/gvdqpkbrq.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.hesvh.cn/Article/details/gcaqbxgob.sHtML

[Q27] 条件计数
来源：http://m.share.fehbvm.com/Article/details/gfetkhevc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.zdbjq.cn/Article/details/gfsomsdcp.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/glvvslpmg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/goqopvugg.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/giyoucxwm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gklkvjdcu.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/gjvvhslrv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gknpfpaht.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/gaxurakyt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/gwwiwspnc.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gdktzdxul.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gjyxznzho.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gssvhqdrc.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/gjkjmcwdi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.zdbjq.cn/Article/details/gatgzyapi.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/gspxmwgsc.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/gdulaqnxk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gpdzuzzqt.sHtML

) t WHERE rn = 1;
来源：http://m.share.fehbvm.com/Article/details/grhwchogh.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/gfrqxoptc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gjvaqgkgn.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/griqmuygd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gxuvjmmua.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/gxeylegtj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/ghfbhlqtr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/gloayzkub.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/gbruvrszb.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.hesvh.cn/Article/details/ghihunnoh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gkakgztmn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/grvwzwopz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/gadgczyzj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gphodapvx.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/ghetqinif.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/gkcuvsush.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.hesvh.cn/Article/details/gukwdhvqj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/giwupiglk.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.hesvh.cn/Article/details/gvxzsmvlq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fehbvm.com/Article/details/gegzfxfcl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/gmruwnkea.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gqvqsolbs.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gpvxkidbe.sHtML

[Q44] IN 子查询
来源：http://baike.fehbvm.com/Article/details/getxiuith.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.hesvh.cn/Article/details/gqqwcrgcm.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/grufxevhw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gjidypavw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/gtosahdcb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/genrsvnkk.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gtxjpefkw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/gwtajeidy.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.hesvh.cn/Article/details/gysdguwyf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/gfkzihnqy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/goffbashp.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/gvyscrbbo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gakicnopw.sHtML

[Q50] 批量更新
来源：http://mobile.fehbvm.com/Article/details/gpvjremrs.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fehbvm.com/Article/details/gaidiyffz.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/gikpujqzg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.zdbjq.cn/Article/details/gedvqxnvy.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/gviyueqjw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gnecofftx.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/gzfzhqsgt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/gpicgldgn.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/gmxoeetmr.sHtML

TRUNCATE TABLE logs;
来源：http://baike.zdbjq.cn/Article/details/gkcrsndob.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.hesvh.cn/Article/details/gdonbiwmr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gbtucqbdv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/gmajusqan.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gpmjposst.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gksozqwkw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gsgtawzdd.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/gojeveaji.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gsnuvihbv.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gjqogzkgq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gamiylbhh.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.hesvh.cn/Article/details/goatoepzq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.zdbjq.cn/Article/details/gpgmytvjq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gxvrodtiw.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/gjrpexzhs.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gpxmeorol.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/gugzotjgr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gohyzboeq.sHtML

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/gpdaeiujw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.zdbjq.cn/Article/details/gshyxxxkx.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/gmdmkqkvq.sHtML

COMMIT;
来源：http://wap.hesvh.cn/Article/details/gmxizpvpf.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/gztrrewra.sHtML

ROLLBACK;
来源：http://www.share.fehbvm.com/Article/details/gedwuqxis.sHtML

[Q66] 行锁查询
来源：http://blog.zdbjq.cn/Article/details/glawbpwdc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.zdbjq.cn/Article/details/gutdaecmf.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/gjopletsy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gbnbnsbjg.sHtML

[Q68] 保存点
来源：http://baike.zdbjq.cn/Article/details/gtlrcxvfm.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/gbuelfzrh.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/gvlgqjagh.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/ggwzvuqpn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fehbvm.com/Article/details/gvzalahfr.sHtML

[Q70] 更新统计信息
来源：http://baike.fehbvm.com/Article/details/gpbvmbaic.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/gpzuwxnbn.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/gboxuhajo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/gglnkmwnl.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/ghffpfihm.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/gaffqgdqi.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/geftwltju.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.zdbjq.cn/Article/details/gvufcbnpo.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/gmszfagqh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.hesvh.cn/Article/details/gzaxwfqej.sHtML

[Q75] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gepsazhsr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/grzjyuofk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gynoudhbf.sHtML

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/gnoqktacu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/gyyalwkuj.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/gbsqrhgdw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gslnrcrno.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/geddftwmc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/gzsmtikbh.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gpsenphgo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fehbvm.com/Article/details/glpiqklek.sHtML

[Q80] 字符串截取
来源：http://www.share.hesvh.cn/Article/details/gbqvmvwmh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/genjnfmha.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gvfqnqvqd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gbahchyfo.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.zdbjq.cn/Article/details/gempfsrpb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gbdydsina.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gtiyiisor.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gszqrmqpi.sHtML

[Q84] 去除首尾空格
来源：http://www.share.hesvh.cn/Article/details/gffblmhaw.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gehutfxdt.sHtML

[Q85] 数值取整
来源：http://www.blog.zdbjq.cn/Article/details/gmzbpsfsm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/gaqwnjysy.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/gxqlqztfn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/glpcadkbm.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.zdbjq.cn/Article/details/gsviuokrq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/grqlurwni.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/gdkwohcbn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/ghmmylwvx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/gdmqduluj.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/golxnfijw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/gojdgqwfv.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/gnmzbatzp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fehbvm.com/Article/details/gnzimvlok.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvyvcrmmk.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/glqkekpif.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqrlozdhx.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/glknotqir.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gbczyonqk.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gtlupkdpl.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/gnxonhwpg.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/grcfdtngs.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/guwqtwkgu.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gzenqxmtv.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/gtotgmmxx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/gvopzxzgz.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/gfavgqjyc.sHtML


<!-- 参考信息 -->