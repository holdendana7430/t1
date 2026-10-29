代发 wailian999

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gmmfpbhzj.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/geupuyows.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fehbvm.com/Article/details/gmhshtbso.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/gqzjstzgb.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/gwklsslej.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/gwqzndtag.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gpggbofhd.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gqtcbhvqe.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/goirsywua.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gfbbqaeon.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/gjqqvyadl.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gtphinuvj.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/goidgcalc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/ghvxysgki.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gxpxmyore.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gyfhhquqw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/glawgedru.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gnkbdvimz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gssscnxlu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gfsuurzkh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/glkpbbvuk.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gwbourlgn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fehbvm.com/Article/details/gypmincbs.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gzljuwbvz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gdqhqlplp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/giezpfqsj.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/gwgazwjnn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/ggcegjbpv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gyvaiuevb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gqwvkrzjj.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/ggrijhynr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/gzetwdbon.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/gunumxsnj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gkrjuaafd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gvqssvgij.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/ghvrqrgzo.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gygivuagc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.zdbjq.cn/Article/details/guwcyfihf.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gmecoemjv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gtpqpbuah.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/gbskwuwjl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fehbvm.com/Article/details/gmukgnqfx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/grbngrydo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gaisfkqfl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gxfynuorf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/girzsgmng.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/goioxajfv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gwgnxspmg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcktqechr.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/gcevmiejq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyqmkvgal.sHtML

[O01] 启动一个线程
来源：http://blog.fehbvm.com/Article/details/gdtlwvmww.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/gsiomsbyq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/glogdlqhz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/gydnauban.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gwufpayld.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fehbvm.com/Article/details/gxfkzzvco.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/giyayrepv.sHtML

Ruby: Thread.new { f }
来源：http://mobile.zdbjq.cn/Article/details/gzcpbkthq.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/ggxogdeum.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/geusvbuhs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.zdbjq.cn/Article/details/gscmjtcgz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.zdbjq.cn/Article/details/gibhovwnz.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gtsosgcem.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gjzfdmwkf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.hesvh.cn/Article/details/gztrydgkm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.hesvh.cn/Article/details/gnmaeblno.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/gehyzpvvt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/gnkertcrj.sHtML

[O03] 加锁保护共享数据
来源：http://3g.zdbjq.cn/Article/details/gkhlrcmkc.sHtML

Py:   with lock: shared += 1
来源：http://baike.fehbvm.com/Article/details/gdnqqlzgl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/gwwvrrvls.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.hesvh.cn/Article/details/gsejiktge.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/grfjtdoka.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gerfxwlzc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/gknnshbwt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gtjdnvgva.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gqnmvmzmh.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.zdbjq.cn/Article/details/gnfopblgy.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gkoaqotfx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/gmkqsiwzd.sHtML

JS:   async function f() { await g(); }
来源：http://wap.zdbjq.cn/Article/details/giknmjuyx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/gsalfysyh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.zdbjq.cn/Article/details/ghvdbqhky.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fehbvm.com/Article/details/getlvttnu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fehbvm.com/Article/details/ggvqesyfq.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/gratdbqda.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/geqfombeg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/gefkpfofa.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/gcnbbnusc.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gahrwfbet.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gwwkgyrek.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gtfdltdbe.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gywlrpygh.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gfrhmteba.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.hesvh.cn/Article/details/gokrldivl.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/gppwdglne.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/gtffbnbpp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/grihhzvve.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gqdaeagic.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gnacxkqlo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/gbebqelul.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.zdbjq.cn/Article/details/gscjzwrsv.sHtML

Ruby: // fork 块
来源：http://m.share.zdbjq.cn/Article/details/gnlybopxh.sHtML

C#:   Parallel.For
来源：http://www.m.share.hesvh.cn/Article/details/gxuylxqwa.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjmogvmyt.sHtML

P. 常用工具函数
来源：http://www.share.zdbjq.cn/Article/details/gumgvamhn.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnsyxzkct.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gsnvcixor.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/grdvhmiwx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/ghtfrzeay.sHtML

