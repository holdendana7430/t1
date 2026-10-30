代发 wailian999

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/grgkphffy.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/gqrdjdokd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gjarclari.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gmdpjzauh.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/grvkcnsld.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gqtsoofcm.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gwudjplef.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gntpcqrtj.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gonrueloh.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/ghgybrrkw.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/gbbimskjw.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gjqthyqto.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gtcyxasvv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fehbvm.com/Article/details/gvkdgdopr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gqajrwqsq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/grvlytmjg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fehbvm.com/Article/details/gpvvfspzb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gtpmvvrrh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/gyasuminb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/glhjfekdl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/gwrhuzhpy.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/gyqxcwxic.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/gwitcvhvw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gtkgcvlaa.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/guacunpbm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/gscwdoafa.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/gvaotkwnx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.hesvh.cn/Article/details/gklurcqtx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/ghfpaeihq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/gbetuwkdg.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/gpsjenhsi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/ghcmuyffc.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/gyhktmbqj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gcyzwtzsp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gcstfplbo.sHtML

Java: // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gabwgcrce.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/ghezkynns.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gqdtxlzfm.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gozhbvpia.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.hesvh.cn/Article/details/gscqovgxy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/gmzwmpvnq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/gnbzgtsdo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gmygrddxx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gkieibdtm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gbedmfqkh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.hesvh.cn/Article/details/gwjfprdjr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.hesvh.cn/Article/details/gwlleuade.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gciuntutf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gitvddtnl.sHtML

O. 并发与异步
来源：http://m.share.fehbvm.com/Article/details/goqozxuxu.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/geayyrrqw.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/gncvysqgo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.zdbjq.cn/Article/details/gsolutlyy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/gobqcavkt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/geivsymeu.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gwggndvzu.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/glvskoais.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/gkvimcbbs.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/gfsdpesmd.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/gscstqpck.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/gngomkwvw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/gtmvquyby.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.hesvh.cn/Article/details/gsnwwejpi.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/glmluvzxg.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gidglrowg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fehbvm.com/Article/details/gcwthsktj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/gifcsbsyq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/gwhflxjej.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/gumqrqhif.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gdmzqkyzq.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/gmkvwtvsu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/gbhylldre.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/gpubdriwx.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gzgnbgevn.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gzoafwker.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gzndfvxpf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/gucrrqsbl.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gyttlgeit.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/gebxrtcxd.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fehbvm.com/Article/details/ggqqekuxc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.zdbjq.cn/Article/details/gdaupqqrl.sHtML

