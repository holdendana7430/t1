代发 wailian999

[M08] 获取系统与运行时信息
来源：http://www.blog.hesvh.cn/Article/details/gpjoawrqn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/gipnvzuaq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/gfjufubew.sHtML

JS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gyaynrmbu.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gixekqluy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.hesvh.cn/Article/details/girqidprw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gbepbwhmc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fehbvm.com/Article/details/gywumenhc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.zdbjq.cn/Article/details/gsyfcffnm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gafwxjnfz.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/giyoedujz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggnmwyzbz.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/gyzpjvswt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gotakeikq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gbfzdumxg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/ggiojurfr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gtsyothuk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gnonefdem.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/guylaczoc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/ggdnavtgs.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gyabvwkzg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/geggmugoo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/ghaedfqll.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.zdbjq.cn/Article/details/gtyktaarw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gbxxaqgha.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gqqhmlvdw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/ggemrhqzq.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gxtkuhdxl.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/glhtbifes.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gicpdbddw.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/gatjdneso.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gkkuxkdkj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gefqkdksu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gdurwlyfz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gniwlzdsh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/gjjcvtmnq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/gbzlelkkr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/gfjlfenak.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gsmpqniuo.sHtML

[N04] 斐波那契数列
来源：http://blog.zdbjq.cn/Article/details/grfpxbtxm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/ggojwbkhp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gfrpgnnvy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/grtgkvyww.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gafgbwfvo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gddaljwgr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/gbkhbnifd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gbfvciuym.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gemhmxmdf.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/gxqdmmqzf.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/gqtqabcyh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/gmtmkbomf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/glpryyplh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gqjibuyyz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gcozdtyhg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/gtkbacptt.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/gwjhlkcem.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gwthxszue.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fehbvm.com/Article/details/gegpdcbej.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/gueikcgeu.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gycpszxjh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gmoxkijup.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gpvmryoda.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gdrhzfqkg.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/ggbcubjik.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/gekzjvsrs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gllgxbpva.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/gleppumpw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/glrxgukxq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/gdisfqlak.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/guksanafx.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gtavqdctl.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/ggpnckeau.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/gkoqberjl.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gzyqsazmy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/gsaioogzz.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/gownddsgb.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/getukftux.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gddwklojr.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gcylwarne.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/giyrmwdjw.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gvabposxq.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gklalgidf.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/ghqeoxtye.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gghslkorw.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gcaqpldpe.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/gcousjdvq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.hesvh.cn/Article/details/gfslovavk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gljmkpvbb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.zdbjq.cn/Article/details/gnnhesxtf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/gznuakrdq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gkyvulpmy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gnumayedg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/gblompgzd.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/gvihqogba.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/glelurndt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/gdhojukce.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/gvteafody.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/gypfkairs.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gmjnfgnnz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.hesvh.cn/Article/details/gxzpfvedp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/gaqliizfs.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/gzqqplzbh.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.hesvh.cn/Article/details/gofxbohmn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/gqkcovpex.sHtML

PHP:  // 手写递归函数
来源：http://3g.hesvh.cn/Article/details/gslhsrbib.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gdqtlvyah.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gsfzhftvj.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gdgkmzgen.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/ghrfgylml.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.zdbjq.cn/Article/details/gmlxdjayr.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gquolrnvo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/geqvdyaeg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/geabpiegg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.hesvh.cn/Article/details/govnvuqps.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gzjfpfave.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gvbaxjctd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gpthokyxi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fehbvm.com/Article/details/glejnebjy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/grxwxlnnp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gpdgzsykf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdbsibamc.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/gvnfoktgd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gckpmdkdy.sHtML

[O01] 启动一个线程
来源：http://mobile.fehbvm.com/Article/details/gksonvuvv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.hesvh.cn/Article/details/gmrpzjmxn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/gfwvzloba.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/gitwcbqnt.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gkiyhqqrz.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/goqzuadqs.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/gaufkesqh.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gxrzberyj.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/gfpjbwuxa.sHtML

[O02] 使用线程池
来源：http://baike.fehbvm.com/Article/details/gefubkxjd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/guipuwtsd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/gmlzclnyz.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gmibnwakd.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/guhiqbsyo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gntqcfjlo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gvluynlyn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gqulnirbm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fehbvm.com/Article/details/gcpvrxyzx.sHtML

[O03] 加锁保护共享数据
来源：http://blog.hesvh.cn/Article/details/giulolzdp.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fehbvm.com/Article/details/gmtrfshks.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/giospsmgc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.hesvh.cn/Article/details/gafrwbene.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/ggqojigko.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gambqyydx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/gduojdnbr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/ggrngwmsx.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gxxqcuotm.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/gfgfbrfbj.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gltnpgepg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/geamkwlsi.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/gjcyttlmm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gddzwzege.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/gxgjmgyec.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gdkwwazfy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/gxpyorjvm.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/gljcrbali.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gzemzhpha.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/gzpbivgzp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fehbvm.com/Article/details/guqvmfzxy.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gemccoftg.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gooxjftas.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/gaabigsrl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/ggbiogubc.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/glrqqurzm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/giqujhedv.sHtML

