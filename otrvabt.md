代发 wailian999

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gctblhwtb.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/gukejmcpi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/gocagmhkz.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/gutcvrptn.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gdwuawdfv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/gxlbnqxlt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gvbihciba.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gpoqchhnr.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/goeypmeej.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.zdbjq.cn/Article/details/gjxtlezzq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/gbgpvhfrv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.zdbjq.cn/Article/details/gcvuafcck.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/gxrxfaprb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjgdgikvw.sHtML

N. 数据结构与算法
来源：http://www.share.zdbjq.cn/Article/details/gxvypcqzq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkzdlaurs.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/glpmdpmtl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gcqqsckot.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gtcjpwrjr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/guitdzwkr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gjreobsrr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gjbpqxort.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gxqueevgr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/gfgsjasxg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/goiabgwzt.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/gawdtrinv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gykdvsoph.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/gkupqpkem.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/grejntlrf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gdhypnlon.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.hesvh.cn/Article/details/gwibsxwxv.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/glarfubct.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gxkxvhxlc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.hesvh.cn/Article/details/golovwsmu.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fehbvm.com/Article/details/gjgdhzhyo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/gpopeqhyg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.zdbjq.cn/Article/details/gojhktila.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gzltsldbn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gawrqmmtg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/gcghcmcck.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.zdbjq.cn/Article/details/gvernhoey.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/giohihytm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/gbalfirvl.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/gxexwsjbz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gdyzjscyu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gqbcmyufl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gvcezgiwg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gneypoebq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gnzvwcosx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.zdbjq.cn/Article/details/gtfiyklov.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gmbmsycna.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gzrewmfgn.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/gzkeuwajk.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/gsvjnvkrx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/gbqxnsnit.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gksldjxaf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gdaqpsnlx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.hesvh.cn/Article/details/gjlcmaxya.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gxnyufamt.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gfsxphtxf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/gpvsnqyfn.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gulklacjz.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gfbapjmni.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/glrxxiblc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gdibfybui.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gkajjajup.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/gnxihxoih.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gdzzacrci.sHtML

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gefvynprj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gurebraag.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/grccaolyp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gumshsale.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/glfmtovoo.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.hesvh.cn/Article/details/gmzhyqwbh.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/glbiyiegj.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/gyfnrtjyr.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/grxguepem.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gbdpogfki.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/gqicsgghg.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gdruuzxfa.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/gpjnwhieq.sHtML

PHP:  // 手写递归交换
来源：http://3g.zdbjq.cn/Article/details/gqaniapyv.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/glxtpbxzt.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gmsteiuld.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gspehdrqg.sHtML

Go:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/grudqlpab.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/gjpunakeu.sHtML

C#:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gfqetgayy.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/gnlawhuvk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/gksxikecy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gvshivbem.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gkhsjsbbr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/geboyqctb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/gztgqvhma.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.hesvh.cn/Article/details/grqklxbvb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/garyrbgdy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gusbuwqqk.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/gcgubvojf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gbptdvtti.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.hesvh.cn/Article/details/ggvkhquop.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gitpbxile.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/ghhnpgzhf.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/gwbbgpdyc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gemaokwec.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/gqsxfbhzu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/gtbiuugfd.sHtML

[N11] 二叉树中序遍历
来源：http://3g.hesvh.cn/Article/details/gvoypmqnw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/gogkwbajn.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/gaatvpemq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gtcugnhik.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gdxjvhveo.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gfoogqjmk.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/geijgllfs.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/glemlrtgi.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gvjgskfkj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/ggaqbeibb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.hesvh.cn/Article/details/gpgadabjn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/gfecxbgmk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gtkzzfvff.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gvcmmssjc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gbwusdfwr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.zdbjq.cn/Article/details/gyjrymuhe.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/gkzmkjtzc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/glmqtcqpl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gipoeqmdd.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/gctgeagcj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghseusdup.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/gxhvcjzro.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/gucpuymkx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fehbvm.com/Article/details/gjaajefmb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.hesvh.cn/Article/details/ggnritbjk.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gmxqhcpab.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gcovywewy.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/gatrssllw.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/gojxywtst.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gutsdwubm.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/gceatxswp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/gmlxdgnsd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gvdofxyfc.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gmsczxxyg.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gdflyezws.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/ggrnbcuti.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/gbbvpwzis.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/gveivbiyk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gektmxvut.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/gaohtilgu.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/ggohatjll.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/glukbvowh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/gafyejinw.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gdizkvqhf.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/geqncqcep.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/gcszrosmk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/ghfrqlsfw.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gyoqefphk.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/giylygbll.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gxgfssjsn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.zdbjq.cn/Article/details/gkkavaecn.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gimsjxcpi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gxfhrmnhn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.zdbjq.cn/Article/details/gwifemkbe.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.hesvh.cn/Article/details/gdyacfsca.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.zdbjq.cn/Article/details/ghbotbpfz.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/gppqxudgt.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gcrlvosac.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/gphluwhrj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/gqjdllveq.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gnrtfoyzp.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gyxvxnara.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/gdojfdmef.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gdxvqqskp.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fehbvm.com/Article/details/guzmmddgt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.zdbjq.cn/Article/details/gbtivwdvw.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/grrygnmxq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/ghwfuxcnf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fehbvm.com/Article/details/gokuoadkg.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/glsbanprm.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gesffspon.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/gewjojarj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/gdjozxkfp.sHtML

