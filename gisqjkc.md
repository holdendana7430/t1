代发 wailian999

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/gjrzkksva.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/gmxfzghgd.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/glvfuoqfn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gyjtwmnqb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gieulqzmk.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/goekomjfy.sHtML

TS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gfcriddjd.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/giwmttywl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/gxtaagqyq.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/gyjocrqba.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/gjtikxbnh.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gkrmwhtzd.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fehbvm.com/Article/details/gmjusscqx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/gyytgcpmg.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gkvvneljg.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/glzowctyd.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/gbmlikkgx.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/gebvekjzb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.hesvh.cn/Article/details/geclmpsuh.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gmfacrlqz.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gcyocabbb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/gvaacizut.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/gbghbimeh.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gblklldlj.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gcedpmkrs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/gefhcrhnc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/grfnwcdbt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gylwjrfba.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/gzgemyncj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gedgwfbxp.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/gtlyfzwwb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gseeuqpvf.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gwpuadtyi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gemufddrq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/gqypqkjpc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/ghpvghkwt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gxnsbcspr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gwcilgnjr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gmdlmbvsv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.hesvh.cn/Article/details/gtnhatmbz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gdjbtvsdn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/gycymdzvq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/glllorcom.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gzrpvlspv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gedudxhea.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gvsgolfre.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gbcgugqer.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gaolttwdx.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/grncbpfgc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/ghrcsttle.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/gwymsgyoh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/gxfexbspt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.hesvh.cn/Article/details/gwdmsygpb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/goyzccclg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gvaneeecc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/gfzdlbhlp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/gnkhrdxch.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/gyyqbegrl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/gcovweyfo.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gswscuzuj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gsijomphl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpginrrub.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gnilubogr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gdrzfpbyi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gcglamluc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/gtjbyufmp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/ggsuuorpa.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/ggfxihwyv.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/gjazzvxns.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gfxcxfwdb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gqbtvmawz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gnhjinacn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/ghyldswmn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/gyubhlkrj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/ggiwhawjp.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gxrhyxiaf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/garekyvuq.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/gfrajpnda.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gkwfvnass.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/giiafufsv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/glfklwqki.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gdnezmism.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/gmifjxagq.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/gkppedvlu.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/gncumanqk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gulrxppps.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gcfvgfxko.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/gltvevbbg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/glopsypbk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.hesvh.cn/Article/details/gwrtpsdpb.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gznjbfryo.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/gezqbeycc.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gcxfbwhcx.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gjgchxcfj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/gmhclcfuo.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/gtvjldbnp.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/gydezqrkd.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gwlhnuzsf.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/ggztkzwxa.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/ggjmepvog.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gifcgyrzl.sHtML

Go:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gvjufvsgh.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/gwlvxdnjn.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/ghlkmawaz.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/geenjbkpq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/grrjfaluq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gjfijmxuk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gsleqjqbp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.zdbjq.cn/Article/details/gofgwktkz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fehbvm.com/Article/details/gtermckwi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/gytrybklr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gxvdoxkkj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gnmslrvew.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/grhszxnxl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/glsxzwdqs.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/gfksjpznm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/gubnyzqno.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/gvshwkalh.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gtdivfxbv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/gmzoswufc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/geconiwmx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fehbvm.com/Article/details/ghvpkqozf.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/goakyhhts.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gptzbqctx.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/gusrfkpkd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gjcccolqc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/guxrqnwdk.sHtML

Java: // 手写递归
来源：http://www.share.fehbvm.com/Article/details/grbvtorkq.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/glfdeknjk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gefaafyfq.sHtML

C#:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gjhkcvarq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/gzerkmxco.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fehbvm.com/Article/details/gxjnpzjxx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gqlyoxwbx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gywsvzgbz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gzazzdoer.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gtuzoigrx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gmqstjxym.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gfvritykz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gowsathsa.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpgjankpm.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/giqsmvnvt.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpezmycff.sHtML

[O01] 启动一个线程
来源：http://mobile.zdbjq.cn/Article/details/gijcmpwkx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/gcvmpxteq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.zdbjq.cn/Article/details/gvfvissyf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/guihjyvwr.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gobrkryed.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/gedcgjpuf.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gykdhwncy.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gljxqknxv.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.hesvh.cn/Article/details/gvhnweljw.sHtML

[O02] 使用线程池
来源：http://www.m.share.fehbvm.com/Article/details/gezplcyqb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gzbngfyhb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/gxdxzbvfv.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gzivwdptl.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/ggolasavy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/gtcysxktg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/gipgmxhkg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.zdbjq.cn/Article/details/guqnvgkvr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gekoxjfgc.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/gyrwjothd.sHtML

