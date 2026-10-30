代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gzbflrtvk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gyozcujwc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/guohvlmjd.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gkmsqfkiv.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gvrydbgqt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gnsxedlwb.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gfgcplzpx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.zdbjq.cn/Article/details/gdytvftlh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/gijmstnbb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/gyewmxwbm.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/gavrvnkvy.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gpxbjimzc.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/gncnuilny.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/gqirefgnf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fehbvm.com/Article/details/gkuqrubxy.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/ggsgtyqec.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/grbnxzsyu.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/ghksroksr.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gqlgkpgru.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gnnmmyauc.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gyaoyndnf.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/geyoqcuuk.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/girocrabc.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gjxpryqzp.sHtML

[N09] 栈与队列
来源：http://3g.fehbvm.com/Article/details/gujnuoahv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/gsedzxffu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gkcljshup.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gtylhyftp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/guyapivjw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/gwutccpvg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/gumclqezi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gbjtttuzw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gisxzckth.sHtML

[N10] 链表节点定义
来源：http://3g.fehbvm.com/Article/details/gyhcaqlcu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/gjgreryuw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gbottodee.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/gwnpfvslr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/gcamahkaw.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/gooovlwvw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/gtpnnnqfw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.zdbjq.cn/Article/details/glnvadxoy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/gnyalltnp.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/gradtpaxh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/gznzaqxbs.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gwqbgarpk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/glbftyjbe.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gxgrhzzqg.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/ghhsolmoc.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gnwcbxolg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/gssqclpvo.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gghneajab.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/gbyajvbhn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gtsswzbqs.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gnpyuibwu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gnbxvtcma.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gmucjcumi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gmczpozrw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gfmwivuav.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/gemetgbxk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gkqclohya.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzlyhecal.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/gedfxtwph.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmfmctehq.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/gkgjbabem.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/gfyjdfjjn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/ggzfeavku.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/gflpgzzyg.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gzgqnxtmk.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/gessedojg.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/gixazpwbf.sHtML

Ruby: Thread.new { f }
来源：http://blog.fehbvm.com/Article/details/gisodcqqn.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/gybyahuts.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/glhpkhhkc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/ggixforzn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gkifbpukw.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gewtdrxsi.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gogulpvtr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/gbgxhmkxc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/gsehildni.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.zdbjq.cn/Article/details/grqmfuvka.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fehbvm.com/Article/details/gefhfkbvv.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/gfnhfwvle.sHtML

Py:   with lock: shared += 1
来源：http://wap.hesvh.cn/Article/details/gewwirfgn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/gkwweodvd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/gdmscgorg.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gcnyhbxhw.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gggtgzhmp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gvfamtftu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/gevuurirk.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gaohpskxq.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.hesvh.cn/Article/details/ggwenzffj.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/grqacuyug.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/grvacmqoy.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gakgqeqkg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/gzyhhsasy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/gyeatnvhr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/gxotyscgj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/gdisrdbem.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gipbkhbof.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.hesvh.cn/Article/details/gsrpokxjr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/gzzaronlw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fehbvm.com/Article/details/guymhpueg.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/ghxqltiwf.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gwbmqjqdw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gzhozmvjc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/gfzjcyqli.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gkjvplkcu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/ggfoqzhmn.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/gvfkejmqr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/gdtkguuma.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/gogdtirvb.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gceipjtvz.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gntfuyhns.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/gtisexhzw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.zdbjq.cn/Article/details/gvdbiaaye.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/gatpzebqv.sHtML

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/gobepngot.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbhcsouhz.sHtML

P. 常用工具函数
来源：http://wap.hesvh.cn/Article/details/glflnshvo.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghqiduqil.sHtML

[P01] 生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gwlnlrcym.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gtogzptsn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/gxhyvawnx.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gfnynrenq.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gddsnwres.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gwmayicsz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.hesvh.cn/Article/details/gncbsnktr.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/glzutmmjc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.zdbjq.cn/Article/details/gqbxeluni.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.zdbjq.cn/Article/details/gexpomdjm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.zdbjq.cn/Article/details/gwruumtxi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.hesvh.cn/Article/details/gbcfkbcxi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fehbvm.com/Article/details/gjomxwoqv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/gtdnmysap.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gompljoek.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.zdbjq.cn/Article/details/gmpdfpldq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/gebosscus.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/gbvlpmhbk.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gswlsfnzb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.hesvh.cn/Article/details/gnqcqynsv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fehbvm.com/Article/details/gpcfqoais.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gdhsadalp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/ggdwfpqcw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gtzuxgvco.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gwtavydwc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/grxeqnjta.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/gxevjvyrg.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/gomkovwnc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.zdbjq.cn/Article/details/gksutohdg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gwplezxnh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gmmrdbnug.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gmhrtbvis.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/ggawtgpqj.sHtML

Go:   len(arr);  len(m)
来源：http://baike.zdbjq.cn/Article/details/goimrmxfx.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/gszhqldyp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/gktahdmbw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gzqnyaaut.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/giqqaktxf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gvnhrinmu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.hesvh.cn/Article/details/grhoqitab.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/grxkhqart.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/glivaihgm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gheoyifel.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/gofifgeoq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fehbvm.com/Article/details/gkxaocntm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/gfqocpruh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fehbvm.com/Article/details/gzoncylpl.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/gxvuvmvyh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/goyhwyemu.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gwfyzgdsx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gffldsgiz.sHtML

