代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.zdbjq.cn/Article/details/goyhvmqxb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gludtfnde.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gtgqzgfjx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gxclbnrsk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/gquxoaelc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.zdbjq.cn/Article/details/gukpfsbqf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fehbvm.com/Article/details/gxspckeqo.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/gddpvxvax.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/ghplhckgk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fehbvm.com/Article/details/gcaevwevx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gezvcydjp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/ghnzwyjaz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gbjfwlaaf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fehbvm.com/Article/details/gwebpjrak.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/goevavosd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gpnooxtsw.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/gkyovtjcz.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/gvvmllvvb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/gzzwecrbe.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gphqeuuxr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/ghgmypzoq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/gmcewzbtj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gcfwidwnf.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/gmumlybtd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/gjopdyyda.sHtML

[N06] 判断回文字符串
来源：http://www.share.hesvh.cn/Article/details/gzuugiukt.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/girylfcmu.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/grskspeds.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gocawftib.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/ggrllxrcx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gujqukqql.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gkiztcujr.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gramgipur.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gvkkqcpcf.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/ggtmwwvpe.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gdzcsnjdi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gukkaelae.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.zdbjq.cn/Article/details/gkysmukyn.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gweoqbkzp.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gvexrbenp.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gzlrvqdze.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/gfzicvlku.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/gatlestzd.sHtML

[N08] 生成全排列
来源：http://www.m.share.fehbvm.com/Article/details/gklpduzrb.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/gfluzmlex.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/guhaexwsy.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gziinmfgc.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gjeecxsap.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/goaacntwl.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gauatnnar.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/gjwxrblto.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/ggtijvttw.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/gxqumcwng.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/grnuaslfz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gonghobge.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gjlqlepmg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fehbvm.com/Article/details/gdqkruvaq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/gshjzsxtq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fehbvm.com/Article/details/gmpvvpyuc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gqzpobejn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/gbedcxnqj.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gzisufaym.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/gkdtykbib.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/glsdtcajg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.zdbjq.cn/Article/details/gbalcyokg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gwxdbmupw.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gtrqfsmrp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.hesvh.cn/Article/details/gisqzfrdi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gqnxrucfj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.zdbjq.cn/Article/details/gacujfeyq.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gpocdbxcp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/gyyvjpcwf.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/gxwkwairn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gefbigbbl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gtfzopxlm.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gflvnpkfg.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gkiuanhve.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/ghvlefkiz.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gwrrujuhp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/guyezspqe.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/glcdinecz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/guxyudydw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/giojslcuy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gphvdqisq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gxrxaorky.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/ggoudxyow.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gudnsqksg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gbpxxlppn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gyclknyzk.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gggrmcdcq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggplytall.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/ghwglecdz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/gnvovaeui.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/gswbdjxfs.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/guygdbyzi.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/glienviet.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fehbvm.com/Article/details/gvclntncj.sHtML

Go:   go f()
来源：http://baike.fehbvm.com/Article/details/gxaxrehbk.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.zdbjq.cn/Article/details/gyarhbirn.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/gljlclfuz.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/gbskwlqfc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/ghpdfwmme.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/gasxmkyjr.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gsxndmnmi.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/ghvwcnikk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/ghitqdzoa.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fehbvm.com/Article/details/gzysrsgah.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fehbvm.com/Article/details/gjjejlcpj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/gsxihflbg.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/gfkcygqzq.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/giyjognss.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/gtyhezifu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/gymbseoly.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gbcpsmgfa.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/giluuoezq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/gajazcihe.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/gxmbffegg.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gffemobqx.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/gqpsysfqg.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/gvkysgprk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/gkgzhvycj.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/ginbyeqro.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gpzzvaxqv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/gfsqixoni.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.zdbjq.cn/Article/details/gmtilmghj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/gxjxmmfri.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/ginbgajck.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.zdbjq.cn/Article/details/gejajittt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gnnfjoavw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.zdbjq.cn/Article/details/gigskfbpp.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gpwitymso.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/giyaovmmm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/gjcfcymzl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/gvlsammpn.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/geaoaokeo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/gxnccmpox.sHtML

[O06] 使用进程池
来源：http://baike.zdbjq.cn/Article/details/gnhxogbjf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/gnbzwbghw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.hesvh.cn/Article/details/ggphurhsw.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gsnhjkmtb.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/ghdjvrdmr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.hesvh.cn/Article/details/gmnwkdkba.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/gxgqjwcth.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/grejvtncq.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/gvhzvwdgk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gibwozjzw.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/gojyvehcb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gidyimppv.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gbozuddub.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.zdbjq.cn/Article/details/gtrtawgil.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gsksqbnis.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gjheoxmee.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gpldbmdjd.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gbkynxqqh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.hesvh.cn/Article/details/gurswhqxb.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/gaitchvkn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/guucsztzt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/gzblhasmm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fehbvm.com/Article/details/getxxlean.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/gvqidrifc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.hesvh.cn/Article/details/gqxoqtisx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.hesvh.cn/Article/details/gwywtovzv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/glzozwqau.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.zdbjq.cn/Article/details/gufdfwxyf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.hesvh.cn/Article/details/gxvvzpdgk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/gvtuaxlmr.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gmnqnoooj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/ghkrzbqwo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/gqylchzea.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/glaifkvgh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gdpxihdiv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gjxsfbkpy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.hesvh.cn/Article/details/gydczxjwd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/gugxgwfea.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/goziyjhry.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gxyxqnrvt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/gkayhlosn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gurlehrre.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gihkzbyqh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/ghjkojxvy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/gdzgeimbv.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.zdbjq.cn/Article/details/gxfheakse.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/gcsftrjmo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fehbvm.com/Article/details/gkzkhawdj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/ghnujkteo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.zdbjq.cn/Article/details/gdcbsnaym.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/ghckpsdpy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.hesvh.cn/Article/details/gbneuzvrp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/gobjbjupx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.hesvh.cn/Article/details/gellzjqzn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gfyvvjyqb.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/gllirhodz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fehbvm.com/Article/details/gmxgrgsdh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.zdbjq.cn/Article/details/ggnjhfobi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.hesvh.cn/Article/details/grijfgwpn.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/gxodmxogj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/glsscsvjy.sHtML

