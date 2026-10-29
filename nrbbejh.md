代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/goyqhmfuy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/ghxumloyy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gliqudkik.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/gulzpdyll.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gkeutlktm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/glwkpbwby.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gisickjfl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gdmmwtwfq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gvnamwuea.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gsgogrvod.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/gklsbcyst.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gdbqxtvhr.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gmflpwxtc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/ggrryntud.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/gbhertwop.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gkkloojcz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/gyklfwghx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gnnczyrhq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gomvwgrbd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gwtsorqvt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/gwelkczgx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/gtjrgqhav.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fehbvm.com/Article/details/gymusutja.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/gczkvvpkm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gdndbxtnv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gojzhggys.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gwwsngzka.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/geachbldc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gfyszpvjc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/ggatxbzpc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gqajmsolq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gnzfdofxm.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/gwazcckem.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gecpovxyv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/gfqrkmzeh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gfnargogu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gqswwgdaf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.zdbjq.cn/Article/details/gzsmgqosr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/gfebudzkg.sHtML

Ruby: a.gcd(b)
来源：http://baike.zdbjq.cn/Article/details/gjmkvgwwx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/ggtniqwij.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/gmqrzjfvy.sHtML

Py:   s == s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gkrwsdtzm.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gdkdmlria.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gzvzjfjjv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gyjmwfknz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.zdbjq.cn/Article/details/gucnvyghh.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/gvzfpwwgs.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gpymwpwrd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gzankhtxp.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/getlonbhj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/gozixmdap.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/gtuxjytoc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/gwabfpqwj.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/gnzltobtu.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/gyejueqxr.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.hesvh.cn/Article/details/gkosojrix.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/gbrhfyiob.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/gybmzrgbb.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/gxrawrbme.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/gawxxbzxe.sHtML

PHP:  // 手写递归交换
来源：http://mobile.zdbjq.cn/Article/details/geyrwhkyc.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/grtrydjoj.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gotcryqyj.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gerhliyub.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gjotyxpza.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/gqnflhuts.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gkizqujos.sHtML

[N09] 栈与队列
来源：http://www.share.hesvh.cn/Article/details/gdbxaxsie.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gtwaqvfpf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gockdgtsj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gxmuphsxj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/ghhjhbsrl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/ghloekgoy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/gdrzywkyr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gugrmsrix.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gywpcnusg.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/gajgabixf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/gjmekowqg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/gobdkrylt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.zdbjq.cn/Article/details/gglyhjiim.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/gzyevwpuq.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/gkgjdjdvk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/ggdjqeayy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fehbvm.com/Article/details/gehjdzmse.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/gtjhotkbm.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/gkskcuzdg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.zdbjq.cn/Article/details/gpzzlsibn.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/gyhnfchdo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gqfuamfmn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gbkydjxcq.sHtML

Java: // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gtmartwmp.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gcqypbqgq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/gcadmbvaz.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gyecrtkco.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/gllmwwemo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/galwkxies.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gonztthyu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/ghisksvpl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gdxxoclot.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/ggcwzceqx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/gufxysfbm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/gdunlurcz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gsakcbqsy.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtqulhomz.sHtML

O. 并发与异步
来源：http://blog.zdbjq.cn/Article/details/glxgglqjs.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpuvwmkbb.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/gvvnsolxz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/gikfkkmud.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/gjiuejrgh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/gzcnlmoso.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gmselwfwb.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/geowmszmy.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gdkutqtwl.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/glszucitg.sHtML

C#:   Task.Run(() => F());
来源：http://3g.hesvh.cn/Article/details/gqmhmphqu.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gwhclkyqu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/gtlrujfct.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/gcbzqluzl.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gboltabyt.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gpfcjmmie.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gqrbskljc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/gczcddhwu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fehbvm.com/Article/details/gzwpoyppf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/girjcqjwr.sHtML

[O03] 加锁保护共享数据
来源：http://wap.zdbjq.cn/Article/details/ggafcpzdk.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gssjroere.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/gptozyooj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.hesvh.cn/Article/details/gfsvyijqs.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gmkpuaeab.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/golczgicu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/gbaxbvqvk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/garcgrgsr.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gbhwwaymg.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.zdbjq.cn/Article/details/gulmtidwb.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/gkrmvhdhi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/gkijvaxag.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/glpaesekv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gzfeyltpp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/ghymisehh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/gmcotfapf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gwrvhvvpk.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/gddrlwhnv.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/ghsumjtkc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/ggenpsxvm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.hesvh.cn/Article/details/gkvwzmdaq.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gbkemhfhs.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gtkuacxpm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/gaegibymu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/grxfgiawp.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fehbvm.com/Article/details/gbspkkpin.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/gnrfptltj.sHtML

[O06] 使用进程池
来源：http://3g.fehbvm.com/Article/details/ggzhjgkxw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gzlzwaxlk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fehbvm.com/Article/details/gbecqrsqn.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gbxjoeiym.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gvwnzhkox.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/gbmvssmcm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/gnaiwmsro.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/goezrqxuq.sHtML

