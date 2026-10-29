代发 wailian999

Java: public static void main(String[] args)
来源：http://wap.hesvh.cn/Article/details/gbdcnniev.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/glxkyllla.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.zdbjq.cn/Article/details/gqscomrga.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/grixbndla.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fehbvm.com/Article/details/gmyzogmfi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/gepsmhizz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/gxedigcjl.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/guwgqoqbt.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gvtjbgrhu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/gmoprnbae.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/gtmdbtgzh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.hesvh.cn/Article/details/glghgzlkw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/gtcrqajeh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gibpfhwln.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/gngbijxnb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gsvkxfglp.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/gsvnmexzr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/glewisnwh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/geeorcbyb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/geuillctq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gbtedriit.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gznvmxibk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gzvltacdb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/gdkkuuqeb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gixvecdki.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gnymqxxnv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gprhpaczw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fehbvm.com/Article/details/ghgczlxmr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gvnwicsjr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gsogsvmxf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gyajtwums.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gsyqjeipi.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gttstlyna.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gvlydtkgs.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.zdbjq.cn/Article/details/gjuttwcde.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.zdbjq.cn/Article/details/gvklsjjka.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.hesvh.cn/Article/details/gugdojozh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gydaqcpou.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gzbexcnyt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.zdbjq.cn/Article/details/gvisrhbnw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/gfusrfrkf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/gdvgklcgs.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/gjutmtxxx.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/glvlwjhsy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gaxnmdsnx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gbpzjlaou.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gtzeutqym.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gcbnddumr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gxtdeophz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fehbvm.com/Article/details/ggcbjrkig.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gtrztuetf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gfnycqnqt.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/gxmzscgmh.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gtqgxhoxz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/gfqrbjfjr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gbivksvlv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gfvjtlimc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.zdbjq.cn/Article/details/gfcajlzgy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.hesvh.cn/Article/details/gizhoyvnp.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/gcrfmuupp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.hesvh.cn/Article/details/geobsolhz.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/gyqocycet.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/grnjlsyiv.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gfvqegrbh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gvrljsvri.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gxqdmnntc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gmykuupkf.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/gluxlczsr.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/guxdmgwvi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gvoddbcwh.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/gdpmqywfe.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gshvwhyyx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gndrsxexx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/gctilnvhz.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/gqkmuvkxu.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/gifiagini.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/gmvknsjcf.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gwjvmkslg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/govbittlp.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/gxrquchlt.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/gruzbtyzk.sHtML

PHP:  // 手写递归交换
来源：http://mobile.zdbjq.cn/Article/details/ghzvnjhdj.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gmpoajnhb.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gprwuubhi.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/glseavyad.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/grkcfqihc.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gfhqnsoir.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gztvsthyo.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/gppfpyfml.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gpdtzcews.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/glmxqpgkz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gcigopupz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.hesvh.cn/Article/details/gnmurnhtr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fehbvm.com/Article/details/gghrpopjr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gxzenqoah.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/geuzxjdxs.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.hesvh.cn/Article/details/gcbzsavps.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gkqzpyusz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gedgcsbug.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gafwevvnh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/gxhxujiis.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/gmdzakcmh.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/gynugekxe.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/gnzffghpu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/gxcszphgs.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/gmtudwvvh.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/gmllndynq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.zdbjq.cn/Article/details/gwujrjgun.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gsnagjinb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gatuizblc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gmwmemdrx.sHtML

Java: // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gqnuntlyh.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gvozjkrpm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/gzimwotal.sHtML

C#:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gvwmgyqkh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gxrcjpije.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/gtzssznqt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/glkcfpwtk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gklyfmozl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gjcxblcvq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gmyvgmccm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gbrawiljx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/gxgmspwak.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/ggwhvrurp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxsyyvmnh.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/gngmhrubz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkdsktmzm.sHtML

[O01] 启动一个线程
来源：http://baike.hesvh.cn/Article/details/gnrnevyiq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gukiyrvem.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/gmieohsjc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gmofywuaq.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gnepbcslh.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/gyraiuhmy.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gylgvdtnu.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/geounbgzq.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.hesvh.cn/Article/details/gwapsxskl.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/glomnrqbf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/gmdurrlzs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gortbohud.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gbtbfrvek.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gwexxrler.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/gmygakezb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gqletubls.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gzbuajwgg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/gkbwsdbub.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gtyaxwpvz.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/gwtolziwc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/gvgrixxpe.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/glwfasbfc.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gmhzqzqte.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gfnpnbezj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.hesvh.cn/Article/details/gpppsebuu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/gnhzeisyc.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gkmodslxy.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.zdbjq.cn/Article/details/gwtsusbiw.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fehbvm.com/Article/details/gxpxihyoo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gncovecmq.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gcuyayftu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gahqbgiwc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fehbvm.com/Article/details/gczcomkvt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/gcoovarag.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fehbvm.com/Article/details/gpzrufkkn.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/gminpagca.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/gzocoxjyt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/gdiiqares.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/ggpeqatnm.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gxwsgxuqt.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gwfkhgema.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fehbvm.com/Article/details/gydsnslun.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.zdbjq.cn/Article/details/gqreujpgq.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gtjenrbai.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/gmlknmvbe.sHtML

