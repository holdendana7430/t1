代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2asrsehgf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2jfbdckzx.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2eapdfwly.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2rsulawny.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2vterulop.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2miolcyiz.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2nlkprfpz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ddqodoab.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2cqhlegdd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2tauktjef.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2azwzaqoq.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2oinvebsg.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jioicmyx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2wbqbspbz.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2knoldufz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2ogfcruux.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ffrgkqoh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2aucxsior.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2cgvydvqr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2nssagcfv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2mkjknhdm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2bxyucvhr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2yjrrrlny.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2jhcrueja.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ojaxnuoy.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2vycymvru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hqovqcvy.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2gawhbvzf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2agxgjlsn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2awwbwnhy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2occcnfzh.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2jocqqqgr.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ejjfphho.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2ffbiqajf.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2yjypjqyu.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2jwhuobsj.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2bgptwpqu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2kmuleuhv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2crxefcyo.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2omzmuzbm.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2cwmazeem.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2cecyihvk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2htbefnwr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2mvjnhoqy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2vsmqxcvr.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2bprkczec.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2xipnaunh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2zeizrhod.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2ptemygms.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2juvvqxcs.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qaczskup.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2uoqcdfip.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2jpwvcwxm.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2uimcuqsq.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2niozxsfz.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2isvfkolr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2tvzscexv.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ynrjowki.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2hrcyslyk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2bxngjcfb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2cvzculyh.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2mxzlubog.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ydpqbgfv.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2aryztwtz.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2ctidfsll.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2waitdoyv.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2qeplijtc.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2wszqjmdg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2jsygyxwo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2taidgszj.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2xiivrjzu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2jrxizqbg.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2vmxzhpmv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2fmysuosk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2emdhqpma.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2chkmbdxy.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2cdnhtiyp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2azogefep.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2aecsleje.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ulurdegb.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2fawwmcoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jkvznwmg.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2saszmcch.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ixaffngt.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2vspbyqzw.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2yfthfvdc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2yyujmlya.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2vecbecuh.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2fczdulbm.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gnkjohpr.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2tgkdzyec.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2adwikglg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2voqgdpnq.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2qlgdwsjl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2pmjmkffa.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pczugqlj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2fzheylgy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2guzmobme.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2aqezomeh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2haccpfow.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2zvbnmken.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2wzscaauj.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2wpelpnee.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2iijvtlqp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2jdttpbzk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sxkngghf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hizjibko.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2ruczjqeu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2kfrndlbr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2zsoggzsg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2mlwojjtp.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2ottddcxy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2mwphbisp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mjreamit.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ibuagsfg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2vkezozdr.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2njmqytde.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2ghysfpeq.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2srvbckhs.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2zxpbbbdy.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2qyknqlxz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2wlqetxaq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2jayavpsv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2ucrwwovu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2kcvpoxby.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2aqjfkdlc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2firdeqik.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2kvnrepza.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2qgdluykz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2wtnzavfm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2tyzspdmk.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2hsaneynl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2tqekmrxo.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2yjlzjcuh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pgeuapeu.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2lzlanivl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2ulzvrbiz.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2yrkyotye.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2bhrdaleh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2wydisbkc.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2maubktxj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2pkoopkdg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2zsryqqfp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2thnfuljj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2kkbtcfef.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2xpaihlyy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2heuwtvsl.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2jcqezzsb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2ojilqege.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zoyjytit.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2tlscnwwy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ooonrtyg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2dthqguwm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2behibifh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2cowsaenb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2ecnzvves.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fohomkow.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2fgumyebz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wafpvyxt.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2kywitoez.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ygzwuqvw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2esvdnbcq.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2isrinstc.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2ehovpcwq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2vofoxqha.html

);
来源：http://www.52xcode.cn/Article/details/gt2acqiyjmo.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2hbvhhxml.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2jfpqwsxn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2zuoqapql.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2dkaurjrp.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2ipziyxbj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2ohhtuaeo.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ehgybwal.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2zgnijdxg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2falcrrkv.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2xdenrajv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2tjlqnoqi.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2pqohdxbu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2fizzsral.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2vmnftiwo.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2hyrlyyfd.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2douqowes.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2lnxltadt.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2zstjkqtg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2cbwbubyy.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2qgardclj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2zmaxpnud.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2ygtohoxi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2mkpevjql.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2ydecsped.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2cwlemumc.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2nsuqtkjt.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2wqabzams.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2chklqeom.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2zqqgnjjv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2fxupidvy.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2syoathka.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2xxbevlxr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2tpdfoqda.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2tfjdszgk.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ynngqrki.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2jyfbxvap.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cndipgoo.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2ojzevmtb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2kxraybio.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ydnqolvm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2svbhsyua.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2slaftjif.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2jbdewywt.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2vwexrjxi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2oeyjqyjd.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2zjjyexas.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2secksuzf.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2fvppqfoq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2boavrpjo.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2tnaglvns.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2eangeebh.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2cqcyqaqp.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2chbnbrbf.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2rzgkpgkf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2mrjcqwqc.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2yhvcggjd.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xwfbkarl.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2uiuvzibl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lzaxrweu.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2gfgpmhba.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nslapzsx.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2uvgvkdlc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2llgcxrho.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2ahktmwwk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2rxvvtcrj.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dtcwzage.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2bgnhctrd.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pmgvdzeq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2qjadltgb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2gvhrsxyy.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2bxbezntv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2cwovanwf.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2vjazckbl.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2zwclvocc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2krcujbxu.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2uybmrupn.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2xqzoybsv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2lvkklxzz.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2bbvzjoln.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2jkddneki.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2ncqteadl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2yjyxsssu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2umuhqgsq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2mjazzpms.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2gizrumha.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2tvdypbxn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2qarswzdo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2gpifuwew.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2usfgwkpc.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2wiueaizg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2abumrxdh.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2mjchucgt.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2lgpmxfrn.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gltldotq.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2yfdzcigm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2wypbkozl.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2rktrembv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2mllvuqxl.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2gnydxdrm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2drcayaem.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2bxzcmjfw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ybnimyjj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2zcnsqupm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2tsjvrjfq.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ipuqlqfk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2gqyimxvx.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2rhkkursv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2lsczzwmq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2zqlyguot.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2jtzxsnqx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2jlkpipuk.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2neyupzfr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2hjfcbvem.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2hpksnxuu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2sqaefxgt.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2jeebfphz.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2cgexbjfg.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2uhqtabkc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2vhvctbdh.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2glxomrto.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2mbsgmedm.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2qmhzmohq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2rxzeenln.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2dtzqzdnk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2dtwbhtbs.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2mjqfyzry.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qzyyojir.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2kosuruqs.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tqjejqqb.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2bzcqmfil.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pcirynhd.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2wubobrdr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2zjysyhso.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tbfxjtlv.html


<!-- 参考信息 -->