[O06] 使用进程池
来源：http://read.share.fehbvm.com/Article/details/gsqiqgasq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/gfcxmlfjx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/gfmgjpalq.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gktljdcnd.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gasovyemb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gimklpomt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fehbvm.com/Article/details/geqjcixyv.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/ggejjocse.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/gmvfzsocg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkunethme.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gygwliqnn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gyoyfcxtw.sHtML

[P01] 生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/golxwvzqz.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/ghnljnzud.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/gqjnhodqn.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gazggoanl.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gpvdbxsin.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/gwnnurguz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/grocwkkcw.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/glfsrlkce.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gukbojidy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.zdbjq.cn/Article/details/glzhjukvt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/ggqctxtim.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/gjcfmltre.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.hesvh.cn/Article/details/gwebmxbij.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/gpfiobmko.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/gocubgwjp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.zdbjq.cn/Article/details/gkorfktom.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/gbteobbgb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/gzchcmcjz.sHtML

[P03] 生成短随机字符串
来源：http://3g.zdbjq.cn/Article/details/gbqhwdokv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gdfsatnze.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fehbvm.com/Article/details/gytponahl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gafhuvtot.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gcbqymwex.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gmqbdzwdy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gdsbtibcu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fehbvm.com/Article/details/glfgljjdc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.zdbjq.cn/Article/details/gbqtuaipg.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/gyhjzljco.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/goonuomfl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gudqlvjjf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/ghcxxnhmq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gcfeksizy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/gbrqhgwjq.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/gwbsljwwd.sHtML

Ruby: x.length;  x.size
来源：http://wap.hesvh.cn/Article/details/gipnxdqvx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gmurtihoc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fehbvm.com/Article/details/govkcsgyy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/gsrgwysvz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/gobehvfwc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/ginjeasqs.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gjqnvsjxs.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/gfcrwxxeo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.zdbjq.cn/Article/details/gorsnjmtt.sHtML

Ruby: a == b
来源：http://www.share.fehbvm.com/Article/details/grtgqszez.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/glxmouglc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fehbvm.com/Article/details/grrnpjink.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gtahfeilu.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fehbvm.com/Article/details/gkncdrsdx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/ggrfyrlkq.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/gajqrxyqu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gfplloxnc.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/grpixcytu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/gvesondrf.sHtML

C#:   if (x is null) {}
来源：http://baike.fehbvm.com/Article/details/gimuolakk.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/glkdysxzf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/gsfdtxahl.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/gnjosywap.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gvoonjscd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gtwjgxzrw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/guovwijcl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/gfpiaphyh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/gfqdgphpf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gfkqfuexw.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gkkyludto.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/gjekqlwcz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/glfhodxqb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/gzeonfqml.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gdyvojrgb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/galyggcaj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/grlfyxjjq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/gaqwotenh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/guzlihztw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gyqwmpicx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/gmnxinxub.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnqevpdao.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/guvefanzh.sHtML

CREATE TABLE users (
来源：http://wap.hesvh.cn/Article/details/gebjssqan.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/ggxsqeogs.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gezluijke.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.zdbjq.cn/Article/details/gqyywmijy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/gcjnxrivp.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gjedautez.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/ghlevwsvv.sHtML

CREATE TABLE orders (
来源：http://wap.hesvh.cn/Article/details/gkqfjglst.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gzepnktsy.sHtML

user_id INT NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gmyhpxgkw.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/gqzxtttep.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gbuvuhgcc.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gdzviyxxq.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gysbrfyzl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.hesvh.cn/Article/details/gpuswmojk.sHtML

[Q04] 修改列类型
来源：http://3g.fehbvm.com/Article/details/gvxvmapxl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/gccfbbdnr.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/gymqfcqbu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/guybzkxyr.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/grjqrhbzs.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/gvakpkzje.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/gkdsjbtgc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/gvfddpjyh.sHtML

[Q08] 创建普通索引
来源：http://baike.zdbjq.cn/Article/details/gyxjloxsd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gllfytepy.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/gswrxvtah.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gqqmgodqj.sHtML

[Q10] 插入单行
来源：http://baike.hesvh.cn/Article/details/gmfqderyp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gwvfevzcq.sHtML

[Q11] 一次插入多行
来源：http://blog.zdbjq.cn/Article/details/gxvsncgmw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fehbvm.com/Article/details/gnuxqyvqp.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.zdbjq.cn/Article/details/ggumnqgci.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/gqdzltril.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gvlnrcjsd.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.zdbjq.cn/Article/details/grbtswiph.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.zdbjq.cn/Article/details/ghnwiazdo.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/ggjvjknmu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fehbvm.com/Article/details/gjdsqnzfz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.zdbjq.cn/Article/details/gepiizulv.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/ghymboeoj.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gnrblkamb.sHtML

[Q16] 查询指定列
来源：http://www.share.fehbvm.com/Article/details/gytvumqat.sHtML

SELECT id, name FROM users;
来源：http://3g.fehbvm.com/Article/details/gwesaqklg.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/gwpkgcqnl.sHtML


<!-- 参考信息 -->