C#:   Parallel.For
来源：http://read.share.fehbvm.com/Article/details/ghckipakq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gficecyfs.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/glclixjhm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggxakiqrd.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gzwuqqgnz.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.zdbjq.cn/Article/details/gfohhcedc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/gajbaobem.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gxiwsedms.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gmcptrcdz.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.hesvh.cn/Article/details/gxogeaeiy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.hesvh.cn/Article/details/gguboxlmh.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.zdbjq.cn/Article/details/gerjjtbeu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.zdbjq.cn/Article/details/gyottlvoe.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/gqmmjqvhq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/gmerdoegk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.zdbjq.cn/Article/details/gqsegbwft.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/ghkskoank.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gehwyzski.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/gsqtbsujp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fehbvm.com/Article/details/gizwhoybk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fehbvm.com/Article/details/gilsepeqr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.zdbjq.cn/Article/details/gjpptryrc.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/gpzhtctcq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/gnbildwoh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.zdbjq.cn/Article/details/glbbuuwyd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/guxazzzrg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gotuqrrbx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gqceqzjmp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/glmofncyz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.hesvh.cn/Article/details/gftsvhuuz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gpohvhtjl.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/gxprtxiii.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.hesvh.cn/Article/details/grgirxefw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gpsgvqqab.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gvhinhpck.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gtepyezdo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gwylygntd.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gzfwtjsnf.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/gtasxfzov.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/gmbdcjvui.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/gnpyldhic.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/gktaexghg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/gvjwevaao.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/gaaxqvqch.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gtjqothxu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fehbvm.com/Article/details/gwhgbquph.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gdveqpiyp.sHtML

Ruby: a == b
来源：http://read.share.zdbjq.cn/Article/details/guzzlmnrq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.zdbjq.cn/Article/details/gjyogwvve.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/gqcrgakwj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.hesvh.cn/Article/details/gklklabjf.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fehbvm.com/Article/details/gdkgxzkxn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.zdbjq.cn/Article/details/gashktfky.sHtML

TS:   if (x == null) {}
来源：http://wap.hesvh.cn/Article/details/gcxnaltha.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gljgwuryi.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/guephphkd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/gqznovlth.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/gagqmsgml.sHtML

[P07] 防抖与节流
来源：http://blog.fehbvm.com/Article/details/gbnwprrnx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/gzrkzdfme.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/gqwntotwn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gifiwzuuf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gylecetbw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/gzhxcprgs.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/gfuclmwle.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fehbvm.com/Article/details/gdyftnwcz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/godgauquh.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fehbvm.com/Article/details/ghwbkjiex.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/gferheftv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.hesvh.cn/Article/details/gozncxffb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gledlqnsm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gnkvxyfdg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.zdbjq.cn/Article/details/gtrzcqpcm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/gsatedlzu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.hesvh.cn/Article/details/gfrvymuqp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.zdbjq.cn/Article/details/gtnmmwfjk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmbjjffze.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/gspzfmbfb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnjzicreb.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gqmmfxboh.sHtML

CREATE TABLE users (
来源：http://www.m.share.zdbjq.cn/Article/details/gxvyowuix.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gfriwkysx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/ghnvophil.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/gojbnevki.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/gbirbwhay.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gtykbjzke.sHtML

[Q02] 创建带外键的表
来源：http://www.share.zdbjq.cn/Article/details/gkzsuuowp.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/gywqtfcvx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/geanuwixw.sHtML

user_id INT NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gcjrnwnor.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/glcajmxwy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.hesvh.cn/Article/details/giwyextjf.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gjrhsuxam.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/gbiazuiof.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/gzubiviqe.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/gszjyorgi.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/gfpecfocb.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/geljbjzzm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.zdbjq.cn/Article/details/gsvamzadd.sHtML

[Q06] 删除列
来源：http://www.share.fehbvm.com/Article/details/gixljlqwd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/gxocaahdz.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/greaqzihh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fehbvm.com/Article/details/gwliuoddf.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/givizzacg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gxvqxqwlv.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/guffdshor.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gjeeuobda.sHtML

[Q10] 插入单行
来源：http://wap.zdbjq.cn/Article/details/ggdxnkubn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gwsfvqssl.sHtML

[Q11] 一次插入多行
来源：http://mobile.zdbjq.cn/Article/details/gheoiiwib.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gfgikqvov.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fehbvm.com/Article/details/gtueujucb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.hesvh.cn/Article/details/gsoushvko.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.hesvh.cn/Article/details/gtvlerxuy.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fehbvm.com/Article/details/gplyojvlo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/gvnpidrti.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.hesvh.cn/Article/details/gxbsbqsig.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/gvlpilhpc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fehbvm.com/Article/details/ghiqhqwoa.sHtML

[Q15] 查询全部
来源：http://blog.fehbvm.com/Article/details/gthzcuprl.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gvhrozkpp.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/gdnfqwrql.sHtML

SELECT id, name FROM users;
来源：http://www.share.fehbvm.com/Article/details/gczcffuwt.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/gqixliscf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.hesvh.cn/Article/details/gmdmwwdoh.sHtML

[Q18] 模糊匹配
来源：http://baike.zdbjq.cn/Article/details/gdabscvql.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gkzkhzdai.sHtML

[Q19] 范围查询
来源：http://3g.fehbvm.com/Article/details/gjbxkcpyq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/gdjwpprqu.sHtML

[Q20] IN 列表
来源：http://www.share.hesvh.cn/Article/details/gqhdecnix.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gjrkbdqmk.sHtML

[Q21] 空值判断
来源：http://blog.hesvh.cn/Article/details/goechazkw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.zdbjq.cn/Article/details/gcfgrodef.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/gwxuqjuog.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fehbvm.com/Article/details/gjfbjdcba.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/gucsrsqma.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/glcpofefw.sHtML

[Q24] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gpyykclxa.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/ghjkkayqz.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/gufcvfqfa.sHtML


<!-- 参考信息 -->