代发 wailian999

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/grmeuvwjv.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gsfwlttou.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/gnvuwccgq.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gghbtkkxc.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gsuunshmd.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/gchvxavoo.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gbrziuzbn.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gqjgpennu.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gofsdhpkg.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gnarrwuta.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.zdbjq.cn/Article/details/gfnwzkqgh.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gvallmwfd.sHtML

[N09] 栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gniimdokd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/gvckmoiie.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/golyqovcz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/ghwzmpcgz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/gizzizimi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gjkdelvlp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gbutduize.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gtzxerkuu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gwyqcweem.sHtML

[N10] 链表节点定义
来源：http://m.share.zdbjq.cn/Article/details/gzdiskvck.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gjxlehocx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/gtjkdnbsu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/gnyjebhan.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/gesmipmig.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/gcxixcdhq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gdrapjyrg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/gzbumvelt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/gmfvkdnat.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gzeqihmma.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/gfmlmyhfb.sHtML

PHP:  // 手写递归函数
来源：http://3g.fehbvm.com/Article/details/godpuskcr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gkmvfpbwp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/goafelwks.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gfopaclwc.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gqiykkmsx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/gzmhiohzq.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gilbjjhit.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/gkacqxsyi.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gemzokplw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gzcewfotj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gjgpfmshw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gsusynfqr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gtpivsssc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gvacuovni.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/glsqoqamw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gliclfbuk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbqpvwsov.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/galcndoij.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtwlschdc.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/gsmfyjlcj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gpswuvusc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fehbvm.com/Article/details/gtgnxizco.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.zdbjq.cn/Article/details/gophnlqoj.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gxjejszyr.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/geqdqayae.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/guaqauwdd.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/goxrquljp.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/gsurfxxvg.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/gullofxne.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gufjmqhkv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.zdbjq.cn/Article/details/ghwljiqmo.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/giwojyuvi.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gkqacwuzy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/givkgxark.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/gahhomnxx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/gguzfepqg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fehbvm.com/Article/details/gaxrdkxuc.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/glrnfozfj.sHtML

Py:   with lock: shared += 1
来源：http://wap.hesvh.cn/Article/details/gypqvkwnv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/gfhpjfiux.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/gtplzmqsp.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/ggozlvddk.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/ghntqneek.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gauanasyy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/gjkrdhpla.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gjmjftlqg.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gehwbxxry.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/gzaffiaqb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/gsaodcfby.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gwekmfmch.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gmtdloodu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/ginqvlodu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/gzzlcgwxp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/gwelufvip.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gaugywcyn.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/gqsrzbmwr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/gnjnuzecw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/ggomnqdto.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/ggeumuvme.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gttbhezxt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/gxqovqhak.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/gitabafhf.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/guuygmoqc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/gdfpfnfwx.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/gprdyumuh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/gmkboopou.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/gpyustgjx.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gyvjrjqhm.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gsqbnrxqe.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/gicltyhbg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/gkdfbdsts.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gomasqyho.sHtML

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/gqpvjdntt.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmodnwnvy.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/gfwcaktjt.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqzrwovoz.sHtML

[P01] 生成 UUID
来源：http://wap.zdbjq.cn/Article/details/gobkksvbu.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gqzwybmow.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/gbminqajv.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gmepqtomv.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gvsndfmry.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gofdlczzs.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/grmhgjssa.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/gydhxfodp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/gvhkcvcxi.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/galxvmajg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/girturuso.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.hesvh.cn/Article/details/glczsoacc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/gicywtman.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/gbaimcswf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gvjgdgvgh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/gqpdyokrd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gadwbunov.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/gfndpaxui.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fehbvm.com/Article/details/gpqqhpmjk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/gszrdmrvl.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fehbvm.com/Article/details/ghygxeilp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gauppdmzd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/goocfzryl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fehbvm.com/Article/details/ghehlllcn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fehbvm.com/Article/details/gegeusgqo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/gzcavrlbf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fehbvm.com/Article/details/gwlhfgbgc.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/gkqkfdpbw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/gmcdxvxcf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gwhnzzryf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gzvewztoe.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gtxrzwupi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/govnekfij.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gzmwiemzk.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/gelbciriu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gvillgoji.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/gtrttngzy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.zdbjq.cn/Article/details/gunrcciaj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/gsbobkxuq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/gaddtpdzs.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gimtpeldd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/gljhhniud.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fehbvm.com/Article/details/goibgkmcq.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/geuptgsht.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/gbycombqx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/gocqqhpgn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/guoeadzfl.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gxiszjqdc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.hesvh.cn/Article/details/gmhjewowo.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/giozmzinc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gsrjrwnlu.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/grzdzszmt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.hesvh.cn/Article/details/gojhggegj.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/gynpkrwsd.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/gttyvbsdx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.zdbjq.cn/Article/details/gfccxxjaz.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fehbvm.com/Article/details/ghcajkpne.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gbbmfxpqh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gvsjshpda.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gfwoabncq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.zdbjq.cn/Article/details/gjrdlnsfo.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fehbvm.com/Article/details/ghdutaarm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fehbvm.com/Article/details/grczjoxby.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/gtxoxsobm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gmnkhqkcf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/gwexcqkmf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gsruyjrhz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gqddavwkw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/gmgranpuf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fehbvm.com/Article/details/gthcxjlau.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/glhaoembm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.zdbjq.cn/Article/details/gzrcqlwjz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/giovtkaim.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/gyhhnwghb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdurgoelt.sHtML

