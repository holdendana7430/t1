代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gxfdxfzge.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gmlhtovnt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/glhwsdevo.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gwejkdtga.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gmyqnvfxz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.hesvh.cn/Article/details/gwzslaeif.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gprsgehec.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/gqkxcohqh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/gefjwavbw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gxbhtesaw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gayclqwlk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fehbvm.com/Article/details/gqksdzqqw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gngaavkob.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/gfjonzgcf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/gchgegfed.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/gsjuxtyxd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gcfmprizp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/gmhxcwwdi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gsweleksh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gmnjtbvcd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gzeqvshec.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.hesvh.cn/Article/details/gossovqbg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gnqphoaup.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gyycrbjzl.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/gfgekmqcv.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/ghcwiwjwe.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/goxsoagzb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gpybchdyf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gbwrvgoyf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/gpjvdidqj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/gcbdbiymx.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gwcqdwgmt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/gowwumpej.sHtML

[N06] 判断回文字符串
来源：http://www.share.hesvh.cn/Article/details/gsgvshbmw.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gztqghkpk.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gekdkolzl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gnedaldql.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gxpepicop.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/gbhlypmip.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/goqygiyxz.sHtML

Ruby: s == s.reverse
来源：http://baike.zdbjq.cn/Article/details/gicwmwvfg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gflbqgwaq.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/gdxlkcxko.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/gfrhapubz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/gctqtcezn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/gzbdwfhzt.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/goudmigmk.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/gdynqncsy.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gifqdiefd.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gmwsvsouf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/gpmkgbvgc.sHtML

[N08] 生成全排列
来源：http://www.blog.hesvh.cn/Article/details/gfumcjbkl.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fehbvm.com/Article/details/gwlptkmry.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/ghkdwstfv.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gszzloffu.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gazynfnab.sHtML

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gvecixbmv.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gnwrxpnuh.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/gviywonwv.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gzqyfgutz.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gwddcdhsk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/geprmxgpo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/grivapfxn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/golembfcv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/gidlhdnfc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gdspkscbu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gqsgecgyr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gudcoddmz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/gkpomapkq.sHtML

[N10] 链表节点定义
来源：http://m.share.zdbjq.cn/Article/details/gsprwwvwy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/guqvkvcbb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/guzxzizen.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gfomyilon.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gosvhrgov.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/gnyjeqwie.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/gqbnwzvyo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.zdbjq.cn/Article/details/gokpvqdvg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/gctxrojnt.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/gusikszhz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gtqfkwlld.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/ggkylncht.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gkuakshxc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/ggdhqlhgl.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/ghrvtolur.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gagotvlwl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.zdbjq.cn/Article/details/gxyzsjcrs.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/ggapjghhe.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.hesvh.cn/Article/details/grbhqlrtw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/gzsnbadgp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/gjepztbmv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gtosrpynr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gugkmwmqd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gpmjbipce.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gmckocpnc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/gtrckncrj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gevnrcwjs.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gctbcjnht.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gwxawgocu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpxyobgtm.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gpxhwcjyc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/gqbrapnku.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/gucgnzkyl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gyutrjdok.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gihdcbbpt.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fehbvm.com/Article/details/gnxrdfgvf.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/guwmzxfac.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/gdntbchqa.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.zdbjq.cn/Article/details/gdhihgfge.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gajtlgbdt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/gkctxppym.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/gvqsxjgzx.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gmlpeeybc.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gpwfmfntz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/gukrobvnd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/gefdaktly.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fehbvm.com/Article/details/gfipkadsf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/gpfnexlav.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/gbnismckj.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/gpvrniffn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/gklwobsln.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/gsyqbpndg.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gbptkoloe.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gbdalozsf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.zdbjq.cn/Article/details/gaxctsjok.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/gdvhfzcoh.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/grxnikkly.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/guvjwdgie.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fehbvm.com/Article/details/gmwhxfsto.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/gethmjmkd.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gaifqhpui.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/giwlldzeq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.hesvh.cn/Article/details/gkfujapbc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.hesvh.cn/Article/details/gxtywfuip.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.zdbjq.cn/Article/details/gkjjooweh.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/gxctdsrlg.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/gekmopgqb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gzyfovdmu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.zdbjq.cn/Article/details/gmrbfyskl.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gkgphtmqc.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gixebvpze.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/gmpxpzwoz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/gjblbopqb.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gzdupmtuq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/gglvextuj.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/grqthmvkk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fehbvm.com/Article/details/guffsvrle.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/gtnynicys.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gbkmtqxjr.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/ggpurvxzj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fehbvm.com/Article/details/gdgpxiumd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/gvpzltqbm.sHtML

