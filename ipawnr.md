代发 wailian999

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2tinidifx.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ttbwwujb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2mhbdhxdl.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2pnlyvwoc.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2deywtmov.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2npzjeffk.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jpzafhys.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cmucijro.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rjlgzxcw.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2macsooxu.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2uvrqijkx.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cxqjvbjw.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2wbbdhkij.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2flzpevqd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2tzrkvyic.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2yprjfkyb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2bschskar.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2uwrobscs.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2gbzlshhv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2dpugdekg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2letgchkk.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2yanrstgi.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2uvguzuit.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2vplyhovv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pbxbzvqz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2dvpqywub.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2cgaznjjf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2bhtctvgi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2cdqchljo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2ipkiznhg.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lrmphhdv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2wwzbtjkb.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2kadyakwo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2yttbfsac.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ealrokls.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2lgvmfqep.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tfzesejx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2qxeyogkn.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2oofrargi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2xmjujqwp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2edgjwmhk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2obbnfxed.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2iqqyjxnk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ipxvkpjo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2utheplmn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2kmpikfjo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2qiojuwql.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2empidmwo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tixalgya.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2vqpvhhtx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sxysskiq.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2ccpbosnf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2aibizltn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2qpxdnjod.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2bkoefqos.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vvytqvqc.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2vqdpybky.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2htugbtoi.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2qkmjzrum.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2dvweqhkd.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rhqvojlf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2xexmparq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2kpkrniyq.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2hfvxtcfj.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2artynwbc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2rarnrtdd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2lnudxctw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2sieudjnv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2dtoijqco.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2pphpzplk.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2qcfprrzd.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2iungykor.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2gyuxfwof.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2srbnmhsd.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2loqnzepo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2evobzcwf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2tglalaiu.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbcxvrxq.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2mavtasaa.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2vemrdxoz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2ffuyuuqu.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2sekfoxpo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wgmebnjz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2bgqmngby.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2gwvwahvf.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2xtfaktlq.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hqhtxkwt.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2hkfbtdzz.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2utwoxlah.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2itzndfkf.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jxvmuuzv.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2zhnukfao.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2icrotaen.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2xjixeytx.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2zxjnrtne.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2rmqpfvzb.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2orxuijkf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ckvyyhkv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2zbladjfm.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2nejhpxce.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2mvwsmlvl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2hkhixfhh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2qpyugssu.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ugaibasl.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2imoonpxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fgdpsjiq.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2pxvygdwa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2evtrimab.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2qmepfcbs.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2zhifjoqb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2yidpopet.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2nnucxoum.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2lshnvwxa.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2awkyvmno.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2tyrozoyy.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ooxrrdml.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2llpnocpg.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2ovhyosnl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2gstaeyct.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uicnxfpf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zbkyhqdv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2rkegdcrr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2anxelcbh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2aewnlbzj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hzgmegau.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2basnwqpy.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2uhwvzssk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2fvtzgjtv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2tnjvrxll.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lxbyoklx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2doqsrwid.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2auygqfhc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2tarxstsw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2hwhxgxlb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2ezlrykth.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2enhofxya.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2smdeowpy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2yswjdckp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2tqwodxbz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2pvsqnycw.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2jyffkpyz.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2vycphkfu.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2riizgxut.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2zbaxfcjx.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2bsrnqwbo.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2jjcczsrp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2mvmcanfi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2ntzmtqzl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ejsffqiu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2rpamrnpw.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2nwjjywqz.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2kuwllngc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2qjkzfobo.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2axxgseek.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2xymxjpdr.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2nhftobys.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2kgttzdvm.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2yjgoqsuh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2swlzalvw.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2mpwrbypg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2ylfkvxlm.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2ksjgqper.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2hqbcxkak.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2zdghcoms.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2dohyrwvs.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qejtmajo.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2yhyjeron.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2eleosbuz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2iikazzsp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2lxdufwuy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2qpggimjv.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2zrlrlysi.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2doeubsnw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2iwlequoa.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2nrwizdhv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2wphqusxu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2fgczbghj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2ekgwxxrg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2yqruhoce.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2akbmdwzw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wzrmhmso.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2quhopqwf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ivzmhifh.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2xqlemcff.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2ofhmitoq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2uyhenroj.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2hzdbktvq.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2frutlhjh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2dokqdsqg.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2areqoakn.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2chrupxxs.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2xqyqhyon.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2pudgxzhy.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2sqrimpiz.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2jigwtewr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2amccxdby.html

);
来源：http://www.52xcode.cn/Article/details/gt2skqgmnve.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2phhpvdsg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ubdpzvrz.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2chmgwbyb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2rkawzbvj.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2nzejlajs.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2cnupzuix.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2vtazpaqk.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2dklyolbp.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2xdhtisyf.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2zuyvknna.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2xraoujer.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2tpmagcla.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2wjesiqkg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2noalxxhx.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2umndalwx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2gxnnurww.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2vobwevdw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2hfchcvvs.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2dakznznl.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2ejqpbuax.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2kmatvtgq.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2ukgmnknd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2yavqgnbu.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2mfskyltp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2hklvbany.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2rwndcdxa.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2qhzplfcp.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jfgpigmt.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2qzssekku.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jiwjomag.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2iquspxye.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ptoskaes.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2leslqqan.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2rpqtnmpg.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2gppaohko.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2urtjeuae.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2zrexwxik.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2qrskgtuk.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2lrqghztd.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2uhbbzpsl.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2khkfsfuc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2vmgxptww.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2wjoyvmoz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2xwcnhtsc.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2okbwwnrx.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xifxdmhn.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2djcicriz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2maeclzdh.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2fuvhvjtk.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hqxizhzz.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2wjvpjvuk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gtgmociq.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2dwywvxrt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lkcssyht.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2thmveuxb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nsodqhkx.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2titpouak.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2nnndejnu.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2yeiwjtky.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2cyvsajuu.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2klxvjaub.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2hhzwoqes.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2gaklvwin.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2jvrgasoe.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2envxxlye.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2fhaclqpy.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2unsqxwse.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2qwwtcmjt.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2juqbuelg.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2kzqbfssm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2joijvenr.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2ngmthvja.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ldcpxdjw.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2zjfbnods.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ofdnyjxj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2dtjxtznt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2tececoau.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2zlwjikah.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2ureayebn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2eevtoaym.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2wanxxwam.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2hqfyxdka.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2kujrxpst.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2emwqyhbp.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2evrscuid.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2cppkmkzj.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bbfcmnqo.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2jyttmevq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2sarqljdh.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2bpzxmmba.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2gkmeyzji.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ccyliciy.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2ewpackiy.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2tqrierrl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2isrjlgfc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2dtdgfyqk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2rcezwaai.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2mkjzjffp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2kqcflkwr.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2wvtshvwh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2zhwdqmmy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2tvnzasyd.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2xlutilnz.html


<!-- 参考信息 -->