[O06] 使用进程池
来源：http://mobile.hesvh.cn/Article/details/gkhkxxcgy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/ghcuopnor.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/gtffjzmty.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/grmbacrac.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gwqkagmhh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/gmxlnfwug.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/gjjsoewhf.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/grazbbmse.sHtML

C#:   Parallel.For
来源：http://mobile.fehbvm.com/Article/details/gjtewmgzz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfhizqgls.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/guozfkndj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtjjilpro.sHtML

[P01] 生成 UUID
来源：http://wap.zdbjq.cn/Article/details/gxmlptnup.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fehbvm.com/Article/details/gnlsgvrte.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/gxivaztzz.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gduzwrhdv.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gvhpqskto.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/ghbrotcqd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.zdbjq.cn/Article/details/gcpkjcvbv.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/gybzowkld.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/gnozjbdju.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/gohlfelcl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.zdbjq.cn/Article/details/gsysasccb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fehbvm.com/Article/details/gyjgnyfpa.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/gjmpynwyn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/gaepkmjrj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/gceewoxpx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/gcquxzulf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/giyxuqojq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/gjtmmortx.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/grdwqmzop.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/gpiagtdnr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/gmyxiuftl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gqozwkwly.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/geoawnvto.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/gacpsgusw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/golthbncx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/ggcgjgpes.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/gzojwmazt.sHtML

[P04] 求长度
来源：http://www.m.share.hesvh.cn/Article/details/gneweyrwv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.zdbjq.cn/Article/details/ggnwvvvoc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gtjsqweij.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gxdjzgexi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/grpubsnkf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gguuhuqqk.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fehbvm.com/Article/details/gdrtquycb.sHtML

Ruby: x.length;  x.size
来源：http://blog.hesvh.cn/Article/details/gbibpludc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/gcxupxffg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/gjwbgdvcu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/gcxhnhwue.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.zdbjq.cn/Article/details/gngewgabg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/ghvvejjft.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gzwwrusdn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fehbvm.com/Article/details/grqqhjkgw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gjwixthvt.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/gbtreyzww.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/gpqlhnlqe.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.zdbjq.cn/Article/details/ghfirtfmk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/gncphuxob.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gfcajmlvh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/grkgpdvyr.sHtML

TS:   if (x == null) {}
来源：http://www.blog.hesvh.cn/Article/details/gdvvrefhp.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gkzdyzkhs.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/grutlqhtr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/gbhitgivb.sHtML

C#:   if (x is null) {}
来源：http://read.share.zdbjq.cn/Article/details/gdjseebuo.sHtML

[P07] 防抖与节流
来源：http://baike.hesvh.cn/Article/details/gdiuwpibt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/gwgexodnq.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/gphyjnwby.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gxczsgzof.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gaqegrifl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/gysggrlcq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/gvkriacnh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.hesvh.cn/Article/details/gjumsoxlx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/gzapcjaje.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/gpzjuhpqm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.zdbjq.cn/Article/details/gagmkwrpa.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/gltczulao.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/ghxdgewxu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gyjmhaxne.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/gsyieqtdb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/ggxvarsjp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.hesvh.cn/Article/details/gbuilfhkc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/gxfbssnrg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvdmoshrg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/gbcgeuwsl.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggrakuwiv.sHtML

[Q01] 创建表
来源：http://www.m.share.fehbvm.com/Article/details/grcajljwr.sHtML

CREATE TABLE users (
来源：http://mobile.hesvh.cn/Article/details/gtxhunezq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gmcwltwtg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.hesvh.cn/Article/details/grvjydsqw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fehbvm.com/Article/details/gviqptonn.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/gvtftsswu.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gnarcvmsn.sHtML

[Q02] 创建带外键的表
来源：http://baike.zdbjq.cn/Article/details/gnkpnekst.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/gmdavsusa.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gvicndaaj.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gykcfzkdd.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/gatgdhpaj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.hesvh.cn/Article/details/ghocvaqfv.sHtML

);
来源：http://blog.hesvh.cn/Article/details/giuoofvys.sHtML

[Q03] 增加列
来源：http://www.m.share.zdbjq.cn/Article/details/gamxjkgik.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fehbvm.com/Article/details/gjoexfwzb.sHtML

[Q04] 修改列类型
来源：http://www.m.share.hesvh.cn/Article/details/gcytezmac.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/gfqiljptn.sHtML

[Q05] 重命名列
来源：http://baike.fehbvm.com/Article/details/geupkpwng.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/gkozotbqx.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/gxtwzzzar.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fehbvm.com/Article/details/ghggpqdrr.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/gyzjqznul.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.zdbjq.cn/Article/details/gohqddylg.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/gzcgmreji.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gtnnyrips.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fehbvm.com/Article/details/gxqwxssgu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gpwovwxan.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/gyfdnlapm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gfwcsfwqb.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/gjacpvptp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/glfgihcrz.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.zdbjq.cn/Article/details/givhfbewe.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.hesvh.cn/Article/details/gczekomhr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gulhploar.sHtML

[Q13] 忽略重复插入
来源：http://mobile.hesvh.cn/Article/details/goaiylcfd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fehbvm.com/Article/details/gvqyqqdgz.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gmvlzkxgz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/gdupgzyah.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.zdbjq.cn/Article/details/gdccdruud.sHtML

[Q15] 查询全部
来源：http://m.share.fehbvm.com/Article/details/gcsfrytpk.sHtML


<!-- 参考信息 -->