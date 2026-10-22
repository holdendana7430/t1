代发 wailian999

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2akyysspe.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2tejnjklu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2wtjjislv.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2gcxuomkn.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jrqpqcjq.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2javlwxuq.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2loikiani.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gqyxjdrs.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qcidbghw.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2medecwmj.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2nhbylffc.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wcmoeztf.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ybfidgbz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nymalxis.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2bbcqzcay.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2pncesdme.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2hncemluy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2eiogldao.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2hcuulfsh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tsfxaide.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2pbtnamqf.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2spvfekbv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2wdayxakt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffohbxyu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2yoosltmx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2nsnjxphy.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2yvocbfqi.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2sbhvdejb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2dkhuhpff.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2eyktoswk.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jvwwwcbn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2xzmuxncx.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2fhljsbpc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2bejgstrj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2jdfqbztm.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2vwqlvqln.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jcivuhkq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2edbhfzyr.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2trubyehu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2plcealwn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2vnybkoqz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2orecokab.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ghoslgbd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2gkgokseb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2uybizoky.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2dymqxtce.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2wdtzwste.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2kybciwgp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yumdiexv.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2kdrkdgyr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ozcovjda.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2nisxinix.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2mdqywsjs.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2gxjokvld.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2yngciqgl.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2sizypzub.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2wqegbmaw.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2xkygygfq.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2ozfxefzf.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2wzgmrzji.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2qkxtmjox.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2yoqrydkv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2drjhtmrd.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2aczsyhgo.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2hastnxks.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2nndvvzxq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2mklgnecs.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2gjtsgqjo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2drlqpjuq.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2buqacvti.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2honxabat.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2eybnneyi.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2gilydkfa.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2epmakaiy.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2skeykmlk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2qyriyslf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2qbrkdwbs.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkbscohj.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2olzsxial.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2asnhujct.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2wnmwnfbe.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hrlgdgmu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ntkzukvu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2isrlhmpc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2sagvilcq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2fxkgwftq.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2nkgkcbdr.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2kafmznqg.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2oggecmir.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2hvjefeky.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jmgjhhfq.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2isjoytyq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2pubgqprb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2atonqjib.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2utvbtnrz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2auwtcgxo.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2ubosxcws.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2icbrvxyc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2oxqrwatq.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2pzkfqqnb.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2yklqaywh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2kzrnvuhy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2xijxgedl.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2mmuqbeef.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2ixxpesoe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ckuyufhc.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2iagcsjej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2frkshher.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2rbpgofgv.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2mrrvqmfa.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2ymndebdu.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2nhakynab.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2poyygcug.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2mxknpzav.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2vlzvwbyk.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2jhcowcyp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2lqavigne.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2dqmdvthj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2dsxvqepg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2ymafknyb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2sxxckbib.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2jbzjqbmp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2fgqiphze.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2poalozfs.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2cyjyzwmz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2gnynuwwf.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2igeprujf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2vnknpgso.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2lfzklbfj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2uejlpfyu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2xxciyayz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2egsodybp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2zrbptcmb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2gzmrmxxz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2qinzeuny.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2hmfcjtfs.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2cxlcufug.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kdntwxox.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2zddgeznh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ylibtcko.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2anusbymk.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2zajieizr.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2iusovaov.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2tuhbutoa.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2yhnfhakc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2vhalamka.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2mslwvken.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2yyyzoeki.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tokosgzk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2uxwalssk.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2zmcyhezy.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2wdqkwhnt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2zfshzigz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2jwgkzkdv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2sdemhgua.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qjypmabp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2wlguvwmo.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gqgotjuh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2nraoywpb.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2ohmmdxps.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2npsacpcz.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2evlykaxt.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2kgzhnxra.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2ykudbnsp.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2orliuggq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ndpjlwky.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2rbpvcyfu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2bubwrkag.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2jbqrpvxx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2pizphpwc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2uteqvwhw.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2ybiuqnrx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2fzyfpiye.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2zfzcxypl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2zvvlszha.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vjteogrm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2dtugltfr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2wmampvns.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2daiacldf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2yzwtnjzv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2chrlzbdn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2hsjkpwjq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yjrmlkxb.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2eewicxuj.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2nspihjlh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2hlsqhaqu.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2nilfmmod.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2vcwqrvyp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2toteamuc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2eagceemi.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2jnnwlypr.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2bmthypsr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2rnlfqppn.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2iwnjyptr.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2dsweyujr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2xhnyhxpn.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2rdsnxmxp.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2giszfgrj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2exprdgcn.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2yaskkumk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2dgohwxal.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2eqtycgnu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2yozswuqr.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2lfuauloy.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2czgtkyqf.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2nmrmjdgq.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2xrhyqfvx.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2rzkxltpa.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2skdwvqtu.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2schytavk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2vgwegqly.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2cfihujvm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2tgdtoflh.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2lvjwxmuz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2kjoynabi.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2jhlilojl.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2pipfswsg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2jhazygvz.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2iujbajgi.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2fcwcwmgu.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2pdnqgqha.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2urnjsnwu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2txgynqdu.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2yxazjddm.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ytkpgxui.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2olgtbxts.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2puscprbr.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2jqncybyc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2dwiytqbz.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gylhaqlo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2ixnqridq.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2fceuxvjf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2uonphfvm.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2oonnorkl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2vestlrtu.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2edottlwt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2eeiqeugo.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2nlrqkvpq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2gkctrycv.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2ijmzfiwe.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2skgmbber.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2xdgddkec.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eioktqmz.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2qtcotdqq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2gaqrolbn.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2ryminhis.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vjbzzgau.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2gxdlvizo.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kwvtqqnj.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2cfjkgldv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fcpdgrrx.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2fxqhvblo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2moizewki.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2neofiqxl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2alwfxvmb.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2fsukmnxf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jcomidvj.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eycezizc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2bjyvivjx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2rbppnphz.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2vhkfksxd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2kvcxbfwv.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2hhyyhrpi.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2hsrsmfry.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2rvhnycll.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2ftmmgghb.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2ylrfevfx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2euddcvux.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2jpegeiza.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2lzgbmhwz.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2szvrgtjl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2uwycnbmj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2zemcsrxn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2wbeqhadq.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2tbjkolws.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2jooxdtnc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2dtyjqglz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2ywsnzwdg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2ljkoyphw.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2lldzmgdn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2xeaopyuh.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2yqagugkq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2nzzpboud.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2llwpvlzq.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2srsawdbx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2hoegfbjb.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2wwkuwoga.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2bcaccbzx.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ogqchvvd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2iycmceto.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2pkbwzmzi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2bfoiqirh.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2kulzprzp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2yrnkfcxn.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2qmgcdooc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2senfgsov.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2mscpyfym.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2letxjntk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2muthbsdu.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2iggmwbgz.html


<!-- 参考信息 -->