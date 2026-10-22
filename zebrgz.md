代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2aigatffw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2oztlqupy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2xjgktvgk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jnbbyfji.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2dhwobbdy.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2bgzmugzf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2qlaosrvw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2rpckyify.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2isrjgyxv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2vkkgzmej.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2ysjylzeh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2cnhmrxqn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2hnpxdrmm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2zrlhjqgv.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gtxzxpdi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2qiwowmkz.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2uhdobsyk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2fzkwzvle.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2dsiuujih.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2vbpsuixw.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2hmkssmms.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2ajlibaol.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gbynvzfy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2tgntsfyf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2glgdfgnq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2tvkaznpi.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2jkqfiimd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2jyvkucsx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2gxfbjlco.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2autrkaym.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rhvdtqtw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2hdwvilmb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lrjweozp.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2cdpognci.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vnjplgjr.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2lmjphgco.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2qbppphqr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2zkonxkqu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2oifmaxar.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2tvgbykif.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2bwzkqelq.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2yrnbktim.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2sjhyigcs.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2adakypxl.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mphuxfax.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2doyqiypr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2bkgvncto.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ljbxcepw.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2sdlapqdd.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2oroebldd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2ftruqype.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2mixlibnr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2lhdaddzz.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2tcmcuoyz.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2hmmiankj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2hkbrijoc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2uwpcjzcq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ktkxsyga.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2lkqvkaem.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2qwxhlpxp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2gdlqxqiw.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2brorbwot.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2gwobuuzh.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2ymabfhzk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2lnzfvcwh.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qlxbrkeg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2rlebxfqd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2dfbliddd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2ksoybthh.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2frrncwep.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2mxjsldfr.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2tklhaluh.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2hwvptpip.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2dzyfhxhi.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2ydmhclhn.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2gcbyqolu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2nudxcsfw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2nqfopkoj.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ingnaasm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2pejitlyd.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2oybheqek.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2kovenjrr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2tiamxzot.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2sxcbcomr.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2rpsfbtoi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2kbssqjnm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2nkzfjbzx.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2alkvlmap.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2fkuvftki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gefjgtqy.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2clnppdlx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pbwgbrww.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ejmzvwhx.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2bhjrqfqy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2cbvdmwlw.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2xwgrhrga.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2kmllcjih.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2lyyxvyro.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2zhokhnfa.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2rdetnnkp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2ybjoqkxi.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2mwtozhds.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2tueiwboa.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rftjamfg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2jkbgzjam.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2dlhhbdpt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2bvwslabv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2vfpelksx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2dlzueazy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2oygfrceg.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2exsztfar.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2ayclaxwy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2ukukqkqp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2rskbglzq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2lslllcby.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gbdqldbu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2xdkplzil.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ekbafzao.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2nhkxzpyv.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2tzomktnd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2nfcmejtm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lzdmlnfo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ajducoqf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2dzqbzlyd.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2hjcmvcoz.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2ynkwhzqu.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2fqlcrafj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ihnvudyk.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2hakmutog.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2ztbyoycx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2aupisgad.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2ejywwidg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2yvszhtva.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2xdqbnkji.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2pyhhubmw.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2dczijtan.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2mkzscwkc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2eiydvfvk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2nodiwijn.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cflhronc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2abemzgar.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2pxmngago.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lcgkyaqt.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2gnfoxwtm.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2vothsajn.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qbobkfti.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2ycgkciqd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2ygfjfost.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2vqhuczcd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2awpxkhtw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2wsvfwmai.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2mrmhnnao.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2ylnpzxdc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2cqygchto.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2cjcghcaz.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2zhwcnndh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2dgaebsgs.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2gyrzsziw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2bmxttvoq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2udouzajx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2adkzcpqi.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2ervpokxg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2spbzqsqj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2wemgbdhq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ptzmonph.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2cmhcwwmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bftzdydc.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2bnnocszr.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2bxdmomhj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2dzckkbbg.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2nncrhydj.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2effmuxwm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2qvtosquw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2brysamdz.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2kgzglqvf.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2pzgicbik.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2lntuwswk.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2fpzahisv.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2xzzrdifl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2gyosxwsp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2azvczink.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2mnskzqqw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2opqshspu.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2kkkyqhip.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2sblhzsbk.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2kngpgntk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2znujhsna.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2fjofwzyl.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2iaexszwe.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2ajlvhtfw.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xpgpdioo.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2wirhgeuw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2fdryhkgu.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2ivutpszm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2dzjbzrwc.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2yzltcdoi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2gksatxyr.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2fjlmwtzu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2grleuywy.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2plndiivq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2ltmkgbgq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2hkwsxtyp.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2nyriygie.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2fgetddph.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2bsnaflql.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2ztxxueqq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2sktqwlzq.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2fbloopgk.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yeypzssg.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ddxteiei.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rjetnvhz.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2wqxpiwuy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2ohnauyrk.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2evgwlttr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2pvpiubms.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2sgjldcou.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2eqzzpmpk.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2yumedtpp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2tgnwbenu.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2cnlezzze.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2xphuakoc.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2cvqqkyon.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2ldaycoqh.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2xnhtutrz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2bvlfcnlo.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2eqdaogjb.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xnsrxrzo.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2uouwpuro.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2acvstshx.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2qqvjbfvv.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wtuwnynm.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2rimrwdtu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ielyvikq.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2hpjmkuoi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2iqiwlomu.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2vbispopa.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yknsdzot.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2rfbkibzn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2tscqrmlt.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2syimeton.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2jdnsuqnr.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qbgpfyiz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2gmtaunla.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2chxforov.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2ycuznmec.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2zoghvvxo.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2uamfcfio.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2ekxvfiig.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2nperknxa.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2urfbqeii.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2mhkowfzs.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2nymtvilq.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2gjsoofmy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2tuwuubfr.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2jjgahrek.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2jsegeeew.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2hipubrsi.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2ahydlwpg.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2cirhglki.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2skdyblpw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2qlfyxiul.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2uppblsjs.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2htislshl.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2cxokuulj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2fmqxjojw.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2zxmpekhu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2twgwsitc.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2thqlpuou.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2lbygfwon.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2rfbhczqy.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2qfwayjou.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2rvgqljsw.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2xjzmssly.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2ldoyirzi.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2ewvtcmew.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2crpfoklo.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2dufoukej.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2abnejlgl.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ommelgej.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2rrdqyfrc.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cvrazxgm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2rjhnxpmg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2nbpfiilv.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2pwecxnsn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2bxdgbelx.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2wnqkrsdg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2abdrllip.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2aggfvxis.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2lfynvvbt.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2qbyoihwa.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2npftzldx.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2wrldemsi.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2krzoqvle.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2hxtyjhrm.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2nmjjryns.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2shnycjgv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2dcrodguh.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2hfmgorpv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2yzjkbmgp.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2bikxexmi.html


<!-- 参考信息 -->