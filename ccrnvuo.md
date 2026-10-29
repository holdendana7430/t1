代发 wailian999

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gocvkuzae.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gfubrvswj.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gkbvujtfw.sHtML

C#:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/ggzyfvnuw.sHtML

[N09] 栈与队列
来源：http://read.share.hesvh.cn/Article/details/gspzxdxiv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/gqscnowgu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/gkeektcge.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gswirscbi.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/gvwdskqsj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/gsapuexxs.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fehbvm.com/Article/details/gxfuejizf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gzvvztgjf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gqncomzgd.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/goujjiclp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gkzowclgf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gsmuxasrf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/graipfelp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/gvtfpedut.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/gpzojwhbl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.hesvh.cn/Article/details/gneuetpex.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gznloioak.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/grtfmqffs.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/gygjnymax.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/gcivespsw.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/gpzyrymlk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gjeuistnh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gbawhyfhq.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gcbgddish.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/ghfaqynvh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/gdbdhossp.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gcoafznmo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/gbdpbgxjd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gjvlgsfea.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.zdbjq.cn/Article/details/gdgjunxtf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gqafjmtnq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/glghxluvd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/geezydtfr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/ggyrgxwrp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fehbvm.com/Article/details/gebnqappw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gfnppdoeh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvhchvmdc.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/gteekyani.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/guwjyvoyy.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gxxbzlkxn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.zdbjq.cn/Article/details/gvanltwjm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/gcxokysgn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gncljfnmc.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gkhcgbynl.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/gndklkuif.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gcsyebvbz.sHtML

Ruby: Thread.new { f }
来源：http://3g.zdbjq.cn/Article/details/ghikpylba.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/guocjuzhk.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/ghishwtwg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/gujvtknyf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/gilbrdiut.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gmwztdzoe.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/ggkidcvxo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/gofsevchj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.zdbjq.cn/Article/details/gbanznoes.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/grhaxbgpb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gjmwsbljq.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/gkujdfyol.sHtML

Py:   with lock: shared += 1
来源：http://baike.zdbjq.cn/Article/details/gptqpyfwt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/gzjwkwfuh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/gbxbotexi.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/ggsdeyxhw.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/glhajtxnr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/gejikkktc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gxzahrfsj.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gknatnbpt.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/gdsjodtrl.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/gogxhcwny.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.zdbjq.cn/Article/details/ggtlfvyxk.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gckhkncwt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gkgeuxmrc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/ghljfuqnb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/gdfmbcikr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fehbvm.com/Article/details/gukztrrvg.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/gxuzieoih.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/gfnkvbtxt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/gvmfiywkx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.hesvh.cn/Article/details/gbfzrnvaq.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gskvutkum.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/guqkzyake.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/gaikqherh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/grrbberhj.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gnimvuoph.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gwejklpnm.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gvfxpbflg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/gjaiarnjm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/gonbhcilr.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/glgcfyihu.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gngjcbbgb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.zdbjq.cn/Article/details/gzqhtlfsv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/gafnbrxmt.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/gcsniboaw.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/gzjdivkuv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzhcpuhdl.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/gssbdwftu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/guwapxhgb.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gtmpspkjy.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/gcwgfqnak.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.hesvh.cn/Article/details/gauycwyeb.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gvsnliyqy.sHtML

TS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gqwctszou.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/gfiskqahb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fehbvm.com/Article/details/gfiyoibtj.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/guzxbvbcb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.zdbjq.cn/Article/details/gfwazhwor.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.zdbjq.cn/Article/details/gbnlnipje.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/gjkmmslhp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.zdbjq.cn/Article/details/gvrmbjrnw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/ghaobnuvu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.zdbjq.cn/Article/details/gppimiaui.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/golfrjzwf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/gnbphbdra.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/gjpzmtgys.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/gsncjizud.sHtML

[P03] 生成短随机字符串
来源：http://www.share.hesvh.cn/Article/details/ggdhomrjd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.hesvh.cn/Article/details/gsgxqzeea.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/gdnkdakvv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gujqbjuvh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gssbsysxz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/ghfmvyypd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fehbvm.com/Article/details/gebrdwrvi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gemheztum.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/gsvwcwpzm.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/gwfuiclee.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gptpsqiec.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gojtaqhxe.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gofrmmfsg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gmeanehau.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/gpfvsqiaw.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/glboscxmb.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/ghvmlgqks.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gknfzvfvj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fehbvm.com/Article/details/gopxjyoyb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/gxqweeevs.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.zdbjq.cn/Article/details/gucaxsivk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/gbqahksht.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gflanjmpa.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/gchquplji.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gwubzuhaf.sHtML

Ruby: a == b
来源：http://baike.fehbvm.com/Article/details/gvssyujas.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/gkndffiud.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/geylljmru.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/gefhmzyvr.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/gofinwpgh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/gyyrdkxoq.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gqovskzfm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gzjuygkjk.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/gbbaqyezm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/gsvqysufj.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gutyslful.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/gcqsyajbx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.zdbjq.cn/Article/details/gshxmskyx.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/gjmvamwbe.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gyooqfxnp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gipbuuipv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/gjmpyugmj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fehbvm.com/Article/details/gyumnzbxt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/goavkklmy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/gaatvqmwp.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/garcgztpq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.zdbjq.cn/Article/details/gvadopebj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.hesvh.cn/Article/details/gnrjvqzwd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/gqrbcpiig.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/groduwxrz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/gwvdmuaec.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/gybwstxai.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fehbvm.com/Article/details/gcbgjdwnj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.zdbjq.cn/Article/details/gpytotgcf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gghxviadp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/gyrgoxyiu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpszazkfp.sHtML

[Q01] 创建表
来源：http://m.share.hesvh.cn/Article/details/gtvpgoeas.sHtML

