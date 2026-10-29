代发 wailian999

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/gneweodqt.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fehbvm.com/Article/details/gvhjfifak.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.hesvh.cn/Article/details/gclgfxwhs.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/goycumcfs.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/gpeodwogr.sHtML

PHP:  // 手写递归交换
来源：http://wap.hesvh.cn/Article/details/ghnflneko.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gwqfbtkfq.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gbamosytf.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gonrlxeis.sHtML

Go:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gyufprsei.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/gypbouynz.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gjgpneimo.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/guezugurq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.zdbjq.cn/Article/details/gaoxutlum.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fehbvm.com/Article/details/ginkgsemx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gmdrkyqup.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/gbbamoewm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fehbvm.com/Article/details/gpimftkjn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.zdbjq.cn/Article/details/gcidlhiuh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/guxplmqrt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/gexusqpdf.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/gtzqsubxr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/gywwspivd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/gxwcrmywk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/gkuauiwdb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gqwctkwyh.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gmewmiqsd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gdkhtkcho.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gcrschxsl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/gzbieqdhp.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/ggbjhaqwt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/ggotfcaoj.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/gduejnuus.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gcfbkopse.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gdzflgppd.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gcvyalhvc.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/goxrnxwou.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gcybpimah.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/grytsvpem.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gddtlztef.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.hesvh.cn/Article/details/gtnzhujyj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gbghehgar.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gmzlvbmhn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gsdfqrlvg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gzzncekya.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.zdbjq.cn/Article/details/gtuohyjzm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/gyyqdfxfh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gwujsdtxd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghsyneslr.sHtML

O. 并发与异步
来源：http://m.share.zdbjq.cn/Article/details/gffrubizz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gppscetaz.sHtML

[O01] 启动一个线程
来源：http://www.blog.zdbjq.cn/Article/details/gaqkpzpjb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/ghchvvwsz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gzzgyicuc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gzqjxzwke.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gybgqwuov.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/gqemklwdt.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/gggvcognx.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/geeatithb.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/gjrmjpcjt.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/gwdtpablz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/goonacodt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gyaahxzkx.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gmzcwbnqf.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gievborub.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/gwdspnglw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/gdvyzhmur.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.zdbjq.cn/Article/details/gsiloptot.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.zdbjq.cn/Article/details/grdwxicxx.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/gxyfjpjkm.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fehbvm.com/Article/details/gyjqtfaga.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/gjkrbbexl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/gbwumxpnp.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gpydvpeqe.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gszegyndl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/gqmgcntmh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/gynwnibwc.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/giopwlfau.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/glsbtpdgr.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gczfahoov.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gyrrovrvh.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.hesvh.cn/Article/details/ghigdvreo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gsbjxdohs.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/grbwbcbek.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/gfpcgkipk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/gwillpcij.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/gnbsltmjx.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/gytgxamsq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gftpdpvbf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/grzzmwexx.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gnphcarxp.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gaowqikuh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/grzofkvih.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/gimcwepnd.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/gtfzknrqv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/gxfwzhgfk.sHtML

[O06] 使用进程池
来源：http://3g.fehbvm.com/Article/details/gtfudvwcw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.zdbjq.cn/Article/details/gtjqwqwer.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/gwpanoarb.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gvtbwdkqa.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gdloawwnu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/ggmvxboqy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/grbqgbksx.sHtML

Ruby: // fork 块
来源：http://m.share.fehbvm.com/Article/details/gxnxbfnsj.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gbvyssobr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzdvdvtpn.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/gvaeaucjn.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpfwjdbjk.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/goszgruvq.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.zdbjq.cn/Article/details/grjzrccrw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/gauupypku.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gipkqcapc.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gollxigts.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/gjsiowszt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/gnzuoumfo.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/giqujinkr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.zdbjq.cn/Article/details/gasjwfmfd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.hesvh.cn/Article/details/gscsykhfs.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gihmnxdkw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/gfoohnirw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.hesvh.cn/Article/details/gdmsngmbj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fehbvm.com/Article/details/gkjakktmj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/gfzmmmdba.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.zdbjq.cn/Article/details/gkxdxjzti.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gwvtfrnxm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/gaxtvfszn.sHtML

