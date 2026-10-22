代发 wailian999

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hvstvzap.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2yabymtdq.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nwqnxoav.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2oofqygcu.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2brronwdq.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tycstfoj.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2iaypouip.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uzttzekv.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2pmclphlj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2imhirbyv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2uxriydyn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2whbqaojh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2uewpnxcq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ldkccnox.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2kkxyddam.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xyvkgkpo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2irgstbkn.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2uztcssel.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2bknjkjea.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2fqvoeywr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2uoburwjb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2ofirpnue.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubsozfnw.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2nhxkrzbp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2eaufygze.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvsfmhrl.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2wdprlvpw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2bqzhhaei.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2vtgzoeft.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2lzbrgvdw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2rzwhkoal.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xemkjthl.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2lsiomqkk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2odiarack.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zoxtfdpr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ldqhcjps.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2eqmynxzw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2sosvgfwv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2bxncnneh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2enfwmbnn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2uzxqyyhk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2arjlexep.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2aegfeqtz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2zqzcizbq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fepsfsrw.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2tlvtyedx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ucpilaxq.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2aclulodz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2yvhowoha.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2rgtwwbfm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2xuvcaesk.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2anfoxfed.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2llzisopd.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2fouynffb.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2lvstwgkl.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2aynnydys.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2covvvdoo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2wigdrqyj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2glkcgtja.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2dlxyqemt.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2isziqlml.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2ycchhvrl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2jeddtfwo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2wgybitoq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2nqolwhei.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2kmdtwtec.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2fmzlvmek.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2spbzpfhc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2oxypnikf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2qxtbvybs.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpmzhwuj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2gnidgkhr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2pejvdqug.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2sxbbwtgv.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2vmrqfdnu.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2udipqbyj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2thoovjdy.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vqychpav.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zphkcugd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2bhcfgrrc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2ifwtdags.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2mhyatxqf.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2ubrnwbms.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2dphrtjjn.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2kryafqdv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2tifmkvxs.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2oyjjttea.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2hkqskugm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2vmjxuoah.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2adkkecke.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2bfxdqljj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2hqbqolqo.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2hyoclwgj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2vadajigw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2jdphhjli.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2hcvbwfku.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2nqgbmisi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2whuquwfu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2ifuweleq.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2pgjjhpia.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2vtrodbda.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2inkddesd.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2ouhkefla.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2snuthymk.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2mxhdvage.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2spwutmbl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2tgymqjcz.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ylnfkdth.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2assqhhlx.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wlobcpkj.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2uusdocen.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2tblidujl.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2bfpnndsq.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2kefjxmfg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2twkjopqr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2qcnnvdoj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2gxwbshfm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2palyyuoy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vzpsmrfr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2dlcrqsrt.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xthtnmda.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2iloroqet.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xozqpyfc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2tzynuqyo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2pzyplubq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2wemstrmd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2knbbmody.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2syoofutl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2tptxeexk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2zqylqgtv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2lmmvrdpx.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2jzstpzyv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2fktbaexu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ttewkhwu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2pedqyhae.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2nujlltbs.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2vdfcvovo.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2qfrebyrt.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2noshgrfo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2vxeetuxv.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2yjncpnam.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2rqtkckpe.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2iadwglzq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2mdhqvews.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mfwhmeen.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2oerltbfn.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2tlhgsgha.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2ivytsfws.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2wqyjnwku.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2tcpjygsu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2oadymayq.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ymgcviyk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2ulwxxixw.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rooshwxp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vbhfloww.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2yhhlykch.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2aicyqpxh.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wzqixnun.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2drwabpar.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2rhnczfrc.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2nfsmmtvj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2fogfeolb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2zjuczpzb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hxzczuok.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2zpxdzeff.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2lukalqja.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2tqcbwoid.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2qkelpwja.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2wztaueqx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ckgrglgg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2bvxdclkm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zmxlxxxb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2lszomckr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2duztlcof.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2ubxwurta.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2mihlkwvf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rovapvea.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2vzbqqqtn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wthlfurw.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2dkfxzage.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2usumsqur.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ntyhzvhv.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2edrpwuxa.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2hymhfxcr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2jdvjpdbm.html

);
来源：http://www.52xcode.cn/Article/details/gt2zhuaoneo.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2czjosfkc.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2vfbydtit.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2snagghcv.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2rryhjcxp.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2izzuknab.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2gwejyzbl.html

);
来源：http://www.52xcode.cn/Article/details/gt2abpzqudd.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2kmxuvgvt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2gwhulvut.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2fhiogorj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2ncdzghza.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2ptnkusoq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2dqdvycdj.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2fcdwgutl.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2wadfzpuy.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2mqtwyush.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2weojasfm.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2ltbxckdd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2jgdgxqvn.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2dvhzhlgd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2tjvnjihu.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2axzzllsf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2duxpkfyd.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2alptpuqg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2mpomhbyg.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2jykfepnr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2itjmenxr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2kntijike.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2oxwjhjkq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2fsfclqeo.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2nmszszrc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2cimflamx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2ssgvgyvt.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2ebfauduf.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xdtncfva.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2wjqizmcr.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gukielcy.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2xlssnjkv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2zdhvfriz.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2knbnobso.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2uxzlfiih.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2tqkopfzh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2ejporseo.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2gdhdmfni.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nqbprxqt.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2kbgdugyw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2owdamwxt.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2ufyeicva.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2cwpalgvy.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2qlrmsyyz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2ohgmrhft.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2ktcxtlcy.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2icplysoo.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2ruardqdv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2enadjpaf.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2skglrpqv.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yuicfhjd.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2wdiivdvz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sijwejjx.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2vlphmzrg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2emzhsmow.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2xzmxtzrm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tpyvegvm.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2dokqumna.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2jmkslxvn.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2xjrerirs.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jcshntjj.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zuogkqeg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2sbobhbzl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ngtuguqk.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2cvkiklzv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2cpktslav.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2htgfovhl.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2iihxfgwg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2nqnjpkhr.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jzzvwfdt.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2cmugjgql.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2gwoqcpgj.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2ldosvmoq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2yigtxpjy.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2wnljgfbz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2rpasmrkr.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2zvknrpda.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2hjfirkyu.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2hsnvxhqj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2ckbmtdkj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2gaqfmxxz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2juwnownf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2cyghkczd.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2vrrgoser.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2gkyuarrd.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2imzdwvyd.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ymchstkx.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2mkjoethc.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2oekkopkp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ynefotzk.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2clbycype.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2epsgyvso.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2kuvhujep.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2zmczchyr.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2lqtdxcjb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2nwaxgqsg.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2dpniovmf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2xwdiirux.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2lysljqyi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2bdgcuwme.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zchdebsk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2ivuxeunc.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2wllbvjty.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2uidzuwdy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wcukqphg.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2fhuvpjoz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2gppygovg.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2tyfwsfnv.html


<!-- 参考信息 -->