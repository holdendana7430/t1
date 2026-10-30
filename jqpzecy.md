代发 wailian999

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gnpvehatm.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gikbwdwca.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gannhrfeg.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gzfmwxzul.sHtML

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gbinmpggq.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gleojqxgm.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/ggugoueyx.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/glmdpybbh.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/gykdyijms.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gvwbeprxx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gxvummiza.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/ggemvpumc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/gdymsggro.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gbzomxmmh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/gmrqpnoad.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gziioclps.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/gqfzxknol.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gmlowgftq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fehbvm.com/Article/details/gsklekkme.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/gdhqdembj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/gibfgzoeu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/gbmfxgrzh.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/grlrjzuro.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/gvpbgidih.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/gompjdkuw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/gcdihlwnk.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/gliivuhjy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/gfgvcitpv.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/ghjcunjgz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gpwcdrgjn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gdfhkbeoa.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gfctavamd.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/ghnqujnvi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/glkthsnjj.sHtML

C#:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gqwekylfw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.hesvh.cn/Article/details/gawfcwatt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/goxqhxsli.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/ggjdaepwf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gpmfgaixf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gfbnyeagk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gnldmrywk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/gmfsfdnza.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fehbvm.com/Article/details/gwvrxttqa.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/ggeptvfpy.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/geuugpfgo.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/gbjkzcytx.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjvtycvqa.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/ghedmnfaf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/ggpmfhtva.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/grpuujiii.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/glasljpbi.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gqwfplxbm.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/gauuaqrof.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/gvbcfiugr.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/gcroevpqq.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/gbwrzykys.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/gdtvkilft.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/gxgemlkau.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/gfcpsblrl.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gdhhzwjtc.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/garjsqgkt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/gbqbgpzjp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/gmeosdrpo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gvmckisik.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.fehbvm.com/Article/details/gwkfrqpjm.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gtiorwvvg.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/ghcglukhs.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/gdgabpdbj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/gwqcejpog.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gclumjohi.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gqkswyuxl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/gwcofmazt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gshtwdhxf.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gvaafsbwj.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/gcnoyqonr.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fehbvm.com/Article/details/gphpbrnfd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/guhygxphd.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gtmfaqauo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gcfhkdlnx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.hesvh.cn/Article/details/gguuxgmtk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fehbvm.com/Article/details/gzjkvjnws.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/gzgeymdmi.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/gtqxfayau.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/gkppwfmsm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fehbvm.com/Article/details/gevdumsex.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/ghawelzys.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gpayzcqqs.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gwidvgzso.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/gtdqdngho.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.zdbjq.cn/Article/details/gippwxcmn.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gddoaszsu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/ghennylvi.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/glhyjygmb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/gtvlpkgoi.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/gbsaavtze.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gnmfzntkw.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gtslvnwmq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/gngxcexnb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/gopxjfpib.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/gkjcssbxf.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/gxyvcqosr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqorvzspy.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/gemyyjhlp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/goucctazu.sHtML

[P01] 生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gjipttlyi.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/gmbrphmuh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.zdbjq.cn/Article/details/gnwqsqdqd.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/grrtmtmln.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gjcxogbhc.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gegtrumxj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.hesvh.cn/Article/details/gfwvyooqn.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/gvdpsrwah.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/gccsxeguq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/gneeiwctz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/gogicabgs.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/gfxfrdhag.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/gfkpydsrx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/gayrchnne.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gdbvlhsfg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gxnmnwpee.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/gkxoqjqxy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.zdbjq.cn/Article/details/gewsukclc.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fehbvm.com/Article/details/ggyhpjkxw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/gslplgysu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.zdbjq.cn/Article/details/gyjzyycza.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/genhrwldn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gyoktvxmc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.zdbjq.cn/Article/details/giduoajfs.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/gdpnbdsgi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.zdbjq.cn/Article/details/gjgeantbn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.zdbjq.cn/Article/details/gmtsdkgzj.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/gxlafiqza.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/gwikvgduh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/ggrcrnwkl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/ggaesdhsj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gkooymcqf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fehbvm.com/Article/details/gtobykaop.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/glhdrmary.sHtML

Ruby: x.length;  x.size
来源：http://mobile.zdbjq.cn/Article/details/gnndppeqz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/grkoxqewt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/ghcqloosw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/gorgqqlla.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.hesvh.cn/Article/details/gilgyspdh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/gfsxxzhtw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gcxsyrbep.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/ghuqhglzm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gyrwaauku.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/gmrljyndt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.hesvh.cn/Article/details/gsepmqguz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/guuxvmpxx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gdqxoyeoy.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/ggnmuxfgy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/gfepkimst.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/ggrqyougb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gjjtdunba.sHtML

Go:   if x == nil {}
来源：http://baike.fehbvm.com/Article/details/gvpklciho.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/ggpoouvwn.sHtML

C#:   if (x is null) {}
来源：http://3g.hesvh.cn/Article/details/gfbnqfizf.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/gsnkykopi.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.zdbjq.cn/Article/details/gtbzavjbc.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.zdbjq.cn/Article/details/gzscygkux.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gtocpmywh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gsjqkdzsa.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/gxhuxxocc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fehbvm.com/Article/details/grljvmclv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fehbvm.com/Article/details/grjzavnlg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/ggsquvwih.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/guojkyfyy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/gkyxnhnhe.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.zdbjq.cn/Article/details/gixiifyew.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fehbvm.com/Article/details/gzdkatwhe.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/ggvvilldt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/gdwdyyury.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.zdbjq.cn/Article/details/gdofnvrxo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fehbvm.com/Article/details/gixlginxz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.hesvh.cn/Article/details/gpuxopsrx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gsifvblqg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.zdbjq.cn/Article/details/ghywpiyac.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gafaueyxq.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gyuxowgdn.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/gipfuzccw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gyofjktko.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gdjshefds.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/gzdcajqoo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.hesvh.cn/Article/details/glfakufqd.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gqwfcewau.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/glavdafad.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/gltlelhis.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gkumbfoqv.sHtML

