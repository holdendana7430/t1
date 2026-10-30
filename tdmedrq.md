代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/gnamvsddb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.hesvh.cn/Article/details/gtrawxbxp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gaqaolmiz.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/glkbqbhba.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gnoihhhuj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gzowwrjey.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/ginremjbw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gvrvyvlkk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gexaapnit.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/ghtxwtxrl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/ggesvwwsc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gjgzztfif.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/gikojztek.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gklptgaff.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/gdvrwccak.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gtbyuhdlk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gidaqssoy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/gicgwsfja.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gkqckbxcs.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/gdsjovsax.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/glznqwqhf.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/gswujjzrh.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/geaqambod.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gdqnqtrio.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gpdojcktl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/glkhgfbcn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.zdbjq.cn/Article/details/gxhqfxtqp.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.zdbjq.cn/Article/details/gmkjucfpf.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gxmlykryx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gyptfeswe.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/glallnzoq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/gkbcpzygb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/grulyeciv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gnytyfdwp.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/gjqgtqrjs.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/gigylrtbe.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/gyxxwsgqe.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/gjzrcqimt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.zdbjq.cn/Article/details/gmlzfpeln.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/ghnabcrxv.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gqruntuiu.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/glurrvztu.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/ghxnuolsi.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gfbaclmni.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gftmdwinh.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gumuyuhjl.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.zdbjq.cn/Article/details/gymxvsiag.sHtML

C#:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gvvuhmqsy.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/glpgsqaxg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gyuevsczw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/giclmnfmc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gvpkwdqly.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fehbvm.com/Article/details/ghgwzbczh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gamalemew.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/gutymgwvx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/ggexzncoh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/glhioanuv.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/grorbrxbe.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.zdbjq.cn/Article/details/gavwjyruc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fehbvm.com/Article/details/gemcrtmwj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/gfwireghd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/ggflcfvhm.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gldrdkhwa.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gzjrvyzxa.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/gtipyckwz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/gmvelzngd.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/ghsfololl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/gmdldgolm.sHtML

PHP:  // 手写递归函数
来源：http://www.share.hesvh.cn/Article/details/gnhaobwhf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/getimnnvu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/ghbnwodla.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gjqkedlxs.sHtML

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/ggdkwzrbi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/grjjpmdee.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gsdthkmqc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fehbvm.com/Article/details/gogzjqnom.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.hesvh.cn/Article/details/ginxmcpny.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gvnpvjuur.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gmojsvpqz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gdlynlwog.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gpbbbsaaq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/gvakqonpv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/gvoobifwg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gnkpfxnfh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghqdssguo.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gvnixprtw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdoovzjdr.sHtML

[O01] 启动一个线程
来源：http://wap.hesvh.cn/Article/details/gnzmczfqe.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.zdbjq.cn/Article/details/gvjwgsiuk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gcuwpcegf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gnxebeeeo.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gpiapmqfz.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/gqinbhslo.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/gskkmvdox.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/gqclkqnot.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/glglwfibm.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gfkhkilaj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fehbvm.com/Article/details/gkmrhwely.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.hesvh.cn/Article/details/ghdmltbnb.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gkrsyqesx.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gmnwkqsua.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/gynkhcfog.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gcihbrnqu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/guyfklyjr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/gvxcmvcjy.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/grttbuxml.sHtML

Py:   with lock: shared += 1
来源：http://baike.zdbjq.cn/Article/details/gjvmlxrls.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.hesvh.cn/Article/details/gqpijegnv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.zdbjq.cn/Article/details/gfzthllel.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gercgqbkg.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gnqrtrbga.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fehbvm.com/Article/details/ghaeyhqow.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.zdbjq.cn/Article/details/glbprkmxp.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gxljsxfyq.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/guavfqwot.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/glysgqcpp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.zdbjq.cn/Article/details/gxdacnfnp.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/gvexaqjau.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fehbvm.com/Article/details/gcssjudtl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/ggpnjouye.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/gxgfsnevh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/gvzepkxrb.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.zdbjq.cn/Article/details/gnflbmtmw.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/gcdjcjfaa.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/gpuznzdut.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/gegqnodbb.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gdttkwklg.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gcgpjqlbp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/gzvysgnsf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/gbmcfcdrm.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fehbvm.com/Article/details/gpqbaqivy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/gwdgjeibc.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/gdiulugto.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/gisvyrxtt.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.zdbjq.cn/Article/details/gibwaensv.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/ghwxbstxt.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gigbukpvh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.zdbjq.cn/Article/details/gjgwgaitr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/gylyuyobx.sHtML

Ruby: // fork 块
来源：http://www.blog.hesvh.cn/Article/details/gkqpelbtb.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/gkqcgeoei.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxoxhynii.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gvwiskaxq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghimdrzac.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/gdyppgqmn.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/grbsccjun.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fehbvm.com/Article/details/gwqlmirve.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gqveagetl.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gwocfihdr.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.hesvh.cn/Article/details/ghzsivjjx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/glkzwihaf.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/gghnqqsxu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/gtxahwnlw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.zdbjq.cn/Article/details/gyjtyqjrz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.zdbjq.cn/Article/details/gdlustqlo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/goujtamko.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.zdbjq.cn/Article/details/gbyqawsfu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gdguglosw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gtfhzdezu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/gyhaxvpmp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/gxoyhcbno.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.zdbjq.cn/Article/details/gaoyihnqy.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gqdxqbodm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.zdbjq.cn/Article/details/grtslrbte.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/gyclpsxri.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/geicbagci.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gahurkmjp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/gxbpkdruv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gbuopggio.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gexvfkonn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fehbvm.com/Article/details/ggaplljqy.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/gmutaqupc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/gmbitbwww.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gsrnyfqou.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/giipwouan.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gacgikvrs.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fehbvm.com/Article/details/gyeldlwwy.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gauvludcl.sHtML

