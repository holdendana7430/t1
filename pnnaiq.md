代发 wailian999

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2wsstberb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2lclnzblt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2phxiawtu.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2ghaasicl.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2usulpitv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2newqkxoa.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2fybfujkp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lnwtpshv.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2wfanxkem.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2rvppjatx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2hdmvwczp.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2bixakylb.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2sgesjpqt.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2wqevkpcx.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2vmtshcxg.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ojqzrwzu.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ckvtpnqe.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2gkzlsbmk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2njcaozzc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hnsimkjr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2kqjiijkf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2tegyvobl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2szxrmzfm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2bcmsfhrp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uwcwmawb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2qhkhywaf.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2onouekxm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2scrziwkk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2pfgsbpru.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2pcoktxyo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2atiuqacm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2aacswpgv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2iduixdnz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2wvsquxzm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2hkqlybbc.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2hdfhgnsz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2gmuvkkfp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2dxqxakki.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2oxpgutqx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ucyhffkf.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2kmofizay.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2jucdwzoo.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2xubfceid.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2smtytfrm.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2ersyhmem.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2zuykvakx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2zfzkzejo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2jofemwpq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ilcvaiin.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2wyqatvdb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2awuhleft.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2eytzbggb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2ocznwmlw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2yldzitar.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2ajmwiaan.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2gouomish.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2kytcdftc.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2egkpdhma.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2koqiyphi.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2zgihrlxi.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2czxsveas.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ogyjincv.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2raxshiig.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2ipichjcx.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2rludddsz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2njujprju.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2gksulznn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2srptsoch.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2bxxpzyml.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2fjrrvmey.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2ldqikmnr.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2cxetbbkf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2xmvvklsj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2yfzjypyu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2owwabazg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2eeayajty.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2qcwvymxp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2pktpbkmm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2vdywjbdb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2lqxqhbwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2umfavpja.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2zmswxmgs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xddtkiel.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2rwbzafjk.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2twrrlniw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2hfzjswbt.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2pxvfaklo.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2rwxvrous.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2gsanpiqw.html

);
来源：http://www.52xcode.cn/Article/details/gt2frukuukh.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2amdwuozh.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2kpzgowmb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2qmfcfyoc.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2moqipgfr.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2dvwbdpbd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2lcoiafvb.html

);
来源：http://www.52xcode.cn/Article/details/gt2gjmheolt.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2uplnojik.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ezqmhjwt.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2aeokhvhd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ehmgoocz.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2pezlidku.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2eibdnart.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2ntkqngql.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2nqxmdznq.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2xpedcnht.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yaxzdjmr.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2qjeokklr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2nmlkpwut.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2xxkfmwim.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2aanevnrg.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2pfsvglwc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2yvjabyvc.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2hskbwlfv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2zzytzmjv.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2xutuwikx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2gtecwkfx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2sbnmholg.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2hwmoycwf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2cuoxnjxm.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2dhvuvvkd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2buwswznb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2kiqlnbzy.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2udrpgbvb.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xncmcqdu.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2gfuttkzx.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mglzckow.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2vtgxoaxr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bdcfgatk.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2zgnpoglh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2lauaaacq.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2vgkpruqf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2yjbwlhfa.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2uwubxaio.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2imgugzhd.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2jgpatzkc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2tlbxrvix.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2npullikc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2kmszxnep.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2pjrgnryt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2txpudzni.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2gevobddy.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ktirawpe.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2nxhwupqg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2mhcggxls.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2qxqdgptc.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cikssyrj.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2wmeaymob.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xptsvjuh.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2thjmayob.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qdogiuig.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2bszdrylu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ieyhnitb.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2mwnogoml.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2vgmtucih.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2ksveeauu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zboxcqqp.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ntbzqcfw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2rcqlbjkl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2zsmjfqje.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2seqojhsk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2blzogcer.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2brqiifkx.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2ojsemgas.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2cfsftczt.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wrjllvsv.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2rcilcrxo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2jvokuvob.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2gzbumjds.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2uylccflh.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2kyoamxun.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2mcintekw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2ebjxoqhs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2cbugccih.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2juwzwtee.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2yvnkrawy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2oqvdkjjt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2bxztpppa.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2iimngtox.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2jcovcjbj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2yxglqkrd.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2nkngjujl.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2uijplcty.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xvnwjcjv.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2dztbfrfu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2exosnudz.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2ggmtpcsu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2gzccqsrz.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2rowyjmhv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2gvvrqkov.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2fnzcxcws.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2qxloumgn.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2fhiqkoho.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2bamdnmjm.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2fgbvuvcu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2xiufojxv.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2dnpghdzc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2ljmdgmdt.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2dtsxyazl.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2hbrjjdcu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ukcpauhn.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2qygtvhtl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2tvtotvwf.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2smoccioe.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2ahsijdng.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2vhvkinih.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2voffmfud.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2mcjsaepc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ebjsobby.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2kpcpkqyu.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2swdbsysu.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2kwylvciu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2glzhjryv.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2zrhtjcfo.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2yzkuivgy.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2tddmevjd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cbqxwyvw.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2fkzdskkj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2efshpnjt.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2ptlebnuq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tzcdqndq.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2nzfzskud.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2rvuwyeak.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ymaeovcu.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2tezchwih.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2onzjsgzn.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2rhnkvmte.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ywoojwlg.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2tsfxetln.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2hcbrhusi.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2fndajflv.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2insgcavf.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2drkhcpfa.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2mxfzpaqs.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2nmfjeoag.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2kusxftxd.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2qvripdrl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2ofcukhwh.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2ajrweuwc.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2bhowpsgc.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2zatpvgsi.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2pjrgkkvy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2sbivbzyu.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2mcynoamn.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2sgacgxty.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2tzhhskly.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2qhtelbcx.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2bguvrhfq.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ydyruqzi.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2qrumvihb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2qxpekuqs.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2plpgggzj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2pcutnsbe.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qbfeoevy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qrmrfkwy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2uzgtpgbd.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2jcpwhwle.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2ymfbttag.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2nzweffed.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2hrggtnlc.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2eyvohijp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2vbrrvtne.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2dqqxkqeg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2bkmfiqmf.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2wrcdegyy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kaudmyjw.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2efxlcbwq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lhqpkecy.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2xahehypn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ynfrscve.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rmtdmqqb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tebrnxum.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2gmmusghq.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lbvotwfv.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2qdwzajbz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2lewrykvg.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2tkaktxce.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2lntyslng.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2dvivdygy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2hrmeubxw.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2hncrkjxq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2yaoqhvey.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2beqfrajf.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2dfmpxwia.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2mjrktsva.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2pgprcsnp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ludxxygt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hzqbyrrs.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ccafsbpo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gtrjnmvi.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2rlwrsufo.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2ajkcphjn.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2cjlrsbrs.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2llcebqrb.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2smkzlfkm.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2disnhmbb.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2osmhajrn.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2tgvdlhmi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2mbvcgjby.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2mbjqkpet.html


<!-- 参考信息 -->