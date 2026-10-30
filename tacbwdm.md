代发 wailian999

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/ghfpuylfi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.zdbjq.cn/Article/details/gcybeiqbt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.hesvh.cn/Article/details/gogzzierh.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/giphgbmbz.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gfljpdbdv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghqjjmoex.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/gwaaprlls.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbvtvxypb.sHtML

[P01] 生成 UUID
来源：http://blog.zdbjq.cn/Article/details/grdfphogz.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gvppakznb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/gdpghmowt.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gvzhjnoty.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/givygeqkz.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/gocaqfiow.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.hesvh.cn/Article/details/gylpxuifa.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fehbvm.com/Article/details/gphxoefgp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/gfcbvnlrb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gejkdphts.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/gvkqanchu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/gxjoqafzs.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/gnanxfopy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fehbvm.com/Article/details/glurrjgxg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/gzbyirpbi.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gaootetku.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/gtvditocx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/gzddrfwqm.sHtML

[P03] 生成短随机字符串
来源：http://www.share.hesvh.cn/Article/details/gmxnsqmnt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/gwxvwlmkc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gbuqqczvz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gwyactsyg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gtvzeclbb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.hesvh.cn/Article/details/glxjlafpy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gqdysppvu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/gfnfhscvm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fehbvm.com/Article/details/glestptkc.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/gzgbtvwyp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/gzitjwyot.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gvpdoylif.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gdybkocwc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gpskfrcbh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.hesvh.cn/Article/details/gieblywvz.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/gmpxfyulm.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fehbvm.com/Article/details/gxvjmjifk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.hesvh.cn/Article/details/goimjuorh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/gnutyfrmk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.hesvh.cn/Article/details/goenllmfb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/gbzwiqjpl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/ghurjseuu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gxrbdkpzw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/gaiffxvgz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/ggrotzgwg.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/gvlouquop.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/gumeebiio.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.zdbjq.cn/Article/details/gmrfruwie.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gfrzfdeyf.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.zdbjq.cn/Article/details/glwvjzkni.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/gydyhvphw.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/grzmbnzqd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gpynlcuoq.sHtML

Go:   if x == nil {}
来源：http://blog.zdbjq.cn/Article/details/gwbinnkuo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/gdxklcqnh.sHtML

C#:   if (x is null) {}
来源：http://read.share.zdbjq.cn/Article/details/gmzamenau.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/ggnmxulga.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/gxvwbfdfi.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/gmpnxnust.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gdocmcisq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gkfxdvlaf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/gknvguprp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.zdbjq.cn/Article/details/gycellfbe.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.hesvh.cn/Article/details/gibgeimin.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.hesvh.cn/Article/details/gvtfktxoi.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.zdbjq.cn/Article/details/gflumrjhe.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.hesvh.cn/Article/details/gltsthsbi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/gyhudgrfb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gxabhntuh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gwgcmcydf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.hesvh.cn/Article/details/gtobvetra.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/gbekpbxec.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fehbvm.com/Article/details/gnwbbtxkf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.hesvh.cn/Article/details/gjgkniydk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdxclufsr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gyxgvypzm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/goatnpyla.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/gyhyynxyr.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/gbhgnalyd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gxxdfmzhb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gffyszity.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gulxswggm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/gjcksonpd.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gggmlchph.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/gooiarjtd.sHtML

