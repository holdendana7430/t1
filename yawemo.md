代发 wailian999

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2mydecefd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2uadlxwsu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2vxqnzhlk.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xpccshtu.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2vsjavlvh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2xygdtpdg.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2eczyzghh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2xiixfink.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2zagqyebe.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2lfgkdusy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2gbfwrufy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2dhblbudm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2djrhxahh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2moimpudh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2phdknkkq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2wpmfieqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sczsazjd.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2mddpnhly.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2acvsrbry.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2prwjnxoo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2erxhchzg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2miittysc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2waauqnna.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xsvrntzz.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ltlnqqrv.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2bhkwpavh.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2dcdlnikt.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2ozudviho.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2panfaobs.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2fnuzltpx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2ceenmcvj.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ttimohhy.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2uyzfshcm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2dmsfjomm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2dcdowjdp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2tmkknvcf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2utkvcaho.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2yxwdbwfv.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2odobcqak.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2oxqrotnr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2ghicsboc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2fgcezust.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hyuqxqsm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2rbrrfvvy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2ioceofgf.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2mvtqigmt.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2nosehieb.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2jhetookp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2zzbatypi.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ubmacnxv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vkghessq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2rebbysih.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2ayqodusw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2dpgvnqlj.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2buzvifpz.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2skmfctsj.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2mzdrwdti.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2nndijjig.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ycmmrxyj.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2fpbjohss.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2iwdfumuv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2nppoqpic.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2sbpvfohx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2dvmfzwry.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2vpzwmqbr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2cdgztstd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2cnrrpssw.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2lpvpoycf.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2kqwrnsgs.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2xszsannq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2fewlfqyv.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2frffndpz.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2szlmwkpb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tyooanwl.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2kgzvsuaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2abluwiqw.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2vgkcahuu.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2unaxcljz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2csbusouh.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2hamwymbv.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ddviugig.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2qqbeaoiu.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ebbdiidi.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2wajwhfqg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2ggutqqbu.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2qskbmxqi.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2mgeunzvd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2fmkyijjh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2kglqwnsi.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2fpkuyeop.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2pvtkakjp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2mkhuektx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2gsiigwgz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2ccucmlvp.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2zaaeastj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2nnlphhbc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2jcfnpspa.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2lymcmdsw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zmhoozrv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mashozbr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2mbxbbavf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2sdtbcqvv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2vwuvvexa.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2zpikvvtt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2twcynodm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2sfelzhlh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2btuqirer.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ctqoqtsg.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2tzpcmato.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2violtzhf.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2pmxjdhui.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2obyglehw.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2omyphyne.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2layqumbt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2utkcvugd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2lhbhpblc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2szmvetot.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2nlzaodbq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2olsplocd.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2doaadhbz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2bcpmvybh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2kgxmodxo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2wwomqywq.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2hbtpdmdb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2ctwatils.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2kzgsltos.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xrkzxgti.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2vrcmfdek.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2uiowfbrr.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2shphnnhl.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2ujgmmrhg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2dzewiugh.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2ghgwftpv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2yxilekzg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hecndiru.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qwvipifg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2nntbqzkz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2psrmvpsb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2fdijgaho.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2avdlflpe.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2kshwqcwc.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lrkwmoph.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2wybbdwke.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2yudzmuhc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2kdeetyme.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2cfpijqri.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2zhodjtcw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2ighcgnsc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dusmczls.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2xxwsjpye.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bvcnyubi.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2qgumvqfa.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2gewhjkcg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ivrerofi.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ndcleyyq.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2ohdfluki.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2tvunuklm.html

);
来源：http://www.52xcode.cn/Article/details/gt2cfjgeild.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2ivtegjfd.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2wczacreq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ebsjdsgp.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2dyuwdrni.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2qfcpaber.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ezvspisu.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2avcqjfew.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2vrlknmyr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2fgfimsar.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2eopzdxdd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2bnhbatdo.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2izbggljl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2pjjylenn.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2blugixmh.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2ynxezpst.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2xzqungdw.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2swnigvrd.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2zgrlzgqx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2mmmwxkiq.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2xyvoguxo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2mquitiii.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2cgqapvot.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2rghekkmd.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2mzjrhezk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ktillnkw.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2zcihfpop.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2yxnkvpgb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2mowtjoqs.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2klrrakax.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2hbhgxvcn.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2edyaiogi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2yzrzunqk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2byxbbjxc.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2lkhglmto.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pjvkjgzm.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2afrlbyui.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qtbwldms.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2zynhhoui.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yvjrhnhw.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2imfrnjsz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2ztvmkzml.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2cswopgja.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2bodbfihq.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2trdmiefm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rrgtlwuc.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2mxmdpmco.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2xfhfytgg.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2bxhstxdo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2utuxynzj.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2sjbotsym.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2qejjyuub.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2xophrhlc.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zalxcsjt.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2uqecxefi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2mtbzlutz.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2nfopzfjp.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hnsgcuux.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2uaiaurjg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bovwlkan.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2bdtpavxr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2evjqtnjl.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2tbtcwzzp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vyiszjqj.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2ejsiesmw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2gvcrcqcu.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2pzyevizm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2uqpoetdi.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zxxnzgnr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2gajfbajc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2zsrhbxuw.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2ycrbyjfz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2wrjhadis.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2jwbevgme.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2lczxlzki.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2rjbgbzwp.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2ttvmbszv.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2dyizgemv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2xjwwfbbb.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2zctrbkck.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2pukwflfq.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2uwunjnrr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2exiomywn.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2nowkulhz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2bbxiqcev.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2tpchbhpu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2dckoxzam.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2rooreinb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2psnygjbw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2iipupoms.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2oosvfdza.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2gkhlvrcy.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ykdznhba.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2wtjhkpyn.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dvrjcopx.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2vhtewekj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2vdjqwxtp.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2xitpkczr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2hbqwjgos.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2vzulgxmx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2pqondoye.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2mduzvwms.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2bloqvknd.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2qwjpzlll.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2bzypbrbr.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2cuizbftz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2tuhvjzoc.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2wnadpcdx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2audtigwu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2jxhkuniz.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2cajctkbr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2sqsnghhc.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2iqlxnevw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2uaxswehd.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2rolxtcnv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2apsefumu.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2znycqvow.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zmawnpuw.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2vzazcldg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2iqsfsqda.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2rwebgxfp.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2lbcogxcv.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2bxistjhn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2dxweocwx.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2warwffuw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ojupxumf.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2caamtoov.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dmgnftwv.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2tsujxefu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2avzezjmi.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2vzvigbyp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cuqblspn.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2lomnyvsk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2dcqrwocs.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dqyywtqe.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2uzpekpop.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uytpjocu.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2jcehtwih.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2mbopypvp.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2lqztuufa.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2vjypcakf.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2hitduufi.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2lilgtshu.html


<!-- 参考信息 -->