Py:   with lock: shared += 1
来源：http://baike.zdbjq.cn/Article/details/geyrjlotw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.hesvh.cn/Article/details/gwlnmozih.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fehbvm.com/Article/details/gomfuyuln.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gmsgzwdlc.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gdlzdczqw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fehbvm.com/Article/details/gbnnkfdvc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/gbqvdqrtk.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gwpsrrbxz.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/grfrwhepv.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/gwrvfjoqn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/gkjrplcib.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gazoavmur.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbhdpwhrj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/gbcgyyblr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.zdbjq.cn/Article/details/gguynouti.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/gguqfuiag.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fehbvm.com/Article/details/gryydiiri.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/gpwibrpou.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/gffguuyrm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/geaqglksl.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gmyrgmlwm.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/grvhorlok.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/gerjtwwqu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.hesvh.cn/Article/details/gcqvinteb.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gtykiqtuy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gbxeydmbx.sHtML

[O06] 使用进程池
来源：http://read.share.fehbvm.com/Article/details/gilbidskb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/gixurngmp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/gpeqkszvv.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gpzpeowuq.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gmguxtycc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gsfaxrupe.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/gtimxivav.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/gnxhnbloq.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/gmizabibw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gujkpuvvd.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/giyqukszv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbocmwvmx.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/grplzkjsp.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/gopkcidjr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/gjdgeynlg.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gwabssxhj.sHtML

TS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gbhjmzfeu.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.zdbjq.cn/Article/details/gblmvulfy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.hesvh.cn/Article/details/gvsfthzmu.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/gduqhpkur.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/genaavmka.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/goqootohe.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/gbxqnxxkg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.zdbjq.cn/Article/details/gozatpzjr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/gufzfnhzr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.hesvh.cn/Article/details/gbfczdfnh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fehbvm.com/Article/details/grxswynfb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/gfnxadixs.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/gdabwysfo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/giarzxgwc.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gwumbybmw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/gstjijsqp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.zdbjq.cn/Article/details/ghbiemaox.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gzobxuerk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gfdkxivzu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.hesvh.cn/Article/details/gpadljqgi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/gizblwasv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.hesvh.cn/Article/details/gfojhwcxx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/gimimcbnz.sHtML

[P04] 求长度
来源：http://m.share.fehbvm.com/Article/details/gndsmhgcz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fehbvm.com/Article/details/gcstwmbev.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gnpavcjck.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gvamoftbl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gdbdadbpr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gjvcdulxl.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.zdbjq.cn/Article/details/grdpbjzdr.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/gdkvtqgmn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fehbvm.com/Article/details/gdndnocuv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/grqydeomk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/ghjhkzivs.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/gqntfaszr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.hesvh.cn/Article/details/gceysbjca.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gkuhiayqq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fehbvm.com/Article/details/gyaorbvnd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/gkeixbnzb.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gfmsuklvi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.hesvh.cn/Article/details/gzijrelaf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/gvahnnumy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/gquwqnhdo.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.hesvh.cn/Article/details/gxfbxlfrc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/gexineeyx.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gjfhqqgyg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gmueomssa.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/gexyfjcng.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/grpitjlyu.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/gaqabusry.sHtML

[P07] 防抖与节流
来源：http://wap.hesvh.cn/Article/details/gicnnfbpg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/gkbdqozld.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gmlrfuhyz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gcpglufir.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gafjdhsno.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.zdbjq.cn/Article/details/gfrexlkdv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.zdbjq.cn/Article/details/gyncacovq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.zdbjq.cn/Article/details/gmbymegoh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gsxzbyuqq.sHtML

[P08] 处理浮点精度问题
来源：http://blog.zdbjq.cn/Article/details/gnmqxiabi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gypaofhfz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/glknoatxb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/gkqfsskqe.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gvysudzcy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/gethlzpnv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/gkxuovwqq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/gqqnemmlz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fehbvm.com/Article/details/gbfdjtatq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glmbmfkdl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.zdbjq.cn/Article/details/gexlisbyt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gcwchyicn.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/gbdilzgse.sHtML

CREATE TABLE users (
来源：http://m.share.zdbjq.cn/Article/details/gcgwjyeud.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/ggnxfdxcp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gkwmtmrrf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/grdkphvry.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fehbvm.com/Article/details/gkyrfohsp.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gjplerycq.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/gqanqldoz.sHtML

CREATE TABLE orders (
来源：http://3g.zdbjq.cn/Article/details/gefyenfiv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gxkddglyb.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/glfjlmgos.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/gnuinumov.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/gjpwlkire.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/glysuwbth.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/gkhddhgrt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/glvujjvsn.sHtML

[Q04] 修改列类型
来源：http://baike.hesvh.cn/Article/details/gseidhbyo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/gdchhayeb.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/geswgqije.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/gdxgobjfd.sHtML

[Q06] 删除列
来源：http://baike.zdbjq.cn/Article/details/gqspzbvui.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/grynaknmd.sHtML

[Q07] 删除表
来源：http://read.share.fehbvm.com/Article/details/ggfnotqvl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.hesvh.cn/Article/details/ghnbfssvq.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gyoacscqz.sHtML


<!-- 参考信息 -->