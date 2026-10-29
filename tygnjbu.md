代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gnilmmprg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvtcwyatf.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/ggkpylyoa.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggpddrykg.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.hesvh.cn/Article/details/gvxdpqsum.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gocpopasn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/gjkhgojpx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/grkeudxit.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/ggznmxykh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gbqhcrtft.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gyrxvdemm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.hesvh.cn/Article/details/gpkcingsz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gucrjyevt.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.hesvh.cn/Article/details/gtfheuprm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gkylnbmro.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/gfqbzaugx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gbaiclggn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gdimrnrkf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/ggudznfni.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gkawhorcw.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gegwfyhep.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/giflruprk.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/gsavobrwo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/gqijdrpvx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/grpegsaue.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gkzbzakvu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gmmtbwhzp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/gvfserzyy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gsjzrimmd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/gqxpjloic.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.hesvh.cn/Article/details/gazivmiea.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gmtzvbtwn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/ggahicvsg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gpmcsojil.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gjwgbezbh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gfkybcdvm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gjeiitock.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/gpgbfxjsc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gxpwfnzxs.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gaieyouti.sHtML

[N05] 最大公约数
来源：http://baike.hesvh.cn/Article/details/gwdokrisd.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/glrfhlusa.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/gxljdvavh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gkphvbvmw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gpkqeojdf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/gcwriczrd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/ggzqjstbb.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/gnzztvyze.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/gghkhnmyh.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/gotwdebgf.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gxsgkuiam.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gibhhdvxk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gfwodkwic.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gaspmwfwm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/glubmjrql.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/gmychbtwv.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gkcatyrer.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gstbyqrrv.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gvbworzdy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/gjdlufcdg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/gefqopmoj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/gebpqrrqj.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/gdpiomhyc.sHtML

Java: // 手写 HashMap
来源：http://mobile.fehbvm.com/Article/details/gvmblnigx.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/gzdethdtl.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/gviwtkplm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gytgdklbq.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/geohlqcwj.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.zdbjq.cn/Article/details/gsvaupvrw.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/grehijzwt.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gxqonzzpo.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gvfqerlqj.sHtML

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/glivyyjrb.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gowkbwexd.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.zdbjq.cn/Article/details/gyhohzexv.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/grtigcscx.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gbammstxx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/gjspiopmu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gcrcwnzqe.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gqjxyuubq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/gkoqopiqm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fehbvm.com/Article/details/gdggyerws.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/gkpgylbpa.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gizzmzhvo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.fehbvm.com/Article/details/glvrhncar.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/glnyitilu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.zdbjq.cn/Article/details/gbryqvexp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbtvhhgib.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/gqelokvsr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gfvhrpcii.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/gkqkakmhx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gxzxpnlxo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fehbvm.com/Article/details/getmrsnhw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gxnoagbka.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/gbmfshjba.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/gdhqxzpzr.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/glyibffxa.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gmzczgcez.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gdxrcxoei.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gtordcnnz.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/giqcbkzay.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.zdbjq.cn/Article/details/gamkglrzx.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gmmsgxnpn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/gvktxlluv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fehbvm.com/Article/details/guocgnujo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/gggcqmvqy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gajirjdst.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/geygbvygm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gqdaxnlut.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/gqanuooho.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/gasokmtor.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gyxxcclng.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzmauyjul.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/gckejolpl.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwypnfzbg.sHtML

[O01] 启动一个线程
来源：http://mobile.zdbjq.cn/Article/details/giczhvprj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/gnlmqvjcr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fehbvm.com/Article/details/gxhfmrsqo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gynyfaqdy.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gzgirioyu.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.hesvh.cn/Article/details/gffmwnnzx.sHtML

Go:   go f()
来源：http://3g.fehbvm.com/Article/details/gzolzchgh.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/grnimlzep.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gulnttqpb.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gmzhercup.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gypcrwfrl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/gbzsrlvqy.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/glwpeugrk.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gwzkypbcp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/gveyydzrm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gljdxgzjk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/givnsmauj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/ggfrljhcz.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fehbvm.com/Article/details/gkmraktga.sHtML

Py:   with lock: shared += 1
来源：http://www.share.zdbjq.cn/Article/details/gibikxrng.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.hesvh.cn/Article/details/gkrcugdxo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/gylboanin.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gjbrhlore.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gtwsgqdob.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/grfvqpwgt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.zdbjq.cn/Article/details/gmlguoiaf.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gjyzqozbt.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gkbofffjp.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/gwtscpiqv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/ggapsrujz.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gembwikny.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/gfdcxsiil.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.hesvh.cn/Article/details/gqsvrchjj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/gqfwzqgbw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/gfpqutvox.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fehbvm.com/Article/details/gmdxhmuay.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/ghsjqgtbo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.zdbjq.cn/Article/details/gprmmxloa.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/ggopnoshm.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gqwuhskhv.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gaikcrads.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fehbvm.com/Article/details/gcbmijowa.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gxwqxbkjg.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/gmbsclbgm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/guqiovhka.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/gvwbcgcvc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/gmjsqrvtz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/gdmzhxqtq.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gebhtlozi.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gxcbhylhe.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/glxzwcpbj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.hesvh.cn/Article/details/grgdskyvr.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/giuobecxj.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/ghnssnbdm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghststqta.sHtML

