代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3romfstnn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3kfgjvwxo.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3azxkhons.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3bsshnqhs.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3fdtitqsu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3lzjmevhw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3aqzdbmzt.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3vwwrizpr.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3uqvtdwfd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3qgfxbwda.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3owghscdg.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3hyiogkdd.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3vnacoogp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3clzupokk.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3hggapnma.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uhryevxg.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3vntsqbtg.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3vauvrdlh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3cfmorkzz.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ddvnvgls.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3tcjaewbw.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3azggakbd.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3admuqqdq.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3xyrnpukk.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3zynrxiub.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3wuguihnw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3tovekrna.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3ykluohla.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3iggwjsxt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3xzcmujrs.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xymtoqrs.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3iuyltjvh.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3oghkfloh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3beegphxc.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3arjjepsd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3rxjqsiri.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3pbqulazy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3iosdpedt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3xbwbqhgg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3hoktgyvd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3qjkupqlt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3hxnzdqfd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3xekuufxp.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3vvcegubm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3tnljkshh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3pmecxtzc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ujxeawln.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3fzffgkln.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3rrcaqale.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3pzeakihl.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3wfxkruue.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3myudktdb.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3lbfgcvdv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3tzkspaab.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3vmswikyi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3fgifsjbx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3crwzmaje.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3xntntbkw.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3rwkbvkwh.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3jeuewqzf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3qfmkyauq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3izbjoyxs.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3iacpzsnc.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ctiugllf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3tdawlcmo.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3otjbycvl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ylsckgcx.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3mlwacwjv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3jrbnykpq.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pxmbvtxa.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3lzcffhpq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3uiyhhxkn.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3nglkstoc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3dabumssu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3qwigcvwn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3atjzoxco.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3kvfsmeql.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3svagpbbz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3ucgejxkv.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3bpdmxuof.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3drvsvmrx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3wcaprxxt.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3qzqprrry.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3osvujomb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3qikqmufk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3hcflqanf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3fwrvcyfm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3upsymskt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wsozvqql.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3trxijxyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3azjaywfa.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3yzsgqspp.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3ieanqwpy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3mtzjwnzv.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3rmsggukz.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3hwaclcvt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3cqvrdcdb.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3kwtxfygn.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3bqvmcoxp.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3slmpvbtd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3dmfczolp.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ezwvshkn.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3zlhtonom.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3hlzjjvjm.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3dniwrhmq.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3rwablxvj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3fztqihij.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3jlsfdnid.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3ygvjjgro.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3eatxsjdl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3rfmvxtgi.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3jykekwcn.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3hkcmrbxk.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3ivhlkhnb.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3owsgmqxg.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3uywoxwlw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3woufczjj.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3brojzgxd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3mzwevwai.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3mzopkkls.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3zofzicuc.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3osmgpqgc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3kmvoxbet.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3dikrzuws.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3mnzpdlye.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3etduaghp.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3ncfmsgud.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ejlokkla.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3akowopoa.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3szlfbdbw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3ioxducdl.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3vrtortcw.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3apyibbvm.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3rhhmkcvl.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iypdttpo.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3sylvcsea.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3dfjqzkch.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3ufeluaif.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3opbxmhyz.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3geuwlfoj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3zkkuxgae.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3nedphyet.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fvddhqrj.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3mmxmliyb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3nxoxzmlj.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3exymfllg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3pofdsyjg.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3bcafraha.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3epamhglu.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3deugdzzw.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sfxovpvf.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3lwprhsgi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3jhelvyst.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3cnmiqvjp.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aehsghxv.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3puyrtbny.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3knzbdirr.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3dxcpafxy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jumakahx.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3uccygnou.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lcezxvpt.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3yxjpwquz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3gaeihfle.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3kvjsbsxi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3objwtdoe.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3tbfkpkkd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3zeurspxw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3jpneswme.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3fhuqozhn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3iyhvimgd.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3nnvczmhe.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3jaxuajxj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3hvkiueef.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3irjvsvof.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3nbolwvin.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3adjxjddg.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3dklbzcch.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ajnwhftu.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3qehucjxb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3oljnlctl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3pophkmii.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3ecvqzwhe.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3llgmykfy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3cyxmotmy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3bifqgybb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3owqkkabq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3dzielfjz.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3dcjxomwo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3qstfdrva.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3pqwvmflb.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3kewyuruj.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lgcjuuwq.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3hljecbmj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3dkcrnkhf.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3qpgglgyg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3liscfocq.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3pvaccjol.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3smnluihy.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3zbuqfuvj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3hxzwswsb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3dtrezojp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3jadsueph.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3tznxicna.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3byxpnwss.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cyzhrlvo.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3nojrlcrf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ahqbvikb.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3fwraasbh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3mfxvxzsb.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3wiozcrur.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3czgopwgy.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3terhajxt.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pzwcsapw.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3wptkdlrd.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3egarqabp.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3azwmbize.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3vuyxvmbf.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3fbdkxyvp.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3ccprjtuu.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3lkdwvgxf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3wyemhard.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3jlafkrta.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3redcmstw.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3miggxufq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vudyyxww.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3slgqgkyg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3useoktco.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3ayytgxqn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gqfpupln.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3rrrmaseu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3tycbezjv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bwmctqbh.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3anwtrobr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3oojfzgff.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3soodvuof.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3zxbrcntf.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3gzwkhhgi.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3wmranqfn.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3uqgawiye.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3eaesvsad.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3rwkavitc.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3hbqxqvct.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3mlsdvwhf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3ghlfswrg.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3gcjnscds.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3suoeglcx.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3rekwpcwk.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ccgohvnc.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3opftrizk.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3diflczds.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3qjbzywpf.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3wgdeipkp.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3kmzddmya.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3ugqyrmto.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3ftpnless.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3tnaejljw.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tqdusqrs.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3vfyivcoj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3okwapdop.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3zrpusyla.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3oqkaagwg.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3jghbgycp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hbuumcgm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3hodjngcq.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3uxjwvthy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3fgwmwrai.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3dcrrxtwk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3bgsrmccs.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3bautgfvf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3uccgidoe.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3chjvqkgb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3cdeeuvhb.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3klyobpkt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pmughxby.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3gcqqrjsw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nnlapaxy.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3wwiykyer.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kclvuhsb.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ghhqxdox.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ziiukloi.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3kcgswulp.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pmdcqfwj.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3asixjipr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3xxgrbtha.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3uhlmfkqe.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3wqiphbcf.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3zzqfhapa.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3jdqjsfty.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3fvxuguia.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3itfacqua.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3htmedoae.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3xpriwmts.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3uqecpfxa.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3oklhnogn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3utcybdxf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lfebyaql.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3xeekawpw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hejuqtnq.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3csujufpn.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3divyrinh.html


<!-- 参考信息 -->