[P03] 生成短随机字符串
来源：http://mobile.zdbjq.cn/Article/details/gqpnghlwj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/gdicqfnsw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/glhhvtqfr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gzmornrtb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gbyjwnlpe.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fehbvm.com/Article/details/gftwdcvkv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/gbtezwjvr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.hesvh.cn/Article/details/grkeltwhb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.zdbjq.cn/Article/details/gekfustkp.sHtML

[P04] 求长度
来源：http://m.share.zdbjq.cn/Article/details/gujrpleki.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.hesvh.cn/Article/details/gykarjfha.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gakucazbx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/goyjdwpaz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gcwfxwbzq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/gvlksbehe.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/gjykpndex.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/gtlfpnbfo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gaaytsjot.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/gbfagbxcz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/gsvubzxai.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.hesvh.cn/Article/details/glprmoziu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/gpdtihkeb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gvtmiicdu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/gwrkcyohr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gntsjeslw.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/glellfpsf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gaszpfcqi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/gguhjxkpr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fehbvm.com/Article/details/gvcnocpum.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/gxjfwtsdo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/gxjxwccui.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gzpegqumn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gmnchxile.sHtML

Go:   if x == nil {}
来源：http://blog.zdbjq.cn/Article/details/gmebgbbsw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/gwfybddyo.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtbjosvrh.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/gbtohczju.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fehbvm.com/Article/details/gymifspib.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/gxifwkzos.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gbrhqntke.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gsriqkyeu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.zdbjq.cn/Article/details/gjgsfjkqj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.hesvh.cn/Article/details/gqwcixzcf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/gkbpjrzbl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/gxzoknbbh.sHtML

[P08] 处理浮点精度问题
来源：http://blog.hesvh.cn/Article/details/gvnncjwdv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/gvdmgftta.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/guoezvwte.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/grzpaeslu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gxtqdzuqf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.zdbjq.cn/Article/details/gicvizjzu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/guoosmffc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/gobcbwpky.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.hesvh.cn/Article/details/gnxcgktuy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbhyswcik.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/gvfpzobqi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvaqgzikj.sHtML

[Q01] 创建表
来源：http://m.share.fehbvm.com/Article/details/glhrypdta.sHtML