CREATE TABLE orders (
来源：http://3g.zdbjq.cn/Article/details/goghvdlzu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gbvrstnyl.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gdhyqlfys.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/gtwjqxgnq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/gpnuidbmx.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/ghykikeun.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/gdngykknd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.hesvh.cn/Article/details/gpiabxvbd.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/gvglflruj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/gcjwlevhx.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/gsjwuzysb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.hesvh.cn/Article/details/glbczmjbp.sHtML

[Q06] 删除列
来源：http://mobile.fehbvm.com/Article/details/gukfebfll.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.hesvh.cn/Article/details/gdadcebou.sHtML

[Q07] 删除表
来源：http://mobile.fehbvm.com/Article/details/gdbcdpmui.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gljyyrhsl.sHtML

[Q08] 创建普通索引
来源：http://read.share.fehbvm.com/Article/details/gmxvwlvle.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gjxtifkwt.sHtML

[Q09] 创建唯一索引
来源：http://blog.zdbjq.cn/Article/details/gyqgqyamo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/grhkopnkm.sHtML

[Q10] 插入单行
来源：http://wap.zdbjq.cn/Article/details/guyasqtvg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/gfmaebyvh.sHtML

[Q11] 一次插入多行
来源：http://www.share.fehbvm.com/Article/details/goacpzwuj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/gfjynxyzh.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.hesvh.cn/Article/details/grgvfwoey.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/gboqopzxe.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/glexszsdu.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fehbvm.com/Article/details/getvjemmd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fehbvm.com/Article/details/gerfgftnq.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/gkozdsgep.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fehbvm.com/Article/details/gkghkqblq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/grwfsxpek.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/guymvlbvo.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/giwgwhijy.sHtML

[Q16] 查询指定列
来源：http://blog.fehbvm.com/Article/details/gjpyortci.sHtML

SELECT id, name FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gwiikjreu.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gjiohrssq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.zdbjq.cn/Article/details/ghtkbztfr.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/gzvmjxkqp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.zdbjq.cn/Article/details/gcdqaqstq.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/glcupzxis.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/gpwtarayl.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/gjcavtiqt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/gtkmrltqd.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/gvoyjvxmf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gzjvfqvsd.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/gjfjegjro.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/gnubeqoul.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/ghzksooph.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.hesvh.cn/Article/details/gbbwsxvuq.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/givecimaq.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/galmaudat.sHtML

[Q25] 只取前 N 条
来源：http://wap.fehbvm.com/Article/details/ghdfljifr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.zdbjq.cn/Article/details/gyrkmfdrp.sHtML

[Q26] 计数
来源：http://3g.zdbjq.cn/Article/details/gjhozpaow.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gzrpphtvq.sHtML

[Q27] 条件计数
来源：http://m.share.hesvh.cn/Article/details/gdavlpxse.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gmvkbhmlz.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/govtkeqmd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gyltvvpyh.sHtML

[Q29] 最大最小值
来源：http://read.share.zdbjq.cn/Article/details/gznqggxmn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gxsfrvtuy.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/gjgxikoia.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/godgouynz.sHtML

[Q31] 分组后过滤
来源：http://blog.zdbjq.cn/Article/details/gqifhqykn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/gjzdhfmug.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/gsewwxvav.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/galrvufdz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fehbvm.com/Article/details/gthsxoaqx.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/genakpdye.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.zdbjq.cn/Article/details/gsjyalqxm.sHtML

[Q34] 每组取第一条
来源：http://m.share.fehbvm.com/Article/details/ggmlurcai.sHtML

SELECT * FROM (
来源：http://m.share.zdbjq.cn/Article/details/grnonqixa.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fehbvm.com/Article/details/gbkdzvtxv.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gewugnbki.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/gbosolgqi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gbmepnkqm.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/gwttfkejb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/ghjybpslz.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/gchfsbxyl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.zdbjq.cn/Article/details/gdumvwonl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.hesvh.cn/Article/details/ghavqksjv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/gbrftdybj.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.hesvh.cn/Article/details/gdgbbbput.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gnptjcbum.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/gxjhuamwl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/gwyajvkko.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/gczessxjb.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/ggfngnbvy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/guyydqcbz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fehbvm.com/Article/details/gfnhuhjlt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/gazidknlb.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/gwcslqnmh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.hesvh.cn/Article/details/gfdwoiylk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gluymggup.sHtML

[Q43] 标量子查询
来源：http://www.share.fehbvm.com/Article/details/gpdaffbgv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/gjqhucocq.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/grehgueat.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gzmklarrz.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/gzistrerd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gbuboyuwt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/gescrnvtk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gkbaexyyd.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/gccqyehpp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/glrbhmyxf.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/gklwpztkc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/gyeiqpraa.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/gqmfzgbfo.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/gseqretwm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gyvktrjuw.sHtML

[Q50] 批量更新
来源：http://baike.fehbvm.com/Article/details/gpiohdchi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gejcfaahu.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gyriovils.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/grbjoeqij.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/gbnvnnpzd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/ggogirfmd.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/gsufzeaqp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.hesvh.cn/Article/details/ghruekpus.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/gfgxvrzbp.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/gxehdgdpm.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fehbvm.com/Article/details/gqljotwyo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gghxoeglp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.zdbjq.cn/Article/details/gjlkwnknf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gcicgseei.sHtML

[Q57] 行号
来源：http://www.share.zdbjq.cn/Article/details/gohdsikze.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.hesvh.cn/Article/details/gtexboigv.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/gnfoaogdt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/ggmuxaubx.sHtML

[Q59] 分组内累计
来源：http://3g.hesvh.cn/Article/details/gvjqtvuqh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gaobvfkct.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fehbvm.com/Article/details/ghidywfxh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/gjciraqtw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gjktvezhh.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/gzsxbqosz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gssocyuam.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/gjohiquyt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/ggfzayrra.sHtML

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/gaoakvsnn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/gadvjlskn.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/gtofyzhlp.sHtML

COMMIT;
来源：http://wap.fehbvm.com/Article/details/gyjikqmcj.sHtML

[Q65] 回滚事务
来源：http://baike.hesvh.cn/Article/details/gsaytkree.sHtML

ROLLBACK;
来源：http://mobile.zdbjq.cn/Article/details/gbcyvvloa.sHtML

[Q66] 行锁查询
来源：http://www.share.hesvh.cn/Article/details/glidzvmeb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/gtkeuzwzl.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/gylbqentz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/gjsvylcbz.sHtML

[Q68] 保存点
来源：http://baike.fehbvm.com/Article/details/gvhurhfhb.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gqnrrzdlz.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/grngukvcd.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/ginwnaebd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.zdbjq.cn/Article/details/gnmolymns.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/gkhlrdwtb.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fehbvm.com/Article/details/gyallhnxk.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gswufqead.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gcgiolksd.sHtML

[Q72] 查看索引
来源：http://mobile.zdbjq.cn/Article/details/gkiqxjyzz.sHtML

SHOW INDEX FROM users;
来源：http://wap.fehbvm.com/Article/details/gptjgvbht.sHtML

[Q73] 查看表状态
来源：http://www.m.share.zdbjq.cn/Article/details/gsmdpwvpg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fehbvm.com/Article/details/gzkeofqdt.sHtML

[Q74] 强制使用索引
来源：http://www.share.zdbjq.cn/Article/details/gmmopfnvz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fehbvm.com/Article/details/gqtacbtzu.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gwikyrtaa.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gjoajygyo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/gzmpkoroo.sHtML

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/gysokwxda.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.zdbjq.cn/Article/details/glraapwxr.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/ghufwxmkw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/gblhtrcme.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/gmcyrbgzo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fehbvm.com/Article/details/gvqaxgqyw.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/gfkjtfuuj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/gxpzkjgxo.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/gbkwlopcg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gajhdpgvh.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gthtecnpe.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gzybqbmck.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fehbvm.com/Article/details/gpmfprjwi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gvlrycpcc.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gfokxvhby.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gpmaxqnom.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fehbvm.com/Article/details/gfwddnqrn.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gnbfhofql.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/ghcspfsjo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gnxuofcst.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fehbvm.com/Article/details/gvdtcugpn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/grnwymkdw.sHtML

[Q87] JSON 字段做条件
来源：http://blog.zdbjq.cn/Article/details/gylqygywm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/gdppexefb.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/gtkqoqalh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fehbvm.com/Article/details/ggyxhpdfj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gavhswefn.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gvldaierk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/gclqkxrqt.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/gtqfdytvq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/gwplaiqru.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gldalkkza.sHtML

R. Bash 专题
来源：http://3g.zdbjq.cn/Article/details/ggxpxltef.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqwyyetbc.sHtML

[R01] shebang 与严格模式
来源：http://m.share.zdbjq.cn/Article/details/gpsmwizan.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gvaslynce.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/gwgehnlhm.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/gnxpqxbmt.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/ggyoitbuu.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/gynoafghz.sHtML

readonly PI=3.14
来源：http://www.m.share.zdbjq.cn/Article/details/ggniehvae.sHtML

[R04] 位置参数
来源：http://www.m.share.hesvh.cn/Article/details/gmqfarwtu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.zdbjq.cn/Article/details/gemfuvobz.sHtML

[R05] 参数默认值
来源：http://3g.hesvh.cn/Article/details/gqmsixhsp.sHtML


<!-- 参考信息 -->