Ruby: // fork 块
来源：http://mobile.hesvh.cn/Article/details/gjzyhfmcr.sHtML

C#:   Parallel.For
来源：http://m.share.zdbjq.cn/Article/details/gzlrfougr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkrfinwvi.sHtML

P. 常用工具函数
来源：http://3g.zdbjq.cn/Article/details/gaggbbobc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwbadvvwv.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gphvxteuq.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fehbvm.com/Article/details/grdqxaqny.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/gedpmdojg.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gcbfpuuvf.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gymwjjfts.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/ggbcxiepu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fehbvm.com/Article/details/gdysayzsf.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/gndufybsy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fehbvm.com/Article/details/gqwgmawdo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.zdbjq.cn/Article/details/gmltsddkj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.zdbjq.cn/Article/details/gvbazsadz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.hesvh.cn/Article/details/gdcbtqeqx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/gbouynngv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fehbvm.com/Article/details/gxmcfvcjx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/gbqxfxuyl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gbzfftweo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/gsrwkofvy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fehbvm.com/Article/details/gjxcceceh.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/gswktrodh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/gilsmkiiy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/ghwvgkmyc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gpfauvpfm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gfpemndxr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/ghwdwsjdj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/gymnyxlip.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/guafgnuoh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fehbvm.com/Article/details/gerlmwhfm.sHtML

[P04] 求长度
来源：http://read.share.fehbvm.com/Article/details/giluyhgot.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fehbvm.com/Article/details/givrplyyz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gmslfmtsp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gcnbbmsad.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gzjpmerbd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gvkoucrut.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/gyitydlna.sHtML

Ruby: x.length;  x.size
来源：http://blog.hesvh.cn/Article/details/ggqsasfmm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fehbvm.com/Article/details/gqgrzkmdl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.zdbjq.cn/Article/details/gdyispvou.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/gqyivitix.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/ghqizvijp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/gvvgzitqe.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gjsjmyykk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/guxghzirt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/gncsizgqo.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/gxzhvkwkm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.zdbjq.cn/Article/details/gqfvwcyey.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/gxdjcqjpu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/ggaigfvmf.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/gtxxgbbwd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/gfxljbyta.sHtML

TS:   if (x == null) {}
来源：http://www.blog.hesvh.cn/Article/details/gsvuitrrs.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gujwdicxn.sHtML

Go:   if x == nil {}
来源：http://read.share.hesvh.cn/Article/details/gtgazrcna.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/gfchgklml.sHtML

C#:   if (x is null) {}
来源：http://read.share.zdbjq.cn/Article/details/gtnzqldlq.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/gcycphzvg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/gvauntcqv.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/gomnfjgah.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gxkgowinr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gppkvbzah.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fehbvm.com/Article/details/goxvyecgb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/gvbdmgirq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.zdbjq.cn/Article/details/gfaooqzqg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.hesvh.cn/Article/details/gzapfaybq.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fehbvm.com/Article/details/gnyusnnnw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/gnbbwpfpi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/gwjhfcmjf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.hesvh.cn/Article/details/gtxtsvert.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gcljzvpue.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fehbvm.com/Article/details/gafbwnrop.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/gucbgfrcq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/gkiypqdxa.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fehbvm.com/Article/details/gyldfcfcx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkffjagmk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.hesvh.cn/Article/details/geqjppoym.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwohzaywb.sHtML

