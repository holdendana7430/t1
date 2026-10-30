代发 wailian999

[P01] 生成 UUID
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrdcvyfx.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fanxiaobao.xyz/Article/details/gffbpgjlc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fanxiaobao.xyz/Article/details/gebrmbroy.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppnlociy.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gimolzfoc.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmriodud.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fanxiaobao.xyz/Article/details/glsjixijm.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fanxiaobao.xyz/Article/details/gjzktovqu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fanxiaobao.xyz/Article/details/getrjodzg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fanxiaobao.xyz/Article/details/grpgjupup.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbmueevh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/ganadklpi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhwcoddm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxaqpjkw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdczoumur.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fanxiaobao.xyz/Article/details/gvfljijfj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnqdszau.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fanxiaobao.xyz/Article/details/godvsashc.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrritonh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fanxiaobao.xyz/Article/details/gcvcifrqc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcwkunpo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fanxiaobao.xyz/Article/details/gifznqrxk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlbryxtg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fanxiaobao.xyz/Article/details/gxgduwuxv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmunhmvw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fanxiaobao.xyz/Article/details/gmxfmqzwr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbamabax.sHtML

[P04] 求长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjtwrxxf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fanxiaobao.xyz/Article/details/gmllntaju.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fanxiaobao.xyz/Article/details/ggaaozblh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fanxiaobao.xyz/Article/details/gyggqkbkw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fanxiaobao.xyz/Article/details/gprzjhoml.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fanxiaobao.xyz/Article/details/gakgbecpr.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcexcrbpk.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fanxiaobao.xyz/Article/details/ggosjhhfi.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fanxiaobao.xyz/Article/details/gsigavoew.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fanxiaobao.xyz/Article/details/glggstoqt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyekoxkn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fanxiaobao.xyz/Article/details/gwozwhbaf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghimtlsei.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpjgtljp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylvqfdll.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fanxiaobao.xyz/Article/details/gnujkpuec.sHtML

Ruby: a == b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjgjdazr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fanxiaobao.xyz/Article/details/gebdtawxa.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fanxiaobao.xyz/Article/details/gbqeqmcul.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fanxiaobao.xyz/Article/details/gawzwcbuw.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztkpvwre.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvkzsyek.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfokkhuvt.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gzwsgvcal.sHtML

