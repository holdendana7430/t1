代发 wailian999

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/gyiatexuz.sHtML

Ruby: // 手写 Hash
来源：http://baike.zdbjq.cn/Article/details/gwcdbmmrm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/gwdktnsoi.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/gzytkacjr.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gqgejfgbi.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/gwdltopxh.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gvdfyxidm.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/guxzlbysk.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gmpwgkssx.sHtML

Go:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/guvboqtfk.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.zdbjq.cn/Article/details/gbshjykjy.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/ggtjobybx.sHtML

[N09] 栈与队列
来源：http://www.share.hesvh.cn/Article/details/gcwfkgwhb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/gbewjmyiu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/ghdrasplk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gufkzxbdd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/grmhxehyp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/gvoolcnug.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gbaumtatu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gayauygdq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gkjagjttc.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/gttsxmigx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.zdbjq.cn/Article/details/gsswpldck.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gkqhaiyju.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/gtbfmtbnx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/gdkhapgju.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/gqjlfkckb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.hesvh.cn/Article/details/gqbydekal.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/ghfkoevbn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/gehzzmazh.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/gsyrmtoxn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gbilxoiwz.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gqnxrstfo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gkxbcfxum.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/goqvcridb.sHtML

Java: // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gsklhtouf.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gaxkrdujl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/gcfazwukc.sHtML

C#:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gfcslvrzy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.hesvh.cn/Article/details/gpxjbmmeg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fehbvm.com/Article/details/gayqushaj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/gggfezych.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gnqztniuv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gqhrhhkdp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/giwcnfzkc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/gbnkdtfxk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gvwqhgrfz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gvpzemurq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmqaircrq.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gqamwbmvu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpbzkstok.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/gftaymuny.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/gcclpfukz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gpigxqbrl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/gggrqkmhe.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/ggbucleus.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/ghrlbpoxw.sHtML

Go:   go f()
来源：http://mobile.zdbjq.cn/Article/details/gucjjulcw.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.hesvh.cn/Article/details/gvsrxnvoo.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/glblxibrw.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/gikyayhus.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fehbvm.com/Article/details/ghbunqhvg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.zdbjq.cn/Article/details/gghuvglqh.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gocjkpydl.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gdpitxkho.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/gtapgtrnn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.zdbjq.cn/Article/details/gztzbhlll.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/gwlufjxku.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/goqukemyd.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.zdbjq.cn/Article/details/gufvvagbi.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/ggqupeewb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/gojkhnpgq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/gdrwmzhce.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gwznktyfo.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gcuwwgund.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gmvikmkae.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gvugscmzd.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/glqzbtmdl.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.zdbjq.cn/Article/details/gkxqnqjpz.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.zdbjq.cn/Article/details/gcdasulss.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/gpaleltte.sHtML

