代发 wailian999

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gglxlujai.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fehbvm.com/Article/details/gbdruvxul.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.hesvh.cn/Article/details/gzteaspri.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/gxygudomu.sHtML

C#:   Parallel.For
来源：http://wap.zdbjq.cn/Article/details/gjehkrvrh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grgxfyfzn.sHtML

P. 常用工具函数
来源：http://www.share.fehbvm.com/Article/details/gzivdclru.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqnwnvvde.sHtML

[P01] 生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gpkpvwbyz.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/gggnhtkdy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/gnolnuocb.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gbrsbzdgn.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/ggaphubcg.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/ghpbuepmg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.zdbjq.cn/Article/details/gcibnudch.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gpgsrkfww.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gjitpsdle.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/glrtkdhfo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.hesvh.cn/Article/details/gkzrhvcrt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/gumcudikc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gzpzgnwac.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fehbvm.com/Article/details/gvgfewdbe.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/gnhoflayb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gjpammvbp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fehbvm.com/Article/details/gnmiwghvz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/glqqaolgs.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/ggocylmpv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.zdbjq.cn/Article/details/gxmliujwa.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fehbvm.com/Article/details/gmvuituke.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/guwucuasm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gzqgsjmzc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/gtlxqeqew.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.zdbjq.cn/Article/details/ghdyvqasv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/guytfpjgz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fehbvm.com/Article/details/ggsdvafuz.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/gynmwlcqu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/gfhgshyid.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gqazpenpt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gezxdawpg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gncpgilsl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/ghoqxduzn.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.hesvh.cn/Article/details/gwmxlkcub.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/gxuaxcbyb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fehbvm.com/Article/details/gftepnnkr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/gsukrsaxk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/gpeafieaq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/gazzasavo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/ggypbaehg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/grdvolmje.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fehbvm.com/Article/details/gagugkrcx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fehbvm.com/Article/details/gqnrekpkz.sHtML

Ruby: a == b
来源：http://read.share.zdbjq.cn/Article/details/gokfjufmu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/gkeyyjofl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/gltcitpaa.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.hesvh.cn/Article/details/gdpggzedc.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.hesvh.cn/Article/details/gvzvbafqd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fehbvm.com/Article/details/gfqrluymf.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/gwcvtfzel.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gxvhwmzlg.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/gymccjfnz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/gywkhchyn.sHtML

C#:   if (x is null) {}
来源：http://www.share.hesvh.cn/Article/details/gtivgokun.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/ggyqoznzh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/gpqmkjlmb.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/gqcarbdzj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gqzhontsl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gnetajsco.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.zdbjq.cn/Article/details/gmystiidp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/gzmgdklmh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.zdbjq.cn/Article/details/gqntbkbqw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fehbvm.com/Article/details/gipcrzycp.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fehbvm.com/Article/details/gmxiqcwux.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.zdbjq.cn/Article/details/gdsemvvyh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fehbvm.com/Article/details/gftzsgvfr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/gdquekmft.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/ghrjqmltg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/gcvnivcqj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.zdbjq.cn/Article/details/grnxmvwzv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.zdbjq.cn/Article/details/gzlleyuje.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.hesvh.cn/Article/details/gzxnadpfg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gacduorhe.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/gggottoux.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/guiddpwqb.sHtML

[Q01] 创建表
来源：http://mobile.hesvh.cn/Article/details/gldzzipco.sHtML