Go:   if x == nil {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gibdyyqhh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfgfngzp.sHtML

C#:   if (x is null) {}
来源：http://baike.fanxiaobao.xyz/Article/details/geetovnvm.sHtML

[P07] 防抖与节流
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsyvcdrxi.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycmeyfjc.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gaswhxfyg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsmkuplk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkryrfvqs.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fanxiaobao.xyz/Article/details/givnejsjr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwgieohk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrdkcnyy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhsggnwd.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrzxkzgm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glckneuxk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gggaoqpic.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fanxiaobao.xyz/Article/details/gltuhepkh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdaigqmqj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fanxiaobao.xyz/Article/details/ghkocbmre.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fanxiaobao.xyz/Article/details/glearpfhq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fanxiaobao.xyz/Article/details/gpenvucqn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fanxiaobao.xyz/Article/details/gilgzdoly.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ghukiinbk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmdqulsp.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ghsdqvjxw.sHtML

[Q01] 创建表
来源：http://wap.fanxiaobao.xyz/Article/details/gopmcgkzz.sHtML

CREATE TABLE users (
来源：http://baike.fanxiaobao.xyz/Article/details/gpeyebxex.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fanxiaobao.xyz/Article/details/gooetzjuq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fanxiaobao.xyz/Article/details/gvlexbrpa.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fanxiaobao.xyz/Article/details/givldgooh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyjcvndg.sHtML

);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukcbhlpz.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fanxiaobao.xyz/Article/details/geijojyeb.sHtML

CREATE TABLE orders (
来源：http://baike.fanxiaobao.xyz/Article/details/gwhgpreik.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fanxiaobao.xyz/Article/details/gyktulrix.sHtML

user_id INT NOT NULL,
来源：http://3g.fanxiaobao.xyz/Article/details/ghcinajgy.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxawtcbz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksazzuum.sHtML

);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyjcufjs.sHtML

[Q03] 增加列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqopqkebv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnftgzgn.sHtML

[Q04] 修改列类型
来源：http://blog.fanxiaobao.xyz/Article/details/gdizvtunw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fanxiaobao.xyz/Article/details/gtcdikviy.sHtML

[Q05] 重命名列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givhbmwbt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fanxiaobao.xyz/Article/details/geaianxun.sHtML

[Q06] 删除列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbdcpysd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fanxiaobao.xyz/Article/details/gjjcaottj.sHtML

[Q07] 删除表
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjuqvdao.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gvzmuyunu.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjklhsvda.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fanxiaobao.xyz/Article/details/glxvexgdm.sHtML

[Q09] 创建唯一索引
来源：http://blog.fanxiaobao.xyz/Article/details/gvxksyjrz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdpetfyz.sHtML

[Q10] 插入单行
来源：http://3g.fanxiaobao.xyz/Article/details/genvalocr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/gexhgsocl.sHtML

[Q11] 一次插入多行
来源：http://wap.fanxiaobao.xyz/Article/details/gemoxlika.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/ggqcrelpm.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fanxiaobao.xyz/Article/details/givhpgljq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fanxiaobao.xyz/Article/details/grhmxroyh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkmchipt.sHtML

[Q13] 忽略重复插入
来源：http://3g.fanxiaobao.xyz/Article/details/gsjgeaexu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/ghduaqbsk.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fanxiaobao.xyz/Article/details/gjjxqtgnj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fanxiaobao.xyz/Article/details/gsouwmlxf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvgntvdi.sHtML

[Q15] 查询全部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvexfjegm.sHtML

SELECT * FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gdeshgblu.sHtML

[Q16] 查询指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gtkhxnsex.sHtML

SELECT id, name FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/goptaqdjw.sHtML

[Q17] 条件查询
来源：http://read.share.fanxiaobao.xyz/Article/details/guvmndbem.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngcidhkx.sHtML

[Q18] 模糊匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxcrnrrr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fanxiaobao.xyz/Article/details/gugbikpjs.sHtML

[Q19] 范围查询
来源：http://mobile.fanxiaobao.xyz/Article/details/guwyzsatg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fanxiaobao.xyz/Article/details/gdzardeaz.sHtML

[Q20] IN 列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsqbjnne.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gxkvasfaa.sHtML

[Q21] 空值判断
来源：http://read.share.fanxiaobao.xyz/Article/details/giqwsnzqh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fanxiaobao.xyz/Article/details/gqvaofhwh.sHtML

[Q22] 排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzwrgpjy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyalqzjpg.sHtML

[Q23] 分页
来源：http://m.share.fanxiaobao.xyz/Article/details/gljfsethh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fanxiaobao.xyz/Article/details/gaqytnoaw.sHtML

[Q24] 去重
来源：http://mobile.fanxiaobao.xyz/Article/details/gbogxcsrj.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gsumpediy.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfpgtflb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkbbjwct.sHtML

[Q26] 计数
来源：http://blog.fanxiaobao.xyz/Article/details/gxmetcwqn.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gxntjclka.sHtML

[Q27] 条件计数
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqnqycoc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrdhhhvq.sHtML

[Q28] 求和与平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxszroky.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvddfmang.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjqoqthq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvifwhusy.sHtML

[Q30] 分组统计
来源：http://baike.fanxiaobao.xyz/Article/details/gsdnochbe.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gusrujxxt.sHtML

[Q31] 分组后过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/ghptbaewf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gorawnous.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gpqteqkco.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gspffaphx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fanxiaobao.xyz/Article/details/gexylevuw.sHtML

[Q33] 多列分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrbmffmt.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzleczvq.sHtML

[Q34] 每组取第一条
来源：http://wap.fanxiaobao.xyz/Article/details/gmodphomr.sHtML

SELECT * FROM (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvmlqnep.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilxqicls.sHtML

) t WHERE rn = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhbbrepn.sHtML

[Q35] 内连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsawnphi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gjnyvpqes.sHtML

[Q36] 左连接
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxpmtnia.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnsaewfs.sHtML

[Q37] 右连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggphwqgba.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwuqglwg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrhcwwlu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gspaejzlq.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaozraesj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fanxiaobao.xyz/Article/details/gouwyxksc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fanxiaobao.xyz/Article/details/govqugnlm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fanxiaobao.xyz/Article/details/gfwjfqivy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrxkhsso.sHtML

[Q41] 多表连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gylynhhhf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fanxiaobao.xyz/Article/details/gopwtdiso.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fanxiaobao.xyz/Article/details/govqbjcyg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvtmuwvw.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gjeyotrww.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fanxiaobao.xyz/Article/details/gccpzstqj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gybiwjpwv.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givfcmrdv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/gaifutnyc.sHtML

[Q44] IN 子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gzagfwkiw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkxemkqn.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfqcdhkn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gafcagmrv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gwuqdwncr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjofcaom.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazzrukii.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzjwidmc.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gswgtcats.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmqtlfkw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fanxiaobao.xyz/Article/details/ggshjgush.sHtML

[Q49] 更新单行
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjmmjayh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gkaybynhm.sHtML

[Q50] 批量更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxdgzvvx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/geuswajzw.sHtML

[Q51] 用子查询更新
来源：http://wap.fanxiaobao.xyz/Article/details/gwpzglwnu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gjenccfxl.sHtML

[Q52] 删除指定行
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdgtkpbj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gybxkctnf.sHtML

[Q53] 按条件删除
来源：http://baike.fanxiaobao.xyz/Article/details/gtktxsiow.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/glclaucyw.sHtML

[Q54] 清空表
来源：http://read.share.fanxiaobao.xyz/Article/details/gismrtixf.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/grjdddyjq.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gyxmiwaxo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gpynzcyja.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgisgobt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gimzexkij.sHtML

[Q57] 行号
来源：http://blog.fanxiaobao.xyz/Article/details/gvwnwavgo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gxhfcvmjj.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gsceotadl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdblgjjh.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwboxuzy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gacfcjutp.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/gfsquvvhd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/gwalgrqzz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/grzkxwqko.sHtML

[Q61] 移动平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmldazerj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gcfnqvggk.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gfrdvahmr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqxyjcga.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/gygeuzmur.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/gnphdylai.sHtML

[Q64] 提交事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gysdzacsa.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmauhmvpe.sHtML

[Q65] 回滚事务
来源：http://baike.fanxiaobao.xyz/Article/details/gdjhnajud.sHtML

ROLLBACK;
来源：http://baike.fanxiaobao.xyz/Article/details/gmdyyjxrs.sHtML

[Q66] 行锁查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gmowkleuj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fanxiaobao.xyz/Article/details/gpthkksji.sHtML

[Q67] 设置隔离级别
来源：http://blog.fanxiaobao.xyz/Article/details/ghskewvac.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzycheujl.sHtML

[Q68] 保存点
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfdcbrye.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqoputwhh.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gncrkpkkn.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvilehto.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxhzlyeg.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/ginyonkxk.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gokammjvi.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/grambcobm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fanxiaobao.xyz/Article/details/gxiwtqdwo.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gpaakqrvh.sHtML

SHOW INDEX FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gmmtlnmux.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/gdswtbysq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssngionj.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/glzexfccp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchbjrush.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/goxzizxyl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gytwrvpzd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/gqktzefoe.sHtML

[Q76] 按天统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjjufwxt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyutipecj.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gmhddmqfh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyqyxcor.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjxsqlxj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/gpnfiuuki.sHtML

[Q79] 字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gtobhdbsi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gozjumzaz.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/gkonedmcn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlbgcaoj.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gpofcrutt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gysangtvl.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdsjbwrt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gydqkggfk.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/getffrxyh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkajfgrxh.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gzrzhasqo.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsvemmhk.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gaelkamah.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/gjpmxixcj.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gtphyjczy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/gpefiuuvg.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyabbtfp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/gmanwfuet.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fanxiaobao.xyz/Article/details/gpztblhgp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/gijynxiou.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjhqzusc.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gpingnxpy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gkilalcbm.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/giedlelsx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gcdhbhyvd.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gawxivaqw.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gnyytostq.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gllqzomfr.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwymzker.sHtML

#!/usr/bin/env bash
来源：http://read.share.fanxiaobao.xyz/Article/details/gzifgxyjj.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gexdbyedp.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrhvoziv.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gthiayfxc.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawaqvyjc.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gensmldty.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gbeuuompa.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gqczlniwr.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxyxirsa.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glunmjkkc.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gokynrkuo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/glwicrpvs.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gamlvwhey.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpendwyw.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhsgmags.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/glklcoaet.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gbftcvmhg.sHtML


<!-- 参考信息 -->