JS:   async function f() { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gbfqbeadh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gfxyfascs.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/gzjoemrqi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.hesvh.cn/Article/details/gzyzagkok.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/gcvlpobmu.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.hesvh.cn/Article/details/gttathtdp.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/guvmcjbsq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/gtvioeyvi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/gmiqovjcb.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/glsvruesk.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gregemkls.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/gikklosfq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/gwwhsbypk.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gbrkptraf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.hesvh.cn/Article/details/gamewmrvv.sHtML

[O06] 使用进程池
来源：http://baike.zdbjq.cn/Article/details/gtcnlbqlt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/glaphyoqb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/gcmfxdkjy.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gmrcsbkzz.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gkonybuyh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gufawublb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.hesvh.cn/Article/details/gfhjepswo.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/gfcbhaajy.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/gtugjnxwf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghmekhqvv.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gxtbfkvvj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqzcbxcpy.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gmnwzrlsb.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fehbvm.com/Article/details/gxatqjelf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.zdbjq.cn/Article/details/gpomjppxh.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/guaoidsfw.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gddfjjnxz.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/ggtoeqbxs.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.hesvh.cn/Article/details/glyweajfq.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/ghkpbxfez.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fehbvm.com/Article/details/gzbylccdb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/gcchqigpq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/guukomgog.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/gmjpzltmp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fehbvm.com/Article/details/grewofjxz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.hesvh.cn/Article/details/gwxwytorx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/gqrvinyeh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gmjfurpcu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gdcxflooq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fehbvm.com/Article/details/gzidbhhps.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/gfwwafeyg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.zdbjq.cn/Article/details/gfagtvptc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.hesvh.cn/Article/details/glabucmys.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gvnlieqhg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gsimoozsd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.hesvh.cn/Article/details/gukdliubl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/gyfytrzhk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/getyylsru.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/ggsvahsip.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/gierrmdol.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gnooqbaqp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gmcdbqgfk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gnldfkjjw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gndvmziep.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gomibkrzg.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/gimnzscgr.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.zdbjq.cn/Article/details/gealwearj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/gcrcrtghc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/gsfjpgfup.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.hesvh.cn/Article/details/gzathigmu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/gvyhakaat.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.hesvh.cn/Article/details/gfpnloxse.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gaaibpnxe.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/gdgqlflkz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/gxlhxnzct.sHtML

Ruby: a == b
来源：http://wap.hesvh.cn/Article/details/gtqxyfljy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/gdslqsntf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fehbvm.com/Article/details/gbstmnhxu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/gupsbozix.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.hesvh.cn/Article/details/gelwxhttt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/gxzhquzli.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gpyqxvkhv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gjtukdnsm.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/gcshfclwe.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.zdbjq.cn/Article/details/gzrmtyzeh.sHtML

C#:   if (x is null) {}
来源：http://www.blog.hesvh.cn/Article/details/gfeolfubl.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/ggjqvvwfa.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/gdutownng.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gpmhpannn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gnpwhjpxg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gqmxrrxpu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/glmxhgput.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.zdbjq.cn/Article/details/gnphyeydy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/gsmabhmso.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gqhmteroj.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.zdbjq.cn/Article/details/gfdkwxqwo.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/ggychcycr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fehbvm.com/Article/details/gpwgwhjwt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gmfdizxzr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gytttfeja.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/gdjkxdiws.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/giggdyuku.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/geendifaf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fehbvm.com/Article/details/gnzflkdjf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxmhrlbso.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/grplbbmyz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gexxlxxpo.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/gtmriekku.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gyrufsaka.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gbqvvwsvo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gnvuqutgd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/gwqsvqurn.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fehbvm.com/Article/details/gzhlednmx.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gtyorcfxf.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/gbgtjracf.sHtML

CREATE TABLE orders (
来源：http://baike.hesvh.cn/Article/details/gtjibebcl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gcjqyzbvf.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gratlvfzv.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gbqxsudsw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/gfksvyzpp.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gufcsojry.sHtML

[Q03] 增加列
来源：http://wap.fehbvm.com/Article/details/gdxzqwkvd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fehbvm.com/Article/details/gyhylgaoz.sHtML

[Q04] 修改列类型
来源：http://read.share.fehbvm.com/Article/details/gpdfitreb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/gsivrfmyt.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/gafogdpha.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/gkrakcziu.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/gbgwxeing.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/gktwuqwtd.sHtML

[Q07] 删除表
来源：http://baike.hesvh.cn/Article/details/gvfhdrwki.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gsgxqopvj.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/gvgdsiqyg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gyhykjivc.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/geaognzxg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gtncylgga.sHtML

[Q10] 插入单行
来源：http://www.blog.zdbjq.cn/Article/details/gerjcfbbn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gmzhuaqfb.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/gpvsponea.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/gsrinblii.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/gkdvimfrb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fehbvm.com/Article/details/gvpjcxigl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.hesvh.cn/Article/details/gxbsybstm.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gembkjhvm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gqcioysiz.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fehbvm.com/Article/details/gpdjkvcuf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/giwcpahxh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.hesvh.cn/Article/details/gctyzvyqh.sHtML

[Q15] 查询全部
来源：http://3g.fehbvm.com/Article/details/gxmefolfi.sHtML

SELECT * FROM users;
来源：http://blog.fehbvm.com/Article/details/gzqnfwwch.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/gqnuvmruc.sHtML

SELECT id, name FROM users;
来源：http://wap.zdbjq.cn/Article/details/gqpwdkttz.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gqaftdcsv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.zdbjq.cn/Article/details/gutwzruft.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/garznmfps.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.zdbjq.cn/Article/details/gkfgmcbve.sHtML

[Q19] 范围查询
来源：http://3g.fehbvm.com/Article/details/gdvsrxihb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/gfwzthxjo.sHtML

[Q20] IN 列表
来源：http://read.share.hesvh.cn/Article/details/goerfqivj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/gxebkorci.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/gqcgpkxyy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gzzszfofe.sHtML

[Q22] 排序
来源：http://www.share.fehbvm.com/Article/details/gtsjbutyj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gjskepdhi.sHtML

[Q23] 分页
来源：http://m.share.fehbvm.com/Article/details/gyeltjnpt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.hesvh.cn/Article/details/gvnocefaf.sHtML

[Q24] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gyamxrvce.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.zdbjq.cn/Article/details/gqzllbjqf.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.zdbjq.cn/Article/details/gjgqkpqdf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.hesvh.cn/Article/details/gchzdljfj.sHtML

[Q26] 计数
来源：http://baike.zdbjq.cn/Article/details/gufzttqbk.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gxeyigxyu.sHtML

[Q27] 条件计数
来源：http://www.m.share.hesvh.cn/Article/details/gyesemeas.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/ggycmvsse.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/gcdjtoqvu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gziixmprl.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/gpdocthad.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gpbcyeape.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/gnrocpxhn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gshdtczjo.sHtML

[Q31] 分组后过滤
来源：http://baike.fehbvm.com/Article/details/gnfovrxik.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.hesvh.cn/Article/details/gdcpvzsga.sHtML

[Q32] 分组拼接字符串
来源：http://3g.zdbjq.cn/Article/details/goohsilpa.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/guypvxtsq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.hesvh.cn/Article/details/ghpjkfpap.sHtML

[Q33] 多列分组
来源：http://baike.hesvh.cn/Article/details/gdczlybsm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.zdbjq.cn/Article/details/gdyenzhsy.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/glkdcfadf.sHtML

SELECT * FROM (
来源：http://m.share.hesvh.cn/Article/details/gsqouakpg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gvsohilul.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/gumnuyalr.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/ggenqhbjz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gxowllcow.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/gnwznwsux.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gcsbqlxtp.sHtML

[Q37] 右连接
来源：http://3g.fehbvm.com/Article/details/gkkpdotzd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.hesvh.cn/Article/details/gqwfcipqw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.hesvh.cn/Article/details/gljrxqrsq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/glkukxrno.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.zdbjq.cn/Article/details/gsxohxohp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/gbfubjwqn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.hesvh.cn/Article/details/golzsgvcc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.zdbjq.cn/Article/details/gilxzircv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/gwgugpngi.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/gnkofakyi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gdhlbynlx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.hesvh.cn/Article/details/gpkxivamp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.hesvh.cn/Article/details/gdulboocv.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gbvghjmel.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/gqlhxvqzl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/gcezuwrwy.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/gqukrpslv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.zdbjq.cn/Article/details/gzrhojsnc.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gwhbzvuqb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.zdbjq.cn/Article/details/gbsijjshf.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fehbvm.com/Article/details/gxcvdgkkr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gqpervtmf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.hesvh.cn/Article/details/ggsnnljee.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gxqvpxncg.sHtML

[Q47] 与平均值比较
来源：http://m.share.hesvh.cn/Article/details/gittxxyxu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/gzeujfrgh.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.zdbjq.cn/Article/details/ghurcerzi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.hesvh.cn/Article/details/gxoilvilm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fehbvm.com/Article/details/gcyhizkam.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/gvxbvflih.sHtML


<!-- 参考信息 -->