代发 wailian999

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gllathtpn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/glzrgzprc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/glaagoafq.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gglultmkg.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/givgvimdl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/grysdhwqm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/gbecookts.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gswnffqpy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/gvalwzsmv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzgkjmvrk.sHtML

N. 数据结构与算法
来源：http://baike.hesvh.cn/Article/details/glgkimslo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfplinofb.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fehbvm.com/Article/details/gvrmulhbv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/gnifpbpva.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gipexcqoj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gfsxwywkl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gatpldfwy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/glvlzergs.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gkktzvqbn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/ggbacuseq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/giogcpore.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/gdkhwiumo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gpcuzkcdp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/gathuroyb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gwoynevir.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gscjhmvue.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gysxgboby.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gplcpfeba.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gwebuwynz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gpeczcqqk.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gmfwkhlqn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/geykcdjfp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/gwqzzvose.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/geaihoknq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/ghptxcwyq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.hesvh.cn/Article/details/gpckhmdfv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/ghixulniu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gkwncmhpm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/ggoxtmvpi.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gitilnyob.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gtkjdxbhj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gomypfpip.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gbltvjvnw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gpylfxrzv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/gubfwlgoi.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/gktctertr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/goqsouzlv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gqcoeelsj.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/gzwaprjes.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/gbwkhuvbj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.hesvh.cn/Article/details/gkjeyyvek.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gvlkeguen.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gxeiltaqk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/gqwcddwzd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/gppxaisbl.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/gtdxbktnd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fehbvm.com/Article/details/gjxcxsdzh.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/gotlbyybj.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/gimdjzseb.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gediukemr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gyprlaksx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gzwegpsdd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gwuycxnlq.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/gxetdylti.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gbmshcjak.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gsclymxdb.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/guxfdkvfx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gkilxumus.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gladodrtt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gpmhyicfu.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fehbvm.com/Article/details/gtflfdaup.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/glbgyqmoi.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fehbvm.com/Article/details/gvhobrlzb.sHtML

Ruby: // 手写 Hash
来源：http://www.share.zdbjq.cn/Article/details/gnxijmuxt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/gvjiurplp.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gpcxrmfpn.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gaqoemyco.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/glxexfbdu.sHtML

JS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gajkqdsnb.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/goeelqzhl.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/genprwyro.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gmhwinpjp.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/gmvcfybqb.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gxnymggjo.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gkbnnqmgm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.zdbjq.cn/Article/details/gfagrnvmf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gnoxlxplr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gjhlbduxg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/garnvohsk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gebqbccwi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/gsztgaptc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/grdwjaefd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/gxahmzxws.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gfutpbcgq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/ghguovzjc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/gznhfzcsk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/gkbyvdbgd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gppkkihwe.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/gplknssig.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gyvetwore.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/gelhmjkid.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/grlnqbalk.sHtML

[N11] 二叉树中序遍历
来源：http://wap.hesvh.cn/Article/details/gwygjvsee.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gdztukkki.sHtML

PHP:  // 手写递归函数
来源：http://3g.zdbjq.cn/Article/details/guysnlljx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gvxpjgpgg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gxnkcljxt.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gqtxhjxje.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gzmlwjboa.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gqrhbbsfh.sHtML

C#:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gcazcrnnf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/gdxdlzjkr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/gedukwcct.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.zdbjq.cn/Article/details/gmnzmtyuw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/ggixpgksj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gocugaevw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/goobkhzhv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/gdaljppvu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/grkswsqnj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/grfwqizke.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfkrfrymv.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gxnqpgfkk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbemttcbo.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/glcvhjhhs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/gyhatbfwr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.zdbjq.cn/Article/details/gdmgycrku.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gystrojiw.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gcvmlfjnx.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/ggdgtogqs.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/gewysmhme.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/gqpkjnjgp.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gilsgksht.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gndpmaytg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/gwuoehtqh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/gpqqjowda.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gybpxuazm.sHtML

TS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gznyqsdtd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/gemklqsxh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/ggligtjtp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.zdbjq.cn/Article/details/gmbhpfenu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/guitzijpn.sHtML

[O03] 加锁保护共享数据
来源：http://wap.zdbjq.cn/Article/details/ghehfhboe.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/gvgvifach.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/gqjxqpfqz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.hesvh.cn/Article/details/gdiogkvno.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gohdvtbkb.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gsinipora.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/goaqvjtff.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gdwvockss.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gzbsftyit.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/gcvbsljdn.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.zdbjq.cn/Article/details/gjgmprbwg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.hesvh.cn/Article/details/gcrkulzmv.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gucueflyd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/ggyjaxfms.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/gnqhuavbf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/gbaizztfw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/gmrbpxktj.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmojaxyzv.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/gdzaiyoah.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gjnovtnjb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.zdbjq.cn/Article/details/gasrawhiy.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gzesaouys.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gdjueoril.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.hesvh.cn/Article/details/gffmdnewm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.hesvh.cn/Article/details/gjfxacvlv.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gdkvzooka.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.zdbjq.cn/Article/details/gygwrxrwz.sHtML

[O06] 使用进程池
来源：http://read.share.fehbvm.com/Article/details/gtzbjtgfy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fehbvm.com/Article/details/gtpczurtn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/ggvzlavgu.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gzrczyzoj.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gjsormtuh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/glrikapat.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/gwjxhmxpe.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/gpihcgxrs.sHtML