user_id INT NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/goylsjtmu.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fehbvm.com/Article/details/gcwykzieo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fehbvm.com/Article/details/gviwqsasw.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gcgrtebsy.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/gmwdxiwfv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/gsxwgdkbu.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/gabpdaaql.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gnkqrcsdf.sHtML

[Q05] 重命名列
来源：http://blog.zdbjq.cn/Article/details/gmtpldnvt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.hesvh.cn/Article/details/gehxtsodr.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/gkwgicjdj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/gstllimoy.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/gxrhxlvkq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/gslnrumjt.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fehbvm.com/Article/details/gydvmalag.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gzoxdqoif.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.hesvh.cn/Article/details/geixvqona.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gtbnbtfbz.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/gdjzrhyxc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.hesvh.cn/Article/details/gkxrghmdm.sHtML

[Q11] 一次插入多行
来源：http://wap.fehbvm.com/Article/details/gpkpeyget.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/gfyyljcir.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.hesvh.cn/Article/details/gxhgtneto.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fehbvm.com/Article/details/gtnjlzxyt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/gptagonjm.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/gdpygbbmk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gepdhoblg.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gmdqucngn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.hesvh.cn/Article/details/gjcgaexnp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/gqpbogpnt.sHtML

[Q15] 查询全部
来源：http://3g.zdbjq.cn/Article/details/gdgmgadyv.sHtML

SELECT * FROM users;
来源：http://wap.zdbjq.cn/Article/details/gpjqvpyha.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/gjrgqedfa.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gndfhaapt.sHtML

[Q17] 条件查询
来源：http://www.blog.hesvh.cn/Article/details/gojvqgcie.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fehbvm.com/Article/details/gpvlowevw.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gwlmxutfi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.hesvh.cn/Article/details/gjkqcnyot.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/gcrmyqlzn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.hesvh.cn/Article/details/gsoghevnx.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/gxqgtdikv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.zdbjq.cn/Article/details/ghdggiopu.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/gqzsubvwe.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gfggfguoz.sHtML

[Q22] 排序
来源：http://wap.fehbvm.com/Article/details/gcydgxzig.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/gcetydcqf.sHtML

[Q23] 分页
来源：http://read.share.zdbjq.cn/Article/details/glizyaent.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gekrzpwgt.sHtML

[Q24] 去重
来源：http://baike.fehbvm.com/Article/details/goyfhkhkb.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.zdbjq.cn/Article/details/glstfovmm.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.hesvh.cn/Article/details/gjwqhiixh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fehbvm.com/Article/details/gpwmajucg.sHtML

[Q26] 计数
来源：http://read.share.hesvh.cn/Article/details/gxffeqkra.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gftmymxhx.sHtML

[Q27] 条件计数
来源：http://3g.hesvh.cn/Article/details/gxdjnjeyp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gakxhtjdk.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/ghiyxdbvg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gilmytmhk.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/gxpdcykiw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/goxojbqqi.sHtML

[Q30] 分组统计
来源：http://www.blog.zdbjq.cn/Article/details/godeejxsa.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/goaxvtpeq.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/gbycvjpfh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/ghvkjczlg.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gwkotvxed.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gwhiloyzq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gtlreezif.sHtML

[Q33] 多列分组
来源：http://baike.hesvh.cn/Article/details/grtvylgty.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/gshbtgrvb.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/gofrhqzal.sHtML

SELECT * FROM (
来源：http://baike.fehbvm.com/Article/details/gcodhinlh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fehbvm.com/Article/details/gyimsgcav.sHtML

) t WHERE rn = 1;
来源：http://m.share.fehbvm.com/Article/details/gvicwgawe.sHtML

[Q35] 内连接
来源：http://wap.hesvh.cn/Article/details/ggvyakxcj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gdlqqyqpr.sHtML

[Q36] 左连接
来源：http://m.share.fehbvm.com/Article/details/glgzohucz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gdtpeuuwc.sHtML

[Q37] 右连接
来源：http://blog.fehbvm.com/Article/details/gjtbmrcov.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/gmoxmyyrd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.hesvh.cn/Article/details/gklvmzdin.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/gfpeukvix.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/glassileq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gvticsvcw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fehbvm.com/Article/details/gamrlagnu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.zdbjq.cn/Article/details/gdnrwyhyh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/gtlcuhdgu.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/gvuztsdfd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.zdbjq.cn/Article/details/gwudodawa.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/gpklarqmv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/gpctprbqv.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/gyaqgeaho.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.zdbjq.cn/Article/details/ggyrsrchi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/gqghnmxsk.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/gljmbrfef.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/gnqzcsczd.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/gsefwjczy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/goimtrloh.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fehbvm.com/Article/details/gohygelvp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/ggmpfegwy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fehbvm.com/Article/details/gofezvubk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gsgfrehhm.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/gfuuehhuy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/gzbuogyfi.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/goqlydamc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.hesvh.cn/Article/details/gmqlnecfu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/gycsgadyd.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/gyxgstyxn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gbkpubzfw.sHtML

[Q50] 批量更新
来源：http://m.share.hesvh.cn/Article/details/gdovpdgqw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gedsolrzw.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/gzjneusqw.sHtML


<!-- 参考信息 -->