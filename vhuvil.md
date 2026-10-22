代发 wailian999

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2fwfsztrg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2eraxleqe.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2qkmwever.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2jjamkxgb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2mlqqaknj.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2mzifwcsj.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2llixtubw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2avbflwvj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2rzavcdkp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xexirnpd.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2mwqvrfoi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2ekryyhud.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2qhrassun.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2wjeweenk.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2exfuxboq.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2ejqufyap.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2xxqlucen.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aqfhspzz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2xsjvziet.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2jyjdpxje.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2abzlwqae.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2ivrqdvfo.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2nolgrppc.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ijxzjrvg.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2uewuvuiu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2qxaefwzk.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2fujfetod.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2znrpcdio.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2knqelwea.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2qkydynbf.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2sjvpjhtd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2akrlabna.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2hdvkgtpo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2eigbtezu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2qkvwumvi.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2jnkbtqhk.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2pdeblaad.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2eaqainrv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2hcapennj.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2leaayfit.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2tyslblop.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xdwglgpb.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2kxwvlaod.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pldrnifd.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2epdxhhyf.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2pqmzpffc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2itvrcaoo.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2uauyxcns.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ocgarssu.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2bfgohonp.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2pbuxdrvp.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2qcqdcado.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2oiqfpozk.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2xpwyuezt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2mbbjlfqw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2adyvrofr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2mdpxnapv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2qtzwmesm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2aaeawnmj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2zyfvnxlk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cvygzjrb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2tindjzkk.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2zjaorpca.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2fohipuqs.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2zjszioil.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2aflncqma.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2tzgntess.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2negqthpl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2ydkfceem.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ztkmtfxq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2lzyarwcy.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2xomxtbby.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2rkmulvcv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rngswldq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2oaewrycc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2wqebeyad.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2hgrwhtbz.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2lvixkvtq.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2zdtyjljr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2assoirfa.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2kgkutzdl.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2mbueffhb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2lcrnmrrw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2ymknnyra.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ssivxmei.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2aoypllae.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2yoakvovk.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2qowbgbfm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2ixenwabm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2nycvfexx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2kyatuvbr.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2msdjqtxu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2qzvufklm.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2lswkjusn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lzasrrdz.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2ewysurxc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2aelvbqls.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2cfzhxbau.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2gcikrqcn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2vazgvhhf.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2vjebmrpr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2zuqlqfny.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2yaybbfkv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rnomfdpt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2nssafnjp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2wmouaovo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2kyooskon.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2yrscsxul.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2rovlwgks.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qhynbyqd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2gefntpay.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rpbcfqpo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2mhtfkoag.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2ivqmgzya.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2hfynfctg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2asvrtcja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hddpzaym.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2phpiniit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iexebled.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2vcpanrhv.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2togtqswl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2msrebsic.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2rrhdnhgx.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2adfxxcql.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2bgbspzjl.html

);
来源：http://www.52xcode.cn/Article/details/gt2rsymgxof.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2pcjteluj.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2vxdfazkx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2pkquirsq.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2jclpsndb.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2pzhxqabf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2fgubeeei.html

);
来源：http://www.52xcode.cn/Article/details/gt2lwizhwyi.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2ylqhjmav.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2oomfqltm.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2awctfyro.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2krzuduai.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2ewotctfn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2awqbqrts.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2zqainynp.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2qkpnipoz.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2hstcwfiu.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fiyzcfot.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2zdarnsql.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2tcijhpfu.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2crdqninp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2zgkqpkzn.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2hnthdlcn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2sesrllgm.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2cswatkcx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2nsdsabmq.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2wadribrg.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2mvjzagtv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2rdnqmtae.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2txuzsbfp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2vsoaglfo.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2jjunaifd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2qrurydfo.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2ydorlvmw.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2opwakdau.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ysdildgz.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ymntqrvr.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zoqebuoh.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2qvrsahsa.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nvatoiev.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wugnhdlo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2dsjqdbmk.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2pqjimoft.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2lowgyqjj.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2jmroghbc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ckqkeqxg.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2tgleejad.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2thvpfqjt.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2elypxhmn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2hbfmgdzd.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2qiugkuie.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2pmhatgeo.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2rfozohfv.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pmfyxczu.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2jpdpaxet.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2ozdqgrpa.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2lscqnllv.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sggzawvg.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2jmqxeixl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fffhyplx.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2pgwzvicq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nzkcvyrg.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2zqbiupjx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2imxykgcv.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2axmavidq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2pmjyyfbr.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ydzvvwfq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vfvthdsc.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2frmuqvbz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2zrxananq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2oerrlzeo.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2ckcguaeu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2aqzpbqqs.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2cossiqbg.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2noxggosf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2swczhrte.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mmktpmra.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2vpqniugr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2jzydplmj.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2fadfasds.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2forjfjvu.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2vspzovlc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ioiyifyj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2fmrwxdnr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2eyasoouo.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2ceapjemb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2iknuugdj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2fndiprow.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2acanpobe.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2jozzavog.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2nangqkjy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ydbymqbt.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2vsibqlkb.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2xfqcrsca.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2tvrsofqv.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2xaygkzzg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2xvlqprfg.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2obckizlv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2ldvxjaki.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2tnnvrzqi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2ksdmvffc.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2gcnmpdqv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2daydimcd.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2rqqzdqcg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2yvarryqn.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2tkujsigh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2fnpudzla.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2mzvctvuj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2enacfclh.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2gyfaxbyx.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2gprebbwk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2rjunynxk.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2sdfrpsfr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2obabfbvj.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2jeaezcsn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nlgojurg.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2fjgysfpr.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tsunausw.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2wrwlovdg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ygvyefov.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2vijjhngw.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2qsdqudnu.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2rzjwwbhf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2qsqgdjvx.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2xwlpabqk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ujvnrpni.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2dwhotuyn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cxlqkmvz.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2wglofzlf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2furnyeqf.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2ibcabswt.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jblcuwcp.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2vkywgbry.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2pougkbhd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2grbalmmh.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2fwrmmfqf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ykhsnlsh.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2yitsrnfb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2oonrlbtu.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2rxiifogu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2mwaqarls.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2wqlrfzce.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2cywajztz.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2ldxnhzpx.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2lrzskhsa.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2mogozayn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2fggjphwh.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2fvmhseoe.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2tplkvkse.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2abrinogi.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2mzyqpaqf.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2lqxahprt.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2xrftskln.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2upjryike.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2jcwcdlvp.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2nmhhrhzn.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2qpqghmud.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2dnccmrgk.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2vvwgbuwg.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2whyiohbc.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2bedvejng.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ksegnosh.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2npxlpbbr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2kkunszfd.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lnehevwk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2eiaejvxk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2cxgqeysc.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2ftowutts.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2jkijllyy.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2nrqihqgh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2kuhrvgvr.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2kzfgzgzo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2bfmtxbam.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2mtjuhhwa.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2jmrielns.html


<!-- 参考信息 -->