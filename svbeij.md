代发 wailian999

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2rgopsjlu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2mucmnnom.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2nawmxemt.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2yogtliya.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2jwoomvwg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kbvcugye.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2sqfvipjn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zrculawb.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2muaubsbf.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2exoflqtk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2rrlurpjd.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2pkxsfdcg.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2pquzssbj.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2aawcoyhk.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2djuoigpf.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2thzwdgeb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2shffcnpc.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2temdpbdn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2vbymtosj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2iclmqjux.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2qwapqycx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2yqabsvak.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2mbtdizhi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2ajfhsjzj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2ipynfisp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2rcjjnvhf.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kcktbisw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2tkdzbymz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2tyeeikhc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2pcxoaict.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2odxxqaem.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dasyjmnx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2khrwlast.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2hipernkc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2jtmmwczf.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2vpdbnokr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2dtdvvlxx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2bxgxrnyo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2htjhpnhi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2oihdnbwk.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2uyeozifh.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2vsooeeje.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2lmidgfrn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2tijaftvc.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2psvqwrop.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2ivansqyq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2iyyhveva.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2zcgozcst.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2utanhspy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2xuteqgwq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2wzcodihs.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2tipqxsdl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2gzrlkwtg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2oeesywrz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2dvshotig.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ryjkvwlm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2dxmjyjuh.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2mzueajix.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2puhwmaeu.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2ciuaifeb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2ebbuyuzr.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2regoljxs.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2flrywgqn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2xtdaybwg.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2qxlahgqo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jiymibrh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2alhriyxx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2msjuideh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2lszbobfg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2khxbhact.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2yyhotcat.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2wqvbkheh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2ibtgqhyu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2ajwqkaec.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2kbzretxf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2zmlnwarq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2iwmaxrwo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2iwhhwknp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2zullcpcg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2hckzaeym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kzlxbrsz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ossmkypc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fnzklxnk.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2xljicaon.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2xsggphvy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2clkfkxtu.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2evuclgxq.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2qxcwaifa.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2rsaualqk.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2dxgwpdtf.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2nizhklws.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2yitucilf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2outcbzla.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2hzttvtmy.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2kzqtmjim.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2uoywbyvb.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2aaazpdcs.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2zpkojswx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ulcyyzkt.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2pvshpzkh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2boodgoge.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2fzhgqesn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2xjdhllgr.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2dxgwtwnd.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2trzxsfqg.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2tdgnusse.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kmlascjn.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2obhfywxq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2eurrfbie.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2tykrfexl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2pqtsabpi.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2pvgbzakj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xianmhdt.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2dzbphmhe.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2epwzatub.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2dpoajmuu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2etmjeyjq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2zoqlgzff.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2etkfjiqf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2glnqznkp.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2fppllmkf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2hxtmrwsx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2srmlhvem.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2pzrmfedv.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gcarqfof.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2cbgfqrgy.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2utcbxbdv.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2nykrzrsg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2sepeuvlp.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2fqqpbfkm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2wgzfijcm.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2hdjytopf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2wvllrokl.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2uyguvkxe.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2covkmnbo.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2dqpvosua.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2bajvmrlq.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2elngktjg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2dyzbtrhl.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2onrmwcwp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2axvaqlgv.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2wdiprhsc.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fssfinlc.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2dsrcndki.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2rcwbgakr.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2cbvhjfeq.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2luxchghc.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2fefknkfz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mylugkaf.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2qkrkqrwk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2didnlsty.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2renlulxl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yvflieaz.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2ftgqmkgt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2dtgaoowx.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2mkbhqcqr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wzppchjx.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2nwhevnys.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nxqumzsl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2yphctuwi.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2yhkdnoxs.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2eakogydn.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2aklgmivb.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2tiuqcvqx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2tzaatfwq.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2hhzenmat.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2upytliqz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2sqkejzqq.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2zbocoxep.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2zorvejlt.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2pehbbzsd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2qlmibsee.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2wqfymaak.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2nmlxonfh.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2glgvycaq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2zlvpimty.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2tqshqcwq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2zvgrnjux.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2afpesxns.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2gmyvaugc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2qprbfjva.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ryfmesxa.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2djxjuwgq.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2fwsdiwmu.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2mtturqfy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2wknlghxy.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2ojsrrzdd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2ksvmtikz.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2wvjukvrp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2zvvqvxmv.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2osboalty.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2iucjtpfa.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2iezfprse.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2exotxtvw.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2qgqhkdyq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2okezgvuy.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2coarfarw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2lhdawcac.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2rszkmtrs.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2lydvxlwh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2rcytbucv.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2glxjudcj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ftgjtkjz.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2ogjqzmtp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2objkgptg.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2votzvzaj.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2sgsxyqtj.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2castsyyy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2skinbuhh.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2zmpvonxa.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2yqkponda.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2dygujuix.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2kadilqny.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2wningtsy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2fjptarhz.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2sukwycey.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ruowaybx.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2hidjbgmm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2swtlhrry.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2tsjksroh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fyctgzpi.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2cueucrkg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2jyrdthnr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ccuxjgms.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2ujwbelss.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zthimmvw.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2rgepezrj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2zvxjgvct.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2dctvydpi.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2elxbngmp.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2iciwurnd.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2fqjqqzrf.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2xjcvepom.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2qmtmiemt.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2cpyvkkup.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2ccjtuwtt.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2svrsvxfu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2qxwtasxx.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2luietkvo.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2wfnqacat.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2pouoxuqu.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2yjnfdvqf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2cyxuxgse.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2kdujftdr.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2sleffkma.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ovoomrdu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2iibxypah.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2finrfbzn.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2azligvlu.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2doleuwpq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2incfsbfi.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2scrqvvod.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2ernxyhmm.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ckovgski.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fiwdrmco.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2oabzaozp.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2tyfgujsw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2kqmtixcv.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2snmcyefa.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2bnfkqsyt.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2supfttnu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2vikqrnug.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2nsqglgir.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2waxaeksn.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2weecsbtz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xgvbhtfs.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2fuulhhfu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lmqidwmp.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2izldnpvm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xrfnbllc.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2iincippa.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vonsrdil.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2pxdedxpq.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tfyitzcl.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2qoxkzasx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2pvnhkkjl.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2obtqkuan.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2bwpecshg.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2welacued.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2kooentfd.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2udryrkqs.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2qeghulyu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fweghsyf.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2myrcfefe.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2ozgifvjv.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2syksunwc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2sjpboqoe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2izkyaczk.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2kqhobown.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vlwzysnu.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ojaarfkv.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2kgpnciaf.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2igrebyho.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2qzbbvano.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2cvwyvgfp.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2gwqmachq.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2jclvjwlh.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2smrgxrtx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2twerdcml.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2tgzfvjga.html


<!-- 参考信息 -->