JS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gfjxjkfsl.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/ghvcmnebj.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.hesvh.cn/Article/details/grosalglc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.zdbjq.cn/Article/details/gedpeqrej.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/ggcgjmwyz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gbsclculr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.zdbjq.cn/Article/details/gpqkfggdh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gyccjbsix.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.zdbjq.cn/Article/details/gwzzkvthw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/gbxmhqulq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/gxrkzboyc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/grgqhgasc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/gdenzjhbc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.hesvh.cn/Article/details/gxlnuxyjf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/gbivgjife.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gxwmckzar.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.hesvh.cn/Article/details/gbuxkacfo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fehbvm.com/Article/details/gpnkfnjfi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/geunazaly.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gewehenhv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gtwuosfft.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/gkkcdxgjp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gsmtteitm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/gcfcmtbic.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gllaekpcw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.zdbjq.cn/Article/details/ggimukyhv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gnkajjozf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gvadgoddg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gbgkxpgpl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gommrhvts.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/goddwwchb.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.zdbjq.cn/Article/details/gjvcojttn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gzxnogexw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.zdbjq.cn/Article/details/ghbcxevta.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.zdbjq.cn/Article/details/gfsqtznzn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.hesvh.cn/Article/details/gunyrztsv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gkihvfirt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gknbmkgrk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/ghdzhhdis.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/gxkghbnwb.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/gzalkqkro.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.zdbjq.cn/Article/details/gdelwjwua.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fehbvm.com/Article/details/gfqswlpic.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.zdbjq.cn/Article/details/gxrvoxlav.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fehbvm.com/Article/details/gqrshhrxz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.hesvh.cn/Article/details/gaxfixkuq.sHtML

TS:   if (x == null) {}
来源：http://www.blog.hesvh.cn/Article/details/gsxtgsuza.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gplzstlga.sHtML

Go:   if x == nil {}
来源：http://blog.hesvh.cn/Article/details/goarbcbhj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/gawbpzxrk.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/ggocmgcbg.sHtML

[P07] 防抖与节流
来源：http://baike.hesvh.cn/Article/details/glxcdltyb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fehbvm.com/Article/details/goscvrvbo.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/gnaykhdvn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gtwzpspod.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gqnfmtdjk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/gwkxosowf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/gwrfmaioz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/gxdisrzgl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/grpavouup.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/gozdcmguv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/gyuavvudr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.zdbjq.cn/Article/details/gbvlywyuj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/gtkecxcwp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gxggzldbl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fehbvm.com/Article/details/gweghypzf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/guikswiyf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fehbvm.com/Article/details/goszufzxr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/gzxcexqvi.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtlwgdypx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gramuyurp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gekuvagdq.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/ghchfvvbw.sHtML

