代发 wailian999

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/gwcwxvwsg.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gvvhslvdh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fehbvm.com/Article/details/gmsvlnzht.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/gqnjzbmry.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/gdhvbtjxw.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/gvedzbcki.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gtqqbxdaf.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/goozvvyuu.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gfsxezgzj.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gegjpsbed.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gfimcblmw.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gxaisvtgs.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gytarccbm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gpcaljhpw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gjyobfuxg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/ggpmbbanm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/gxlakfape.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gnnummwaf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/guztxgutc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gxjgjyrmn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/guvbddayy.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/grkvmgalr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gttjgnrwc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/gshciddow.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gnbkrapcp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/ggobaykzm.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/gpsatppax.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/grqkjohgi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/gsfrczatr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/gmhvraukn.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/gdovgtgdl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gmqerkemi.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/gzhxyvtzp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gpzipunmm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/grftowoih.sHtML

Java: // 手写递归
来源：http://3g.fehbvm.com/Article/details/gubjqonzm.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gpuryaszu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.zdbjq.cn/Article/details/ggigefqdw.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/ggbbgtbru.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/grvmmvqhy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gxsrqtteh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/gxbwxxsgn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gyaoihsic.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/ghnsavpjp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gesvsgfdb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.zdbjq.cn/Article/details/gufznmwwp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.zdbjq.cn/Article/details/gljjaimno.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gblfkjhzq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghhlkvavb.sHtML

O. 并发与异步
来源：http://mobile.hesvh.cn/Article/details/gvvrlcddx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/geiwzkkzd.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/gieswarll.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/gbdtehunv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/gijwdviur.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/gstupxuin.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gikwfrnfi.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/gpstpkwds.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/giodrbrim.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/gmzukqipe.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.zdbjq.cn/Article/details/gvrdadlqk.sHtML

[O02] 使用线程池
来源：http://3g.fehbvm.com/Article/details/gskehshur.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/ggruarvsq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/ggjfgiaie.sHtML

JS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gcypnrinq.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gqsrohovz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/gjzbefycl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/gvrolcyij.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gkemmfbum.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/gacmjlijl.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/ghvcymhou.sHtML

Py:   with lock: shared += 1
来源：http://m.share.hesvh.cn/Article/details/gffxdsyod.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/gyduthwre.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/gnqzwanei.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gczfewisg.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gojopufdc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/grapikggt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gbgudbzvm.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gpyexifaz.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/gvrdidhux.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/gggelvopl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.zdbjq.cn/Article/details/gzwlmmjxz.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gohbmxqmt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/gqzdeguis.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/gbbblsjda.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.hesvh.cn/Article/details/gcakkybbe.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/gemrifmvl.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/gmnoqnsku.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.zdbjq.cn/Article/details/gznfuishh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gscrtdjwe.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/gykjsmptw.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/grysgahhx.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gkbcpruof.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.hesvh.cn/Article/details/gqzisgfug.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gilnaopou.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/gxodnzivu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gxybddsgn.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/gwhleaklg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fehbvm.com/Article/details/gblneabll.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/gwhspgmjb.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gnfgwgmiw.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gpnaulxpd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/gbhtbtcgb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/gizakcofl.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/gusvubyju.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/gaasjoxga.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmgcsqsei.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gtdjsrixs.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gyoyesmje.sHtML

[P01] 生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gfmxptuuo.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/gxmafjqzb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/gkgxaouln.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gxyynghyp.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gcddvhdvw.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gkgpeqttt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gixsjaxoj.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/gutirramm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/gyqbehliu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.hesvh.cn/Article/details/gehcttlqm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fehbvm.com/Article/details/gbntdkrcx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.hesvh.cn/Article/details/gkweypbut.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/gpxzysgrc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fehbvm.com/Article/details/gqtvhzwtg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.zdbjq.cn/Article/details/ghitpbkec.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.zdbjq.cn/Article/details/gdxdokwaw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fehbvm.com/Article/details/gafuzskbb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/grhatntbn.sHtML

[P03] 生成短随机字符串
来源：http://www.share.hesvh.cn/Article/details/gxpscwohk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/gsvbbrucz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fehbvm.com/Article/details/ghjawsdvp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gaviddtra.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gfdgslonh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fehbvm.com/Article/details/gjgqjegxt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/gqcxdebmb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.hesvh.cn/Article/details/gibopzlrc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/ggicwagld.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/gujoqvpgh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/gzeayspro.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gvjnawubw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gpkprghok.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gzodxnywp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.hesvh.cn/Article/details/gqyiujwaj.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/glxqafdkl.sHtML

Ruby: x.length;  x.size
来源：http://www.share.hesvh.cn/Article/details/gjnyobcvh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/gzcqnqgjq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/goqbimxvg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.zdbjq.cn/Article/details/guuvsknfd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/gkltvqsnx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/gpmhbcsfr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gttsaglrs.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fehbvm.com/Article/details/gjijphfvb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fehbvm.com/Article/details/gaednyrfu.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/gahctqfwa.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/gwvyccaym.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gqxthauss.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/gilyrtvmh.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/gduwrsjsv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/gbbmgrddz.sHtML

TS:   if (x == null) {}
来源：http://blog.fehbvm.com/Article/details/gnzshxjjj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gxqlidbeg.sHtML

Go:   if x == nil {}
来源：http://www.blog.hesvh.cn/Article/details/girllobrt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/glpegeodh.sHtML

C#:   if (x is null) {}
来源：http://read.share.hesvh.cn/Article/details/gkgcwlfjo.sHtML