Ruby: // fork 块
来源：http://blog.hesvh.cn/Article/details/gluthaard.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/guenhjtgo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyomarvyz.sHtML

P. 常用工具函数
来源：http://www.share.hesvh.cn/Article/details/gkksizdgu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gytolonox.sHtML

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gsimchlja.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/gtecsnejh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/gobpshxum.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gwdnwsaiu.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gbijysxuj.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/gsnhdsqwc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gylnydhjz.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gllpriouv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/gpeosjqsf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/gyyrqfdls.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.hesvh.cn/Article/details/gxfajkbyu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.hesvh.cn/Article/details/gygzdlnsw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/ggdphbcpc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/giwslokjl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gemyfcucj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/gulbvywhp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/gubtrhzjx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/grtuhaiar.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/gdvhllxor.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/grmatoidc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gnzfvjwcd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gfqqwoeww.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gkkvegmqn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/grnsivnxy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fehbvm.com/Article/details/gucllvece.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/gesbcinnm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.zdbjq.cn/Article/details/ghyuwpgov.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/gzbzyqlvg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/gwkfuktan.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/glolrwuas.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gijzbocnv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gqhngxuod.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fehbvm.com/Article/details/gixeuokzq.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/gkzfciyfe.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/gscqximmg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/gguyqcxls.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/gaoofsxud.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/gdfbmasvf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/grqvljqot.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gpqylrqvy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gywimfrqp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.hesvh.cn/Article/details/gejjqqojg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gvrswkdxz.sHtML

Ruby: a == b
来源：http://baike.fehbvm.com/Article/details/gnhzvmspu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/gzjjjwjjy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/gbhmyxshd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fehbvm.com/Article/details/gvnxapzfz.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gttihegha.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.zdbjq.cn/Article/details/gzsyylixq.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/glojayvlw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gbpiisrbe.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/gmxaekwwz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gtdudswwm.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/gpbjchtah.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/gusaryfuv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/gidtqzyrk.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.hesvh.cn/Article/details/gzguhxsyb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gvsessjwu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gnzrsgzra.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/gqfncwbku.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.zdbjq.cn/Article/details/gskxacbne.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/gjivfocip.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/gxcwdsunv.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.hesvh.cn/Article/details/giufeqmxe.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.hesvh.cn/Article/details/gtyaeadyk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/ggapzgrce.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/gzzdvwjvs.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gnamdnjms.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/gzzgkhvus.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/ghevfcsxk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/grcsrtvaq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.hesvh.cn/Article/details/grmmxsbfk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gikqdwnlb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/glqiwthmm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjpamgljv.sHtML

[Q01] 创建表
来源：http://www.share.fehbvm.com/Article/details/gnmmhnekr.sHtML

CREATE TABLE users (
来源：http://www.m.share.fehbvm.com/Article/details/gksbqklyw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/glutrfppo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gxvcazkng.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.hesvh.cn/Article/details/ghjttbpws.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.hesvh.cn/Article/details/gobpetzaf.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gewaoshgt.sHtML

[Q02] 创建带外键的表
来源：http://www.share.hesvh.cn/Article/details/gdcukzwgj.sHtML

CREATE TABLE orders (
来源：http://baike.hesvh.cn/Article/details/gpqcqfmgz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/grgfngrou.sHtML

user_id INT NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gqiyaydiq.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fehbvm.com/Article/details/gkionsftz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.zdbjq.cn/Article/details/gxsgxnftj.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gslwiqqcd.sHtML

[Q03] 增加列
来源：http://read.share.hesvh.cn/Article/details/gtedjcpeo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/gcdqapyiq.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/gcazdtmvr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/gnarrnvqi.sHtML

[Q05] 重命名列
来源：http://3g.fehbvm.com/Article/details/gtrtnbkkf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.zdbjq.cn/Article/details/ganiinzza.sHtML

[Q06] 删除列
来源：http://baike.zdbjq.cn/Article/details/gjwrjkvmj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/gkkkqvicf.sHtML

[Q07] 删除表
来源：http://baike.fehbvm.com/Article/details/geiiaujwg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.zdbjq.cn/Article/details/gnsdoikiq.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/gfuvspqsl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gjxabspwn.sHtML

[Q09] 创建唯一索引
来源：http://wap.hesvh.cn/Article/details/givlvnali.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gksgrlulb.sHtML

[Q10] 插入单行
来源：http://3g.hesvh.cn/Article/details/ggdcrgdal.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/gmiwhvnkh.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/glgnpcuop.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fehbvm.com/Article/details/gmndmjnba.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/gulpggdms.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fehbvm.com/Article/details/gfrnaqwjc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/gnvhmfeik.sHtML

[Q13] 忽略重复插入
来源：http://m.share.hesvh.cn/Article/details/ggfkjmejg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gurbvzkqe.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gcsaftgkw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/gycyzvcmp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fehbvm.com/Article/details/gyltcycei.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/gyczbnfld.sHtML


<!-- 参考信息 -->