代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3dgsuqlsv.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3gctrchuw.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jlngslfi.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3nrtaymvy.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3bpjxzwyy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3kbsoejwt.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3reohmkkp.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3odiqtyzz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3bzgfebrp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3dledbkdb.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3hserczhd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3hqydarqa.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3vptbkozr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3fvwqyaqi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3njdzfbjp.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3iapjsqfu.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3yzvjhuqr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3imzvwinz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3wmufwnmt.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3tbkegmrr.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3byykjqcy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tlbciles.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3jqtyjvxf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nfxwetxn.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3uoitrrco.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3ddyrqrwe.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3delzmrpd.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3owoqwssj.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3oxnwskdz.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3xzsxpegs.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3izhkiiej.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3kwuomxqq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3dlwubafm.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3awusmzdp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3gxjuklhw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gefznoly.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3mppkmmpo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3vecbltwb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3zueiqdll.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3sdusypro.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ggzitoen.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3izsboden.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ywahxemm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3nmueejfz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3mffwzear.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ilwtnuaw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ajwjwlyj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3rngkgomo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3vdobtasy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3blofehdh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3rmjgwiyd.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3qfrydvrn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3erqxcuid.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ivedcajx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3hzurobdz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3lvddhvus.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qkearotv.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3ipuouepe.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3ecwwyajj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3kuhqpywu.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3plaamtkl.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3rpbcjrym.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3ilibrtfd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3zevtadgq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kxrbpoqn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3rwknhhgt.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3zycbvmgk.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3lmukchgy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3igczajzu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3hyptomjn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3dreayaqv.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3wtlzosgk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3dfpnrgai.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3lunyxqus.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zlfcqehc.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3qverxwcl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3fwjsjfhh.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3flrobznn.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3qopacilt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3pqnqlakp.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3gznvpiib.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3gzmpoqpi.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3dqnncvyk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fyaskmrc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3nshkkrvt.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3omeyvgyg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3lyslmqhm.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3dbxznqse.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3gixqlrhx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zqobkqey.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3aakddnci.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ayfkgyzy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3jchbzugv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3umqftjuj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3pmjfwzmw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3yhpakkcu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fzngcevq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3ceztravc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ctsabezx.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3ixwvmwvp.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3hssnyqpb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3sgonaglh.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3xhqckfvs.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3ccziqhfd.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3xjsadlcz.html

);
来源：http://www.52xcode.cn/Article/details/gt3mthypxya.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3syonlvzx.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3lnxfqsmk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3nmydpfha.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3qkoaujmh.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3ypjtwsiv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3ennvvjug.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ayboqxmk.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ibvkchuk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3xjifbceu.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3smuxrtje.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3nqsgqihp.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3jsbiojuo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3lfmyvdzs.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3fpipwbkh.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3spocnnqu.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3bkemlfob.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ptltllxi.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3fxtvjbot.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ikzrhrbm.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3yjjkkufe.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3jqpgmona.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3ivqyqprh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3gpbsmquh.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3uynansqk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3frcblvrr.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3mjohnfsd.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3bpjfbkfu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3yumvqopa.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3plxjiweo.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3depluers.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3zpurxseu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3ftxigxuw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3zszdalrn.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3xwvwhimh.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ynvutvlh.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3cmxfskyk.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tghjpqeb.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3lxxpfasn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gyrniznb.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pepcthpe.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3qfhvipxo.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3pwtoddyx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3fahthcjn.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3dukpcywu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3mvuejpbp.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3kwvehclz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3vpcurlut.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3rcmfgrot.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3njqsjynj.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3etcephnd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3tpxsgtuh.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3azasxbcz.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ngiqitwx.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3yeczzegd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3yfloajpw.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3vxrmjuub.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3flmsldkk.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3akbrcpqj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ugrzdzbr.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3vtxfdkah.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3onrrurzf.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3iqqbikqu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3avdebhsk.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3bgctcbst.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3lnigkyzk.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3lduuckcc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3cjftqdbv.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3utxiayqu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3odkjjzjx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3yhgdbtlh.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3ymnzpsgh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3abrnmakr.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3hqvjloig.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3xgodrgwb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3ueupspzg.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ihxvkgud.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3npbodkwt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3rrqcqyyo.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3gyjbgjyl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3cottozug.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3okrcegfm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ftwietxa.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3govxbasm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3ftsminpo.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3ergaynar.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3oxymjheg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3tbatbtyy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3oxftukyh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3sxfqapsl.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3xdourqdb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3ajsolwab.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3fcvouwev.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3stpazdhv.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3cykzrata.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ocztuenh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3imwegngx.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3kyxyvqwv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3laytsbtq.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3hbnxrmac.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3hngeynwt.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3ffvatrnv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3rtiwudnl.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3cfcuvmzc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3zxwgsjnz.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3jnmyjybh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3epskmzon.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3cnsyjuwd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3jusywqvu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3oytyfsuy.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3byadukts.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qmefqdgt.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3kdvoktng.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3fkodrpyf.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3hgijjriw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3etaplbky.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3wxlfzzzt.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3vdlytmti.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3beptupvx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3yyrnqfbl.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3kxwskjzb.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3tvllbflw.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3zfoaxbzp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3dfcuzwtf.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3uabvnufa.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3yzszwvyr.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3fmjdcwlj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gajsubdq.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3httutahx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nnhottjc.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3hpdvlfhq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rsjjjvbc.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3ekpbyeyo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3buxqqily.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3uyqzoagm.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3mnxqydrk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3iccvzxqv.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3zrbledky.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3biknvwub.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3ktdixnbo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3adnjoiqn.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3nfhxrkif.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3qsxxrhrg.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3xdalabgz.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3wbtxbhhh.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3kcmjuoul.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3nafofnob.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3hfdwikta.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3lhwnamlk.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3enzijtkh.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3sxjqufuj.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3iqallnum.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3ubxioxhe.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3kkesubam.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3buceolar.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3uacvpslt.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3xpqvlslh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3kixtxqsh.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3mucfhtnz.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qtfmdnfn.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3vhhwxztd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3slxtapkw.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ztcvhoeu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3nrbzjezu.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3spdahizj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zitzxuet.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3ruovwkwg.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3rzvuejbc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3ogqfzlny.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3nrhilofv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3xsohcrgq.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3zkoihprf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3tyterupn.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ikpdybxy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3btdhzixm.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3hrnnrjtv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kuqezoki.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3wopazgky.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gsncmmmq.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3ajaomyfd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wbetvyax.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3rkybfrdc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fvpuxrft.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3xlirgbcw.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fffkqbve.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3qjorgnxa.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3ynlucsta.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3vdwzgron.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3dmzebero.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3alhwgizw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3ekahhaic.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3cjednqte.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3rdutngql.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lyfyyhxa.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ijduaewh.html


<!-- 参考信息 -->