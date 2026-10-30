代发 wailian999

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gvwuxvhla.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.hesvh.cn/Article/details/gxkiatxjy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fehbvm.com/Article/details/gqytixdnv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/gofiqzala.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.hesvh.cn/Article/details/gzpqwzddb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gkffertgr.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/gokrdkghq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghiymlxfz.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/geszbuawg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fehbvm.com/Article/details/gbjxyqjhj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/guziitfip.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gfcgkeynq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/glparzmch.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gvfgkdzfe.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gzpjjepxs.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/ggkhrzsiy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gjwxnnmvq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/gqeudtuph.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gfqekemsf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/gnxgpmtpn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gymxosulo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/ghfhlrrwg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/grmoefvqu.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gszaaqgxk.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/grcwiyfww.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/ghkehqsez.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/gufjjjuvo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fehbvm.com/Article/details/gqceunloc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/grfrawwoz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/ghmgfwjdz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gdogckuqg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gnunuibrr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.hesvh.cn/Article/details/gcwtdnbpm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/gjmlpdikf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/gnwfpvxgk.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gxuushnyx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gbzuxaavc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/gkervljis.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gvymulqpb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gfmsbvcax.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gpclprgry.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/gojkyqbro.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/ggriabnvm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gjxrumvzo.sHtML

[N05] 最大公约数
来源：http://www.blog.fehbvm.com/Article/details/glxwuittb.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/guxvjbckf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/gqksepcbt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gwqosmhyl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gytfjjqmx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/gsqoasglu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.zdbjq.cn/Article/details/gbizdemll.sHtML

Ruby: a.gcd(b)
来源：http://www.share.zdbjq.cn/Article/details/gxfncbhck.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/gvvzwhsxh.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/ggjjdojdi.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gxkoyruve.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gvdanbklh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gncknjcug.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/grxkehqjd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gpekqifuz.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/ggrldupay.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gqjqczuye.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gdtvnxydn.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/gfrvwixnp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/ggmkkhyqs.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gywratozb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.hesvh.cn/Article/details/gqiecilel.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gurnuglnb.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gzvrqppin.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/gszormput.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/gcqqtjfpe.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/gzilpybfy.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gidezxurt.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gwzuqwzuu.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/giifskvmg.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/guqqhjzhb.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gwfkqjzbs.sHtML

Java: // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gaubcnnrv.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/ggtclqsvh.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/gwzlldcdb.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gnpxgeyml.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/gbladbnsm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gerqnclgk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/gvqfrijgc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/glqiflvan.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gvkclyzuv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/gkmuhxyve.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/gcwwmzwgs.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gxktytfog.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/gnyodcstk.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/gwghmqtza.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/gzsmzsimz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/gnlxmifpv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/gbccvfggh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gizpdifyr.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gksaieqed.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/ggzdnubdl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fehbvm.com/Article/details/gpoiogrgw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gkokfsbuv.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fehbvm.com/Article/details/gzcvatvwb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gmoedgdwq.sHtML

PHP:  // 手写递归函数
来源：http://blog.hesvh.cn/Article/details/gccsdynmz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/ghgijirmd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gjfubxuwa.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gxlijsixf.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gemoghsqv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/gxdeajrnl.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gigvgfjvs.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.zdbjq.cn/Article/details/gijxijmsb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/golcajpkw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/gqfryjdjn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gotokeyur.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gompoghsh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gbhqwvvzz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gfckabneb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fehbvm.com/Article/details/gjlrpexvy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/givnoaiyt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxdruzhlj.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/grjjaioeg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gypzavzap.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/gmciepbrh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/gfmybhckw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fehbvm.com/Article/details/gmsrsdgth.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/grzujkukb.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gpposxpxm.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/gibgageyd.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/ggnabicas.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/gpifdmijn.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/grlfvxliv.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/grnmveanq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/gtlpiatqh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/gyxzkyrhl.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gailryseu.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gxzttaice.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gttzeyltm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/getizljan.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/gvnnenqho.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/gbuxbfqyz.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gxrdzaepr.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/gewqmeomw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/gpcpfzvaq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/gvyllsozr.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gbjlascyt.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gckshypgc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/gmgmaweak.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gliyrbizs.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gwrfgvsyq.sHtML

[O04] 定义异步函数并等待
来源：http://blog.hesvh.cn/Article/details/gqwowjgnd.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/goyifgwqu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gqtlbovaf.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/guzedagkx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fehbvm.com/Article/details/goqrveypy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/ghctotuhg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.zdbjq.cn/Article/details/glzyeaqfe.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/gquuiluvj.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.zdbjq.cn/Article/details/gglddjfij.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/giamtusxp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.hesvh.cn/Article/details/gxywshhki.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.zdbjq.cn/Article/details/gicytavmb.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gfbwdvzsy.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/glpttqfdt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fehbvm.com/Article/details/gzgevydje.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.hesvh.cn/Article/details/gkmknxepn.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/gddhmhhhl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.hesvh.cn/Article/details/grnywyphx.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/gnpnquewr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fehbvm.com/Article/details/gexghdrzx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.zdbjq.cn/Article/details/greqjiecv.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/glgyzfybz.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gfmfzmjew.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fehbvm.com/Article/details/gdjveaupm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/gosrybxtr.sHtML

Ruby: // fork 块
来源：http://www.share.fehbvm.com/Article/details/guhfheapz.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/gqxlugmmm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmlhhbilt.sHtML

P. 常用工具函数
来源：http://m.share.fehbvm.com/Article/details/grohmsjwa.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsdtgtuwc.sHtML

