代发 wailian999

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2swwxcylg.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2bqydyzme.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2zzwthoha.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2jlnqshgy.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2okpgiyzr.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2osodlfjt.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2seuvwazm.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cqibfpek.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zndznktl.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xggrqyec.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ziutklpd.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2eopeatih.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2rcmelwpj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2lkmzptft.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2hukhmvcu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2mhracyjv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2walcdumv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2vqeiauem.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2ivqlntuk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hvwyndpk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2chabboxh.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2ucfaigol.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2rpzcsplk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ecofhvde.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2sqhlvbow.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2aozrxsfe.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2fvbpmfua.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2zyyhrfyx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2axenabti.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2afhrbtxa.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2fhoaaxoq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2lbbqnnkb.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2wtkcqkun.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2izsrlwte.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2tocfkgau.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2emywwjva.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2phfxrewc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2kwumpwdc.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2dvrwnrme.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2hxmxwels.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2wtreqjqu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2hysxiitt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2npxuyytr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2bllhuwdu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2hgxjcoxi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2eqfukmdn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2wanpjcdi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2zhfwwejm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rtrbzhdn.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2cwuifnzs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yoypvzim.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2dortfwiu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2snjlmygk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2vqqgvsys.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2ztmzlocc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2dqrtaajr.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2eogrilgd.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2fhgygrbq.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2jflhzwbe.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2lkjxmwmf.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2ftldzkze.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2fvjygccj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2atfuqfrq.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ksqmtrfg.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2megesweo.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2rnhzichh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2mdqpgtji.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2txafcpiv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2rlijnost.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2kwgcobvq.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2lwlmhueh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2ngewrouo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2igtgfcwv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2yxbtwclq.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2duepcunk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2qgdezurq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2yvtekjle.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2hbffyshm.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2fodlfohb.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2tshwcnku.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2nubnczqb.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2liarmnbz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bhoxnedu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2qtjwispd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2vtnnejlk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2vllrslwt.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fmyyrmwz.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2mfflvolv.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2stqyisej.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2iczzbtuf.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2wbmmdeps.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2pqbmlfsw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2dbtelocg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2jdfmtalh.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2befxbroq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2ndcjqpqg.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2gqkdtxts.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2rtqpowxg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2irdmxhds.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2pwxqjtdi.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2nzlbdckl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2wyvmbbww.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2dqnjrlyg.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2nipsdctr.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2mwtraexx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jkikjosy.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2uyxepcry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cbpoaucl.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2okxbnngv.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2jsctyuun.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2lsutdoty.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2hznmotrn.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2itnlouak.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2nygcmxyy.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2bibwtcef.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2zbbjanbm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2knaaeepg.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2fusugxpx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2fstbgohe.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lwcvhspp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2gmvpdnew.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2wxzpwjmv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2wabxhuua.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2kgkirmou.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2axgpvpgl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2wstjvplm.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2alcbcrdz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2ihddchfs.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2cfaostce.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2kkwadelk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2cwivsdsk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2mijmhnnb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2znddkwzr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2jwpchmdi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2daamoejc.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2qvkgxinx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2scvzsrvn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2shrpdkrn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2bnwnrevt.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2tmaxunya.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2kvrvemkp.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2yogtcgaf.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2cjnhuwpi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ankeyvch.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2vsndkuoj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2subczqzu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2rdthhcpn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2ohpromzl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2hpkaboek.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2giscfslf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2xelwrcjy.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2mxwhzsxz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2ryfpmsmf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2vptwaxtu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2jhcacavj.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hwnklfkg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2dmukixph.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2beizkuve.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2whswzwkl.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2sbfhwrbp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2iedtajsa.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tcglojxr.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2getfomce.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2xcrxohzf.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2fecjhqlt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2fgdoikkf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2npviprqi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rbvmpirg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2msifbcqo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2yedydsrv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2vwuvroph.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2gprfcxth.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2nknwsnnl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2slqgskyv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2ibtuffme.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rldxdnju.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2lbfjfshb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2tcaeimmy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2wldrbdvl.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2rqbxluwh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cwdzqjjj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2zdedzdxi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zgffgemm.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2jjpifptr.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2oqkyteqt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2nihotkgx.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2vqmcksyl.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2pnybyica.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2hucfxopv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ngnpbpbm.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2uskhblxd.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2wxpntrqd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2tmrybyiv.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2qjurshzv.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2pmnawlih.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2bguvhipc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2xollmxsr.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2fwjqrrfk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2pxnfutxs.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2lqtzhmpg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2stobqcvr.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2unrcpltd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2itkixuns.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2rlatpors.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2lubufqpo.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2cmsehyew.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2svikkxfk.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2cwkjkplx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ozsioeac.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2dqthfmxa.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2yrcrbusm.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2yzhoylgo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2nwdujovb.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2trqgovuv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2sktxmmme.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2bjfdngqy.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2nqmkfxea.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2lhmyjbpz.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2gnjordbc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2rpzinoto.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2vlnlonhv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2dmhgvesz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2gqkaknbs.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2mlornfbk.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fbngtehw.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2erpqzryh.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pgapqjnq.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2hjinkmzv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2eowgejbr.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2icovmicu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2bcihvivi.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2aexzhcoq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2csryxyxe.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2yqfbjpkg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2wtnvbtql.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2nqffaqcs.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2gsaenerh.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2cwdqakbk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2dzproxqi.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2nrqhdkrw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2luynthbs.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2fuvrgmds.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eametqug.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2qnhmeoxi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2qfmiyyyq.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2jgodlhxa.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tfnyyujy.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2okgzrqlp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vktkuasz.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2dtjvrvks.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nfubptjk.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2nnvdzjev.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oxgyqthp.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2fjeokikb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2quyzkfxk.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2ffggceir.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2cumybcpq.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2gttvpfoh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ouuvgyks.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2onnmevpa.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2wlsloqqe.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2romzqxby.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2qhmobtpr.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2pjssxcwq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2rwcqxtrx.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pumnhocx.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2inblnhhn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2jzmgwopm.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2dcsptdif.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2nwbqjtfj.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2macukltc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2gkrnxlaw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2zfvlgart.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2qoxqfiow.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2ewddpsej.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2iyztzlvx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ckjpmtsa.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2giiaplzw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2pcfcpmgq.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2qqeitgbo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2cwkuvlsf.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2dtznhtfu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2uesrwrit.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kifutzua.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2wylvefzt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2bhfcbkct.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2etfvlvxz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2zdxsxful.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2srkhbjnd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2lcdbwcsb.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2cdyzhysu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2gcxpjsyi.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2buctbmre.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2jtxkeduk.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2czdwlmnd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2uibjjnoh.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2uzxbreqz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2lpcjauiy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2zrbkbfud.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2hymymvhb.html


<!-- 参考信息 -->