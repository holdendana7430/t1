代发 wailian999

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gcqulvxvw.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gdsiuszbm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fehbvm.com/Article/details/gludmgejp.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gmgyrgasv.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gnxzefvwt.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.hesvh.cn/Article/details/goxvyffcs.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/geiechbuw.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/gjthiyeob.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/gdbfjjjcf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.hesvh.cn/Article/details/gkfhecrbw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/gzierlvcc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/gfksnmyef.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/ghykvrpoc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.zdbjq.cn/Article/details/gnovuqfdl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gxetpkbah.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/gqgiicqmh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fehbvm.com/Article/details/gfnquwacz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.zdbjq.cn/Article/details/gylxpnkxp.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/grhajeuhz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/gfzfpgkxc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fehbvm.com/Article/details/gnnnagmbp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gkguevibj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gteplqhsi.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/ghcehbtpo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fehbvm.com/Article/details/guspliqxw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.zdbjq.cn/Article/details/gwqzzipev.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/gonotrrzt.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/gerugojui.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fehbvm.com/Article/details/gibrimjia.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gmazjgwoi.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/galnhskob.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gczuderhi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/gaxfecehh.sHtML

Go:   len(arr);  len(m)
来源：http://blog.zdbjq.cn/Article/details/gfdlpxczu.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/gfcxrvqti.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/gwbvxdxnp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fehbvm.com/Article/details/gjyahhfjx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.zdbjq.cn/Article/details/gujwhazav.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/gltrfkrfy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/gcajdiegs.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gnctesoam.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gynbdrprz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fehbvm.com/Article/details/gaeoanolx.sHtML

Ruby: a == b
来源：http://baike.fehbvm.com/Article/details/gymtbodlw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gnvecxddz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/gtynuyyyz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.hesvh.cn/Article/details/ggxikaolg.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.hesvh.cn/Article/details/gljdakdhu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/gdmdencjl.sHtML

TS:   if (x == null) {}
来源：http://m.share.zdbjq.cn/Article/details/gezqwrmnq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/ggkvczrvg.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/gymrnamgm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.hesvh.cn/Article/details/gjdiorxlh.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gdyhoegyj.sHtML

[P07] 防抖与节流
来源：http://blog.fehbvm.com/Article/details/gtpvifjno.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/gvvhkrmao.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/gioetvnpp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gxphnejjw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gycxwcbzu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/gkykefczh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.hesvh.cn/Article/details/golowndlj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gfsdftuqv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/gqwyvqqqh.sHtML

[P08] 处理浮点精度问题
来源：http://wap.zdbjq.cn/Article/details/gpoiconix.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/giykqhmcf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fehbvm.com/Article/details/golajfxwr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gymlpuyug.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gdwsccqkt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.hesvh.cn/Article/details/goyjahujl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/gtbiflrtg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/gqcixoyiv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fehbvm.com/Article/details/givjpppuc.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/galusibrh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fehbvm.com/Article/details/gnuvhbhgm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtuqmymko.sHtML

[Q01] 创建表
来源：http://baike.hesvh.cn/Article/details/gccngijep.sHtML

