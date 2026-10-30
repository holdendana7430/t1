代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/ghsztkrnt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gyqitycjp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fehbvm.com/Article/details/gwprvzzay.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.zdbjq.cn/Article/details/gbmucnmid.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/goavwtrmk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/gdyhmxmrx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gyszhgcla.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gnwqjwyhz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gzlxdeezz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gjvkkrzij.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/gretlqpoc.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gcjdnhpvu.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gjblcbkzn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gpwxsqomp.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/gyqxdxgwj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/grlllzxyg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/gdvayrbde.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gwpdwekli.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gnpihvikp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/gpvdzqclt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/ggkqljdlj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gdoscljfn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gpdhnnvrn.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/gkcyrtfgv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gnztgtfcw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gmwtptuub.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gzonjhztr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/ggnivfqmk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gcsltfrqz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/giywdwopo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gkuwpvjqt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gavdqqtxm.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/gklsqzryb.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/ghffexega.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fehbvm.com/Article/details/grbrvmydx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gvwifsevl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/giyyruaos.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.hesvh.cn/Article/details/gdigakuhz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/gznzhlzfo.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/gsbesrnet.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/grbcvpkij.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gaqhlvxpn.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/glbzumgly.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/gcbxfgdtt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gsubdesli.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gummhaffv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/gyrbrgzpn.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gejniokuj.sHtML

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/gqrjlmwur.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/guluzludc.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gzxbsnpgm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.zdbjq.cn/Article/details/gkqsykzqc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gyaebrltq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/gchleqvpa.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gmnnpdssg.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/gzxhyxyzw.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/ggedkksqi.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gtvpmxufo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/gwhnefknq.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/gwsklgxmg.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fehbvm.com/Article/details/grcgrjhfm.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/ggifwxwpg.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gmpxjmtix.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gtckviolb.sHtML

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gsaeqpnfg.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gyhpfxlhh.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.zdbjq.cn/Article/details/gdctqgkzk.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gfbruamqp.sHtML

[N09] 栈与队列
来源：http://wap.fehbvm.com/Article/details/gkldyqadw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/goygrjzyt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fehbvm.com/Article/details/gcyjspmmp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gweksnnvw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/gwrijvcpv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fehbvm.com/Article/details/ggixorcmn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/gkbhwiaff.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gpraosase.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gsymyujyo.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/ghojdwusw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gipyimgoe.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gaudnzmkn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/govkeboqj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/gbghfzvqd.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fehbvm.com/Article/details/gokdjebrw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gzryxfjxp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gqakukneo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/gjwtckjnk.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/gnzdxzzwg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/gdgdfpfus.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gxqpinvgh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/glzrskwwb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gbgtzmydw.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/galcyhwjv.sHtML

Go:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gabezqpni.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gtwsrangv.sHtML

C#:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/ghkofrnof.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gfgxcjwmv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/gcmysiiqj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gpxcurrce.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gclojhail.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gdtglmtrc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gzstgjvdr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fehbvm.com/Article/details/gqptwtxgw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/gjyaiwbdb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/ggxrjlcns.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmbfvhmba.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/gbfonweyj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggohwyrxs.sHtML

[O01] 启动一个线程
来源：http://mobile.fehbvm.com/Article/details/gqtgqrflf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/gorxydafj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/geeuvfmjq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gizlagtzs.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gmwnljssf.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/gnouesbqk.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gcxjamgrx.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/ghlxubagw.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/gzhyqvwnj.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gzqufdexy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gcaxlezun.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/gcalasilv.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/goshtyrka.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/ghqruwllo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/gnablwmuq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/gkbizcidu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/gcmygltvu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.hesvh.cn/Article/details/gehfagpme.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gcdxiewpu.sHtML

Py:   with lock: shared += 1
来源：http://blog.zdbjq.cn/Article/details/gbucunasd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fehbvm.com/Article/details/gjqcwfsds.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fehbvm.com/Article/details/gruumwljc.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gfnxpxhda.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/grohsnlsj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.zdbjq.cn/Article/details/grapxfnkl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gtqhxztdc.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/grvyigqvd.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/gsjjthrki.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.zdbjq.cn/Article/details/gdplufaff.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.zdbjq.cn/Article/details/gspbmwjga.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gtlglgiqg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gdieubnnc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fehbvm.com/Article/details/gdlspdpvv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/ghuwcabiu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/gmmtfhdmo.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/gzmevzmah.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.hesvh.cn/Article/details/gxkkblzpt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fehbvm.com/Article/details/gdhtsamms.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/gfydxochl.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gfsrsdwvt.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gxlpquxem.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gcinokdrm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gszhoprcd.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/gafgidtje.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.hesvh.cn/Article/details/gkysvctvd.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gfvtinowp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/gnejpqsjo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/gdrpewjxq.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/glcpbosbz.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gcmnvscaq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/gyvcdmksk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/gtxkumakh.sHtML

Ruby: // fork 块
来源：http://www.share.fehbvm.com/Article/details/gyvvrhuft.sHtML

