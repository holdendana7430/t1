代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2rximyxoh.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2fbvcsweu.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gpojelxq.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2apbslyel.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2imnthtsn.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2cqrruiel.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rbhzxvry.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nobgkosl.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2mrvzvshr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2alcfwxtx.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2iawztmpr.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2veelcxql.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2fvxjhkeh.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rmwwxdqp.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2lloztkuw.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dzixcfve.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2iuzyukzg.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2nrnepcmt.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2zuozahrz.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2wimoubdc.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2uymdlsie.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2gzzocsfl.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2afneotie.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2zgqprrai.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2kojbdyys.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2akjkrvem.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2aorbieep.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2hccsjubs.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2rnktidbo.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2tjjxnxcy.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2tixkicga.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ytemnslp.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2cqbtebia.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2xxgbviqz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ewenhxub.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2rirmdhin.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2tsdbdynf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2axjxyfbo.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2qtjrjyfn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rbzybsla.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2teoxlylw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jewaupiu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2hrsbfwjt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2offfgcgx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2nqdxpenb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2geiwteap.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2benrxvee.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2xjhivsof.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2yamnumtn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2wcqcrrgg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2esgazkpw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ahnqqjft.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2dvlcroap.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ffozaldj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2ljznyfhi.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2vxuylitg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2uzklypak.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2jwbxhgyh.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2pevagtlb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2pxbshuam.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2exqrtbdx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ssfgxpxp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2icleuyyc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ijyyvesm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2yhnuqxwk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2jmwbzzdb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2rusknmnr.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2lavenydm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bjozvtjo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2yduzipgv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ygokwsnw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zrkgodsa.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2tukcmnms.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2doqjdubc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2cpitmemi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2dfgcxeks.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2wclxeirg.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2swmrgzyy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gguibbgl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2jozosryq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2wsdaellh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2lnayymdy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2ijimhvhm.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2vgtewnnk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ghnessew.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2xtpozoqw.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ysfgtrwx.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vmngunvj.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xyqycvzt.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ekyfqdpt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2mreqwlbg.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2tsjbfiby.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2oxcqkmkp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2wudrfhyr.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2odjskmek.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2jryutvyw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2zdrkmuxu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2khguqyra.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ytlntysr.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2bjwlgrri.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2uweboqci.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2iznhgwsu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2jgisoije.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2iesfjuga.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yxvrlmmm.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2tnwwxhdu.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2epagstpc.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yyxwslkb.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qxuoalkv.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xarmtfwa.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2cpxstfvq.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ahhdkuxk.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2fbrwzjod.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2agtuttkg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2egsddvjn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2gxgmgvif.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2cmqbwapv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2vauogtnc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2wmrcgboj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2amcziieb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2oabxffox.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2ejpncxcb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2xghcpedu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2boxlifbu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2uhgozopz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2cshburao.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2cunljcdm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2bljhtcak.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2cdbjeioe.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwnumocf.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2penhzcam.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2dqdrzria.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2mkpapiiq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2lprrtqte.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2iytctcbx.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2sojuqgbr.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2stpbcuso.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2gihtbjxm.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2tzubsgpe.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2pizuyiho.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2hcwhmplu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2zjygbvhn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2wgsgmoib.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2xrrozevl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2gsmurqln.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2fejemlse.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2dofdisgu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2qdxusaqx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kgbhsaew.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2djeuzfsl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ybzfoacv.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2yrszvgnq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2xuaskpqt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2qhavgloe.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2fklfrcgu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2pyhqijom.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2jvaataym.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2txweucml.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2usifxpgo.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2cyeqvzvq.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2loysvvha.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2hcipywkf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2njsgbffq.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2bqptnsrs.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ouobchub.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2rqcaufre.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2fnotjvww.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2dnfbtdau.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2vxcsvnpr.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2xqaybxee.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2alpdmuwa.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2nkggbnvp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2tfspounu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2vvkqnidx.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2gkcfgasg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2kywdlsls.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2zmdhlpcq.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2azftatmc.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2rijlymmf.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2xzcyswwk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2icebvaba.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2qplfrdiy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2rdttfqlk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2nsumjhqs.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2esqkhohq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ziylbccv.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2fhjbpjcm.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2icacplrv.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2twsytllp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2lvrlchul.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2jvchjuhy.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2xzmjuhqx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2hmnoymgo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2fvsnirgu.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2grgcfwom.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2bijsysej.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2poejfjky.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2sjrsblom.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2conjmbkr.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2lntaseto.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2hvejtjuz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2fnyxafmv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2pbfvsmiw.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ynjcwmgx.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2gcjrcjro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2balbthfb.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2wcajrnum.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jqlrtjuw.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2mieplnpo.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2mvvkxcfg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2rcfneyqb.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ghrdryiv.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2issognum.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2hsodbsvg.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ibixldme.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2tbpswwjz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2niowwhfq.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2dpldtojv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2igledkvr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2kcrwxfol.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2profunrz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2hhsbbshq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2zcsxtpbh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2ayppyamj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2qirlcqke.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2unqlnmmg.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yeefqhwm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2jlhpxgfm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2gmzwhset.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ohglpcwu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ctqjcnnj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2utmjqkvc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2iizzldrw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2jpankdga.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2ogswsurh.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2ffcdkfwb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2gcsvnhaf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2oavsvjvp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2eblbtcrk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2opddioga.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2vuschdpu.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2gdegtyxt.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2idbqifdm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2wyacarng.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2pludvzjm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2sgcdvlon.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2vibxwedo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2svywtgay.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ienzqrbn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2ytlfsmml.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2kysabqck.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2xtrbytxy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2brviqyrg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2qlhflmpl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2dzqebkyl.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vxvdgwxt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2cnmnbarv.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mtoddkhm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2saqslmvg.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2uquuvndn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2xemiuvqy.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qvlviznv.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2pzbbwzob.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2xkcyrkdv.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2bwgbnwyf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2kclsofdm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qiuuwshm.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oamiuouj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2wzijyeix.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2luhhesnj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2rxjabait.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2yinboxmf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2trynbamt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2skibtisd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2evoamwja.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2znrjxisu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2jpxtxkpi.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2yoqhihof.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2wmxavmjc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2fohbdxmw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ekqirkgz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2nneavtyk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bjixbtny.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2mmvrzjtp.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2fpwschde.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2aqgfdaxp.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2bjbglxvr.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2bsqhdtme.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2knfkkvoq.html

);
来源：http://www.52xcode.cn/Article/details/gt2ualpwsxv.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2kxrvzjuq.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2jhatsebz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2oemkdrjc.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2qfqswfit.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2yosmahyf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2zytstvke.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2sidtbdpp.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2zeuzinzw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2fvqknlke.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2sgylhrmd.html


<!-- 参考信息 -->