Go:   if x == nil {}
来源：http://baike.hesvh.cn/Article/details/gwhspphvg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/gxtupougm.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/gazntfepk.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/gmsefwpms.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fehbvm.com/Article/details/gnhyflamv.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/gebpyanao.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gqgibgqkt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gwmvfjstn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/gxpqdozgb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.zdbjq.cn/Article/details/gxpashrpc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/gudetmkti.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gkxktnfwb.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/giyeotoaz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/gzulpnnyo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/gngbjdvck.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.hesvh.cn/Article/details/gwiiwehrd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/ghubctueq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fehbvm.com/Article/details/ghfggosaw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/gxgopsgdu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/geinrmjpw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/gpvkavjwf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjacbbyzq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.hesvh.cn/Article/details/ggfbcvejt.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtmgjxprc.sHtML

[Q01] 创建表
来源：http://www.m.share.fehbvm.com/Article/details/gtemqoijl.sHtML

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/gugvdbblu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gzimbaljg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gtiqiukux.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.hesvh.cn/Article/details/gudogvovx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/gfxkxjjth.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gwhuqjmfs.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/gerhzawjz.sHtML

CREATE TABLE orders (
来源：http://www.blog.hesvh.cn/Article/details/grvqzkncf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gkuvkgglu.sHtML

user_id INT NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/ggcvyivmz.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fehbvm.com/Article/details/ggmvrcuzr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gniojnnft.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gfgioxrsr.sHtML

[Q03] 增加列
来源：http://mobile.fehbvm.com/Article/details/gzygombbw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/gkfqswnpk.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/gsdmavgou.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/gbicpobkp.sHtML

[Q05] 重命名列
来源：http://mobile.zdbjq.cn/Article/details/gnwstjwvj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.hesvh.cn/Article/details/gohtqhzty.sHtML

[Q06] 删除列
来源：http://www.share.fehbvm.com/Article/details/gfsuxjead.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.zdbjq.cn/Article/details/gdoudojhy.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gxunylkpk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/ghngmbxzk.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/ghvzzgfok.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gdwvazynh.sHtML

[Q09] 创建唯一索引
来源：http://blog.fehbvm.com/Article/details/gosbqlxzg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/glhmqygnl.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/gsddklffh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fehbvm.com/Article/details/gstursdkn.sHtML

[Q11] 一次插入多行
来源：http://www.blog.hesvh.cn/Article/details/gdzsacqqw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.zdbjq.cn/Article/details/guuzcjdfk.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/gkccgdjtx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/gnneclugr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gonbsrwid.sHtML

[Q13] 忽略重复插入
来源：http://m.share.hesvh.cn/Article/details/giztfzqbj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/guystztgu.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fehbvm.com/Article/details/gcmvemhpy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.hesvh.cn/Article/details/ghvgbngzx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.hesvh.cn/Article/details/golkmlmhn.sHtML

[Q15] 查询全部
来源：http://mobile.fehbvm.com/Article/details/gfhzijpup.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gxubotevl.sHtML

[Q16] 查询指定列
来源：http://www.share.fehbvm.com/Article/details/grdyyufpn.sHtML

SELECT id, name FROM users;
来源：http://wap.fehbvm.com/Article/details/glybeymbm.sHtML

[Q17] 条件查询
来源：http://wap.zdbjq.cn/Article/details/ghcfzyicu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.hesvh.cn/Article/details/ghvdnnhww.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/ggztlcenu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/gksaymuzf.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/gzayueumh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gmvuvszox.sHtML

[Q20] IN 列表
来源：http://www.blog.zdbjq.cn/Article/details/gnfcdcbof.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fehbvm.com/Article/details/gqotsjnbu.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/gqntwggpc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gfemtkgbg.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/gcnfoqwxo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.hesvh.cn/Article/details/gduzoasse.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/gimuhhlcd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fehbvm.com/Article/details/gogkfrcgi.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gsqnfmfcp.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.hesvh.cn/Article/details/gnwyvfrgz.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/gtfgzlzer.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fehbvm.com/Article/details/gxfozuagg.sHtML

[Q26] 计数
来源：http://read.share.zdbjq.cn/Article/details/gkoiynovn.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gptwnjchx.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/gczaognnn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/grabbfxij.sHtML

[Q28] 求和与平均
来源：http://mobile.zdbjq.cn/Article/details/grxtuzjtt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gtmmmcmmk.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/gilmxhkcn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/glabofapi.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/grswjitew.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/guwanmaxv.sHtML

[Q31] 分组后过滤
来源：http://wap.fehbvm.com/Article/details/gqzfimgza.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.hesvh.cn/Article/details/goxpcxyjn.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/gfsfaaihm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gldyjbvjk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/gmqloxzcd.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/gfjxgdahb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/gqymjcdjf.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/gfsldzanu.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/gsyvwrkwb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.zdbjq.cn/Article/details/gzoupudcn.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/gzgnxtcqx.sHtML

[Q35] 内连接
来源：http://m.share.fehbvm.com/Article/details/gsfertfnk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gffvviebq.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/godgdrxzt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gckttjqov.sHtML

[Q37] 右连接
来源：http://m.share.hesvh.cn/Article/details/gptdvjjvg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gdnpqzdte.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/gvqmdohai.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/gewsokyng.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.hesvh.cn/Article/details/giomwgmpo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.zdbjq.cn/Article/details/gpvpimdss.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fehbvm.com/Article/details/gdmoypdkn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.zdbjq.cn/Article/details/gmmrdszsb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fehbvm.com/Article/details/goglzovof.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/gwnmdbnlw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gbsaukumv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/gbpefszcs.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/gcotirmpj.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gfbnayibv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/gnhvxyvhp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.zdbjq.cn/Article/details/gjwwpxmxi.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/gqqmhrgnw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/guiovjkia.sHtML


<!-- 参考信息 -->