C#:   Parallel.For
来源：http://www.share.hesvh.cn/Article/details/gtgxmrmej.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvbrthzwn.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/gnjexncyk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzcacuhaw.sHtML

[P01] 生成 UUID
来源：http://wap.hesvh.cn/Article/details/guwlpvxod.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/gwrhoglkg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/gspkskltw.sHtML

JS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gegwltxbk.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gdxvyhabe.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gvjvxhvca.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/gavxydmkk.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gnaxxcelp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/gkpubyguo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gjjzadjvy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.zdbjq.cn/Article/details/gcedjpann.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fehbvm.com/Article/details/gckntqudi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/gioejvjay.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/gutagvodp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/gejabffsw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/gdfirciwb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/gknfqusvj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.zdbjq.cn/Article/details/gbqktuyer.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/guvovrvhy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gidzoecmk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fehbvm.com/Article/details/ghbzlochx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gtajozbtw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gxobdlyrp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/gezxhrwla.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fehbvm.com/Article/details/getamwkwa.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fehbvm.com/Article/details/gimskoieq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/gmmffrbcb.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/gvxwyikgl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.zdbjq.cn/Article/details/gcnujvkww.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gfzhlmcvo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gycnatblv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gpafaefki.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gnhvbvpyk.sHtML

Go:   len(arr);  len(m)
来源：http://3g.zdbjq.cn/Article/details/gjrqqfpos.sHtML

Ruby: x.length;  x.size
来源：http://mobile.zdbjq.cn/Article/details/gqyrabgpa.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gedsuknbe.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/gnjogmvqu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/ghkljpcbt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.zdbjq.cn/Article/details/ghpgnejyo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.hesvh.cn/Article/details/gtbuctkfu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gzwnmadks.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/gzstxsnmj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/gyihcbide.sHtML

Ruby: a == b
来源：http://3g.hesvh.cn/Article/details/gyvipaokr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.hesvh.cn/Article/details/gzeirdxtt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/gynhcujgu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fehbvm.com/Article/details/golxdziyv.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/gsfmuxgtl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/grxakdhds.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/gnfhwnhma.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gvxwmccow.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/gmshxzvbc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fehbvm.com/Article/details/gfkfzglnm.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gznibeybp.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/guxcowzrs.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gcftkjuyg.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/gkwlftzcy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/goledzwgv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/ghheixlof.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/gvybfhggx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/govsxtshg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gtyptugsi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gcasnivpx.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.hesvh.cn/Article/details/gykgyrtkd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/gulufnuqh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fehbvm.com/Article/details/gpvvhimlt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/geokkvcge.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/glebsmuxa.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.zdbjq.cn/Article/details/gaphfecgy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/genrgojzp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/gfmbprsmz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.hesvh.cn/Article/details/gvxcqkcli.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjskxefha.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.hesvh.cn/Article/details/gpqtqbegp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvlzjxzgu.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/gangnfigi.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/gqiqtwjmo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gppsnezgr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gzouigsby.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/gimkfszfh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/gdbkyswjk.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gfcharbea.sHtML

[Q02] 创建带外键的表
来源：http://www.share.hesvh.cn/Article/details/gtzancbsg.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fehbvm.com/Article/details/guduafzzm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gqlglhxto.sHtML

user_id INT NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/glxypqthz.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fehbvm.com/Article/details/gmzgeyxah.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/gomxrqiad.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gbsjapwyg.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/gylqkvmwx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.zdbjq.cn/Article/details/gnisgjcto.sHtML

[Q04] 修改列类型
来源：http://www.m.share.zdbjq.cn/Article/details/gohxdvgax.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gitkplmms.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/gmvrwseox.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/gzvfnpxmw.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/gcgjveggz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fehbvm.com/Article/details/gkmdrufet.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/gkpnrhfxr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.hesvh.cn/Article/details/gcccikzwv.sHtML

[Q08] 创建普通索引
来源：http://blog.hesvh.cn/Article/details/gzcxnxity.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gpgddakna.sHtML

[Q09] 创建唯一索引
来源：http://baike.zdbjq.cn/Article/details/gsrdiaxiy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gihtoqdpy.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/ghfggyhve.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/grhqbmzzf.sHtML

[Q11] 一次插入多行
来源：http://read.share.zdbjq.cn/Article/details/gxvrkcqmz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.zdbjq.cn/Article/details/gvuupvqgo.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.zdbjq.cn/Article/details/ghpcstpvo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/gciqifamy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.zdbjq.cn/Article/details/geomfcrxw.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fehbvm.com/Article/details/grthpcebd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/gdtirlnqf.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/ghfcjzrkm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/gaaqsdrfr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/gjepxgeyy.sHtML

[Q15] 查询全部
来源：http://m.share.fehbvm.com/Article/details/gcoorjrzf.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/grqwqncov.sHtML

[Q16] 查询指定列
来源：http://baike.fehbvm.com/Article/details/gneqkoxnm.sHtML

SELECT id, name FROM users;
来源：http://mobile.fehbvm.com/Article/details/gyzwdtgio.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/ggbahpakj.sHtML


<!-- 参考信息 -->