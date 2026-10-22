代发 wailian999

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2shobjwhn.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2ejeyoqry.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xtofefmu.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2joarbsqc.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wmksfzzj.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hjjeqdxw.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2ktdqqjyz.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fgpjywaj.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2bwhzynjf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kybzuans.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2nbfudzbs.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2hvvtouyd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2qcncebsf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2qqhqymap.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2dtdykapx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2onhchsmo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2mwqkxvtg.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2qewrpfrr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2uajooslw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzlqsuhc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mzcgwgmc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2dpxwdsjz.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2nwhtpifw.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2sxumvenn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2gqiotnlw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2whfcdaer.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2upwoltps.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2upccsbrl.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2xdypiras.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2pyvksvbm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2wogrcair.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2rgikfrbo.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gunudchl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2ojkyxtfc.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vwtwcsqz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2cpjlemgq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2udjmlxkl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2rnmffwxn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2aczfykig.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2sdrfvylx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2eiwstptn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2crhijpns.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2tceokxsb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2twhzcmui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2duwsqlkz.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2alufmdcm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vhrhwwad.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2qekgpfqd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2qcjbccia.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2dzutaiiw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2iyqigcvb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2vqhxsprq.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2jklikqel.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2cqtmdzya.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2lnotvdlx.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2imzihvau.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2kbhiyxxg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2qqsxmezs.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2fnxfgqwe.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2lmerogic.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ajqnobvn.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2hxourcdc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2rlgesscv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2wdircbod.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2oibtcwsr.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2dcxblwru.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2uhutyriz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2eceutxpl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2chirmpej.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2aunzezav.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2urrxuani.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2lfxiigob.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2rhfuflww.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2itxybsei.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2uojlpkbm.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2saupdrls.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2odlojvwi.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oaiquiuf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2rawnfqow.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2cahkhmij.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2liwsabof.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2grisxtih.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2buokmvwv.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ssnxtatr.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2duceavix.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2vnczwlgg.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2jqrtnlot.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2wggappka.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2rpjsmciq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2mnakzfuh.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2lqbuvqlx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2rexwgxsq.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2grkrydju.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2jyllcyyd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2iqrmnllx.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2wnxvtlps.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2dqyrjnhp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2bcgkrswo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2eciyxuts.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2kkimamwq.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2kslmnlhs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zqxqhauj.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2livztezq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2enkroyga.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2bkijjddx.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2rowqnvjl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2tuadpfzj.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2gcncyskd.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2hzkdfwcz.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2frczclut.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2vlzhqake.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ktlkkwdi.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2quboohjq.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2woqpohal.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2brlztbte.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ehynrtpw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2qnzadvsh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2qiptextc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2pszsdpkq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2pqopdjjb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2swvcqjls.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2dojeaaij.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2ovsbscex.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2rmrtgmtz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2fpktqexv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2qkbznjam.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2zojpttbc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2odpwmqcg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2glgymdhr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2owafloej.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2wxzxngqf.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2wgszzisw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2nndxtbcp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2mmydjune.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2cnkwufzq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2zikmnotm.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2utvlxgqq.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2ilhtntus.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2bieucdtl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2zcwmsdxw.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2jdnxkwfd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2isqnwncz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2zemfgbgf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2zdqtjwqb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bimnanod.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2oezelnss.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2nvmhfaid.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2vqqpximg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2kckuxmls.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2nvteddsu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2hllrwocs.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2mzrybntd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2yfbtvdhs.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pcgwmiic.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wptrigcs.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2vobrqjwi.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2vfdignuo.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2nytndsch.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2xiirrxre.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2mktmnvai.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2qxbvlzcd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tlasaxxs.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2vwokcetn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hoyuevtq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2rfufklfp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2hjxlzxew.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2hqwfscby.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2cfsjtcbf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2yrkmcyvi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2ehskqmsq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2lqbigglp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2fqfsdjyf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2mfvpbpcb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2ihwygjxn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2wkjqdose.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2koobnvji.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hasafibr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2jsmgsrzp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xafporaf.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2yvigkxxy.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2jrmwjwjj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2vcccamwr.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2gbnzopvi.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2ekpzqjwn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2wjfqccvj.html

);
来源：http://www.52xcode.cn/Article/details/gt2edydbapv.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2uiunavjp.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2nzioqvxb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2icilgvmz.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2nsuyobjm.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2xdbcyplu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2wvihtcfo.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2nokzyqjx.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2soazerfw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2mngyzsxl.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2uercltjj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2izemcczp.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2mbexledc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2nhajxpmg.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2uwbqakwv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2lnqfgwab.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2fvvprpha.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2xndxtwob.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2ebxuffdw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2alneipew.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2yryjkcpz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2cscjtpwv.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2kpbspjtj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2xrypphsw.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2ozseypkg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2lcgplsxg.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2zcomebpk.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2rbcyeoku.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2bvccyczq.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2viabnpjn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2krsdiunb.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2aubouhhx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2motxhlny.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2evuvqqen.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2ncbvhyxu.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xfqgimyw.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2yiayzvgf.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ylmuprwe.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2oygdwayv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2vsvjfcip.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2jnjdiqha.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2ffktmrvr.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2zbvbdajo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2eqijynrx.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2omjjysvt.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2jsnxvvfg.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2hlmmooki.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2lehjcgkd.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2heqphmtu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2ikcxuoxl.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2euhypfmo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2fnbiispi.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2cnucoysd.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rwtdslzk.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2aazhpjzy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2vllaezka.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2qlnkphvj.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aggnyaua.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2rqyzhbja.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ctnzumpy.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2reykhpek.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2azgukyew.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2romjqeyp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jwnkuflb.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2ecclqykj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2aodpcnvs.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2kbejhjmz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2cprvubur.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qirvrsng.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2nxqnjmxd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2prwbsdag.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2yluygtkb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2lfdbxdrd.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2prtttxse.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2dhlwjtyw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2znjkwvmy.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2dbzhnumx.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2kuvdqndt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2cyxauljr.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2wifmvcsw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2kurmytmk.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2mftqgdqe.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ypuanosy.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2loorrzof.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2gendevwv.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2drhpvmgh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2xmzipcsw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2fvfvfiii.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2jegxiiqj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2wqcxktev.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2lsrusfdc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2zuzogqpw.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ifjbvxzk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2zzzxmtip.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2ouitarok.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2qegntiag.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2czlgstrk.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2wlvbiwwk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2muiysgcw.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2kflombsu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2hwmzdovn.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2fhtmccdc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2jvawxkhz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2ekihapsn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2gqbtnzbl.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2rstytdbq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2bticbotv.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dtrekypa.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2qpfwreop.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2peakldkt.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2vmjzszht.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vzovmeqe.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2kgyzozpk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2httuypuv.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2mlelrppz.html


<!-- 参考信息 -->