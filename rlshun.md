代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2uzoiiquz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2yiryhvku.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2frbnnbgr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2qzvtxrxn.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2ynltovoq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2obksfcxw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2czvooopq.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2jnlmqend.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2trpebltr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2uwiriafw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2fbpbukwi.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2lbifpzgf.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2uddoetkc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ybdmvgzu.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2rorppxng.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lwnozvwg.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2twytuobj.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2ujyddzns.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2bvdpznuh.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2zyijhuax.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ktavifse.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bbnlcnal.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2nazrzqfd.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2kwxrtvjd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2gzyjnpcv.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2oewxdewi.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2wezhswbq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hscebjcd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2lppicszf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2mkqrnhwq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2lcpssmxu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2oeyahpmx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ywselvfn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2urnhdunc.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2xrnyjdua.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2bjaoavor.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2gjslzuql.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2imqcsycd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2bomzruas.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2cgppwbni.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2aykumhjn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2nyzjnyhp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2vqhmlvml.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2auoipdgh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2jbrobdek.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xzhjbvpy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ecpqjcoq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ngwgpfab.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2teqworrs.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2wojhqvyg.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2ljsqdvih.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2hofczrau.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2rbzezxga.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2wfhrfxcf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2xgwqlmpp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2xospyizc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hlwtdkhh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2ahwzweww.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2lwrdpfhx.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2nhgkoeyh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2ezshbgyy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2mpphbdtx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2zrqozida.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xkvmnwsu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2cvvyyvij.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2scplfftz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2iolpijhk.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2yschtzta.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2cppsubja.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mbaeyoun.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2eknbixhi.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2kwadahau.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2jzglqdol.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2evdcixwl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2oljwchew.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2owutuuey.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2rqcxjsed.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2rqzsywey.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2qsuyxtdm.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2juvfndrp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2hrfuphka.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rkpvuwvk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2lccqhgvc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wozgppei.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2kbngowfb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2bcukiwwv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2jbgofedq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2gnwtmbat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hyqnqdtc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2bsucuodt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mpmbxfey.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2uoqbbiot.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2twjseuhc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2kmvduirv.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2bmqabesu.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2wfonoben.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2wempbkdl.html

);
来源：http://www.52xcode.cn/Article/details/gt2dkryysdm.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2umqcokxu.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2nypoewnb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ilhkqhyd.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2aibhjdzd.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2zqbtuifs.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2zdnuzitk.html

);
来源：http://www.52xcode.cn/Article/details/gt2ylbdmjym.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2hskmmcnh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2hyxauhhv.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2vygpzaiz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2xpavabdi.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2ywgdqtwb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2bggelrlb.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2daogayok.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2boneezvo.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2xohrrbif.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2bjpfixut.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2yzwpzamt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2oentvjar.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2jbhxlgrn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2wtwlbhzd.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2fenmhplr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2vqqlrwiv.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2pgebixat.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2jdgzrjhs.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2qjmgcuti.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2pcvjvoik.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2hqigizbf.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2hndfupql.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2udgdepnj.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2gnwjldpg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2pzypemid.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2xdaxmlll.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2ieffkjlr.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kmhzxgza.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2wsbhpssb.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sbfwhjak.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2xrjfifrt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hqbqlttt.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2swdzwdrh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2ruuzrtjc.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2ywysfgjk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2mknoxgsx.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2kojeppkl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2mgnfwmyi.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2sdmvhqgh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2bwxgswho.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2udgvsxhh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2dunetiqb.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2itsuquat.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ikaeeskk.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2sdlaeaqj.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bwbszdis.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2becikakb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2ogpdxcur.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2kcopksga.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2saglchii.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2kyrfvvtk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jxjrbapb.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2plnworvl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gdqyuquo.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2khnxnttz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2olinsasx.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2frcvqeev.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2wyxjnlti.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2fohmwfeq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2kjvtweps.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2uehmtzzu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2zsrfelzm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2fkaxkhep.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2dcmbvlpk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2xviisykm.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2ewcproic.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2mrqdzdqj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2vdbrxzpb.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2pfxfnpaw.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2qrpouooo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2cdznfquo.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2wodlljdg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2zqvnqujl.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2cmdfekor.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2epscmxyd.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2qlcdexzt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2ygmodmen.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2gqiqizqb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2nbqglewl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ztkwgxkt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2cjctublm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2hvjmzzkd.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2rxhuxbee.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2svmsfjjf.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2vhoovpuf.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2skytddzj.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hrbzyriz.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2suqvjddd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2vxpzmokz.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2idkgthyl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2nducifor.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2xmcbdiji.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2eouezlum.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2agffhnnf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2lxlreqvm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2bweqbeil.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2iveulhzs.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2iyfxyqdf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2iveautnb.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qzfouujh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2jrzrjbjz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2wfvbupwm.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2gfrcbedd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2iyulgjwr.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2tcqonjtd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2jennccvb.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2gutpigyi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2ddsaipbu.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2noosnbsj.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2abuhqqsn.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2gidsicza.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ixrsqmav.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2mzbzrgsr.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2luagpvcy.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ejncppwu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2psqrldss.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2tkyvdyvs.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2eglasxux.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2sdpmxqyw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fxsfnisi.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ucovsdsu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vxudnkmb.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2ejvfybrn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tzzoeddl.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2llsoyprx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2ilodrfbi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jicnynje.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2uovimrmf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xptyzgnq.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2mjrgwzqq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2lhzwoamr.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2xmumdlhw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2kbutdgwi.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2eyoszxlb.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2pulrguut.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2awctifrk.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2rzlqrwvv.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2wdosygjx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2iueurpfq.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2usxmbrdl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2jmgcqycq.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2iuhzscms.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2sjsxkwiu.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2frcbpfkr.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2fzjllgna.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2efqdfyxa.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2nzyzymda.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2vhlvurvg.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2xvytbtcl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2fotbjfye.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2vamtbveq.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2suhbblgl.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2tfxwpydi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2paonjmgk.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2idsrnlgr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2ncowabmg.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2rbkabyrw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rtwhtyly.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2nhvokfun.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2otblhurq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2mmgwrxut.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2tjswwjnx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2lfhxbjdi.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2iwsryadx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2zcbvopnv.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2qxhisxka.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2gfyxiqfm.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2eaoshhxt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wrjivrlx.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2oxcvaeww.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gtvbghpo.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2lzizgehd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jglkaccs.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2scsvdguv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2myqnquow.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2gwtxwese.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yzuptorl.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2stigxhbs.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2rlklcwyu.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2ezxzwhzo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2gousbipg.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2gipaypxn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2widrifjg.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2tmxqiclm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2zniijlfa.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vtpvjlbc.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2iesbzcoo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2mrkaujqw.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2lrakbqbd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2poqjgzhk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gvxcbchs.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2xpykfzyc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cxfyfyrh.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2tciitgxo.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2dhdnskhe.html


<!-- 参考信息 -->