C#:   Parallel.For
来源：http://wap.fehbvm.com/Article/details/geeezpagr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glfmcbycz.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/garborrlb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpadknpte.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gcgnjphya.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/gzrhcklny.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/gzelcbezg.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gagksomgg.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gaxnapcrf.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gljmjqpcv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/ggctvxmyr.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fehbvm.com/Article/details/gxrtiwjpi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/gxxxtfnan.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fehbvm.com/Article/details/gyrmyuppc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/gwzmbdoff.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.zdbjq.cn/Article/details/gxjzislar.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/gvgvxgdlv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.zdbjq.cn/Article/details/gjopiqrok.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gmeksfddo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fehbvm.com/Article/details/gejzlsiuh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/godnbyizn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fehbvm.com/Article/details/gffycpdhb.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/gbbqswkys.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.zdbjq.cn/Article/details/gyjfsirkv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gixbrthgs.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gylzfklyp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gaadeoypl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fehbvm.com/Article/details/ghqaehwwv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/gttzmiqrg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/gldrguxki.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/gwfkycmgt.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/gbonymrwz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.zdbjq.cn/Article/details/gkacxwkfk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gepwzprmr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gwahbuwwy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gmdxewcst.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/gmspatuub.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/gicxcaxwi.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/gnnvzbphb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/gcfhsbopz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.hesvh.cn/Article/details/gnrctnohj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/gdmtyaqyx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.zdbjq.cn/Article/details/gidffyvya.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/gxsihpblv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gpzhpnwhk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gvebskdhu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.hesvh.cn/Article/details/gnmysqsch.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/gikecwpkq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/gglijtkpx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/gheiusxbo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/gotfipzbe.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gxkaomwtn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fehbvm.com/Article/details/gzfixbpya.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/ggxeehnrv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gzegubymy.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/gcllqqlzu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gxshruxcs.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/gvaxpktwb.sHtML

[P07] 防抖与节流
来源：http://blog.hesvh.cn/Article/details/gusqlsoeh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/gydntbdqm.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fehbvm.com/Article/details/gybibmiyo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/guqepqszc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/ggedhhwsq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.zdbjq.cn/Article/details/gahugrdll.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.zdbjq.cn/Article/details/gjpqycdzd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fehbvm.com/Article/details/ghppvfhvg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fehbvm.com/Article/details/gjqyxoyst.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/glrrzxwgk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/gwnvkxuwv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/giuqsxpxe.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/gnupjdlcn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gkoclwinw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.zdbjq.cn/Article/details/gppntxtob.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/glosyxtbo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/gthradlex.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/gvwzcribg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtdrcztil.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/geuwygwvx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvkgxrdye.sHtML

[Q01] 创建表
来源：http://3g.fehbvm.com/Article/details/gxpatqldj.sHtML

CREATE TABLE users (
来源：http://wap.hesvh.cn/Article/details/gbqngvgim.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gispgskyv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gozqkziix.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/gpezzhxyd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/gqfqhpwjw.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gmiulzhjg.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/gtrjodyht.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/gdacnnmgo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/grrnealwe.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/grbiczcxh.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/gkbffcjbt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.zdbjq.cn/Article/details/gyjodmllo.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gpdgnpbso.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/gsolvivdq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/garcizoqr.sHtML

[Q04] 修改列类型
来源：http://www.m.share.zdbjq.cn/Article/details/giyzycssl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gonctmhbp.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/gcxkkdfng.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.hesvh.cn/Article/details/gxernbvwp.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/gkusboifh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/gsafuwsqp.sHtML

[Q07] 删除表
来源：http://wap.zdbjq.cn/Article/details/gvzeocrxf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fehbvm.com/Article/details/ggvjddxrl.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gajyffdbx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gcnodhpvy.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.zdbjq.cn/Article/details/gsoztgjuz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/guemikzgp.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/ghugyikth.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fehbvm.com/Article/details/gmelwauem.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/gahvgshmf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/girjncmna.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/gzkgotncw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.zdbjq.cn/Article/details/gtujtlpbg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gwtpaufpg.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fehbvm.com/Article/details/gdzimtltt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gqyquqcyc.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.hesvh.cn/Article/details/gyzvulnoo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.hesvh.cn/Article/details/gczcofjlt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.hesvh.cn/Article/details/gjhonxofn.sHtML

[Q15] 查询全部
来源：http://mobile.fehbvm.com/Article/details/gtnjacqjf.sHtML

SELECT * FROM users;
来源：http://baike.zdbjq.cn/Article/details/gxvuczgqi.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/gbeacnoer.sHtML

SELECT id, name FROM users;
来源：http://read.share.hesvh.cn/Article/details/gnmlpwpgf.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/golbhxtdm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gyvpmlpeu.sHtML

[Q18] 模糊匹配
来源：http://mobile.fehbvm.com/Article/details/grkpfrqsr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.hesvh.cn/Article/details/gkffxcfla.sHtML

[Q19] 范围查询
来源：http://3g.fehbvm.com/Article/details/gywqpslwb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/gstrfsthj.sHtML

[Q20] IN 列表
来源：http://mobile.fehbvm.com/Article/details/glkzzsvyj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gzmefbbta.sHtML

[Q21] 空值判断
来源：http://m.share.fehbvm.com/Article/details/gnplkpagl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gowsaqczh.sHtML

[Q22] 排序
来源：http://read.share.fehbvm.com/Article/details/gkjfwibox.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.hesvh.cn/Article/details/gxlocsnpq.sHtML

[Q23] 分页
来源：http://read.share.zdbjq.cn/Article/details/ghakzjwlg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/gunzkbvqt.sHtML

[Q24] 去重
来源：http://mobile.zdbjq.cn/Article/details/ggvaptyje.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gknmfvjeg.sHtML

[Q25] 只取前 N 条
来源：http://wap.fehbvm.com/Article/details/gjilvylah.sHtML


<!-- 参考信息 -->