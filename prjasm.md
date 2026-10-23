代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3nhanepjr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3vpvchnze.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3fwviqkli.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ljftkjqi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3qgqyorbt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3wfmhhzdl.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ikxhjhqg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3sizrnotn.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3letwnkme.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3kkdmshep.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3yjyjemwr.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3bmfaedoy.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3eydzjzcf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3kcpcwedd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3rcvrzoma.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3hnmzatxf.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3atyzklok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3btorbmbz.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3oxmljhnp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ohwgdrei.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3oxileuta.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3heakbfzy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3xuiqiciz.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3bgetwtzd.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3skdzussx.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fwdxxwbv.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3tohoutyt.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3vbadmqan.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ylgqigkx.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3nolamuyd.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3yeawbebn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3nvjpkcyq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3mnenetfm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3ilxlpaak.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3geyeodel.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3ethykwsg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pdkquecx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3pqokbpzk.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qiadwlff.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3mkbastnu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3vgeiycid.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lmsdouye.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ocnrtntv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3sdqozvbl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3lvrbskui.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3hjieecrb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3hwkbdaoo.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3fkelyyyh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3zmdonsmd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qigyhoxu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3wyemhzyw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3rxmabpkd.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3npvycuqe.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3ppcwqmhz.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3jugbmbka.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ligbtwtc.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3jwkdhblu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3tbjbfsuh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3zakxapgv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3bbzwltfv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wggcfwwz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3jexncvjb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xjwlvyje.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3lkamsnfa.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3fibdmbsy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3ucdjlqon.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3uthkiegj.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3eflnssgd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3tyfqzqdj.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3avbqjgzr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rrsoefcw.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3lancejku.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3maaxzoyh.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tpqkreuk.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3ttaixeqx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3radvqzgn.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3wndxacbd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ynahvryd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3qzhtgrfv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3pifgfkdw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3fbjpdrip.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3hbyuzcho.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3wpxjqlla.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3scbsveom.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3jfezoomf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3ypxkfbtx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3awdcjiqi.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3xujqkklm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3wtcebvql.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3caaxudwh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3rzxhphgu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3pghcljnk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ktyqjain.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3qnwgfzin.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mogqrzrx.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3zcghtarw.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3minctgcs.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3oedxynvj.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3vhmkqnmi.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3sgvijkvw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3whcyjslx.html

);
来源：http://www.52xcode.cn/Article/details/gt3iexxkrtb.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3zpfzxjet.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3jnzcynas.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3bmrokatm.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3hzsrknwc.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3tpawwfll.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3gbhqtzfe.html

);
来源：http://www.52xcode.cn/Article/details/gt3fbqqnpdo.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3cwnsyrfh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3mlaxksye.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3kodwtgnm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3pyjjxsow.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3yogxztqo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3ciprufcs.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3mjabudbf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3anmblwxo.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3afgxxrah.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3htearkuy.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3gitophpz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3srqpqlbc.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3shswxpss.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3vajehtbx.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3lxqwmrgs.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3sgkmdswo.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3aingysdc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ujtybhiv.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3lfhouypi.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3aprnalon.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3qgbvkafw.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3cvmjbvhl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3hdxecptt.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3esbboxga.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3wanjdujl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3wnbdmcas.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3vcgerint.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fodmztiv.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3lqyahdvu.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gaqvgyyk.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3zinopfwx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ssecwyno.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3bfthaiwa.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3pwrgbdoo.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3eaqzpdfx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3tvsdecgs.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ifozxltq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ugqwkbtm.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3bnyhkmhi.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3otdtrsai.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3ngnexhyf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3pcmqffly.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3uxeganrt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3kosgeixm.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3owkczoji.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vljrmhnn.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3scixmhrw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3nnzbpspw.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3kkhveizz.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mbwnkqgy.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3lskdaqvj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3egzrkjrv.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3hnfwsatx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rbenhwne.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3dqidcldn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gdnbxspr.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3qlmiobiw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3oiumohsa.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pmiheihx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3qukkqlex.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nwigpgnt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3kkedppgh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3bqqptkhc.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3paiqvesm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3pcxgmqee.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3lgxcwaja.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3yjdkooox.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3lnpnhroq.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3nlsjvuga.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3wpqdwygp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3mokselwm.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3rplgchib.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3mtefkhhw.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3ihbjsivp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3jqgbpkvk.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3rsjbtymq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3psgpjjbh.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3wsolvmay.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3nbrqhofw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ceqjocwp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3uvaeoomj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3esbaivpo.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3htajzwnc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3jrabmkcx.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3mkvxjubr.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3bdaaittb.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3xjxcxsjv.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3tjzngoyp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ewqmsmiq.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3cectkbtw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3hwidmpln.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3qscyiczp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3fnoeljdk.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3yazvfern.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3cbkaxwia.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3eajovyxn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3izlcfrqo.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3xaecousa.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3qctlnlby.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qluzogxe.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3pcjcxjha.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3cnrghqbs.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3ajihncjc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jxhkpuve.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3cxeemzdl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3atzheniv.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3nuvzxqws.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zobxgvoj.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3neksbomu.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rmawfuya.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3jccgwcei.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3royuanhs.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3rbjaivtp.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3qfxysehv.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3eysffhwp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3zhweriaa.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3lullygfh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3dspfkpjm.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3ifzohhfu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tukwztwc.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3oeqaiqgr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rtbvmovb.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3ykruvjfu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cezuhhtk.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3rhladelh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3tvhplfnl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3aiugnhlc.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3rwrzmuyz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3imknkyqr.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3uybjtfkw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3xdpcbhzc.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3lnaguomx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3uduiiivz.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3cccixoav.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3amewttvo.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3fempmdge.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3coyuafyq.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3tifxuyzq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3aoukaxil.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3vzlzumbk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3mncckqkj.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3tuhbdmzo.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3bkpdozji.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3kaxtropj.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3iabjzhbt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3kymxanis.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3vtnamkii.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3fvvommin.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3ukbadxdh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3zwgljdxz.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3frggdirq.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3czwfezox.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3vqmdclws.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3izdsawix.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3wmnixkvh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3ywqpewzj.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3fwvxmboa.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3leiqwbmo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3teeycjvl.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3wradvxop.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3qbfmjcbl.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3dbqpcprx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3psmjuhmy.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3bcdtcebj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3thaqukje.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3oupfcjdo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3ritfbkcr.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3skuvipaa.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3otlzmmmw.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3httkotrj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3abchcmkm.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3fiufscpv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3izosogaz.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3vmfiutjd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iyvpqttr.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3dacyizig.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ujlvrwvl.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3qipfindn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3nggyutwr.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3iiugtuhf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3bninvhps.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3vsyuzbks.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3jaujefsa.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3oditebmz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3fgueyexb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iogbsdqn.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3bdonurvv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3wnltqoph.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3tiunqtwb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3xwlotqqg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sypnbzpf.html


<!-- 参考信息 -->