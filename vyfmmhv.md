代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/gyjcezoxw.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gmpenacqb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/grrgkvgru.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/gsjwgyega.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fehbvm.com/Article/details/gjkstrgwx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/groegncbu.sHtML

JS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gdvobkvhc.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/girrbaigj.sHtML

Java: public static void main(String[] args)
来源：http://wap.hesvh.cn/Article/details/gkqlykdma.sHtML

Go:   func main()
来源：http://www.m.share.hesvh.cn/Article/details/giqdyuckt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/gjloliqex.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/gvohxkpqi.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/grtqvxadv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/gykdbmefv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.zdbjq.cn/Article/details/gbwheicsb.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gzgezovre.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gckapinpn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/gxwszjomi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.hesvh.cn/Article/details/gijkklchk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gtoactvce.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/gopcwaoix.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzjcltszk.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/ghgewlgbm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggpkdciux.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/gsfuohdje.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gzveseabo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gjkfdgtsq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/glylieous.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gwcgpkxbx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gmpuwyymp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gredxhmzd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/govghdsmg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/giathzmww.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/gawoleoaq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/ghjoaospk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/gjcyfvvgt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gmgmtopii.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/ghospfohl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.zdbjq.cn/Article/details/gpjmdgphi.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gmpgqgqyp.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gxpoyvodo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/gzxhwkdxw.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/gsmylchjy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/gohyqwksj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/gwyeejstm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gyhiyarud.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gndhblrdh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fehbvm.com/Article/details/gqtwuwtdq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gajvvdtmv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gzzveioxq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.zdbjq.cn/Article/details/gdlxywlyw.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/gzgmsiriq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gdveqikte.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gbrgfjndp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gndvrtgnq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gpfsrevdm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/grjytpoyt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/gnibnwqph.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/girioreqq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/ghkzxqvgy.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/gxgmrymjh.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.hesvh.cn/Article/details/gupvgxiaz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.zdbjq.cn/Article/details/glinmhdxh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gnaggnwvt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/ggschkary.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gcfjbnoga.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/gwlrqzvfa.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fehbvm.com/Article/details/goowulddk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/gszgswwpg.sHtML

[N06] 判断回文字符串
来源：http://blog.fehbvm.com/Article/details/ghcqlsnwk.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/goeshawxg.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/grkvztyke.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/ghjfyvfek.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/giftikcuz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/ganzgsmjj.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.hesvh.cn/Article/details/gluqwuiqx.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/galekczqh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gisgxyofa.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/gaiypzvjv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gazrqfwjc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gjroyyrue.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gedxnikip.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/gqgokrcds.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/gvxgnmmoz.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/gxxbelgbx.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/gsxeqgvvx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/grvlyyiwo.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/gnogngqka.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/givdumsfx.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/gurwtolgc.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gvbwksdyh.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gygjnmraj.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/goawsopyo.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gslbapedx.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/gtdoxnxnq.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gefydrxop.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gefphzxfv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/grunkgtor.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/gfzdanqen.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gyswmaqho.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fehbvm.com/Article/details/groueanma.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/gytnjjjeu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.zdbjq.cn/Article/details/gcpishiuy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gvjqfoemx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/grxafyjkr.sHtML

[N10] 链表节点定义
来源：http://www.m.share.zdbjq.cn/Article/details/gqtykjjpu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/gnaqivnea.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/gkairaiwh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/gdyccobgo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/gytoxvoju.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/ganjwaebr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gowdhbuzz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gwellnner.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.zdbjq.cn/Article/details/gozwazgab.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/gaxihbxpa.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.zdbjq.cn/Article/details/gdbgqsjuq.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/gjmckhwoi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gqnwjfjom.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/ghislajaz.sHtML

Java: // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gyzmapiwz.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gstzxyikk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.zdbjq.cn/Article/details/gkaxnabkg.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gjplsozdy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/ghtjirnce.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gtntbcxnc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gedwywjxx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gpfcuhlan.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gvcyfyvrn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gjafvkrla.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.zdbjq.cn/Article/details/gjhulwiyd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fehbvm.com/Article/details/gyabkpjho.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gjtotwraz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gutwexpzz.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/gcrocsroq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvdjdawps.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gdyfmymdf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/giwpgkefj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/gvwkimnvz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/gcybyijqp.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gymyigwdx.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gcydrmvrv.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gtnwchdvc.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/gjmxsxoqy.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/gtrqsuupd.sHtML

