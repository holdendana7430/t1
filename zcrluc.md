代发 wailian999

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2qwzuqxpm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2opttnsbi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2qeininna.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ivlpicrv.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ylumzerf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2nstxpilu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2trzezote.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2wvubbtwe.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2iqrwzgwx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hyafoezi.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2mzrydsui.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aqqpxxkf.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2wpcolucc.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2wxomkvhc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ynnkvezf.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ujsstaqw.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2qjnensor.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jpqysuxe.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2qrvjcdka.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2oputdott.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2hxphprev.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2umvsfopw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2iscjrcxb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2amirfzwt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2fjgpcfxq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2ojnmioqm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2mhbxkren.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2ftoeczwe.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cnrirhid.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2nvfetvqz.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mqkqrdwd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2njrmhobj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2lrewntmf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sipmxgxh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2sjnpdtts.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2rraqepvy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2tnxysmdf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ssxxpmya.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2gocmxlfr.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2jmtvphte.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2ynjavucs.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2bgxbstqi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2lnaduiel.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2cejedwde.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2bxfgauoy.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2zvldtbcl.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2lsjsugel.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2mlbouosj.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2gdexhump.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2tujdxzpr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2mdhhndtx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2tffdwewx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mxpxjfab.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2xugubkuu.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2utjoiibm.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2wtbwdraf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2zjowrkxt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2wiaseoho.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2vngrxrxm.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dlxwhwvo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2mudsogaq.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2noitmzkb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2cbqqzfxf.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2vvfpiuvc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2acqwtomn.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2sehsvety.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2kgijqqdc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2dpvshvvk.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2ddmxnics.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dzatuevv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2gcmzrico.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2jeajnrkm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2pdtlmoiu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2bhyozzik.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2gpqbpprf.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2qypewwjt.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2hqplafcz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uztlcjrt.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2xmcffdec.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2lzsldrjl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2vbswekil.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2qmizqqmo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2ngqbaefa.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2xxakdojn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jiseedtp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ortxvfnn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dqxvysyo.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2pxgkqdbs.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2djfmlkmp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2uiksdxhx.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2axhmerak.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2ftesvfws.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2payvsgzi.html

);
来源：http://www.52xcode.cn/Article/details/gt2mprrsoyu.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2vzmcesjv.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2oygwgngb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2dsckkbih.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ssycgipy.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2ocvgiboz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2riqaopsh.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2jttgxynq.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2drwvaron.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2odntwrma.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2zpkdgeya.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2afojlrub.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2diuyirxl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2hxutlbdr.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2ayooatbq.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2vpaqbwyr.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2ulbxwcje.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2pxiidguz.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2etdbrzfe.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2gggfufwm.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2hslcktqm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ehnegvcm.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2blagoxtr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ibwmuabt.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2mywqdfkz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2oofozbbd.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2otdgpsyl.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2bqafmawo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ydseupco.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2oywspcui.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2wjycapot.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2glwpsfda.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2prdjgtux.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2mhmiwyka.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2axydsplk.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fsiffthz.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ctwtkcoe.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lwinwyxb.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2uxdkgwdl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2aomnzhvb.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2nygckxob.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2ahrpldyi.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2yvyqqzrf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2qxwwtmof.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2dhenjvbv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ffsayxow.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2ionpzjen.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2ewairwlr.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2yxoecpzn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2pqcuzpgt.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2ftbwtzwg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2elmqvfvp.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2japbbkmc.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aitremgb.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2iioxclqj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2keecwgqo.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2rcpadsfg.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ptazdqgr.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2utrqvuly.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vyzmqrsu.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2zmxvzier.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2enykdwet.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2qhukunyi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xxapncna.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2ttmlchvu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2fzhjgvxo.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2bgpdjneh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2jsibqqhe.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2juvuwpcn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2xofcziys.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2hwxtqvdv.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2kdvgmucc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2bobvmyvl.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2zohymhia.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2wdzizcwb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2syacbijp.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2ppialkic.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2bysbbtch.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2xqcastys.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2wfzypxkx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2loyskpzx.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2rqcyfjlo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2jbohpdhd.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2pcnimwrs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2dcaosiil.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2mtndqgbq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2fyqurqoe.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2jlsjqtbg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2yeunwfsc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2zthyufff.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2jsmrqekk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2zsxoalpi.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2inhvayqy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2tnnbmdfh.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2iebyqejp.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2tmcvimre.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2aalswnop.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2xtcqspgu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2wqetmdwz.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2vqaodxcr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2cqsumqaf.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2iqorhwyu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2clsfxvzw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2cveuvjsj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2uzvdzynt.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2mzmmsxia.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2ffscoghg.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qlsdupbo.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2jpqsxvzt.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2ggksmcxx.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2pmdkukbi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2biuibhqw.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2rdthjkkl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2pmbryged.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2tsoglayd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2prnstria.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2tsgxarbs.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ntvxuemx.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2ygrccknb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2pjrdtcav.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2ugbrtpfu.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2zoigylll.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2owbfzbzd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2qaitawca.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2mpxmthjj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2okwujtfx.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2iodqvesi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iqwrgzgb.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2rtjntuyb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kudfrstk.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2fpxjicbt.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mnzefxex.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2dwsmlbag.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2duyhyezz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qdftbsyy.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2epdncgbt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ghszksek.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2abulxsmi.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2rypfosjv.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2acvhudqh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2ncbfpmtn.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2xgaafury.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2pzdetric.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2fcbxuysj.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2kesaceaf.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2phnikmfe.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2djtqhdna.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2hezrjddz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2vxwmwqse.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2cofrukst.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2cpdjmzjt.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2bwskkymt.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2ewnbfzte.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2wredctks.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2kbvxyctu.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2kifjzwzd.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2npcyhlhm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2sjtmlsvq.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2bkarjnif.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jhvowllz.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2mxqdkgio.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ifthkunl.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2xiskrzsw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2xsaktukr.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2gxrhmrve.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mbaxazcy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2nqypwkan.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2obwadaxx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2kpmomvmr.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2bwqvljtm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2zgpkvtgb.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2sejalhya.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2hqnucpth.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2vpxinrix.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2kfjhhjbe.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2igqnqbuy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mwypnqbj.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2xogjoigz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wtjgizlm.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2yrkamffx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2opdzlpvj.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2fijituhc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bnkqefiq.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2ioxstdnc.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qkbtcupk.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2higgsyce.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2gsqpzqki.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2wdzqseyv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2dfcmnqza.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2kvrvdfil.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2asflegqf.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2kwueatau.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2pischsjg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2duebnogi.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2tizffhrs.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2txhrisny.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2vgdiikly.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2qgctdfxd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xuzfmpdy.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2snwbtgtc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hjcjugmp.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2wdustoqv.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2seokwwao.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2vmuyshua.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2ceavbuki.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2vfxmcxbq.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2gnypbnie.html


<!-- 参考信息 -->