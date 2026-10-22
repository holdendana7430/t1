代发 wailian999

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ueqwzmmv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2jfrgwjes.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2cwhkjmcz.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2xciimnhy.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2mkpgscer.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2evpjnwlp.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2yfxgmjoc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jcusxxmp.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2pipmhtjm.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2iwtvccgb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ncnrouuj.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2syutalfo.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2crkymtgi.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2eptusqgt.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2tsqarsia.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2vfpltzyt.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2jmrojrsm.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2htetvztb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2yqvxgmfs.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2dahrczkb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2gvxrdgqz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2occceodk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2cxzfrnqi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2kprmgfkr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2tirjluph.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2bsobaegu.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bhydqlmp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2rzeyieqo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2xwcyxpew.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2flyrqbbi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bihopfoc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2wkmytkcv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2kroeghpg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2witnpprd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2yoqinnwc.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2ynugafyl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2faxzwmmd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2sscgnzqb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2hgvhjhll.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2neybtjux.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2zzinjrud.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2mfemsica.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2ukspyhpj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ccbkmpfu.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2cmzefwxu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2tiynccit.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2jccortck.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2wdekjheb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2rigbfocj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2zvtxeovj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2oqenydoy.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2bzjhhcdd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2cuxgfkau.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2ltlnsjgw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2mwuvytlw.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2rhhbpyws.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2akttjzke.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2jyzfhcft.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2uzrnovre.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2ybyjycln.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2rpdmnxqs.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2muzgjdym.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2ltawmovq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2dsyattaq.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2mlikqdkt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dwolcevg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2gdrhrkih.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nymkcfah.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2gyhnqxgg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2gykuzubf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2bfiupqbu.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2aozfzwjo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2aakuxcrd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2oilwutgp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2unxweefg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2flvynaem.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2wqlaspgr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2abgevkxq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2vteefrxu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2vtdivmty.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hpoohree.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2amofhvfo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2baiayjnh.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2xjfsshwt.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2piswdzsl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ortkorpd.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2oyvshfld.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2vpyorngr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2iallzerg.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ginhsaee.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2lhxirjux.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2muvekheh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2gqtizzgn.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2jtmqkajd.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2bceuunws.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2cfyfkuoy.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2klxjfpaw.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2lurplrpf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2lthpwskm.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2vsozyzas.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2qifyydgw.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2iwkqgtaa.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2ivsqgtaz.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2ojzkrirv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2dminhpji.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2kcpmzfpf.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2owicbqmo.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2qixdnkwl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2qjyfqfkj.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2ovygduwj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ihpfgrbt.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2xcjuracw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2bfahbqnh.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2whfljvvx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2uuufdljp.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2qubpemzr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2hrmgjhym.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2waurhoiy.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2cqgeeezi.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2hmqqyltv.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2wjszmqwi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2wofypext.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2twrmmxsf.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2uabmjatj.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cqjwpwvv.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2pwmgcuyy.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ncjpurql.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2tnwmzydm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ilwllzzg.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2iihsidbe.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2blsmicqg.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2hhxrktru.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2yvaveewt.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2acbwnopj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lnxebndb.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2igymfdqk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2uxigkkbh.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2wogdfmab.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2ythtwafg.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2burrminc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2bimlsrcp.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ngvigbqs.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uomwunbq.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2kfhqkcrh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2olhzstko.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2dztzgsmi.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kvwilzni.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2zzbfykyv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uzbaalhz.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2qesbxikc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pbvwelxr.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2lxwsywff.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2besjpjht.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2rivbscgy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2jtonxzyc.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2ubsikspj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2fhhhhhhz.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ovapjfhc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ktsxnwkl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2qippelap.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2uhhigozk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2rkiujblj.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2kthrsgeo.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2drfxhxbr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2rapwjwta.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2abbmejbq.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2bipvwdbe.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2mlgubbrd.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2mauifjrk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ipxofzcq.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2egpkayly.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2dnpwzrgp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2tswgxllf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2jllrcwpr.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2gwciicop.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2yjxyhhvu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2letntuew.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2izphtabu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2zzdqwhcn.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2wiqajelo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2inlrnbdp.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2vvvmrdpm.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2oibdlppy.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2fczssvki.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2zemrkjtm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2vbwmaqhk.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2yvivyrgt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2ncpizboq.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2gtsrveic.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2wygubiyt.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2kisfaeqy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ycwsjthp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2kojigryi.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2naicbasx.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2pbwoydsb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2zoaakrro.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2iijudkzu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2riqtwtnj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2xsihibbd.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2zerxldwh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2qbvkniyf.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2yurljfat.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2hadejzqg.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2kinqczmy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zalsyzew.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2sebbnqvc.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ruubrfad.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2apophisy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2jczolqxm.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2wcdemrps.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2bubeijez.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2jkawgrwz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2zbbqjyhe.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2dcudjfyr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2bhmlhzob.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2ajmztgbl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vulpzznn.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2ogllotkt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hkupanpp.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2bhhounin.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2iwzqwexy.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2ifsyxxgr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2nbbfhuts.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gyfjrzqj.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2tqdoypry.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mnaanqjd.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2ffgvrhiw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2paenfhpy.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2ndfcyoho.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2widopimb.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2hnvuyvur.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2vjtufzim.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2qivxeglr.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2hadparmm.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2faguflyn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2enkhxvqd.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2dqsmxlan.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2hikgyyla.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2srgsdcxo.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2viqhujsa.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2aiergebs.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2inztfqym.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2loudsiwt.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2ilqgging.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2qiiwbpqp.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2yxobviwh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2dvgzjywm.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2ixwurohw.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tzhcowjp.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2vzyfholh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2qnhipnqz.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2itouggsz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2cskwgijw.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2dxffpecm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dasqnagi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2ooenwzfg.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2kjremklp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2tlbnwlwh.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2uctmbbeo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2wsykyqaz.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2bqbeuece.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2teyjfvtb.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2mxcrzcsv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2ougpdbsl.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2wqcfdzpc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2taqkcfxg.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2pieqftrn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yvgzzlod.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2dakbvalj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oqvesmjv.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2fjlqafhk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ggrdexzv.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2innhbbtt.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bedadmzh.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2qgsxougy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2bbqrkenh.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2iwbkrzzj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2spfwpzgy.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2jpmrimpo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2nmjkdmbc.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2ahacpopg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2wqatmksm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ilcnbgsl.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2fiztoiyz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2fnrtxpdx.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2sekvjwfn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2qglhqboc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mcvswgep.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2wciglqmz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rvyorick.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2rgjtccrz.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2ngnigbij.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2tnnyrgne.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2ciflkgco.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2cvhjgzae.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2aalsxdbj.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2lootfbij.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2dsemkjjj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2auxbvrfr.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2opcrxtad.html


<!-- 参考信息 -->