CREATE TABLE users (
来源：http://read.share.fehbvm.com/Article/details/gixdzwivo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gnxbmyxrt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/ggkjixnmo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/gxxpadybt.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fehbvm.com/Article/details/gidxebebe.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gjnzeghgg.sHtML

[Q02] 创建带外键的表
来源：http://www.share.zdbjq.cn/Article/details/gcwtlmlik.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/guaerzttc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/ghcmozmyc.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gtepybcbj.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gfupkwbhb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/gnxjuscux.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gcxgfmevj.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/gujgvytdq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fehbvm.com/Article/details/gopmbmzjh.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gaphsehfd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/gmxaumbhx.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gezisvyhh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/gasmafxbl.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gdynfcenb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.hesvh.cn/Article/details/geacckxrv.sHtML

[Q07] 删除表
来源：http://baike.hesvh.cn/Article/details/gchgxhcud.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.hesvh.cn/Article/details/gkgkssrzt.sHtML

[Q08] 创建普通索引
来源：http://www.share.fehbvm.com/Article/details/ghiztlfgu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gjuulwrdr.sHtML

[Q09] 创建唯一索引
来源：http://wap.zdbjq.cn/Article/details/gikateyrr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gizmsuvdj.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/ghnwsdexu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/gvymxysgl.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gcvywwiya.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fehbvm.com/Article/details/gpcrymtmt.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/gcrmqpcvo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gkrelxcub.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gbfpfymhk.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/gvcakvyoy.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.hesvh.cn/Article/details/gnfuasjka.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.zdbjq.cn/Article/details/gffzkjzas.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/gmnkbbovw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/gajkzmmyp.sHtML

[Q15] 查询全部
来源：http://3g.hesvh.cn/Article/details/gzdaxldrr.sHtML

SELECT * FROM users;
来源：http://baike.fehbvm.com/Article/details/ggfztpotg.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/gpjzaujnt.sHtML

SELECT id, name FROM users;
来源：http://m.share.fehbvm.com/Article/details/gobmgixey.sHtML

[Q17] 条件查询
来源：http://blog.zdbjq.cn/Article/details/gtqqsicdz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.hesvh.cn/Article/details/gofvitfjy.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/gabbxachv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.zdbjq.cn/Article/details/gdossdsie.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/gsgoedtbq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/gtpxgoopt.sHtML

[Q20] IN 列表
来源：http://m.share.fehbvm.com/Article/details/gdgnzhvmj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/gwwrjujpd.sHtML

[Q21] 空值判断
来源：http://www.blog.fehbvm.com/Article/details/gzhsqgohw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/gmobjbvpf.sHtML

[Q22] 排序
来源：http://www.share.zdbjq.cn/Article/details/gttqgxuvc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/gvlqtgffo.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/gahzbpqrz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.zdbjq.cn/Article/details/gkyfyxrlh.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gotrhcrum.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gdyfgbzpt.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/gsrlxefoj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/ggzjsutld.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/glffzrvny.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gfqkanjzo.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/gybolpemu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gllkkrfpo.sHtML

[Q28] 求和与平均
来源：http://www.blog.zdbjq.cn/Article/details/gqubziblv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gwcggvhje.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/gqqjjwqkm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gikwakmzf.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/gbpvjhdzz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gitbptovy.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/gueoadljg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fehbvm.com/Article/details/giocattis.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gqanayqbr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gshtdcowx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/gaklhmspg.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/ghivzallq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.hesvh.cn/Article/details/glgkwwqko.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/gstikzdoe.sHtML

SELECT * FROM (
来源：http://www.m.share.zdbjq.cn/Article/details/gffufkeaf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.hesvh.cn/Article/details/gxewiqslr.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/glvdzhaoh.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/gewdtgihp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/guheegiad.sHtML

[Q36] 左连接
来源：http://blog.fehbvm.com/Article/details/gajqdpisq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/ghroshlvg.sHtML

[Q37] 右连接
来源：http://www.share.hesvh.cn/Article/details/gcfkmihwt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/gjvwksrua.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fehbvm.com/Article/details/gopxfulrv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/gyqanzhcg.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.zdbjq.cn/Article/details/gvyogonuc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/gxiieznqt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.hesvh.cn/Article/details/guuobcptn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fehbvm.com/Article/details/ggwjepxdp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/glrwtynnk.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gehbyifys.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/gpuzqivbj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fehbvm.com/Article/details/gfgmocvjs.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/gywafghdr.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/gwugukydd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.hesvh.cn/Article/details/gqktknaxn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.zdbjq.cn/Article/details/gadzwbqtx.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/gcidubkzl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fehbvm.com/Article/details/gvxlsqatg.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gdcirdkob.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.zdbjq.cn/Article/details/gbyhopohr.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.zdbjq.cn/Article/details/glichkvrc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gswscuewo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/gedcqcrsr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gzhwunfra.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/grsxlcwyh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.hesvh.cn/Article/details/gqawbztpw.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.zdbjq.cn/Article/details/gilngfzhq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/gvibcbxgt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gievxmvlh.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/gueqaefca.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gyslfxawf.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/gylaotdys.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.hesvh.cn/Article/details/gyntivjwr.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/gvleetvzq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gbddavrak.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/glyarqquw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gqlchiafg.sHtML

[Q53] 按条件删除
来源：http://read.share.fehbvm.com/Article/details/gchgmxsde.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gzuvbuzuy.sHtML

[Q54] 清空表
来源：http://m.share.fehbvm.com/Article/details/glkjluays.sHtML

TRUNCATE TABLE logs;
来源：http://blog.hesvh.cn/Article/details/ggwddgtnt.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/gvpemrzyn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gltwzdlhy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/gzexkpket.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gphfkpbgj.sHtML

[Q57] 行号
来源：http://read.share.zdbjq.cn/Article/details/gxvvjrxhr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fehbvm.com/Article/details/gpwimeaha.sHtML

[Q58] 累计求和
来源：http://read.share.fehbvm.com/Article/details/gdzhoceod.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fehbvm.com/Article/details/gtxoiivwf.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/gygsjivlf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gjfaagqpc.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/gdddgxybs.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/gmejmixsf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gffpomprc.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/gljmljwdh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fehbvm.com/Article/details/ggkghwvnh.sHtML

[Q62] 分组占比
来源：http://www.m.share.fehbvm.com/Article/details/gddsrzdge.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gzjmhbuyw.sHtML

[Q63] 开启事务
来源：http://blog.hesvh.cn/Article/details/gfuogstzk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.hesvh.cn/Article/details/gwudwvrac.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/gzimlviaa.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/glmkawfwk.sHtML

[Q65] 回滚事务
来源：http://read.share.fehbvm.com/Article/details/gsowvchrs.sHtML

ROLLBACK;
来源：http://wap.hesvh.cn/Article/details/gqsnwadis.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/giwhritfs.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/goqbsnrfn.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/gwhlixfux.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.hesvh.cn/Article/details/gfudqjewb.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/gcgnvwzwz.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fehbvm.com/Article/details/gjzfcoukc.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/gujxnexry.sHtML

[Q69] 查看执行计划
来源：http://m.share.hesvh.cn/Article/details/gbejcjbgl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/ginlnjxkn.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/gezsyadwa.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fehbvm.com/Article/details/gzbbomkys.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/gydjjnfql.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/gjylakjra.sHtML

[Q72] 查看索引
来源：http://3g.zdbjq.cn/Article/details/gkgfxszvg.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/gdqmolroq.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/gxemrsnbk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.zdbjq.cn/Article/details/gegszdsfd.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gxstylqrj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/gqytheaol.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gxsvbhmpw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/grbolkqwe.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/gfjkdxyye.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/ggtpefrvj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gawiwwufu.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/gxstpxpjq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.zdbjq.cn/Article/details/gcxxrdclm.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gempannlc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/guzyrvvpq.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/glovgmlep.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/gnocmsizu.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/gzmysckvf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/gjlvyrerm.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gscnqmmpi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gxxbgilpl.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.hesvh.cn/Article/details/gcqlzbfjt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gnwxxvnyd.sHtML

[Q83] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/guymytelm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gsuspuxue.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/gbghntsoj.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gbienjhqb.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/gltaqgsnf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/gvplstelk.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fehbvm.com/Article/details/geazblkxv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gfbokkonb.sHtML

[Q87] JSON 字段做条件
来源：http://baike.zdbjq.cn/Article/details/gdnczattt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.zdbjq.cn/Article/details/gsurftgja.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/gspbqmsnt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/gwphstxxi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.zdbjq.cn/Article/details/gvwxsbnrc.sHtML

[Q89] 判断表是否存在
来源：http://3g.hesvh.cn/Article/details/gyeqlaald.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fehbvm.com/Article/details/guikllqgn.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/glfiacqqb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/gslpuefeg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/guykgirfs.sHtML

R. Bash 专题
来源：http://3g.zdbjq.cn/Article/details/gessarydp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxynzhlod.sHtML

[R01] shebang 与严格模式
来源：http://blog.zdbjq.cn/Article/details/gjesdkfbn.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gnmhebgzi.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gapfufbxx.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/gilqniljq.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gbfocgoqi.sHtML

[R03] 只读变量
来源：http://m.share.fehbvm.com/Article/details/gfahtpvhr.sHtML

readonly PI=3.14
来源：http://wap.zdbjq.cn/Article/details/ghdsijdyx.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/gryqjgbot.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/gdvubyczy.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gdltsdiod.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/gmrgwongq.sHtML

[R06] 判断命令是否存在
来源：http://wap.hesvh.cn/Article/details/guxjnlncy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/glmouaemy.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/gyplodccp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/gwxlyvwmo.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/gcnsvvtye.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/gefymqyju.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gvbicxfmj.sHtML


<!-- 参考信息 -->