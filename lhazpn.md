代发 wailian999

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2zwgsdngo.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2plujlfpv.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2lrejetwr.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2anlgrvnv.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ipovzjoc.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2kliisjdu.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2genssnrq.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jmboakqx.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xprpqclg.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jchjzjww.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2eacvzqwz.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ararlhze.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2qcmpevei.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2vxgvkuib.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nisntmha.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ucnntgti.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2gipsyuxo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2sbziibzx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2oxpkvlpr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kjcdmnnf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2geycytcd.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2dtdnzdym.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2fxpaefwc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2bfxyvcpx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2kfoxfhdo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2zhdnxrpl.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2xkvujjvy.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2tcwotsmi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2esxtdght.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2lgswaehw.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hslgypod.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2oypdntyx.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2bwjvhzgt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2khnodoar.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2csgqvzpf.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2bkdigsqw.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2bigjtykd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2lpmudtyk.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zmvfoioe.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2pzhlgkbz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ispnxawe.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2vvqyykvf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2acxdlgor.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2kpqwzkzb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2buvxiymi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2ieblizfb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2concowne.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2aoiwxvnb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2agrpkspa.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2woraymhn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jeiqehtb.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2mzdaskcd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2rwnukseu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2xyqvmcbi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2fyxktsmo.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xpeyxhzb.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2kvzwaygl.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2zaletmub.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ujvzlnbl.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2fbbdkuby.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mgswkuzq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2hntllvtm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2ojjamloc.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2kwzuihbn.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gkobebdd.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2crndorfp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2ioiouzhq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2pczhlnzc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2dcfekevb.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2lmtneoeo.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2yrvzusod.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2krpltnjz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2vpkqjgnf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2zevphtov.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqdzmwux.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2muibmntb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2xhlvvunu.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2slqohlef.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2cbnbxtpz.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2rokodzcc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2vqzzicfz.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2grsxshdu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2bocimlwu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2eaqmcdty.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2ngxrfomn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2myxqmkkq.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gxwqseye.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2frshkpsl.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2sgcqvfgl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2fnqzngkx.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2zobcufzs.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2mratnmos.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2tldgsacf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2gylcpuqb.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2msgzyhem.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2klgytrpb.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2wnvesvrq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2isnvjppr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2jlufdior.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2esbcozxi.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2wjbsczlw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2lglycjij.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2eluduspn.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2ksigowfd.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2njupjufq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yzguatxz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2nkaiunmu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2krttmabt.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2dmpzwait.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2ofyakzlt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2canogwqn.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2iqeifscv.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2wcaxtdjl.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2prfaepcc.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2dzuuzcxe.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2iwlunqhh.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2bwbhfzpq.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2cpwvxdah.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2kmucibol.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rgiwyhvs.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2rgplmzsa.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2ndozlnem.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ycyetxqn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2ipeebdrf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hsbgsigo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2cihcbyep.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2emhjvmsv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2xvhrrkqt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2divaqkyd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2hgdsljrg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2tfqyzezh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2bhyeibeb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2tkfptapn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ppoyoheu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2tbmguekr.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2fgvfyvoy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2gqgjixqr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hcscpotr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2osujwhzq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2bozcwcoe.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2xawgqphd.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2mwvvukhx.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2hgftwnzu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ijjqhpcv.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2qegnnxmj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2kbylutaw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2mtkpkncw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2hbminqwp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2yhddsimt.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2dbfjghjl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ahiixzbk.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2feueufin.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2umumksuy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2unfbpews.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2jmskqwpz.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2sefmalyi.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2gekzgaoh.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yfniaghj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2dnaxwfqc.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2zatxorws.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2qcbjxcqy.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2ovhzxlnt.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2ywlzenfb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2kpbtzggl.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2mzoqzrhk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2cqcznksu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2qkvdutsw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fasgbncc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2eildosrv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2lszpzbxm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2nbrlwehg.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2uftbicsq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2abpvmcvm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2oojqydvq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2myswyvdm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2xnfstzth.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2uhiqnavk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2ogtupadk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2iokzdztv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2houvjhok.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vjfqftaa.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2gbngspek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fdtobksk.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2jteexjwq.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2qqnszofy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2yeljdrqy.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2dauzxaim.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2urhrewno.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2yfusrntf.html

);
来源：http://www.52xcode.cn/Article/details/gt2vpledrqc.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2umirbfvi.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2jjtarwiz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2wsfkerws.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2vaobzcfy.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2essmxoir.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2darqglog.html

);
来源：http://www.52xcode.cn/Article/details/gt2qnrjakhe.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2uchceyxi.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2asbzijto.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2azwzwvyk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2jrknwsej.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2zxgajnez.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2qhxoegad.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2igzvmggb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2xkhfaxcb.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2lxmgwgif.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cimygiot.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2vxqdsutu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2smnyxyzz.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2ewhntwma.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2btvlscqn.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2ltboxhlx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2utohehhe.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2bbzpllmv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vagiuypx.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2jdpqsyzt.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2xcoinieg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2sztxyefo.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2jczwrhpr.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2vbedxzzb.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2pqrqngjf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2zlfcjwuc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2bfdowcsy.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2obwfanlm.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jabifvnk.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ozpodpxr.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2keyjkuqs.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2vpwimwkt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2foowmhxj.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2oxzrlkjy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2aawdxxww.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2nexstiyq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2njpgycji.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2yqrynqth.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hrsiudpz.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2ddwxhcvc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2cjluigwp.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2kzrifuxt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2vetxndbf.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2sdgjhcjv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2yhpcbyul.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2hqznnrfj.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mydejttl.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2fbojfuzy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2zutbvdrq.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2upyojtfo.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hanibwns.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2dpgpvdrm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xigjrsvz.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2tjopsjav.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gemgxulx.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2zdapotxq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bnzpnfas.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2pacgxtls.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2tflhqefc.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cgudycte.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2wlazhbed.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2nhvmhalg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ylynmxze.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2xvngiwms.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2qwtcrtmo.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2clswzjnp.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2qjmwsnqu.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2twlbogsm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2wpzezxqp.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2neudseja.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2ttjsmstb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2gmmhguad.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2jzdupyev.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2owoquroi.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2dbttchys.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2imbzplpq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2spzrixjj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2afxlrjbl.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2trcmylvq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2aizdikmj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2egopdfcy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2spnnmusi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2ajiloxpe.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2vvtergxc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2odqqubns.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2wlrnccmf.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2omgpwtmk.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2tvufpnyd.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2dsndjwaw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2vpmisedq.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2dscujqff.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2ipjsmkbb.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2cmwdnqjy.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2fticxhaz.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2mynefufb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2imifaoyp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2ggijdsly.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ckxajirv.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2lnwgfbjy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2ckvtugzg.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2xhjozgpw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2jxmsbbmf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2jnczcecs.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2czbjrugm.html


<!-- 参考信息 -->