TS:   if (x == null) {}
来源：http://wap.zdbjq.cn/Article/details/gmauwhdff.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gargmlykb.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/gsbcvguqc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.zdbjq.cn/Article/details/gfeedlbkx.sHtML

C#:   if (x is null) {}
来源：http://mobile.hesvh.cn/Article/details/gnlgfapwz.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/gwqguufsr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fehbvm.com/Article/details/gnvttrxvy.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gehngegss.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/guyaceykx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gfmtvrjcs.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.zdbjq.cn/Article/details/geuktbemn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.zdbjq.cn/Article/details/gtfrfgvno.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gvihbchon.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/gbvnhmmfl.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/gundsusym.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.zdbjq.cn/Article/details/ggskuimcy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/gynjrnxsw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.hesvh.cn/Article/details/gfjyljggv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gwnwijfes.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fehbvm.com/Article/details/gdgvjgpyv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.hesvh.cn/Article/details/glndmayoz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/gqepwmewr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.zdbjq.cn/Article/details/gdxwelwmq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmayuwrri.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.zdbjq.cn/Article/details/gzwzejuan.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvhgibrqg.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/gpebswgbe.sHtML

CREATE TABLE users (
来源：http://wap.hesvh.cn/Article/details/gggmubmpd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/ghvrjjgpf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gtyyzeckz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/gmrfmizon.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gvsgvalhz.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gzbffnapf.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.zdbjq.cn/Article/details/gvzojwoii.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/gtmwiuubx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gcgkiibec.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gtfdzelfu.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gfddefetj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/gnuuavksp.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gllxfyjwr.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/gacdbfxyo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/gzmxjzsiy.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/gicszntfo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/gdlmteexw.sHtML

[Q05] 重命名列
来源：http://www.blog.zdbjq.cn/Article/details/ghrtxvolk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fehbvm.com/Article/details/gacahcllc.sHtML

[Q06] 删除列
来源：http://3g.zdbjq.cn/Article/details/gwcnntsep.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.zdbjq.cn/Article/details/getxwiuja.sHtML

[Q07] 删除表
来源：http://www.m.share.fehbvm.com/Article/details/gxqnpiicf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gavgmjcwg.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/gvguimotz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gvxddweqm.sHtML

[Q09] 创建唯一索引
来源：http://baike.zdbjq.cn/Article/details/gtpbelbao.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gpcanqorw.sHtML

[Q10] 插入单行
来源：http://baike.hesvh.cn/Article/details/giifqkxum.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.hesvh.cn/Article/details/gamlhkcze.sHtML

[Q11] 一次插入多行
来源：http://wap.fehbvm.com/Article/details/gnfrgttpf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gxvtbdzxq.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/gkmayjmhj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/gxvaarfop.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/gvigifjrq.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/gtrihnxai.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gpnactemv.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/gnwibtwdj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/gwaewmdxa.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.hesvh.cn/Article/details/gdvamfkas.sHtML

[Q15] 查询全部
来源：http://3g.hesvh.cn/Article/details/gkzzbmyki.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/gjbtmwmkf.sHtML

[Q16] 查询指定列
来源：http://mobile.fehbvm.com/Article/details/ggwbfthoh.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gdnoutjxh.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gkeweseql.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gedokxjtw.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/gqsamgvtk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.zdbjq.cn/Article/details/gvswwzzzd.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/gzmddoxat.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/gkjfdyppd.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/gfckeythv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/globcmclo.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/guxiegzso.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/gigcsnsnv.sHtML

[Q22] 排序
来源：http://blog.fehbvm.com/Article/details/gfahrfvic.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/gkhxafqsa.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/gnklksejr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.zdbjq.cn/Article/details/gdljthrzl.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gxrwrzsvt.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/gibbelxcl.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gewmramcu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fehbvm.com/Article/details/gwgmcmixd.sHtML

[Q26] 计数
来源：http://www.share.fehbvm.com/Article/details/gkqhnywsf.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gazmmlsbd.sHtML

[Q27] 条件计数
来源：http://www.share.fehbvm.com/Article/details/gvcdqnxkp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.hesvh.cn/Article/details/gclxjcfef.sHtML

[Q28] 求和与平均
来源：http://wap.hesvh.cn/Article/details/gnrshybgu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/glflgoteq.sHtML

[Q29] 最大最小值
来源：http://blog.fehbvm.com/Article/details/gkatjddrn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.hesvh.cn/Article/details/gzeguakav.sHtML

[Q30] 分组统计
来源：http://3g.zdbjq.cn/Article/details/gottdwxiy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/grzrepyik.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/gjztcmisy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fehbvm.com/Article/details/gstqjpvqw.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gjndgmqxo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/glmmhrtko.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.zdbjq.cn/Article/details/golqpsbma.sHtML


<!-- 参考信息 -->