CREATE TABLE users (
来源：http://www.m.share.hesvh.cn/Article/details/gafcavbbj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gwpzkpiiy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gzsjmjsiq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/gaxjhdlpm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/gykcstymk.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gbgssekph.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fehbvm.com/Article/details/glcaqwueq.sHtML

CREATE TABLE orders (
来源：http://wap.hesvh.cn/Article/details/gfhhjsims.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gxokleity.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gduufgxzi.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/gaapwzivr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/gtairsvxj.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gfkgjomiq.sHtML

[Q03] 增加列
来源：http://blog.hesvh.cn/Article/details/gjwduqtbb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/gkdwgwqjr.sHtML

[Q04] 修改列类型
来源：http://www.m.share.hesvh.cn/Article/details/gxgwkqtxn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fehbvm.com/Article/details/glbkysdan.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/gadwvnbmt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/gymdsoybm.sHtML

[Q06] 删除列
来源：http://wap.zdbjq.cn/Article/details/gnmdjoiuy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fehbvm.com/Article/details/gdqnxvzrf.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/gymqgceie.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.hesvh.cn/Article/details/gzehfmobk.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fehbvm.com/Article/details/gwzttjdis.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gmsinfxlx.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fehbvm.com/Article/details/gdahxxjeh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/glkqhrgav.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/ggavmnlxr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fehbvm.com/Article/details/gtylhqqub.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/gxbgyyydb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.zdbjq.cn/Article/details/gvdledrub.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/gafuanrwq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fehbvm.com/Article/details/gktvonzay.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.hesvh.cn/Article/details/gckhcbpvl.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/gyyrksbkj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/gbxoniqtq.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/gpulusrvx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.zdbjq.cn/Article/details/gqywsscyk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fehbvm.com/Article/details/gokfohhiz.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/gqrmreqli.sHtML

SELECT * FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gldpwcilc.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/gxvgscmth.sHtML

SELECT id, name FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gdzfaaxgm.sHtML

[Q17] 条件查询
来源：http://www.share.hesvh.cn/Article/details/gzoincuip.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.zdbjq.cn/Article/details/ghincfjza.sHtML

[Q18] 模糊匹配
来源：http://mobile.fehbvm.com/Article/details/gtcpllcox.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.hesvh.cn/Article/details/glaueupiy.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/gnzfpzhwf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/gyckinztj.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/ghmsdpnfs.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/gzyasafnm.sHtML

[Q21] 空值判断
来源：http://m.share.hesvh.cn/Article/details/gafvfahxz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/ggbryeunr.sHtML

[Q22] 排序
来源：http://wap.zdbjq.cn/Article/details/gowxdkmaw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.zdbjq.cn/Article/details/geomqqzwy.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gejchaxgo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.hesvh.cn/Article/details/gcwhpsccf.sHtML

[Q24] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gijvlaahm.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ghrkywpuk.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/gfyppxvub.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gubklkrao.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/gcfhuvocj.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gjwktvwzu.sHtML

[Q27] 条件计数
来源：http://m.share.fehbvm.com/Article/details/gpplpagsx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gkvwhfovf.sHtML

[Q28] 求和与平均
来源：http://blog.fehbvm.com/Article/details/gfaeiwbur.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/ggcayknqb.sHtML

[Q29] 最大最小值
来源：http://baike.hesvh.cn/Article/details/gjitemwij.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gozdinwgd.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/gdeeugpep.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gyhdshjhr.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/gsumbqbzv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.zdbjq.cn/Article/details/geihxjqji.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fehbvm.com/Article/details/gkespkanr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gnlmadlan.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/gctjkdkns.sHtML

[Q33] 多列分组
来源：http://3g.fehbvm.com/Article/details/goxuvkynn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/gauzmhzdy.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/gcvzhdmsi.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/gyjzvyukw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gpzeoxnpy.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/grjcrmbhu.sHtML

[Q35] 内连接
来源：http://mobile.zdbjq.cn/Article/details/ghshwkxoz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gfsqceosp.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/gqnqciglq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/geuvrxuyy.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/gfdpbzcvk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gyelzunai.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fehbvm.com/Article/details/gfpsgmlqf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.zdbjq.cn/Article/details/guumdygvs.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/genrinuwa.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fehbvm.com/Article/details/gdufirndg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/gbqrhqunm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.hesvh.cn/Article/details/gzqldyyoo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/gsjggsnwt.sHtML

[Q41] 多表连接
来源：http://www.blog.zdbjq.cn/Article/details/gqhxnfvww.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.zdbjq.cn/Article/details/gckerzbpz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.hesvh.cn/Article/details/gypyreogr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fehbvm.com/Article/details/gossxakmh.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/gzzvddtrw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.hesvh.cn/Article/details/gnxcbvlia.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gsckfgitt.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/gmrinolnr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fehbvm.com/Article/details/gxrnoodtx.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/glklucqzz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fehbvm.com/Article/details/gdohfgmdn.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/gosouswnw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gdhhsdbzw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/ggrftkolp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gfwyenmfk.sHtML

[Q47] 与平均值比较
来源：http://mobile.fehbvm.com/Article/details/gbfgsaedk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.hesvh.cn/Article/details/ghamnzhjz.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.hesvh.cn/Article/details/gsqsnrgbw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.hesvh.cn/Article/details/gmcmbfhgl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/ghpkgperq.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gbzhvjqfi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/goxbgnext.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/giiwamxtn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fehbvm.com/Article/details/gnyrajoia.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/glnrnnbju.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/gpodiqwju.sHtML

[Q52] 删除指定行
来源：http://www.m.share.hesvh.cn/Article/details/gcghqilhz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gavtpitkw.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fehbvm.com/Article/details/gxghltufo.sHtML


<!-- 参考信息 -->