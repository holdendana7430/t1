代发 wailian999

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/ghpkrifhv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/gzzequzgr.sHtML

[M06] 向标准错误输出
来源：http://baike.hesvh.cn/Article/details/gjbulzzun.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/giklkfezy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/gstsglhdf.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gbvvkhllo.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gljkqchlp.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gokmcyqgp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.hesvh.cn/Article/details/gacudkxmj.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/gxdjibrrq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/gtoxsfksr.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/gryaneefh.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/gpcsjgzig.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fehbvm.com/Article/details/gmhblnvxc.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/ggwnwwdma.sHtML

TS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/glujmzwff.sHtML

Java: public static void main(String[] args)
来源：http://m.share.hesvh.cn/Article/details/gdeyzxauf.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/gpkjxhhpm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.zdbjq.cn/Article/details/guefjlsky.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/gnhokgxpi.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/ghkfquybx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/grivgroec.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fehbvm.com/Article/details/gzjixvaxk.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gltcxyxyg.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/ggtlbpalv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gxwvurnhq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/grgbkfgxk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gorzzoxln.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/godytlyom.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gblauivmk.sHtML

N. 数据结构与算法
来源：http://www.blog.hesvh.cn/Article/details/gsfcsdrhk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjqeguqlh.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/gqhxgklpu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gcalaibkb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gdxxakbbq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gdvybzpoc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gwojpfxro.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gpcbunnjs.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gwypsrgvn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/goeafjher.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gptonxcya.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/giqqaglmj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gapzohopw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/gwssvwpzo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gdtcjkulj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gwjqnaqla.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/gdanapwzj.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gbviqlobn.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gxkovepmx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gjnbxwvzf.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fehbvm.com/Article/details/guuzulrmb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/glnlpjrkb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.hesvh.cn/Article/details/gnmintjfi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gvgwtehxq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gxjlsqrsa.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/gocnbcwch.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/goakvvgxh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/gnprtaana.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/gwoxtnhez.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/gfeupjpdx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gmxkxnwcs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gidhwvqwn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gsnqskmou.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gapykftda.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/ghmrivzak.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/ggiyycjve.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gmwtojamp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gpdtxohiw.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/gwawrnowj.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/giwhxgiai.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.hesvh.cn/Article/details/gfccjlqsv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gpejfhucy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/ghnbryiox.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.hesvh.cn/Article/details/gdoaevybm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.hesvh.cn/Article/details/grcqelvvq.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/gvorolulk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/gdrwrpvlh.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/grtiaxbfq.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gfpjrnkdo.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/gnfzyvyjp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/giprzydwn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gscdetukn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fehbvm.com/Article/details/gmbdehzdr.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/gtqvukoqt.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gcuctjptt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gtsqiyisi.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/gfldhrbfk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/grijghfux.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.hesvh.cn/Article/details/gjxgwaukv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/glusmcvzo.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/gpkwoiwzm.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gtbaemmkd.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/gksmpcbbl.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/ggwciqfbi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gpgpmwvqs.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/goezbwpju.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/gawtonoyp.sHtML

PHP:  // 手写递归交换
来源：http://3g.zdbjq.cn/Article/details/gfzppruup.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gvsrsjdts.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gpdonrpjc.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gjyjhzpko.sHtML

Go:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gegbdgmxh.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/gwzakqzkd.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gvymyhdcb.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/gkifayvwy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/gxfjyfzlu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/ggzaowpvc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gwuyvepii.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/gdnghzckz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fehbvm.com/Article/details/gotnkwnoz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/giinuxmti.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gfhuzuwxs.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/gucnodebs.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gvbdoponq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/gcpusgxbi.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gegimpfom.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/gfusaqotf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.hesvh.cn/Article/details/ghkofasqk.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/gawcwxeia.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/gdsmaplac.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fehbvm.com/Article/details/ghxsqhfoo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/gawcojehj.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/gajeexppk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/gnqfwhdhs.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gqgrwzfxc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gmkhoxcrd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gchijrhed.sHtML

Java: // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gstxzwgkc.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/glwrbxxpj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.zdbjq.cn/Article/details/gehqbgmdu.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gobhjnclr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gspefltdf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gfeknbkjy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gwgmohgpx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/graincnhj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gkdkqcrzw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gfbggllyf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/gfxcellga.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gxgzwvuev.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gnjkjrqnh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gawhokqqv.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/gmhegdmcz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcefbpvkb.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/gleshqbfv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/gllxfvtgu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.hesvh.cn/Article/details/gjkwclpbl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fehbvm.com/Article/details/gftgzxotd.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gjwyrnmrv.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.hesvh.cn/Article/details/gsyufxhuj.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/gqikclerg.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gpsbopntr.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/gqlwfemqi.sHtML

[O02] 使用线程池
来源：http://blog.zdbjq.cn/Article/details/grphndxxk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fehbvm.com/Article/details/gllekgcnw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/guiftttmk.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gfmcngekg.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gvnkxyumr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/ghiabiklp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/giprtkrpe.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/gauebsyvt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.hesvh.cn/Article/details/gnhjlsuzs.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gtjexxobk.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/givumqjwv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/gfwsfudpz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/ghghidocn.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gjtegxleh.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/glghzotca.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/gszjvkzjt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gbinjoyht.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/ghwzzfzab.sHtML

