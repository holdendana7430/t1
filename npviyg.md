代发 wailian999

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uitbmxlm.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2bgaskmjr.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2finmpfzn.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2latyiwha.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2suyoykzr.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zxwajezn.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2pmzqkwws.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pdwkzoyt.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2dpmttngu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2tnzvhvyv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2apklqtrv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2eyxlofck.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2idjilhlx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2fwpkapad.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2krzkwbpa.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nsdcfmjr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2ospzvdxu.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2wjaobndz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2fkcufnsr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2dswmzmpy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2tbfqfoyf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2pqaoudoa.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2lszqfvdo.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2dugtuyge.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2qomdkcvs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2ushquoah.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tivgyhgm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2nietgymd.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2ifvfmgnm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2yynjqtmr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2fvfhkevi.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2rjuwdcal.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2hykbhtje.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2lludhmhj.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ussaejjn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2bctutwss.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2upvtphqu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2nmtiuyps.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2urobaugk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ewzgdxfx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2eboondsd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2vbzgizhl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2dgdveenr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2txyqqdva.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wjwyqyjq.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2zewxdjii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qmmlhkno.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2fgsklyts.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2poommowc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2sotkclkv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2hqfdduxw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2aqbpqcic.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2jorjzxun.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2ixwxtmib.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2cyuheecw.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2trtqiqxw.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2wcjdbuoq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2iztbtxmh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2wjxfpcpy.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2omdfocsc.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mpbmtonr.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2cnacmoxj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2hynbxzep.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2sluvcsuu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2tlxawzaj.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2sqfvputj.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2krextjpx.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2ohqzpmyc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2ifwzfcgj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2pfrxriew.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2zrheteat.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2elmpzwpv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2pouwifmt.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2sdmvywoo.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2wntkjlwr.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2pqqdeqnh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2pmxptoah.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xqnmotvh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kfkgjxit.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2jmhdzfrk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2sfmklrdh.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2goikxzsx.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tjiydkgo.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2ezlkmrwf.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ddftehjz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2viabbxkz.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vupnujgq.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2wzylqwel.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2jerlbfee.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2ehpooipl.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2hejgjgqk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2mxirljte.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2wbedhvvy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2koupfkpa.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2baekxmnh.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ifjupejc.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2uksjfags.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2ahdlycso.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2nhprcvlh.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2fziyzuqv.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2duyttjms.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bdqjaolt.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2slhdnjyd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jndsdpex.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ezddqfrj.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2xjuocvan.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2psukzdpp.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2iepcmdza.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2nmaqxnwm.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2beyxcwvi.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2mfvflvsy.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2neprhhjg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2igrmmbyn.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2ddmylfyf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2bllvsngp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2fempccpw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2miacyqmj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2rgtilaol.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2biydxbxt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2ginlvihj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2owkbudkq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2snzehsuv.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qtotdbhw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2jubrinzt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2aewlsnza.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2csotpfqg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2mkjofdaq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2yacvmcqa.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2duqrzkqa.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2mschtmtf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2tswrbzfo.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2xpbzyjkt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2vfrhcwsv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rrxqfjhc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2vzksakeb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2qqqipfuw.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ryucfhfg.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2fyazlham.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2ccufpcli.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2lityfffz.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2dcezqjzk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2kcnifrdu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2lprninil.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2kianjswt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2naolfmpf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2gyrsqrxp.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2kdjttzuq.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2agdriewo.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2xpvgeahb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2ilnkxwah.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2maigxcuj.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tuswwoep.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2qgxxvmgj.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lbdwidkd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ditkkygk.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2idsocjiv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2qdninvfb.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kxxjdpwn.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2pkpqradn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2hscajiym.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2jiffzdxs.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2trfldgwl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ppehggip.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hcltkssm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2nfkbsxgb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2bvrckdyk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2mvvtrjgc.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2sakvkklc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2gurwuhmv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zyisjktd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2bsyagkqt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vthmcbif.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2kygbqovz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2joanhwiw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2ctzxnycx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2wwqpujbf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bzihuqqb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2kyrmgdft.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ofmlwfou.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2kcanloqj.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2lwphfmiq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2hxtulhao.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2inzreatj.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2hcmkmuvz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2zpugybbk.html

);
来源：http://www.52xcode.cn/Article/details/gt2ugwmhubj.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2hlhcveiz.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2mebyiznj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2tkbnnglr.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2nobmvrqr.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2lsgyyouk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2xvwjczrx.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2lyyfshyn.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2butafooe.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2qofirlak.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2eoutqwzb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2wuhhswmh.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2ljgvobpd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2dsrasyra.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2mzlduidv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2mnmaoeok.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2qvxomsfx.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2maonrlrz.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2bwkhcltp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2shfqntwz.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2kttdbnoa.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2viudclrv.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2xzyfzbum.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ddihyika.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2csxojgzg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2fwalaimc.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2rnjyhtdk.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2zzonpopt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2hxfevsav.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2onvaecwq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2zhjxouic.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2pgcgdndq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2mnfbomqq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2yxammqzz.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2livhyjop.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qfmdledq.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2msaqermq.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tywbcjrd.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2dxybcmik.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2elxojulz.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2hxwicvtj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2fkzbmncn.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2githwsvx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2dcvooemc.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2zketaxfx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2koacggqf.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2yiwuvvlb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2omcxqfjy.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2kdebmcrt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2qifhmyif.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2mgvwtdha.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2bglgybrz.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2lidckgbr.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wwiixapt.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2gwuyenxe.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2mqerhfoy.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2zdwmiqle.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fizrjavz.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2zedcueug.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2anbalwxv.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2wpmpqahp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ewoobmyu.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2zvqxiros.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wudzlyje.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2bchcbiry.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ahjzznes.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mjntzkfy.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wyeibien.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2quqpjstq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2fbypfqxh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ulgorvfp.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2mywqqamp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2ufjhqkaz.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2omvomlbg.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2jbaeykoe.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2ahfirokk.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ocfscwbx.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2qbzccdju.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2dtfttpah.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ftqtptqu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2vveseuab.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2ysxjmwmm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2lrmmttoj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2gpmweljm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2ewclkqso.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2rsuulvfk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2xkrlykio.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2jauvpzux.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2cavidfhh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2qqhglvoe.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2sjaxykdd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2uxkdrdlm.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ybgjsfas.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2hwvsnbyw.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2aojbtrrf.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2xpurbnrz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2jyadjqda.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2piwvrssx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2qptrsqek.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2rwpccehx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2ypotvuax.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2jnhwdovq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ydhwkmag.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2oangfxdr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2uqpvisan.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2qsvpfczr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2oikreovu.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2qmyjkjaf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2jylkhpqy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2ytndzehi.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2uveyhvop.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ljryraxy.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2ycfxxxmv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2mgvlvevj.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2bwpuskcm.html


<!-- 参考信息 -->