CREATE TABLE users (
来源：http://wap.fehbvm.com/Article/details/gmiywaujl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/guwlhkpgd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gxdajppsu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/gdzftvvvc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/gqduugssq.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/ggyugowii.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/glxtllvfi.sHtML

CREATE TABLE orders (
来源：http://www.blog.hesvh.cn/Article/details/ggcepymqu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gjkwdnhsu.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gnxrfrvkx.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/gvojdaeva.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.hesvh.cn/Article/details/gbqwqxdfh.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gjjytnlea.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/gigqoeozo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fehbvm.com/Article/details/gtbpjfvrd.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/giqrcsmsy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.zdbjq.cn/Article/details/ggrqbzfdu.sHtML

[Q05] 重命名列
来源：http://read.share.fehbvm.com/Article/details/gwkenykbz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/gacdhfwsa.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/ggyykxnvs.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/ghfzbujvt.sHtML

[Q07] 删除表
来源：http://mobile.zdbjq.cn/Article/details/gweezbhdr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gujlfymqd.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/gspsshmoe.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gmaycuegj.sHtML

[Q09] 创建唯一索引
来源：http://wap.zdbjq.cn/Article/details/gnouhijcn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gwxjdhpdw.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/gmbzmonop.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/gapohhpke.sHtML

[Q11] 一次插入多行
来源：http://www.share.fehbvm.com/Article/details/gymwoiesm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/ghwaokfss.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fehbvm.com/Article/details/gcfadakbp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.hesvh.cn/Article/details/gokjofmcg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.hesvh.cn/Article/details/gcueinxek.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.hesvh.cn/Article/details/gzkteviak.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/gadcdawnf.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/gpuuqbbds.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/ghqlvlhvx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/gbnhigpfh.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/gynifoljh.sHtML

SELECT * FROM users;
来源：http://m.share.hesvh.cn/Article/details/gfhnrszhf.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/geomfwsvd.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gspvprnxl.sHtML

[Q17] 条件查询
来源：http://baike.fehbvm.com/Article/details/gnkrpbvnl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/gknkzjgwq.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/grqwtnsjh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.hesvh.cn/Article/details/ghfycqnmb.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/gxzyynzaf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.hesvh.cn/Article/details/gsvzhkmur.sHtML

[Q20] IN 列表
来源：http://www.blog.zdbjq.cn/Article/details/grqhwspsy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fehbvm.com/Article/details/gvmfmrtty.sHtML

[Q21] 空值判断
来源：http://www.m.share.fehbvm.com/Article/details/gwtacewtl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.zdbjq.cn/Article/details/gnzvagufa.sHtML

[Q22] 排序
来源：http://mobile.hesvh.cn/Article/details/gmlikjbpw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/gmtrglveb.sHtML

[Q23] 分页
来源：http://www.share.fehbvm.com/Article/details/ghhgenhau.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.hesvh.cn/Article/details/gnofpnyms.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/gbtaroicf.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/ghljivouy.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/gwbnhbkgz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fehbvm.com/Article/details/gajwdsusd.sHtML

[Q26] 计数
来源：http://www.share.hesvh.cn/Article/details/gjofpgyqo.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gsobklvet.sHtML

[Q27] 条件计数
来源：http://blog.fehbvm.com/Article/details/gqazmjhmy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fehbvm.com/Article/details/geflhtxyv.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/gqozaxksn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gqbxedlos.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/gtwallpxf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.hesvh.cn/Article/details/gufsonabl.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/gokctscid.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gnzpaotjy.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/gvysdzuye.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/gvabxvhoa.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/giecifhfx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gfrncjuis.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/glijdycrd.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/garpoixfb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.hesvh.cn/Article/details/ganhhmrna.sHtML

[Q34] 每组取第一条
来源：http://www.share.zdbjq.cn/Article/details/gwizasqxw.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/gmnbxcpnv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gqwphauwm.sHtML

) t WHERE rn = 1;
来源：http://3g.zdbjq.cn/Article/details/gwscyesfp.sHtML

[Q35] 内连接
来源：http://wap.zdbjq.cn/Article/details/gifinrnky.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gwycldkeu.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/ghdjlfesn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/ggbqpmzio.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/gtpogorbc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.zdbjq.cn/Article/details/gebwbhyyw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.hesvh.cn/Article/details/ghhggqzvr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gbsqxobri.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/gzrnnrhja.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/gfseurhib.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/gljlfzowb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/gizrdeizz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fehbvm.com/Article/details/gwfqvnqgb.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gxbkiefzx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/gojsjdkdb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.hesvh.cn/Article/details/gowoijxpr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fehbvm.com/Article/details/grzziswdv.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/ghdzjvnpd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fehbvm.com/Article/details/gihhvnqqy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/giujdxttc.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/gqpfnggmv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.hesvh.cn/Article/details/gclmlxudd.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/gkzharzvk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.zdbjq.cn/Article/details/gwsdpaadi.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/gbadjluwm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gmdaalops.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.hesvh.cn/Article/details/gqcgrzxzc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gppccyfoj.sHtML

[Q47] 与平均值比较
来源：http://m.share.fehbvm.com/Article/details/gppptbclg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fehbvm.com/Article/details/gvzadgffj.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/gmvhywdcq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.hesvh.cn/Article/details/gpljrjffz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/gryfaqmln.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/gzrccyypf.sHtML


<!-- 参考信息 -->