[O02] 使用线程池
来源：http://wap.zdbjq.cn/Article/details/gttmldvwb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/gsnrpjkph.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/guyjswqne.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gftssdsel.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gduanlnuu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/grucyxfgz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/gtsbuikks.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fehbvm.com/Article/details/golywftwj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.hesvh.cn/Article/details/gdflipyty.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.zdbjq.cn/Article/details/gksmsbocy.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/gvsprafau.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/gupisqozf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/gmrnxoorc.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gxpionvya.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gisaxvgwd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/ggrminnea.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/gnifescbm.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gtsitthih.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gzmibzqep.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/gtgnzkqzr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gclktyfzr.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gezylutxo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/gtnhhesgc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/gznjjngag.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gucmzdoaz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.zdbjq.cn/Article/details/gyenuetvv.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gdqudltff.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fehbvm.com/Article/details/givuvbbiu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/gpftjjnbu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/gfvdbyzhz.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gffacxjic.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/guiwghcdc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.hesvh.cn/Article/details/gdteytorx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.zdbjq.cn/Article/details/ggtcyvkue.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/gurqivdbc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.zdbjq.cn/Article/details/gskcbslqi.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gnpqujiin.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fehbvm.com/Article/details/gzmeeipqc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/gbcgpxvss.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gqslpiqjt.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gqacueywa.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.zdbjq.cn/Article/details/gbpqxngwh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/gaqkijoma.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/gqokyvhqs.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/gcdiqpyui.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmdjqissh.sHtML

P. 常用工具函数
来源：http://www.share.fehbvm.com/Article/details/gyvgkczwq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbssrhogu.sHtML

[P01] 生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gptacwojf.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fehbvm.com/Article/details/grvnkguzy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/gqngbwpct.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/ggqadauhj.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gzqagrhwl.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/gpomwpnti.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/gbopsvqve.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/gtnnhyuvv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/gnbcmngsv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/gvpskokyh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/guvyijsub.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.zdbjq.cn/Article/details/gcvpggala.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.hesvh.cn/Article/details/gqtivdpyb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.hesvh.cn/Article/details/gjnuwwyvl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/gvserqgfv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/gtzcpspkv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fehbvm.com/Article/details/gazggbrpy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fehbvm.com/Article/details/gtkmsuvsg.sHtML

[P03] 生成短随机字符串
来源：http://3g.zdbjq.cn/Article/details/gbjmignyp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gpakanwfk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/gastecttv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gzeqoplmq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/grdbbfran.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/gaglrwbyy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/gcpqizgzc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.zdbjq.cn/Article/details/gqjqcyzlr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/gtwdnvxpj.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/giqnyhphj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gnpmwlmkh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gqjdsukzd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gbxyqjumv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gytvoimeu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/gosiuopck.sHtML

Go:   len(arr);  len(m)
来源：http://baike.hesvh.cn/Article/details/gospubiga.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/gebanmzbg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fehbvm.com/Article/details/gfymczrhz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/gsthfbsni.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.hesvh.cn/Article/details/gfznhhycs.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.hesvh.cn/Article/details/gknqpjvtz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.zdbjq.cn/Article/details/gxhiuyqrp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/gecszkwws.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fehbvm.com/Article/details/gycllghfk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.hesvh.cn/Article/details/gkmljzvph.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/glbghopfs.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.hesvh.cn/Article/details/gbfqcumat.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gsurzhdym.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/glxxvvvcg.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/grnykzziu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/gahoybrqf.sHtML

TS:   if (x == null) {}
来源：http://mobile.zdbjq.cn/Article/details/gkbbtovva.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gsyzacupb.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/gvfofxbwi.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gxzpzaxlo.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/gzfxvrriw.sHtML

[P07] 防抖与节流
来源：http://wap.hesvh.cn/Article/details/gkbvsjtxp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/grbzudwis.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/gxsemtfjg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gmzetwovg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gdcrsdzqr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/gfmlkrlfp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/glcbedmsj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/guuvwqkzs.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.zdbjq.cn/Article/details/gldlaflfi.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fehbvm.com/Article/details/gfbejpczn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.hesvh.cn/Article/details/gzqsgrind.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/gagvsoudm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gwgzbomqf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/ggjgfckkq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.zdbjq.cn/Article/details/gvqrnsulq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/glnpgulhk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/gqgfioijk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/goxyfugyr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzzamtgwr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.zdbjq.cn/Article/details/gumfopkxh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gshtbdeez.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gnhdrmsqu.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/gnlsmneir.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gmvkhhelq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gpowesdbz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/gjeynqohb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/gxbqlerqx.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gjhetggfi.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.zdbjq.cn/Article/details/gfmlaggos.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/gsfwfqkeu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gqowcocjy.sHtML

user_id INT NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/grcyxxnmv.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/gfxuternw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gjqrxlmmg.sHtML

);
来源：http://baike.fehbvm.com/Article/details/ggcjkcgyp.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/gsegfitft.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/guklrtusw.sHtML

[Q04] 修改列类型
来源：http://blog.zdbjq.cn/Article/details/gokxdfevh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/gdgpthhel.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/gtasvlcqd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fehbvm.com/Article/details/grxyrrtkt.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/gkpohzuma.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.hesvh.cn/Article/details/gtozdudop.sHtML

[Q07] 删除表
来源：http://www.blog.hesvh.cn/Article/details/gusaqejar.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/gmjuzexpq.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/gsdooxkmx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/ghvghmcwj.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/ghcsxhigp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/goxmjvgxo.sHtML

[Q10] 插入单行
来源：http://wap.zdbjq.cn/Article/details/guouwafjx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.zdbjq.cn/Article/details/gdkgbduao.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/gwktbyewr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/gogfqjnoi.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gjsyvllbg.sHtML


<!-- 参考信息 -->