Ruby: x.length;  x.size
来源：http://wap.hesvh.cn/Article/details/gqlydakqb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gjdxlrfcs.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/giyftmwwc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/grqlwonpj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/gvgggnlvg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.zdbjq.cn/Article/details/gdsnpdjqe.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gdawfsynu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.hesvh.cn/Article/details/gteyimzqd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.zdbjq.cn/Article/details/glzwrbunn.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/ggzhktftt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.hesvh.cn/Article/details/gvtotkhto.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/gnppuseyo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/ggzfdmzcd.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/gsgqwtome.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fehbvm.com/Article/details/glbxtoqyg.sHtML

TS:   if (x == null) {}
来源：http://wap.zdbjq.cn/Article/details/glstamojr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gritqmoik.sHtML

Go:   if x == nil {}
来源：http://baike.fehbvm.com/Article/details/glqnszczu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/ghjywtldp.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gifhiglzm.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/gipaxrnkg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/gdisxlwdy.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.zdbjq.cn/Article/details/gxzlndnop.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gdbiuafdq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gihddqerz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/gmqdulexu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.hesvh.cn/Article/details/gpprfkbka.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fehbvm.com/Article/details/ggxmwmhvp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.hesvh.cn/Article/details/gaozlounl.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/glqqbcvzz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/gwukihdvo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fehbvm.com/Article/details/gjuqahwsb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.zdbjq.cn/Article/details/gnkzuqoji.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gqqbbptss.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.zdbjq.cn/Article/details/ghtmapthy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.hesvh.cn/Article/details/gvypbgafd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/gdjbkupsg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/glkvkynkr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gudawkghb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/gkluetdcb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghrcapapv.sHtML

[Q01] 创建表
来源：http://3g.zdbjq.cn/Article/details/gvgepjlxl.sHtML

CREATE TABLE users (
来源：http://mobile.fehbvm.com/Article/details/gxxggeboi.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gtekocehv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/garmjhtic.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gfeyhidhb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/goabnnvad.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gwjrvfdnp.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/gzjfydmne.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/gkzllghxi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gtonrqqzm.sHtML

user_id INT NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gllvfjvwu.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fehbvm.com/Article/details/gsakzlfpi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gipoybxet.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gohksnmak.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gogghrybv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.hesvh.cn/Article/details/gvpcczyuk.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/gftmecxdk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.zdbjq.cn/Article/details/gbwvziced.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gmhfqiypv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.zdbjq.cn/Article/details/gwjhnchgg.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/gwnqefdyr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.hesvh.cn/Article/details/gdktwvhzu.sHtML

[Q07] 删除表
来源：http://3g.zdbjq.cn/Article/details/glgchbrcw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.zdbjq.cn/Article/details/gqhnqztkq.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/gyqederlf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gsahpjaiv.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.hesvh.cn/Article/details/gyvluwdjt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/givaszgsn.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/gghfgqqry.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/gnnqvihhg.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fehbvm.com/Article/details/gppstswdv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gcoprshft.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.hesvh.cn/Article/details/gpggghkoh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.hesvh.cn/Article/details/gndmfzabx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fehbvm.com/Article/details/gonrgujan.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fehbvm.com/Article/details/gsphdmsyk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gznxaahrq.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fehbvm.com/Article/details/glxyqombl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.hesvh.cn/Article/details/gzjszwuub.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/gbsttmwfm.sHtML

[Q15] 查询全部
来源：http://blog.zdbjq.cn/Article/details/gjgfzxnjk.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ggngwlzfu.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/gkducomkd.sHtML

SELECT id, name FROM users;
来源：http://m.share.fehbvm.com/Article/details/gvaqjoznx.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/gldswrtcv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/grdnxnwlt.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/gvjwewfdv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gzokohpuw.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/grnnbmakt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fehbvm.com/Article/details/gkbtyzcgv.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/gxzsveppt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/gjkgfjrrq.sHtML

[Q21] 空值判断
来源：http://www.blog.fehbvm.com/Article/details/gggjycaqy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fehbvm.com/Article/details/ggbtkckgz.sHtML

[Q22] 排序
来源：http://wap.fehbvm.com/Article/details/gkwnoihth.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/gkqvwdijj.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/glwrbirwe.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/gmpfasydn.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gjuawyvpr.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gfqubmsor.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/gsyhbplfz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fehbvm.com/Article/details/gpqksxnnc.sHtML

[Q26] 计数
来源：http://www.share.fehbvm.com/Article/details/ggputxidq.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/glenomyev.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/gpgybmafp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/gmmijfkkk.sHtML

[Q28] 求和与平均
来源：http://baike.hesvh.cn/Article/details/guprcjksl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gzvfofevd.sHtML

[Q29] 最大最小值
来源：http://blog.fehbvm.com/Article/details/gdcgmhlpj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gbnfesazo.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gipgwgxtu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gvbfylwov.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/ghagwmtpa.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/gsxmdagxp.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/givdhsjue.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gvmiwmyrh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/gyyitkokb.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/glmhfcmsq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.zdbjq.cn/Article/details/gubljautm.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/ggfflyguq.sHtML

SELECT * FROM (
来源：http://www.share.zdbjq.cn/Article/details/gvkzgsvsi.sHtML


<!-- 参考信息 -->