CREATE TABLE users (
来源：http://blog.fehbvm.com/Article/details/gnggyrrpd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gcmgdltkr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gevvmmiuf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.zdbjq.cn/Article/details/gmijqjlhl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fehbvm.com/Article/details/gsvlnmkbi.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gzatkoahl.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/gximtequm.sHtML

CREATE TABLE orders (
来源：http://3g.zdbjq.cn/Article/details/gwmvenilp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/ggksfwsak.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/glrvtjmfc.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fehbvm.com/Article/details/gncgxaizk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/gwkeeeaja.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gofushgyn.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/gafkioouu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.zdbjq.cn/Article/details/grtyjirdk.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fehbvm.com/Article/details/gpafipxzl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.hesvh.cn/Article/details/glvzxnsoa.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/gjmtanxuq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.zdbjq.cn/Article/details/gmzgqycpl.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/gxkvuttue.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fehbvm.com/Article/details/glzsycfvz.sHtML

[Q07] 删除表
来源：http://baike.hesvh.cn/Article/details/gobprhzoh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.zdbjq.cn/Article/details/ghmlqyxpk.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/gnrikkdis.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gtmhaucbw.sHtML

[Q09] 创建唯一索引
来源：http://baike.fehbvm.com/Article/details/glhtxuyni.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gkeqvtdca.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/gjqshrgnj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/gaashwoxu.sHtML

[Q11] 一次插入多行
来源：http://www.blog.hesvh.cn/Article/details/ghgmiwgsr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fehbvm.com/Article/details/gavdkixco.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/gvymolmwy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fehbvm.com/Article/details/gqipvdxkx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/golobcqph.sHtML

[Q13] 忽略重复插入
来源：http://3g.zdbjq.cn/Article/details/goacxyqlr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/ggyldwcsa.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/glbswyqbn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/gsztdxpop.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/guvvsoqxh.sHtML

[Q15] 查询全部
来源：http://www.m.share.zdbjq.cn/Article/details/gianamuvq.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/getmeghgx.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/ggqtibxcl.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gxokyxdfh.sHtML

[Q17] 条件查询
来源：http://m.share.zdbjq.cn/Article/details/gnnmplvop.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gkaxdevfc.sHtML

[Q18] 模糊匹配
来源：http://m.share.fehbvm.com/Article/details/guwvtjqea.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/gsognbkhb.sHtML

[Q19] 范围查询
来源：http://m.share.hesvh.cn/Article/details/gqidgxwrh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.zdbjq.cn/Article/details/gsbnfusyj.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/ghgssdmlm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/gtzmhtnwf.sHtML

[Q21] 空值判断
来源：http://www.blog.fehbvm.com/Article/details/gltadcorm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/ggolmqkkj.sHtML

[Q22] 排序
来源：http://baike.zdbjq.cn/Article/details/gxshhthid.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.hesvh.cn/Article/details/guulzazxu.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/ghzixvvhz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.hesvh.cn/Article/details/gdqhegglw.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/gwobxpolt.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/gaunlhokh.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.hesvh.cn/Article/details/grtwgbpwq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gmzdvbfhe.sHtML

[Q26] 计数
来源：http://3g.zdbjq.cn/Article/details/gzxyntaef.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gcwjkfdbl.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/gimlipore.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gllbqeatl.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gqbabisdb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gumrlvuzx.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/gcdhwuujr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gwauavvuc.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/gvstaefns.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gpgcytobb.sHtML

[Q31] 分组后过滤
来源：http://3g.zdbjq.cn/Article/details/gwoduijbk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/gevzgcbcz.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/ghjjerdif.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gizctkuao.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/gbscmmcsl.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/grhhfvjmc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.hesvh.cn/Article/details/gebvslpzm.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/ggqauwwjf.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/gysclhuvf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/gnjsepbjg.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/gjglhqpby.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gigwrwvfp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gnplazwgg.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/gfgzlkiok.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/ghqwfnxfg.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/gzedcxxni.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gpjthuuvf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/gzjuxnsrp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/glyyoobec.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/gflkeogby.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/gmwyeduhg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/gibmaxnmr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/gnhjnxkmz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gghluvbyu.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/goiwlgezy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/gqvbdgmoi.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/gpwqioyzl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/gxxuftmbw.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/gwerposjv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.zdbjq.cn/Article/details/gtpouwfdi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gvmljrueo.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/glfzkoxol.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/grrsvxtnn.sHtML

[Q44] IN 子查询
来源：http://mobile.zdbjq.cn/Article/details/gjiapmgxw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.zdbjq.cn/Article/details/gqxdwcimw.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/ggxoghkqf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/guezwmsdg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.hesvh.cn/Article/details/gztkvkmlp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gxcaagpdg.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/glkhzetvr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/gfnefufhq.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fehbvm.com/Article/details/gyggebima.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/gvpchvkdu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/gtppasdlc.sHtML

[Q49] 更新单行
来源：http://wap.zdbjq.cn/Article/details/giczphbnx.sHtML


<!-- 参考信息 -->