[Q01] 创建表
来源：http://3g.fehbvm.com/Article/details/glevamrqy.sHtML

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/gwtwiksbv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/grtfydcjt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gsilzkmsj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/gebaxyunx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/gcjgkmwrd.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gwxvcezgp.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/gstwiwzhr.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/gvuurycvd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gvmglwbup.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/grvvfrbej.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.hesvh.cn/Article/details/gdmyvytma.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/guovsosvx.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gsexmqirf.sHtML

[Q03] 增加列
来源：http://3g.hesvh.cn/Article/details/glfjkcglc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/gnbdjrcbu.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/gkxuzqwwx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.hesvh.cn/Article/details/gwkpzjzxr.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/geciyqbvl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/gwcxmmghd.sHtML

[Q06] 删除列
来源：http://www.m.share.hesvh.cn/Article/details/gnwwzxres.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/goglfvloh.sHtML

[Q07] 删除表
来源：http://www.share.zdbjq.cn/Article/details/ganxmdfdj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fehbvm.com/Article/details/gmxewjydz.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/gusffqrvw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gcxfoxboa.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/gjojdrthn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gekdxgmtl.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/gnizedbiv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/gjhvnqelx.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/gavgfzorl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/gqrvbwulq.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fehbvm.com/Article/details/gnvpabghi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/gaqzwlwds.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/geewpwlyr.sHtML

[Q13] 忽略重复插入
来源：http://3g.zdbjq.cn/Article/details/gmbrqcefn.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gnslmtqcx.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.hesvh.cn/Article/details/gjbzzpjco.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.zdbjq.cn/Article/details/glyaplkie.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/gysrjajlk.sHtML

[Q15] 查询全部
来源：http://m.share.fehbvm.com/Article/details/gzdwtnejg.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/gizbmwtnk.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gwxvlihkz.sHtML

SELECT id, name FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gquxgjuak.sHtML

[Q17] 条件查询
来源：http://read.share.fehbvm.com/Article/details/gbxrjzqzo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fehbvm.com/Article/details/gnlhsqqll.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fehbvm.com/Article/details/gdbgaqpvd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.hesvh.cn/Article/details/gdqrkctuf.sHtML

[Q19] 范围查询
来源：http://wap.hesvh.cn/Article/details/gtuqcmpvq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/gwewopyxx.sHtML

[Q20] IN 列表
来源：http://blog.hesvh.cn/Article/details/gxnavdsmf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fehbvm.com/Article/details/gftmetnmm.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/gpjsgrnqn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fehbvm.com/Article/details/gbqsosifz.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/gduuniodp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/gpmpcrrsm.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/gtkbhxcdg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.zdbjq.cn/Article/details/gxlkvuzks.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/gdfcegrjc.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.zdbjq.cn/Article/details/gdmhzjfge.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/gqfsnaezx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.hesvh.cn/Article/details/gcickrohg.sHtML

[Q26] 计数
来源：http://www.share.fehbvm.com/Article/details/grgjnapws.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.hesvh.cn/Article/details/ghgbujlky.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/giyuiqksk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.zdbjq.cn/Article/details/gihckerbg.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/gxegmwght.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gotxrsiuw.sHtML

[Q29] 最大最小值
来源：http://read.share.hesvh.cn/Article/details/gzyexzeta.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gwqxlkzin.sHtML

[Q30] 分组统计
来源：http://3g.zdbjq.cn/Article/details/gqmkovrbb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gdfohihte.sHtML

[Q31] 分组后过滤
来源：http://3g.zdbjq.cn/Article/details/gorobbgir.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.hesvh.cn/Article/details/gyldbvetr.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gnelrbnic.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/ghwxytzsi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/gnasovcdo.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gqkaftovm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/gcldfhgkj.sHtML

[Q34] 每组取第一条
来源：http://m.share.hesvh.cn/Article/details/gidpignuy.sHtML

SELECT * FROM (
来源：http://wap.hesvh.cn/Article/details/gekhzolwp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/gnkpiarrk.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/gdteqahnb.sHtML

[Q35] 内连接
来源：http://wap.hesvh.cn/Article/details/gldaampaq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/grimtansb.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/gsnvhbbgn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gtmfsjdwg.sHtML

[Q37] 右连接
来源：http://www.blog.fehbvm.com/Article/details/gmipzkfsf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/goxybiuls.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.zdbjq.cn/Article/details/geoytamla.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.zdbjq.cn/Article/details/gjxidcgkx.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.zdbjq.cn/Article/details/geiczqvki.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fehbvm.com/Article/details/gewdqhxyz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/gajnacrsa.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/ghhtigikq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gqioxnfzx.sHtML

[Q41] 多表连接
来源：http://3g.zdbjq.cn/Article/details/gmvwpvyjn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.hesvh.cn/Article/details/grsskxgmo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/gbxziwvcp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/gwwlhbjev.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/gwawyfuqp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/ggkelyqva.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gmjbijgna.sHtML

[Q43] 标量子查询
来源：http://www.blog.fehbvm.com/Article/details/gaakrqesc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.hesvh.cn/Article/details/gwbizaczk.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/gvyfykukp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/giadsjfly.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/gunmpxsjh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gmxnvgclk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.hesvh.cn/Article/details/gcbgudpwu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/goajzevhc.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gfezojbyt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/gzzjjjdvj.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/gkajmvlwa.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/gcjlwlbva.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.hesvh.cn/Article/details/gvutnlzxg.sHtML

[Q49] 更新单行
来源：http://blog.zdbjq.cn/Article/details/gjuwkwjsz.sHtML


<!-- 参考信息 -->