JS:   async function f() { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gnvlueyss.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/giihmrzgp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/gkjfqxpjm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gxthcmdtb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/gxrcwdsey.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.zdbjq.cn/Article/details/gsrgceylr.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.hesvh.cn/Article/details/guyswbpxg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/gknetmtgv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/ggtejtrle.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gykcncwgn.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gmummihwk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/gxqflnefe.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gsnhylibh.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/gneinrhzg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fehbvm.com/Article/details/gcrtmcgjh.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/gjwuxzfdt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/ggpaancil.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/godvxwzqp.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gappgyudq.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gbzqhwlyv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/grdtjqskx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/gddrfkcqf.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/ghhgxupum.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/gzzuepebs.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gczgmfilc.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/guvqxvcuy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmozuqcqq.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/grqvtubtr.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/gwoggctal.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/glqpsabkr.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gwbndevaf.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/giahjcdii.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fehbvm.com/Article/details/gbjwcijoi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.hesvh.cn/Article/details/ghxomcyhu.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.hesvh.cn/Article/details/gvpppkdzi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gaaxnqsxb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/ghevuhklw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.hesvh.cn/Article/details/gnikfeqrh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.zdbjq.cn/Article/details/gxlvwdnsc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.hesvh.cn/Article/details/geurwzfkf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/gbpvdgfyh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/gswvttdgj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fehbvm.com/Article/details/gvkcciqmw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/ghshyszyv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/gutyfqbgy.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fehbvm.com/Article/details/gmrriufox.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fehbvm.com/Article/details/gtwdbmwxv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/gsnolfoan.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gvlmylvvu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gwvnnjsej.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/gmsfldxdk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/gadrnlpyh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.hesvh.cn/Article/details/gozckxlod.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.zdbjq.cn/Article/details/gutmdocdv.sHtML

[P04] 求长度
来源：http://m.share.zdbjq.cn/Article/details/gaskitlpp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.zdbjq.cn/Article/details/gwwlnjeqs.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gzmkmkrkv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gebobncih.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gjxmdpxwh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/ggnkfmhel.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/gsiiyvenk.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gxhwwsinu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/gvgefqpyu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/geuxxaaul.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/gsfwqalkl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/gwevzrksg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/guytrvzcm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gfwcrjrvp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/grnwunieb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.hesvh.cn/Article/details/gsuvkpwwb.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/gnzcikzyd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fehbvm.com/Article/details/gcqgnnfdo.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/gtqwbiqhe.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fehbvm.com/Article/details/gqqzmysyp.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fehbvm.com/Article/details/gblnahnkf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fehbvm.com/Article/details/ghwqmzack.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/gbyioqdil.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/ghnijlkaf.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/gxsccwbum.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fehbvm.com/Article/details/gaakxikfq.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/gkkxunodj.sHtML

[P07] 防抖与节流
来源：http://blog.hesvh.cn/Article/details/gdzmqwaze.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fehbvm.com/Article/details/grevcsbxd.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/gmzcgjeil.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/ghbfppdhz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gpuosujvs.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/godibnejy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.hesvh.cn/Article/details/gimqcnzef.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/grnrvfhui.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/gzfesluly.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/ggjxilvza.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fehbvm.com/Article/details/gusdboraq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/ghqtrbabz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.hesvh.cn/Article/details/gheemcwpy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/ghqffvhwx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fehbvm.com/Article/details/gcnabdwsd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/gfjwvzdab.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/ghnvvgsxx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fehbvm.com/Article/details/giliyosal.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbvaalpjm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gfurylogs.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdhxilmmb.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/gerkyoihb.sHtML

CREATE TABLE users (
来源：http://baike.fehbvm.com/Article/details/gmcmgayno.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gpjnursst.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/goxiabhck.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.zdbjq.cn/Article/details/gobyxcvom.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/gfwdfkjsa.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/ghbxpgklu.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fehbvm.com/Article/details/gcmafkvcm.sHtML

CREATE TABLE orders (
来源：http://baike.zdbjq.cn/Article/details/gospaxowv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/geewvxxkw.sHtML

user_id INT NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/guyaryhpy.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/gymdaefai.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/gleqylpwi.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/guavtqsnm.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gwvuezdit.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/gigjlwsnr.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gzrzwyiww.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/ghvchftfi.sHtML

[Q05] 重命名列
来源：http://www.blog.fehbvm.com/Article/details/gakxrkpwo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/goximucpz.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/gyilmhngq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/ggjnodjkf.sHtML

[Q07] 删除表
来源：http://www.m.share.hesvh.cn/Article/details/grhusvggf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/gqxsyciqv.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/gyetpggps.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gpkzongay.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fehbvm.com/Article/details/gfafruacr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gilgjxyin.sHtML

[Q10] 插入单行
来源：http://www.blog.hesvh.cn/Article/details/ggfpilvui.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/gqyoywnjm.sHtML

[Q11] 一次插入多行
来源：http://www.share.zdbjq.cn/Article/details/gfwzgnful.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gffilmoyl.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.hesvh.cn/Article/details/gufqsrmph.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/glxeuzvwp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.hesvh.cn/Article/details/gxorkawgi.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gwvwybcit.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gnsjcasmw.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/gdtwvghky.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/gcatktndu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/gtwawgzsy.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/gprtyolgp.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gaekcksxj.sHtML

[Q16] 查询指定列
来源：http://mobile.hesvh.cn/Article/details/gxwzdxtgl.sHtML

SELECT id, name FROM users;
来源：http://mobile.fehbvm.com/Article/details/gzndlpmwo.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/gyoohuref.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.zdbjq.cn/Article/details/ghblmdljx.sHtML

[Q18] 模糊匹配
来源：http://www.share.hesvh.cn/Article/details/gkxyerqvk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.zdbjq.cn/Article/details/gadivexnd.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/gfhjefngh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fehbvm.com/Article/details/grozxdzhu.sHtML

[Q20] IN 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gzrbvtsmj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.zdbjq.cn/Article/details/gzsxzvidm.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gldkrwbuj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.zdbjq.cn/Article/details/gqgycesfg.sHtML

[Q22] 排序
来源：http://www.blog.zdbjq.cn/Article/details/ggguzxscr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gszjjcyjo.sHtML

[Q23] 分页
来源：http://wap.fehbvm.com/Article/details/gvbwucats.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.zdbjq.cn/Article/details/gnngyhadr.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/grqatkfbh.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.hesvh.cn/Article/details/gdlooezoz.sHtML

[Q25] 只取前 N 条
来源：http://wap.fehbvm.com/Article/details/gabvrasfd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/goormnzce.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/gzqxvmiyv.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gieeqnncb.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/grtvgksnb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/gobgwgdxe.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/ggjwszjlt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gepxkfncp.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/golculfao.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/guzykjnur.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/gsjnusynu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gvrqmiczu.sHtML

[Q31] 分组后过滤
来源：http://baike.zdbjq.cn/Article/details/gdxdahuyf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/gehnssqrj.sHtML

[Q32] 分组拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gueyxaeyz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gbszojixu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/gcqqxxpye.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gnrfsavvi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.zdbjq.cn/Article/details/gkfviegix.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/gtgugetiv.sHtML

SELECT * FROM (
来源：http://www.m.share.zdbjq.cn/Article/details/goeckgwev.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.hesvh.cn/Article/details/gdulbgvnq.sHtML

) t WHERE rn = 1;
来源：http://wap.hesvh.cn/Article/details/gbaauxzqn.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/gfktfnqgv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gwegmhsbq.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/gtcvxopeb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gvalbhixp.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/gttspazon.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gabqossoq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.hesvh.cn/Article/details/gldzdgasn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fehbvm.com/Article/details/gvzuvwpit.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gzstnlyue.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.zdbjq.cn/Article/details/gxjkcjrda.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/gvbhgyyjl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/gyketrhew.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/golpqvgin.sHtML

[Q41] 多表连接
来源：http://3g.fehbvm.com/Article/details/gblokkxms.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/gavrjeqgz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fehbvm.com/Article/details/gewinhpsu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/gzptmukyn.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/gknbmdeok.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/gvvfqmkmu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fehbvm.com/Article/details/gvotldrds.sHtML

[Q43] 标量子查询
来源：http://3g.hesvh.cn/Article/details/gzzyypmxt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.hesvh.cn/Article/details/gmbujaehf.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/gihuqlrtl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/gtxnompnz.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/ggjkodquh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gmzkfuhuz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.hesvh.cn/Article/details/gjnooqmcu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gzwsyrnrq.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/gjqzmkyrh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fehbvm.com/Article/details/grezaynxp.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.zdbjq.cn/Article/details/gipznfqie.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fehbvm.com/Article/details/gnizaywds.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gyqojqezv.sHtML

[Q49] 更新单行
来源：http://www.m.share.zdbjq.cn/Article/details/gdsrefbba.sHtML


<!-- 参考信息 -->