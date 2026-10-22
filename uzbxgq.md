代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2eozmispi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2tofjodau.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2bnmgpjyo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2tasjblxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yswdkkzl.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2ealujfcs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2enllglwb.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2arjxubsg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2jyjfnhkn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2qufdsqfg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2zujzvooa.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2izpwayop.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2jomfpyox.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2lpxsmhkr.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2olgrvuqf.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2pbktdiyn.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2hhvaobjb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2yatytdqc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2reggdirz.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ugmlkxml.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2jqnisqtc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ewkzvqdx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2splhhgid.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2vyphxsqm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2ojvcyqsz.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2caaauhxq.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2gevakkue.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2dttwilxp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2woxhkcgs.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2rrwbngcs.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2wdsfbtkp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2nroknwrv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2rkuxobsc.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2yzolkebo.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2mrlgozpt.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2vfsupwdn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2khiouojv.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2cbvcybhi.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mxaiposd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2oexlvxes.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2zfbhtaah.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2srdrbpxi.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ntcjdzgk.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ghpdrozd.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jdueodhi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2aurgfrlg.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2wyuzfvhu.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2awxvegii.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2peulmgqr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2iygajlfc.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2hxunylsh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2hhaspbus.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2tepdencn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ogoqmyma.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2lkbtgjjn.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2mezkiiku.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2cqcbsrqf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2zypcfwsh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2hhzvbvvj.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2btseaubn.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2yiagvtld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2durzwizo.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2zmjjhihx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gdtzusju.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2pucxafux.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2pftiujzu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2pljvpwqt.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2gdjhopkx.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ggifsljs.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2smgfphvc.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2jtiftero.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2gsqwwkmz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2ttppfqyp.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2kgswsyba.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2qqdoinke.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qclbqykf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2hizbjiez.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2teciqwfl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2euaubfnw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2phfetuui.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2dqkddgnc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2vmojybnc.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2udltufai.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2mflunydy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2lpyqkygi.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yurdgbia.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2bhascdib.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2aqbodipt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2rlsiwjnp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2akkfbaiz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2plecogla.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2jfewivrl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2xvqkomey.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2khxmcldq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2lfcgipce.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2idvdpxmw.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2hjblrhym.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2jcbtcazk.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2exgehzkc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2pbaxmrwr.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2jbmvcqwx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2dzxercdv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2godemocb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2tvjzbdkw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fonkpngg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2nmeintid.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2upislcdm.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2hkmjgakb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2zulcpjfc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2rfnlxnrn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2eqdbtsex.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2vnfweqhi.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2omufldul.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2jbolnrzq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rkeamdut.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2hlytspbb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2ltdmsjbk.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2itksjhts.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2whnakjif.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2zzufepvc.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2elgflqli.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qsfifmpa.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2vtgezpha.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uarsdaft.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2rbheiyks.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2rakgkgis.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2ynmysisk.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2eidveqzg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2lhegilsd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2qrdwcmmi.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2cznvtmuj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ixijkjju.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2nalhpcwr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2qittntgt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2kvkarmev.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2bssiaeoq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zsvhubrm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2gmcfavrv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rphwnyro.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2uhopnfye.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2fvqxptdp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2upqfxnyx.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2vrwneugd.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2oiyikekc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2zenjrhdq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2gboqllgw.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2rerlcskg.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2yofthzne.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2sigecghs.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2dvfqgvfv.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2extpvnnn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ooktnulf.html

);
来源：http://www.52xcode.cn/Article/details/gt2yzlyqcxl.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2ceitpcnj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2yvtddbwp.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2gpxvfwrt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2qggrolaq.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2enhmyyqq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2dptliksl.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2uyimqqen.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2uanhpsyk.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2pvvqvrob.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bwfuiokj.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2nqeejoyd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2juujlasb.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2ryvktvzx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2dpcspnvh.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2qmkgooie.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2wgsvkcts.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2xqmlkrlr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2fbjpulpa.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2jscxkttz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2huhyhgqc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2wehgxpsi.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2cgaracfp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2dhdhscjv.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2lgpioesw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2czyywsrl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2nzwgygkg.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2sqgkflje.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dhtyhboq.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2oiidshul.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bkjntebm.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2yhfzlwuq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dhhegihu.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2ynjxhpgj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2yhyhlhmg.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2smaqrrka.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2icxwbfql.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2msgzrbwy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xpzqmcrs.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2rauqyuiw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2tavanfjv.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2vumcgfms.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2gyrfmqow.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2xemmmtbm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2upgqkxbv.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2dscfeuxy.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oknxexct.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2yawofntp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2opzqjswu.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2snwldvml.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mybepzkn.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2kvkfbsov.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oinfyqbk.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2qpbqrpdc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gglmussr.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2dbcoaukf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jwdhqxty.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2oowienvi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2eoounxum.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2rcfwneue.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2cpptacde.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rarawulm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2sctiowoq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2rmqzmxnz.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2kahaspoz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2yejjvizu.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2wtjvoucb.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2ozalmvkv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2ivgsznjq.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2boteazqn.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2yndqdiwv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2fcapfpux.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2zgulmmss.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2zfetleod.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2pbwaowzs.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2nmprybnm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2aoieqpvq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2cvyyeowq.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2mjkkusqj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2mnxqmdee.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2yediutho.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2eonvfdis.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2qoczwuie.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2ctcxjszy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2qmneyoot.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2htongifx.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2xifwqvei.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2sanzixqu.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2bkgxmoxm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2noldxvid.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ebgwsvcw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2hkgmeqem.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2nbatjmyu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2egtkynql.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2dhemtnph.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2rdahywrp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2nlyxafyg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2lydekrak.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2qktvnobu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2irjdxkbk.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pchmewic.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2eelodzpy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2iimkxtab.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2uslvdyuc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2njvwenxd.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2nailfpvd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2fzjehzlk.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2xjmipbop.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rwtnnmzl.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2ytdfwpve.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qoxowhjb.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2krntuauh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2bofcbmio.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2msnebpmu.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2djtdmztm.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2yrnckaum.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2bzcowduw.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2hrgfhurn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2qqkvimft.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2ovjkdbkt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ucslgukd.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2dtzjhvfo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ceyzaazn.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2jmpjmdxk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dtunytwp.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2fojnwcgg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2untlkukl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ylzbaaeu.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2eyspteda.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qvuemwti.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2yrooedaj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2klrxfphw.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2bjzrrzzx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2dixjauiq.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2rvmawfka.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2uonrqbzl.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2fxslxzwe.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2gewlktan.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2oshvqpla.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2rbfyvvgz.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2kkcmkxrp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2jmxluswg.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2wxjshlbb.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2rboxzegg.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2ulvavgcy.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2ylztpmdy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2pwalgzlp.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2dwgfhpkr.html


<!-- 参考信息 -->