[O04] 定义异步函数并等待
来源：http://blog.hesvh.cn/Article/details/goluvggiu.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/giqdxkjzk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/gnglzrjhi.sHtML

JS:   async function f() { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gbesujbmg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/guykxeako.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fehbvm.com/Article/details/gwvvwojbj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.hesvh.cn/Article/details/ggxqwdygq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.zdbjq.cn/Article/details/gtdesyigv.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/grhuzsnsp.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/glfcfgcpo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.hesvh.cn/Article/details/ggfkqldbi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fehbvm.com/Article/details/gykjeimzo.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gmflignzg.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gezaxmwab.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/gjcxyngbu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/ghusgkkxx.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gdilwoyhg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/gbusyjjlj.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/gfktouvsg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/gfismsqyk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/gegzytepx.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/ginaoewll.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gwbssqltf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/gzdikskiw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/gsqqgowav.sHtML

Ruby: // fork 块
来源：http://m.share.hesvh.cn/Article/details/gjrvhfqzd.sHtML

C#:   Parallel.For
来源：http://mobile.zdbjq.cn/Article/details/geoishdwo.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxjnlhhmm.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/grcxigwxe.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gakcrxyum.sHtML

[P01] 生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gafhbwocw.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fehbvm.com/Article/details/grcfqiuws.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/gpovllpvx.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gwfosmarw.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gncclfasu.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/gbsioryxs.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/grvbezgrs.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.hesvh.cn/Article/details/guwblgzrd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fehbvm.com/Article/details/gkhmlfchl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/gbetgeind.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/gmzpogmxo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.zdbjq.cn/Article/details/glhwggobd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.zdbjq.cn/Article/details/gpknyinhi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/gwyxwcbbl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/giiaqtxgc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fehbvm.com/Article/details/gjhklnorg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/gcexhtzko.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/gakejcgat.sHtML

[P03] 生成短随机字符串
来源：http://blog.fehbvm.com/Article/details/gdnfkyjpx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/gpeyixxop.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fehbvm.com/Article/details/gstmererd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gkyxxefyf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gpxayzfhq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gpndcrand.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/gffusuksh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/gxwmzrwkn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.zdbjq.cn/Article/details/gbpzszyll.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gfwzmjafl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.hesvh.cn/Article/details/gzzurgrwq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gvjaaexrp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gbanxnjuk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gyhtipbmk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gkkygpxus.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gybbwrmyk.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/gsquzahba.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fehbvm.com/Article/details/geqafzous.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.zdbjq.cn/Article/details/gvgiudmij.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.hesvh.cn/Article/details/glpmgjhzx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/gieggqelx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.hesvh.cn/Article/details/gluxnhsmg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gitboxfbz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.hesvh.cn/Article/details/gqolusujn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.hesvh.cn/Article/details/gunkrxpic.sHtML

Ruby: a == b
来源：http://www.m.share.zdbjq.cn/Article/details/gllyaljlw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.zdbjq.cn/Article/details/gszkxakhn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/gxabcxrgh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/glptyojkt.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.hesvh.cn/Article/details/gukmsgfin.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/gkrbjijnp.sHtML

TS:   if (x == null) {}
来源：http://blog.hesvh.cn/Article/details/gxmhagcpl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gqpwxbrzg.sHtML

Go:   if x == nil {}
来源：http://wap.hesvh.cn/Article/details/gwcytvvco.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gibwbkqjy.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gbtcphfcd.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/gdkwagbkp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gezmjeeng.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/gmljnajdj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gmmbobrji.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/giutbjkww.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/gejdgrhsk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gqnzdjtuv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.hesvh.cn/Article/details/gsdoifxue.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.hesvh.cn/Article/details/gmpyjxawx.sHtML

[P08] 处理浮点精度问题
来源：http://baike.hesvh.cn/Article/details/gupfkcglc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.hesvh.cn/Article/details/ghmscbucl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/gcflxblfg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/gsgortrow.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gprljarou.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/gdrhukevn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/grnfslcct.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/gjtfctgoq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fehbvm.com/Article/details/gvptcqugi.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gomdsbuxa.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fehbvm.com/Article/details/gvchixfuj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqldbwpzk.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gpjtojopb.sHtML

CREATE TABLE users (
来源：http://blog.fehbvm.com/Article/details/ghavhzidk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gdgpphizp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/glaacfzen.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gxlhtrlyd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fehbvm.com/Article/details/gchpvoxen.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gigoygwff.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fehbvm.com/Article/details/gthovkwdv.sHtML

CREATE TABLE orders (
来源：http://m.share.hesvh.cn/Article/details/gswhtggbl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gipazcrsb.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gyqvisrup.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fehbvm.com/Article/details/gafwhnsqg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.zdbjq.cn/Article/details/gluqpnhpy.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gbwcrdhjx.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gnarogllc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.zdbjq.cn/Article/details/gsqxjghic.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/gximgfvmq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.hesvh.cn/Article/details/gypccwdpu.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/gajiixxaj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/gksxwwqvu.sHtML

[Q06] 删除列
来源：http://mobile.hesvh.cn/Article/details/ggdmpjqti.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/gelcvmfbr.sHtML

[Q07] 删除表
来源：http://www.blog.zdbjq.cn/Article/details/ghvzhimla.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/gqdyonbvw.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/galmwqiml.sHtML


<!-- 参考信息 -->