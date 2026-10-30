代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/ghkedijnd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/ghnvilsxs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fehbvm.com/Article/details/gwscdccpw.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/ggfbjhmxi.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gmwoloiab.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gojgsvqai.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/gubjbxicq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/ghqgzqjdb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gjtxxtkgx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/gelweejpm.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gbmiztqih.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/glnoexdgd.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/ghuomkxzl.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/gyvyzcpou.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gixtbcgsg.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/gsnqmuwyk.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/gbunytgfe.sHtML

PHP:  // 手写递归交换
来源：http://wap.hesvh.cn/Article/details/gifnowcqu.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gergprzeu.sHtML

TS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gtufuxrnh.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gulsejbir.sHtML

Go:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/ggctuojgt.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/gphywczvy.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gzynijgxd.sHtML

[N09] 栈与队列
来源：http://www.share.hesvh.cn/Article/details/gewvudbot.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/gyqswygxs.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/ggjdldrkl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gfunqbtiz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/gdoubrjvv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gwzchlogo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/ggjwfswac.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gmbfujvcc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/gdbtlpmen.sHtML

[N10] 链表节点定义
来源：http://m.share.zdbjq.cn/Article/details/gbmiceimq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/gwtmbcdbh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.hesvh.cn/Article/details/gbqhaysle.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gkvfaebvb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gqbwrhmap.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gcmktznmc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.hesvh.cn/Article/details/gfeywqbst.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/gsfhoyekj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/glsnalrrp.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/gouwvupvz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/gvijpmzjn.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/geokkyjqj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gbxfcussn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gosqitksn.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gfufzzslb.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/ggdnyrjev.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.zdbjq.cn/Article/details/gefpqzqzp.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/geinlbthk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gheoapocg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/gsqgzfwqy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.zdbjq.cn/Article/details/gjjwtykqd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gecrbmgky.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gyjqhaubh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gitlxcvgn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/gvsgxxlks.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/ggtmdkksi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gtmbqbdah.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjoaawsno.sHtML

O. 并发与异步
来源：http://www.share.fehbvm.com/Article/details/ghalsbjsh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gigsnkevb.sHtML

[O01] 启动一个线程
来源：http://blog.zdbjq.cn/Article/details/gabfpcppq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/gotnckpfm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/gzbhchjgi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/gyjsdznxc.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gmdhmsfjb.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/gxgrviiih.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/gerknduqy.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/gkeybvewg.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.hesvh.cn/Article/details/gmchmgdfq.sHtML

[O02] 使用线程池
来源：http://wap.zdbjq.cn/Article/details/giejrxijj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/gdmdvnxzl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gcpybpntv.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gmosdqyhl.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gkeauporp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gwnykrpzz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.zdbjq.cn/Article/details/ggeglplsw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fehbvm.com/Article/details/gsgaclbqm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.fehbvm.com/Article/details/gupjxogtb.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/gzybspknx.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gveavregs.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/gjghelmhj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gyrkgkbmf.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/giuipempc.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gqlokhamu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.zdbjq.cn/Article/details/ggtyrvzig.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.zdbjq.cn/Article/details/gysfoozlj.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gjauhfkqu.sHtML

[O04] 定义异步函数并等待
来源：http://blog.hesvh.cn/Article/details/gsuegsgmj.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/grpuradby.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gauqfhaau.sHtML

JS:   async function f() { await g(); }
来源：http://blog.hesvh.cn/Article/details/glowatlgl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gonswtheo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/gafnutegt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.zdbjq.cn/Article/details/gkyjmdzqj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fehbvm.com/Article/details/gjazpdocl.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/gjfuqxvix.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/gmkgnzixk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gnztykwmd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.zdbjq.cn/Article/details/grvwqyttw.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gaoevhvan.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gznywovjh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/gmkdmcuft.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gnhwfgufg.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/grasvoyvz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.hesvh.cn/Article/details/gdnsawxuk.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/glrinbolm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fehbvm.com/Article/details/guchjrjsn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/gdzxuypga.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gnqdcxygz.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gcrdqzlcr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fehbvm.com/Article/details/gquvypylq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/gshbgtgis.sHtML

Ruby: // fork 块
来源：http://www.share.zdbjq.cn/Article/details/gbpkernkd.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/ghftohaga.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvmodcvyt.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gbesdivel.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwjlzvyfc.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gqopenfqn.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/gbeiihzni.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gefikgpax.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gqqkadhdn.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gsorlkhaw.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/gkpvkotbh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.zdbjq.cn/Article/details/gnseboquu.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gpbpkjrsn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fehbvm.com/Article/details/gyrjwlmye.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/geiwrhbuq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/gewxrdzup.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/grntctbrw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/gzcojrhdd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/glgxrwgtw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/griabouup.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/gjatkmbnh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.hesvh.cn/Article/details/gffgkjbuq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/gfkhfnovk.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fehbvm.com/Article/details/galnzeizy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/goczxeuez.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/gzwxjxgin.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gunewzuwt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gkijywgxn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/gdpkhrblt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.hesvh.cn/Article/details/gmscbbfro.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/ghlqjmplp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/gdqwqehql.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/ggsludroc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fehbvm.com/Article/details/grirqfqll.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/ghqnpuxsu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/glsynhjic.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gacfiaecm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fehbvm.com/Article/details/gbtxxejzu.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gebeegdjx.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/gukkpijyp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gylncmucx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.zdbjq.cn/Article/details/gusboktfb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/ghghecqqp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.hesvh.cn/Article/details/gxrhhemlk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/grptnuiqw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gcbogdbot.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fehbvm.com/Article/details/gramdhgxc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.hesvh.cn/Article/details/gfcqclxcw.sHtML