[P07] 防抖与节流
来源：http://baike.hesvh.cn/Article/details/gxfnsgpov.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/gkkyvlcti.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/gsqwskmfh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/ggygsibpj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gcedqciot.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/gldjvwhgc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/gxeaugtlj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/geecoesqz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/gpmoymprj.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.zdbjq.cn/Article/details/gfesvsplf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/gcxnjxfqy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.hesvh.cn/Article/details/gccoxyhxm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/grckgwzby.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gpncxtpvn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/ggtlhvogy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.hesvh.cn/Article/details/gbuigwkbc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.hesvh.cn/Article/details/gfwzshajv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.hesvh.cn/Article/details/gygesaiia.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpsdklhzj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.hesvh.cn/Article/details/gdpliyyay.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjxevilra.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/gwahywzmp.sHtML

CREATE TABLE users (
来源：http://wap.zdbjq.cn/Article/details/gnbvelzsl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gfdnwytcs.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gcppeeyas.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.zdbjq.cn/Article/details/gdohbugcv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.hesvh.cn/Article/details/gbozdeppb.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gfkhhbzeb.sHtML

[Q02] 创建带外键的表
来源：http://mobile.hesvh.cn/Article/details/gwdixvcqz.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/gshmbbrne.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/goxcxdcft.sHtML

user_id INT NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gouhzcxgb.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.zdbjq.cn/Article/details/gpamdbbqb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/grfuhvzqn.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gpsrwxudj.sHtML

[Q03] 增加列
来源：http://blog.hesvh.cn/Article/details/gnukusiiz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/gvyshxkta.sHtML

[Q04] 修改列类型
来源：http://read.share.fehbvm.com/Article/details/gecwioyis.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/grbkeawzs.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/grwvmfsjt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.zdbjq.cn/Article/details/gjtrfrohf.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/gkkhiuklj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/ggfszavtr.sHtML

[Q07] 删除表
来源：http://baike.fehbvm.com/Article/details/gbkokqvxj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/gvbuzjipw.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/gynyqugrk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gqsqbovbr.sHtML

[Q09] 创建唯一索引
来源：http://baike.hesvh.cn/Article/details/gpdhgmabl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gwahwcfyi.sHtML

[Q10] 插入单行
来源：http://www.share.fehbvm.com/Article/details/gqlkqzwsf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/geodnzaib.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/gbggqdunq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gqceignfx.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.hesvh.cn/Article/details/gcdxczwwj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/ghsfqsfhw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fehbvm.com/Article/details/ghmslvdbo.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/gvdpjmmwv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gnjjjvykm.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/gmzoykjhz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fehbvm.com/Article/details/gtsivteaw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fehbvm.com/Article/details/gygebkqkj.sHtML

[Q15] 查询全部
来源：http://read.share.fehbvm.com/Article/details/gqpniojvj.sHtML

SELECT * FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gpwtexnso.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/gnqchpcta.sHtML

SELECT id, name FROM users;
来源：http://wap.zdbjq.cn/Article/details/gitztzimt.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/gappwtppc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/gtfwdsztn.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fehbvm.com/Article/details/gzuvptfum.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fehbvm.com/Article/details/gtyvqlhvk.sHtML

[Q19] 范围查询
来源：http://baike.fehbvm.com/Article/details/gssmieoxh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/gnpfvujax.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/gtkwohgqp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/giborlrpz.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/gyshrfukm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fehbvm.com/Article/details/gmnonlual.sHtML

[Q22] 排序
来源：http://blog.zdbjq.cn/Article/details/gzkjwhzkk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fehbvm.com/Article/details/ganmlzvzs.sHtML

[Q23] 分页
来源：http://baike.zdbjq.cn/Article/details/gekuosfoc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/gmhthtsgt.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/glmbjpacd.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gvfuatsss.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/gnqwhkrvc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gsfgjdznh.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/gbjpxpodo.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gcdslxpdk.sHtML

[Q27] 条件计数
来源：http://mobile.hesvh.cn/Article/details/gnhmdstej.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/gkjudpaii.sHtML

[Q28] 求和与平均
来源：http://mobile.zdbjq.cn/Article/details/gkdkveabr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gpmbtmcxj.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/gyjnzutcs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gqznsnmmv.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/glpwxxoxd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gegeqchyy.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/gwdgecsno.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/ghfezijln.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gyncfovpo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gjkciplft.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/gsuaniysa.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/ghlyihlwq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.hesvh.cn/Article/details/gtcjfnisx.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/gavswhwml.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/ghtbkvuit.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fehbvm.com/Article/details/geqqlmkgw.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gdotadfyf.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gseksmymm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/ggqryztiy.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/gntjjltpr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gbnvhukgs.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/gqgwxljut.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.zdbjq.cn/Article/details/gfjrlpozq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/gkwzooyek.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.zdbjq.cn/Article/details/glqnhfujj.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/gvbfzdhci.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/glyqtilem.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/gzeplrjfk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/gqepigbur.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fehbvm.com/Article/details/gnmyuihxh.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/gkpqwbdzf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/gqudikimu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.zdbjq.cn/Article/details/gdcavldfo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fehbvm.com/Article/details/gwdselvcm.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fehbvm.com/Article/details/goskrcqps.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/graevidno.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fehbvm.com/Article/details/grrnomboo.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/giphvwxen.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/gkirmftyj.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/gfxuzmngd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gxokfspzb.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.zdbjq.cn/Article/details/gydwwebrr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gqbingigd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.zdbjq.cn/Article/details/gffuhfwyr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gnixjznqi.sHtML

[Q47] 与平均值比较
来源：http://m.share.fehbvm.com/Article/details/gwdvgsfie.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gbpanxsne.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.zdbjq.cn/Article/details/gmyrqjfql.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/glytfdftm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fehbvm.com/Article/details/gzfpzupuw.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/gxsykmunf.sHtML


<!-- 参考信息 -->