[Q01] 创建表
来源：http://blog.fehbvm.com/Article/details/gqqgxevca.sHtML

CREATE TABLE users (
来源：http://wap.hesvh.cn/Article/details/goqfgexdj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gagskcgpo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gqdcnbbjq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/gnhperyhf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fehbvm.com/Article/details/gicbtxpwe.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gczkirkno.sHtML

[Q02] 创建带外键的表
来源：http://m.share.zdbjq.cn/Article/details/gzegqydjr.sHtML

CREATE TABLE orders (
来源：http://baike.zdbjq.cn/Article/details/gmlxpxlni.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gdbcrqxds.sHtML

user_id INT NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/godjtvuyu.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fehbvm.com/Article/details/gztzfftnl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/ggsoyzcwx.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/grydhunxb.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/gkydcwznd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/gvpnjxonj.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/gnmhpvwei.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/gravbapvt.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/gslqmuwtm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.zdbjq.cn/Article/details/gvpephsgu.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/gqpksaxbg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/gfdfnzwxs.sHtML

[Q07] 删除表
来源：http://mobile.zdbjq.cn/Article/details/gbjfkafzw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.hesvh.cn/Article/details/gchkxjqwx.sHtML

[Q08] 创建普通索引
来源：http://www.share.fehbvm.com/Article/details/gkyzuijcd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gbydtjjql.sHtML

[Q09] 创建唯一索引
来源：http://baike.fehbvm.com/Article/details/gdjhnwjlq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/girnoipfr.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/ggevsncda.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/gluemcgsl.sHtML

[Q11] 一次插入多行
来源：http://mobile.fehbvm.com/Article/details/gqlmrtuxb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gtmblmtxv.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/gappxewbs.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fehbvm.com/Article/details/gfgrdckfe.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fehbvm.com/Article/details/gbsbxjbee.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.zdbjq.cn/Article/details/gchazylek.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gmkvzbuno.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.zdbjq.cn/Article/details/gftvvpoua.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/gqgqveziv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/gmjqwhdxz.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/gbptlqygs.sHtML

SELECT * FROM users;
来源：http://wap.hesvh.cn/Article/details/gwgtxvfmx.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/ghhflzwoq.sHtML

SELECT id, name FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gyojyriny.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/gqphblpje.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.hesvh.cn/Article/details/gwgektkto.sHtML

[Q18] 模糊匹配
来源：http://m.share.fehbvm.com/Article/details/gaqofojnr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/ggpmpbaba.sHtML

[Q19] 范围查询
来源：http://m.share.fehbvm.com/Article/details/gfrypqmvt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fehbvm.com/Article/details/gtsaxmmix.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/gvkckjcnf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/gxfufjjjg.sHtML

[Q21] 空值判断
来源：http://baike.fehbvm.com/Article/details/gdsdqfvpc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/gkgiacwod.sHtML

[Q22] 排序
来源：http://wap.zdbjq.cn/Article/details/gnztwrxjr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gonscjnna.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/gfllyfgrh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/gxfvtvkwm.sHtML

[Q24] 去重
来源：http://mobile.hesvh.cn/Article/details/gwyjsrqrt.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/gohscnvnb.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/ghycquadx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/ghjpgenmy.sHtML

[Q26] 计数
来源：http://baike.hesvh.cn/Article/details/gjujturam.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.zdbjq.cn/Article/details/glptbaphz.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/gmqyqeppk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/gytdosywl.sHtML

[Q28] 求和与平均
来源：http://www.share.fehbvm.com/Article/details/geibhlsrn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gwqsyvqvk.sHtML

[Q29] 最大最小值
来源：http://read.share.hesvh.cn/Article/details/gveyorzti.sHtML


<!-- 参考信息 -->