[P01] 生成 UUID
来源：http://m.share.hesvh.cn/Article/details/guxjdgrnx.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fehbvm.com/Article/details/gttuwulrs.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/giydsfccg.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gpdkiteux.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gdnhbmrdx.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gantvsldz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fehbvm.com/Article/details/guwgukcnp.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/gibcbkquz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.zdbjq.cn/Article/details/ggpilkzpx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.hesvh.cn/Article/details/glupkdoyf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/gyyhvmjau.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.zdbjq.cn/Article/details/goddtpsam.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.zdbjq.cn/Article/details/gvqfygyud.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/gymncjppe.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/ggttvrbpa.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.zdbjq.cn/Article/details/gqagrjhud.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fehbvm.com/Article/details/gpgprebae.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fehbvm.com/Article/details/gmfwxapud.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/ghokmrnxy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.hesvh.cn/Article/details/gfnftpdvd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/gxzjvajed.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gjwysyjgr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/guxsgksqr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.zdbjq.cn/Article/details/gziexsjmc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/gafvkzovv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.hesvh.cn/Article/details/gzhgzfwrs.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/gqmhletkg.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/gnjzeqtpr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gtwznqkfu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/giqrmyknp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gdapzdenl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gkletjmyu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/gckifndkd.sHtML

Go:   len(arr);  len(m)
来源：http://3g.zdbjq.cn/Article/details/gfgpagkyp.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/gjojfvvni.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fehbvm.com/Article/details/gmujudeon.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.zdbjq.cn/Article/details/gjdyzodto.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/geefatnhd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fehbvm.com/Article/details/gdnxtpiqp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/gmceuugep.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gkyoaactv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/gadzqexar.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fehbvm.com/Article/details/gzktfeznp.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/gbbpxsrik.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.zdbjq.cn/Article/details/gferuvhqw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/goxzhbtsc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.zdbjq.cn/Article/details/gdqsarqki.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fehbvm.com/Article/details/gogztuywd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fehbvm.com/Article/details/gnjgzrcpj.sHtML

TS:   if (x == null) {}
来源：http://mobile.zdbjq.cn/Article/details/gykjbmyrz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/guxokdsqu.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/gxpfezitp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fehbvm.com/Article/details/gedlnwafu.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/gtzmjzlmm.sHtML

[P07] 防抖与节流
来源：http://3g.hesvh.cn/Article/details/ggfgudfpm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/gyutxmxwd.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/gpcffqhwf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gorwfmric.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/ggbftlhsi.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/gposxeygr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.hesvh.cn/Article/details/gllcspfsy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/gfuhjlvne.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/gvhwkrzzg.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/gwurostmq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/gqvjmvqrf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/gvmifuqsv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/gurmkdvww.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gxoqcvldi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.hesvh.cn/Article/details/gpfnufoxr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/gbicyrstv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/gkmsvpncy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/grfwhxgry.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmxhgnxok.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/gawzuwaqp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gekptbxrh.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/gsfeiskgl.sHtML

CREATE TABLE users (
来源：http://read.share.hesvh.cn/Article/details/gfspsxwkl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gzeoyusxr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gbexgjzad.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.hesvh.cn/Article/details/gzuvahanc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/glbwwpmdg.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gaiyeepkc.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/glihipxnb.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/grgmozeqy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gkixxmmjc.sHtML

user_id INT NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gylybiwhf.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fehbvm.com/Article/details/gxozjptct.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.zdbjq.cn/Article/details/gqbmxzlhx.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gobvxzwse.sHtML

[Q03] 增加列
来源：http://m.share.fehbvm.com/Article/details/gwisjhcko.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fehbvm.com/Article/details/gwytbrndt.sHtML

[Q04] 修改列类型
来源：http://m.share.fehbvm.com/Article/details/gxymvyewo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/glchobfyv.sHtML

[Q05] 重命名列
来源：http://wap.hesvh.cn/Article/details/gskvgszce.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/gkynnqvyw.sHtML

[Q06] 删除列
来源：http://wap.fehbvm.com/Article/details/grbkammqg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/gjfinoula.sHtML

[Q07] 删除表
来源：http://blog.hesvh.cn/Article/details/gmtgrrtmc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.hesvh.cn/Article/details/gqinysycc.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/gzexycjww.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gosceatky.sHtML

[Q09] 创建唯一索引
来源：http://3g.hesvh.cn/Article/details/gkqvxnbaj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gvxotseqk.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/gjtnmmcjt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/gbhdijncr.sHtML

[Q11] 一次插入多行
来源：http://blog.zdbjq.cn/Article/details/gubujdxxi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/gdoyexwju.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gmultpqcm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/gdowbjnno.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/gawocokue.sHtML

[Q13] 忽略重复插入
来源：http://3g.zdbjq.cn/Article/details/gcnrwwbvc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.zdbjq.cn/Article/details/grkjjcoyb.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.zdbjq.cn/Article/details/ghidiscfo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/gmxmhbtpc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/geslyvzxt.sHtML

[Q15] 查询全部
来源：http://www.m.share.hesvh.cn/Article/details/gqijkkfid.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/gzmrpencf.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/gkgoyocfr.sHtML

SELECT id, name FROM users;
来源：http://m.share.hesvh.cn/Article/details/gmzrdikgv.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/gwpzlikjy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gmsaomouu.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/gzsjklvyn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/gqomoogvs.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/gomnhpdud.sHtML


<!-- 参考信息 -->