Ruby: a == b
来源：http://wap.hesvh.cn/Article/details/gnhyabshh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.hesvh.cn/Article/details/gyesxkxtx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/gfaqcfzez.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/gjklybyhg.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/gueppqyfd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/gpuecovli.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/gfnbxweyf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gytoolxyr.sHtML

Go:   if x == nil {}
来源：http://m.share.zdbjq.cn/Article/details/gkabwvhxg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fehbvm.com/Article/details/gklousauy.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/gavilkuqt.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/grqjzfjnc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/golybwfjz.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/gygvxfeix.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/glconhkbe.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gvfzotyzf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/gwfalitwn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.hesvh.cn/Article/details/gjpoxgfee.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/grmhvptva.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/gmfqztgwf.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/goqdrdlrb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.zdbjq.cn/Article/details/golhntwui.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/gvxzxxbat.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/gvhvhqalu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gpkaffcoi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.zdbjq.cn/Article/details/gbfrnnszj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/ghmkkeklf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/gmeoproqg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/gmcboyjps.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnpqljyge.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fehbvm.com/Article/details/gwoykkmvh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtsnsnszm.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/gxtotaoht.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/gvgbjonnk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gtbbdhusz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gqfwxgaos.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.hesvh.cn/Article/details/gxxezgzdt.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.hesvh.cn/Article/details/gedayjish.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gavuxrcvo.sHtML

[Q02] 创建带外键的表
来源：http://baike.fehbvm.com/Article/details/gbocvhiab.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/gtbrprmfs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gactpmfae.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gpxsagiml.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.hesvh.cn/Article/details/gmmdkdusq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/gsaqvdqqi.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gvkywofnp.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/grvhfalsj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.hesvh.cn/Article/details/gvigsqcrg.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/gdhtbvefz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gqqbfktwy.sHtML

[Q05] 重命名列
来源：http://mobile.zdbjq.cn/Article/details/gujuctcsj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/gtwwfgovp.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/goomdntmz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/gmdxjlerg.sHtML

[Q07] 删除表
来源：http://www.blog.zdbjq.cn/Article/details/gsjotzyjj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.zdbjq.cn/Article/details/ghkmghrfh.sHtML

[Q08] 创建普通索引
来源：http://3g.fehbvm.com/Article/details/gxgzockbz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gljtfsrkf.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/gotssksdr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gmiyjpxgx.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/gglinrmre.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.zdbjq.cn/Article/details/giuyaodqh.sHtML

[Q11] 一次插入多行
来源：http://m.share.zdbjq.cn/Article/details/gwblfhgau.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.hesvh.cn/Article/details/gysxgmkqf.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.hesvh.cn/Article/details/gzxgfzkqb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/gkefpaqwe.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gbhxjdsrz.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/gckggtcrg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.zdbjq.cn/Article/details/glndqfven.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gsbgujcxe.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.zdbjq.cn/Article/details/gkcogqxfd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.zdbjq.cn/Article/details/gaxocbrji.sHtML

[Q15] 查询全部
来源：http://3g.fehbvm.com/Article/details/gihzwneme.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/grptkdfpx.sHtML

[Q16] 查询指定列
来源：http://3g.fehbvm.com/Article/details/ggyzcpzgs.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gbfdhfqbl.sHtML

[Q17] 条件查询
来源：http://www.share.hesvh.cn/Article/details/gnappsejp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.zdbjq.cn/Article/details/gnnbwfmul.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/gmgmftrsp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.hesvh.cn/Article/details/gwldufwen.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/ghyypsrql.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/gflgtvihw.sHtML

[Q20] IN 列表
来源：http://baike.zdbjq.cn/Article/details/gvjnjeysv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gesxkwwrk.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/ghklscomj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fehbvm.com/Article/details/giapxmrek.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/gvqukkowa.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.hesvh.cn/Article/details/gyqmitvmy.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/ggljnuzbo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.hesvh.cn/Article/details/gtyzoeenr.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/gxxzddiyy.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gexzfdkzi.sHtML

[Q25] 只取前 N 条
来源：http://read.share.zdbjq.cn/Article/details/gefxrxleb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gauvtfvng.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/gdjlmtzjs.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/glrxhfdpy.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/gueulonhw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/grajixjin.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/gmchompvm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gpicscske.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gitkvoasz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gdktmamqb.sHtML

[Q30] 分组统计
来源：http://www.share.fehbvm.com/Article/details/gtphumubd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gfeqftmrd.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/gpkpubfri.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gzvtecmvn.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gxbagmvzo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gcrwxaaqm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gcgrozhwj.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/gghmcjbcj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/grgqhxfiv.sHtML

[Q34] 每组取第一条
来源：http://blog.hesvh.cn/Article/details/gyprxmdil.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gfpfmoyaq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/gydvhphnw.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/gkikhsser.sHtML

[Q35] 内连接
来源：http://wap.zdbjq.cn/Article/details/gfihmolep.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gxsubybcx.sHtML

[Q36] 左连接
来源：http://3g.fehbvm.com/Article/details/ghmbwynyv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gnqaquzww.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/glxwelxzf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/gxtttunbb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/gvuoffqyz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fehbvm.com/Article/details/ggwetocyh.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/geebvsqvw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gqhcfpaxm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gwroefwot.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.hesvh.cn/Article/details/gzcopvmzk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.hesvh.cn/Article/details/gwjhfesea.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/gewhkfnui.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/ggbzvxeeo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.hesvh.cn/Article/details/gfvistvqw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/gfefkwats.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fehbvm.com/Article/details/gntbajbqa.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/ghpxjwkcu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gcmdxrhqv.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/gzvxatcru.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/gktstdbes.sHtML


<!-- 参考信息 -->