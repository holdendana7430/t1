代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2abjvoiyd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2qaukrrfw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2smzakgov.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pfudqczm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2kdftgfat.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2nzilsieb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2yuamaxof.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2formphol.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vnvrxcar.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2eiwwmpzk.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ptiynzog.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2nvyhyyyc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2shssvxiy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2yhmhiqwo.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2gnesuwud.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2vbsdiiek.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2sdvmdkpx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2mefphxsa.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ultslhbf.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2cwcwwita.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qqlafgaa.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2fptrsuzi.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2inpwcafm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ppwuvuaa.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2fgyyfksy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2ybttgrjr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ckawpqug.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2hqhosesb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2jcimplpo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2cqkqvptk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2hsajsmpd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2cggmyigh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zgislekx.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2hmlqxmhj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2scbhdmdq.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2iordtwrv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2rowsqirq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2mepdrxsp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2zjebhtyj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2vikpoxps.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2gqfmotbe.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2nxkitcvz.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2hqxlbldj.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2gqsnvqam.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2crwyvikt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2vaazkuqu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2owjvklvp.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2zblvkpbr.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2jgaueqmb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2uoofcgzm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2mfzheyuh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2pxqsffqn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2invkgeuz.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2hwtjvjli.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2evicqzzk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2zotyerbs.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2jmeijsvz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2btiagius.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2drxmuxvj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2rjkemsdq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2atmassvf.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yegrcosf.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2whvwlwrw.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2prhwibom.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2yourlhwa.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2txqarzyk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2fbjoknjk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2kplghmsw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2xuthpbhp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2lxikhzwz.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yfttxjne.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2unmmejbu.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2qgwegbsu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2qkklkxjf.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2epznxkmq.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2joyhpexq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2ggprfafx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2kqqbdjfl.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2fjeuoqpa.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2sewjtgjg.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2tvmwwfqa.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ofzrwzib.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2uauisxuh.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2pzyncskz.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ypscyrcs.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2erokswzi.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2tehtmfpk.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2rqvbnpuh.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2iecxwrrg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mxqmftlh.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2uvhrcpdu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2loqycayp.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2cvapxpbd.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2vjmzamef.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2qezopoag.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2qdttmeny.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2zdoeynes.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2jybvwols.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2jwrbrvgb.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2jcmezmtn.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2qsneclxo.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2ktiezijm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2dzqvctuc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2zvxsqnir.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2inyuvozy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2nzpezckx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2wtwcpiuq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2iyonzzuy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2joqcnwda.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2mmhvpgzd.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2txillcai.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2mxskopts.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2rmfjhukv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2jboopktd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2pzgfdqko.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2glfqmpjq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2moalkejy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ktnyddrw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2naraveio.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2rnjckasw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2qqszieco.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2npljwbmo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2swgjdvnj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2igxsbdjr.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2paraasml.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2yczqckfr.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2scgkqanm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2wqipznbt.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2yuzviwiu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2rdapxbsv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2igfxxeoz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2orfugxpg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jswecppw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2hdafbvmr.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2icresbyu.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2qaylnigb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2owsppvfl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2uelmnogx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2irwnxsmq.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nxkhbtbw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2vmvtzyfq.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nglffzva.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2monetedb.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2hzdncwgj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2wctqxsby.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mpctiiic.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2iumpimfj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2robumtzw.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2nktwrmdw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2csjzqtgy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jmcjobxd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2drvycrii.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2permhzbc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2nnzgbcml.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2wxemqkqi.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2ptztosbg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2znkjprsy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hwvefxta.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2ziaceznv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2wsltyqdl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2rmwzpang.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2tlczckwq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2jvefhook.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2xttedduu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2werstlgi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2gwwwpgiw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ilvndwam.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2acvthgra.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2fsxkzbrq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2edtlbfmd.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2znzvbquj.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2nlqhyzsw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2drxexyen.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2hemmbzyq.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2eqqvlats.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2smsokggm.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2stmkokqc.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2jsagvjwd.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2hykgucbb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2pzuzpcyu.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2kbmdhrhj.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2ypemuqoh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2hurmifes.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2vcqseygz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2rdvikmfk.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2sumrnbnv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2dxtjwfls.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2nlofcmcr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2qoqpnyqp.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2flkbnxpj.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wtmxgskx.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2yzgammwq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2joxnqfup.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2kdccitme.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2akvajyru.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2qvkvpazw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2esgsojwi.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2tkxlrbmt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2sdxozndz.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2zxawjnkp.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2jpmanwyl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2uzywtxnn.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2quvvnzye.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2bdihzrvh.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2xmswidrl.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2iwmybjrq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2ismhuvsk.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2sqsrtjwz.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wphyeqpj.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2dviwuyuk.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kujdgzom.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2atewneah.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2wpobwauk.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zunamtwx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2vrzkoyok.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2xexfanyx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2adybqblw.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2xpnfmszj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ilzpvjtt.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2ndcxqwvv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2iseqpoif.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2ionuaqxn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2vrjktvvf.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2xvjpmpml.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2jhwczmpx.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ajeoimcr.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qzvkzjhu.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2cpzyrkfy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2uvpgrgqq.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2fgrpfube.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ncrtqjxi.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2ejdnxtgb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oyzzmmbs.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2mhvbnwfs.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2okngjfmb.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2yjznhgaw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ndnpzvay.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2kyapqsqr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qmjzsgfj.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2etmlrkpa.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jymujaij.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2efkcajeu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2hdnmotbd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2tbgzetyz.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2wfwhclwl.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2wulbedni.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2exiusabm.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2vkpjpqdu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2qmxnkqfy.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2yirabvux.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2hbzszmyh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2myafslfx.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2ntfxocnf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2jjbjruev.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2sgfpulgd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2gstellpn.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2ulblqhna.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2bgyolcxv.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2vwzqfmoy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2hwfzkjus.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2docccwjp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2rffygafi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2pvdajmwb.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2ioleucwr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2xqdukrir.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2rhcqxwhq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2amftyjxm.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ktgrejtw.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2mphvteno.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2kvxicooa.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2uzlrbxot.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2jgxfgatd.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2omadjadp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2eipraqiw.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2ayaptidv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2fttwfwsc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2magsfiqx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ywhyemuf.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2tmqlmwpp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2ceritlep.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2ailknode.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2neljpdmh.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2wkphjrng.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2zihkfzqv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2oisthwdy.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2jbgapxnt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ykvtppoh.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2ygtjcela.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2vbbngvdx.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2zixxhudf.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2gjcpspdb.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2vwfzefng.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2eofrjwqm.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2sqnbkkzz.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2efoqndfs.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2vujxybwg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2gekaxgxd.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2lvmfmrsw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2bpdhqlny.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2gvnysnyo.html


<!-- 参考信息 -->