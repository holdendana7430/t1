代发 wailian999

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3xsypiqfu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3klxrgpug.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3iyjjptvk.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3fdgkviln.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3hbrnjqrx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cqyswgpz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3fcqhklqc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ngxfgfdk.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3wubuadza.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3hnfomimn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3ytfxamhr.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3deypulmh.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3nevbnhlm.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ijruhqyg.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3tzbvenpn.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ntfyqcre.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3lmvmjazy.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3fugislfi.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3cxnrgglg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3jptopynl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3llxijccq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3earrjrrh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3jyuabrqn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3vkuvajpn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3vbtmfqkt.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3qqgwneys.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fwwirtap.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3jxfijdsr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3ygsckqoo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yoweuteh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3zymhpvot.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3gqsonewa.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3ptuauyuq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3hgivbdtk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3yqxvuboj.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3mkxzqssv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3mflxjfcc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wxxppxyw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3luzwrhzd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ckrxjdmr.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3jawycovd.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3tyybkmuq.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3pgtdbixs.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ohuzhzth.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3zvkblbgz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3oxjtzoda.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3aivogpzo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3iixajfev.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3rzmatkmw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3olpnuofe.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3uamurlnc.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3vaysrvrb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3bhyuodkk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3bfvoizzn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3exwiwxbk.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3gvchxwcp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3lplgauop.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ohkidhpz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dstsqxyu.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3wrjkgohx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3uofmumpf.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3unvjsfzo.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3bsdqphbz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3cwfhawit.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3ielzryma.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jvlazemx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3wiunxsil.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yarmtesf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3mdncleov.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3yrpbtdss.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3zpginkey.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3lytsmsok.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3fhaioogv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3ltacpfyg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3creghjbh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3tbkzfkwq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3ylesxeaa.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3jbpiotym.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3qcnjhhca.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3doachbrc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hsqiipmp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3lowmrxdl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hnfwnhfx.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3mduedcuz.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3sywkgpbg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ubfdpaup.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3qhqwkwwz.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3qlabqtbz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3tamhsdsy.html

);
来源：http://www.52xcode.cn/Article/details/gt3ocslwwnl.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3cohvmcqb.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3lcijxqwh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3amsvtpbi.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3yksgdmjy.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3ozmekzsf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3qengtqyn.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3isfygupf.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3aocbsoac.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ryhwapkd.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3mqzfkvwp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3ibmlfiyx.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3wdpwawsf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3kopijcli.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3bmhuofmi.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3oregzzfm.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3apxqxptq.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3ftxakyiw.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3akpzaibs.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3gdbpdhco.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3dvbsafxb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3lryoziyg.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3sxkebhih.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3efydxmrw.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3rdkktbny.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3btehkbcg.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3gxgssqmd.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3awwhpctc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3ubveciwv.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3hglgivef.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3symjsrxv.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3bdkiwoub.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3zmlxqqut.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3mckhhhen.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3mlmzwbgw.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xggytefl.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3tllueuro.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mgjkxdfn.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3rjrsrljw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3tvlyiiho.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3dcqmjtkh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3krwdhize.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3gzbfyxbu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3myxbpdhw.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3wmjlsats.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3wqumpguw.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3vsuwkocl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3liymtqoe.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3mhisasvb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3pftrkxic.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3wsnlmfre.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3gnpbuupc.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3zfsigedn.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3szcwityv.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3hvqdsnlv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3sdpvimdf.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3lbqbbopl.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3abhphinp.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3liteebob.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ebhfdhph.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3jcbqzwmc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bgdlbsap.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3lxyfyync.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yvcejlle.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3rmizejuq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3cmlqorkj.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ehfcjwcp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3pbklxruj.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cdrwomls.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3vqtxkqbk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3hemncuuc.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3xyuhlidw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3wvsicdti.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3jdovbwxo.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3zintzsfq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3cxeqftig.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3eybcwzsp.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3cbxymtor.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3cwrhsogp.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3uctllehl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3elrqstwa.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3zmqrwrsd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3hotzytxv.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3ostijkms.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3ljgylpdp.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3izsphufs.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3fodlnmwh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3onspmimb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3ijtjecsj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3jrgmpbea.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3tbcuvqlj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3wycbxvmw.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3eafuyetq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3zipozdfx.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wetntinc.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3kknmfphe.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3eiqqrhlt.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3qjcszpgi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3mmceiluq.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3swezizqk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3opebjvwm.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3petcsqjx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3aojpvolx.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3ubpyinht.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3fjsbmxaa.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3oemknaye.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3knhmoxua.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3nsvatxed.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3ozdbvoyf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3dwhfkleb.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3bzkqqtwu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vgkqotke.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3dedolacv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3hfyeorhc.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3rkjhytlo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3szftiewr.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3cohqxuuy.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3trhuxuvt.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3khjtpfgx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3agxkyzmk.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3avxghicd.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3tycvzfav.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3cpzatkqf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3gscsrybc.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3vlefyxqv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ihtrhuex.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3zhtkaydv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3trcohnik.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3vnjzvaze.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ulzzqvza.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3hiwfjfom.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nltbljsb.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3mogwoimb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3xumnpyfy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rywvymcy.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3odjansuc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gpevlgvh.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3dyoszaoz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3xiafuuwe.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3hnrkmrrb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3tcikzxpw.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3dgvtfjaw.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3zavrpkrk.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3iysmnrml.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3ylgtqryo.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3smososyw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3jhxfylal.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3tvofkwdl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3renxeruj.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3kollzbqx.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3czzufpop.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3lgwddpjk.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3abeismgr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3jamghthu.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3okvlzolz.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3aczuynwb.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3nhjjobmb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3edlvqdhl.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3aerpepcn.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bonwjwan.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3goshnymp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3kxqdcfiz.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3idwlvvyr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3qmxvypfm.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xfcylyht.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xrezhhzr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3yyybxvjz.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3zaipkoot.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3vbqmixlm.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3uhxdxacy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3xcashykz.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3pcsdkywy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3osgmwyjp.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3iiqbvuwz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3gsmnlwjj.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3nlxilpok.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lggzadmb.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3pbksrfqb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qoeqlhzi.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3jrhtzzwa.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jprpsjzl.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3skrqlsdg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zofmdfpo.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3djhanobb.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qilwlewv.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3dfxbmhcf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3cencgeyk.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3zyuzdhmy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3xpdxmomz.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3ephspqrl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3bqctjerb.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3fylfdsjh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3gbungjsq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3etnugajm.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3acgxgofy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3luzsumhd.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3ferxtdbe.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3wptvupvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zcvoxmtq.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3wmicgjhk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lhdceres.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3ghuwckzc.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3klhvyiqj.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3fhgvajsb.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3abypfckf.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3kwvcynse.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3irjstiwr.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3sjzxkxdl.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3ccznbwqr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3aearwkbe.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3kfstxudo.html


<!-- 参考信息 -->