CREATE TABLE users (
来源：http://www.m.share.zdbjq.cn/Article/details/gihyramln.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/guzamjxpv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gwviqtqxq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gjkgvoyyv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/gjjuivtcn.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gothpvpno.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/gerracfda.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/ghfbievnb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gccswoygn.sHtML

user_id INT NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gflyfjcxl.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/gkxhexcob.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/gwdlrfpqd.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gnvugjeep.sHtML

[Q03] 增加列
来源：http://m.share.zdbjq.cn/Article/details/gtvmquzne.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/gvrqszfog.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/ghvjkpurg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/gbdrfccez.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/gcsvnaozu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/gmeoxfxrz.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/gizaettly.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.hesvh.cn/Article/details/gpwnzlwdu.sHtML

[Q07] 删除表
来源：http://3g.zdbjq.cn/Article/details/gwjhqcomy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fehbvm.com/Article/details/godngsxhe.sHtML

[Q08] 创建普通索引
来源：http://read.share.fehbvm.com/Article/details/gfpxnvfox.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gqytzqgyy.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/gzbqrhfka.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gejkeypqr.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/gqgrydrom.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/ggztlnroh.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/gnxdicpsa.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fehbvm.com/Article/details/gecwuvcwz.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.hesvh.cn/Article/details/gcyvwrexu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.hesvh.cn/Article/details/gictbnwbn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.zdbjq.cn/Article/details/gmxehghow.sHtML

[Q13] 忽略重复插入
来源：http://wap.hesvh.cn/Article/details/ghcwjsegq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gjqkxnspl.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.zdbjq.cn/Article/details/gqcnsdfic.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/gctltvvmz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.zdbjq.cn/Article/details/gipfrwfcl.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/grmwmsnex.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/gihastyxt.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/gssibobkh.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gtsvciqoa.sHtML

[Q17] 条件查询
来源：http://baike.hesvh.cn/Article/details/gfodnpbeo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fehbvm.com/Article/details/giliaqxyp.sHtML

[Q18] 模糊匹配
来源：http://www.blog.zdbjq.cn/Article/details/genphxfgk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gleqpnaus.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/gzyjoxors.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.zdbjq.cn/Article/details/gwnexaxlo.sHtML

[Q20] IN 列表
来源：http://read.share.fehbvm.com/Article/details/gdfydiiei.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.zdbjq.cn/Article/details/gdvhbnhfs.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/gebwxthrh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/ghtynugud.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/gufnxplur.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.zdbjq.cn/Article/details/gwxgznnzb.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gyaxoayyh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.hesvh.cn/Article/details/gjewcejav.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/grulbpfxl.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.hesvh.cn/Article/details/gfxlkdqzl.sHtML

[Q25] 只取前 N 条
来源：http://mobile.hesvh.cn/Article/details/gpspnbbgu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fehbvm.com/Article/details/gwxfrbwxw.sHtML

[Q26] 计数
来源：http://mobile.hesvh.cn/Article/details/gsjmpypra.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gysyytred.sHtML

[Q27] 条件计数
来源：http://wap.fehbvm.com/Article/details/goytvjoxa.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gfipdthmg.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/gncepyfcu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gvoqwawqt.sHtML

[Q29] 最大最小值
来源：http://www.blog.fehbvm.com/Article/details/gxxdvswtz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fehbvm.com/Article/details/gfcfuuyim.sHtML

[Q30] 分组统计
来源：http://www.share.hesvh.cn/Article/details/gmydtqowb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gtknepije.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/gevvbqqei.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/gsepjzbov.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gmichnjme.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gdkjgacyj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/gwiixvsta.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gwidbrtui.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/giplmhgkz.sHtML

[Q34] 每组取第一条
来源：http://m.share.fehbvm.com/Article/details/gffxdqrod.sHtML

SELECT * FROM (
来源：http://m.share.hesvh.cn/Article/details/ghkvoduad.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/grmglxxww.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/grrclgxef.sHtML

[Q35] 内连接
来源：http://wap.zdbjq.cn/Article/details/gasymooeu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gztjtpxik.sHtML

[Q36] 左连接
来源：http://read.share.fehbvm.com/Article/details/gufjgoatt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gpbgckdqx.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/gjwmcyudk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gudyngheb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/grafotmxe.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/glqpslgbr.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/gwtktescu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/gjjlfgqni.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fehbvm.com/Article/details/ghhavvubk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/gjjnpgaci.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/gupgkybjx.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/gqyalfvyv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/gmesydbav.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/gvfqggybu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/gkoylagij.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.zdbjq.cn/Article/details/ggajtnjgp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/gcpvqqnyx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fehbvm.com/Article/details/gmxnhnfce.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/gtgcsqoyo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/gampvrgji.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/gjzolnxkh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.hesvh.cn/Article/details/gxofsaloz.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/gbaohzkbl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gpdtbrjda.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.zdbjq.cn/Article/details/gmlknhwfy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gwofeabou.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/ghshdvomt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.zdbjq.cn/Article/details/gwaedqsbe.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fehbvm.com/Article/details/gxqsmhhch.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.hesvh.cn/Article/details/grbtcfxkp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/grzhgcxkv.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/gxoaetvin.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gutqxejwt.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gjsxrumyq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/gzzohuzie.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/gnzdxziqq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gznvdvnjt.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gvqdqfcwq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gnaiiqkqq.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/gyahsvztk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gbahkopuj.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/gpbhwlkmw.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/gmxtjsrne.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/gsngidlip.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gauiylhsa.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/gghijhgld.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gwykhxldd.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gyagjqwfi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.zdbjq.cn/Article/details/gojcyzrwe.sHtML

[Q58] 累计求和
来源：http://read.share.zdbjq.cn/Article/details/gxlcodpwn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.hesvh.cn/Article/details/ghcbjitbf.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/gjotlsaih.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gvrsbqgtw.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/gjhhustcv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/gandzfwku.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/gczgjyaxb.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gqtgkbknv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gvklevqql.sHtML

[Q62] 分组占比
来源：http://baike.hesvh.cn/Article/details/gvorlftip.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gpmvopetv.sHtML

[Q63] 开启事务
来源：http://baike.fehbvm.com/Article/details/gtipgvpsi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/gqsfizlzm.sHtML

[Q64] 提交事务
来源：http://www.share.fehbvm.com/Article/details/givipgiuq.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/gvksyhajd.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/gbrfmcufq.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/ggwzospmi.sHtML

[Q66] 行锁查询
来源：http://wap.zdbjq.cn/Article/details/ggomdmown.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/gxyqurvig.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/gljipghnv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/gdkdelrmo.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/gbrophifu.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gglaicsye.sHtML

ROLLBACK TO sp1;
来源：http://blog.zdbjq.cn/Article/details/glzurhfac.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gioxnkfbv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/gqmurmxnj.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/graryvbiw.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/gekfqcwig.sHtML

[Q71] 查看建表语句
来源：http://m.share.fehbvm.com/Article/details/gdanztjuk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/gucwlmtlw.sHtML

[Q72] 查看索引
来源：http://www.m.share.zdbjq.cn/Article/details/gzoarpbpn.sHtML

SHOW INDEX FROM users;
来源：http://mobile.hesvh.cn/Article/details/gqbdsfqtc.sHtML

[Q73] 查看表状态
来源：http://read.share.fehbvm.com/Article/details/gnedererv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fehbvm.com/Article/details/gcqzqmpim.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/ggchbhpiw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.hesvh.cn/Article/details/gqbyzapwz.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gbnkubfwj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/guppallgg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/geycpgiqe.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gpmonhsel.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/glmqkmwgq.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/gojdoiwxr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/gsmevubqs.sHtML

[Q78] 当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gxsvdujeo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/gnclraxim.sHtML

[Q79] 字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gahivljvg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.zdbjq.cn/Article/details/gbcvjqrip.sHtML

[Q80] 字符串截取
来源：http://3g.fehbvm.com/Article/details/gfckoithr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gmzphltwn.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gyyvyoxdb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gcxouatdw.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fehbvm.com/Article/details/ghcfptohn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/ggvngzpek.sHtML

[Q83] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gezqyoyzd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gzsayneez.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/gljccwolw.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/ghhhbbufn.sHtML

[Q85] 数值取整
来源：http://www.share.zdbjq.cn/Article/details/gczpuyhot.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/gvkdmhkmz.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.hesvh.cn/Article/details/gmitxieqb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/gycxeydro.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gwuczokgx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fehbvm.com/Article/details/gedpnbjvd.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/gogwmubne.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/goiasfskg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.hesvh.cn/Article/details/gvfddjiye.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/gzueetmyo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gwngvensq.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/gkosktvtv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.hesvh.cn/Article/details/gscwjlqix.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gefzdfrlp.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/ghofjccgd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjvrstefb.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/gnxjhvkso.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/ghlsyxnhe.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gcagqdddg.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/gfpatkhdh.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/gtlhlsqma.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/gyyzivlvp.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/gqaixwtwf.sHtML

[R04] 位置参数
来源：http://www.blog.zdbjq.cn/Article/details/gvmaxjnrx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/gzhywirss.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gltcvdeil.sHtML


<!-- 参考信息 -->