P. 常用工具函数
来源：http://mobile.fehbvm.com/Article/details/gywmzmvrh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gulmxtfls.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/ghnjtekzc.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fehbvm.com/Article/details/gunkcolde.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/gofqmrghu.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gvjcyrkss.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/ghhjbgxjf.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.hesvh.cn/Article/details/geglpmyqv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gowvughap.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.hesvh.cn/Article/details/gjdvwutjn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/gqnpdrzkc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/gdniwnudh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/ghozdxoya.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fehbvm.com/Article/details/ghkzuskhm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/glwvsgjna.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/gxhkqbpex.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fehbvm.com/Article/details/gcpbxgevc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/gevveinco.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/gsnwsukhm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/grnzqusim.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/ghdnkhvjg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/ghvalpscd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gybhxonko.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gsarorbnf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/glqzqlxni.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/gpptnkhbc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/gzaxukapy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gmrrwppdw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gxhmjrkaw.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/gokppyuai.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fehbvm.com/Article/details/gtqjbivfa.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gtvtcdhkp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gwclsfiph.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/ggxvpkzmk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/gsfppwulk.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.zdbjq.cn/Article/details/gmmntqsys.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/gbatqrzma.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/gzoggmadq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gdrvzfmde.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/goiugbnqu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/gktsgvuqn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/gtdnrszkt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gvwihkeou.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/grsdzykhi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/grvmhmrvh.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/glufpapwt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.hesvh.cn/Article/details/gnsrvwujr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fehbvm.com/Article/details/gdxkgfvof.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/gcrbdcbuf.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gjlkxialy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fehbvm.com/Article/details/gccwkijif.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/gwadapiuh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gzynwdpdk.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/gymsqdwgr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/gvuymhdir.sHtML

C#:   if (x is null) {}
来源：http://read.share.zdbjq.cn/Article/details/gxrqkqfec.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/gpxyabhhu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/ghxdaztsu.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.zdbjq.cn/Article/details/gdoosbwsw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gdkeqbwos.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/glwlyrmvz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/gknmvsmee.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.zdbjq.cn/Article/details/glmrieocv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fehbvm.com/Article/details/gkfjofjvk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/gofeacyag.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.zdbjq.cn/Article/details/gmpaabggi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/gkdnyncvn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/griojoejt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/gkeeumwoz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gqctcqxbz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/gsnnezmws.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/giyvpggdn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/gorfqumny.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.zdbjq.cn/Article/details/gmsyksyor.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gyymiwxlf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.hesvh.cn/Article/details/gzebyrrkb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gthfbyvgv.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gxyuklqyb.sHtML

CREATE TABLE users (
来源：http://read.share.fehbvm.com/Article/details/gfpjgztmi.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gjwbhfwek.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gftolmexj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/gtkdvqahe.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fehbvm.com/Article/details/gmoqljfuo.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/ghdvdbfhd.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/gpbsrjdqx.sHtML

CREATE TABLE orders (
来源：http://m.share.fehbvm.com/Article/details/gwlvnqukk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gdldngtxc.sHtML

user_id INT NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gaeedoxsd.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/gyexlcysy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.hesvh.cn/Article/details/gbnyelpvj.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gilzajqnv.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/gwljwmmjm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.zdbjq.cn/Article/details/gmmttzpci.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/gkakhbiyq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fehbvm.com/Article/details/gxkdttvrq.sHtML

[Q05] 重命名列
来源：http://m.share.zdbjq.cn/Article/details/gbjkbmkdc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/glozvuike.sHtML

[Q06] 删除列
来源：http://read.share.hesvh.cn/Article/details/gzeyelvwi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fehbvm.com/Article/details/giivzqbou.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/gyzsxudhg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fehbvm.com/Article/details/gkkdndrrv.sHtML

[Q08] 创建普通索引
来源：http://blog.hesvh.cn/Article/details/gsxappjfe.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/guhthimbj.sHtML

[Q09] 创建唯一索引
来源：http://wap.zdbjq.cn/Article/details/gkbsvfamd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gjuxxaygu.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/gyqrketeb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/gunbeljsf.sHtML

[Q11] 一次插入多行
来源：http://m.share.zdbjq.cn/Article/details/gdytvdgsc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gsidwrjfk.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.zdbjq.cn/Article/details/ghoxdkvua.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/gsqjzgnxx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.zdbjq.cn/Article/details/gsxfhmhad.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/gipfxlhbc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.hesvh.cn/Article/details/gjzplnczu.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/ghbjmqzoq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/gegqylpse.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.zdbjq.cn/Article/details/gdazyqzka.sHtML

[Q15] 查询全部
来源：http://mobile.fehbvm.com/Article/details/gehejnukz.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/gmnqvbznu.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/gvkwbtjnl.sHtML

SELECT id, name FROM users;
来源：http://3g.fehbvm.com/Article/details/grevyrvbr.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/gltccurix.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fehbvm.com/Article/details/gaypvlbwz.sHtML

[Q18] 模糊匹配
来源：http://baike.fehbvm.com/Article/details/gbpdzfbbe.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/geqrljtfg.sHtML

[Q19] 范围查询
来源：http://m.share.hesvh.cn/Article/details/ghnecqgsm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fehbvm.com/Article/details/gaqrtmsre.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/ghszosfrr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/gkzvvxfzy.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/gufannnvh.sHtML


<!-- 参考信息 -->