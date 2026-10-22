代发 wailian999

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qzobkwgb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2obupnfut.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fxdkplky.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2ijvpkfgd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2apxoighl.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2upwnotok.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2plcjdyhp.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2atbjxdpc.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2iswguucx.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2itwxmded.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zhixgkkj.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gltimnvw.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2llrqeptw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2iyzlolpz.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2fnqpkuyy.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2zslkhbkr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2qajlbexa.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2cdbavmex.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lfulnlva.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mpwlkbrs.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2xuhzuqkz.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ofzgybuq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2obwqcfyn.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2xmnwxinh.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2pogeqbiu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2hkgymmrd.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2wscioopb.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2sgevobqe.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2junhepnm.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2ljmrkbzo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2yjfmlafp.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2bxglfmco.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2gncbgobn.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2xqsjnevu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2oyesikov.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2yqbvordv.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2zevebfrw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2kqulvfsj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2oikaawka.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2tvsaeljw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2wugqglam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2snouuxxq.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2fvkrlnhu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pnnvelff.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2fcfgmlkf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vfcglhag.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2qbyiclnd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2csktjkku.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jrtpncxu.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2omriltzi.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2aaixhmmv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2qzvqxjep.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qnqopbxu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2vkscrjlv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2xlcxeqjf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2awukinew.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2pkrosyeh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2rsibpufr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2sljlwhxf.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2cmfunmes.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2spoppxhg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2xcmaqdls.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2ncpajggf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2skdpemjl.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2myerfsda.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2vhzunkgx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2wvbohvnl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2zhvpmauo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2vjbjsfkp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2eztasnub.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2wlqhlimw.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2mhwhiovs.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vppuxnls.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2fknvevem.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2hinecngn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2etompsfh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2dgnkflsp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2gadigtch.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jrbnbypm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2fbghnhqt.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2iplmbxaq.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2qtzqlnce.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2tesdteqb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2fapugjkd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ytckcksh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2hlaoacdv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2gubxxgsa.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xxwrnspn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2tfhbwkfe.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ghfdgfbp.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2yhqdtgtg.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2elzbgfpm.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2dqxmselq.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wvvhcmej.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2pyqvjonw.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2bligbscv.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2gpoirech.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2oltcrixa.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2fdelqiwl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2qxtzfskh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2rcigajcw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2xcutpqsu.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2wornznle.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2bxeolcei.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2pjckqnut.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2zfebgair.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2fqjbsxya.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2nnhskmim.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2gkbzaolg.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2vudpxono.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mischdmc.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lwyadwku.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2obvjwxop.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ldwbzdpz.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2kpgrsnvv.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2goteyzeu.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2szgvgfrr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2qgxebiyq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2dbuffrnq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2sclaidtw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ylyyecpc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2gkuwtzbh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2nlrawvuz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2oawbfcex.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2uhstkaiv.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2snmqxlqm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2kwbtbfjy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhqzhnbp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mduwwwaq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2tqrwjwej.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2xomdxend.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2ysrpbfxp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2dvxgqpik.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2yiumltsb.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2bmhgvmge.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2obsyjfoc.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2yqkhhajy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2akpkczhl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2yawjuaqd.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2wsacjjdw.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2wujopimn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2dyxopywe.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tcgjbrqa.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2xfelatyb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2isbgmaqh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2wpqggvxw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2qnwbrspe.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2lvqzrpvq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2vrpntxxa.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2sblcadzg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2bbhnmiim.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2qcwsavcx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dhyiikbd.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2ykdhgfuk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vwxycnko.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2sfcorapv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2lmrhqlcw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2jtaefvse.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2apjzpaok.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2wtudeezu.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2glaepqsg.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2axzyiaxi.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2ryoesqps.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2jqljuosa.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2pbwtjvsj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2dzifuwol.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2mxwkeuht.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2yjvaeohq.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2cnkxibsg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2icnusask.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2psdwksah.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2xylnbhvc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2suqlkofz.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2juzfsmiq.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ovbhajfm.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2qiugqpnq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2uvhspwxc.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2luxxysrz.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2xnhlttdc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2rnwmnbxf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2sjadsvah.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2czwxpuad.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2mrqjnjur.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2ubnmziyp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2ztrlpxye.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2xzaoyfme.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ojspigku.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2fbnbxdef.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2zrblotsh.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2gmilggef.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2xtiwndji.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2unpgebuv.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2uwkvgzxx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2atfldyah.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2puklbirk.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2bxmhbhsx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2ozkwgxzs.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2dovligdi.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ohfdezyz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2zqirhtcj.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2znknskej.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2oimtewql.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2ijbtrhzu.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ndxzdlik.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2rfybrehz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2uyuvvooz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2jttqkkrx.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2wsefwckp.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2ymlmyhkf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zxkqnadb.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2uziuukao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tiqyolbh.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2zeemqdgz.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2trqfykhr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2cdvvmngl.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ltrphztf.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2onblwagz.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qemivwsn.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2djuwnlty.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2qxenxwkw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2csxbbiwq.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2qlwxrsau.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2swybemyo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jslawzmt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2yyogtlcf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2onuqmrzh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2enlbywth.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2infirnjr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2zibqmkba.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2glpltfpp.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aupytkma.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2upygwykw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2tkaibdka.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qvohdbfq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2jskjbqjy.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2odzlvngc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2ujqhafpt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2yypqetal.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2schanfpw.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2czvfmlxl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2sbiziqwx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lssgtuok.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2dytathes.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2vimwxdmw.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2wehnukrs.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2oghysvzs.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2uevdcnpt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2fbwmeefo.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2dhgzwoxa.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2mpqvklau.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2ijzmnfaq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2zubcqkgm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nkquvema.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2rasvjzgl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2fyuxdiwg.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2gjpdmctv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2crmdhxhx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2wozksmry.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2sgidnwgx.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ejwyzzrc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2xcibcfpy.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uuzcvdvf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2lyucddlm.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2yenczcwv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2chrwfwhg.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2ufgfxnbc.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2abhhnfcl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2vddjxjfe.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2xtbwlxrb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2zoiybmid.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ksewawdy.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pbyxfmtj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2cpieqwfe.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2exnkftut.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2ofmufbkh.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2zpksvahd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2ygttwgrs.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2oimgcdku.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2qrrzbkwm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2blflwkye.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2wvkfbuib.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2ztyxdrzj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2yxyavyfi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2lbkzpxbl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xahrslcf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2jaovdvwv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aeqlslpo.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2adaalzwd.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2honrxpwv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2zciuhmfs.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2tfifrnid.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2icnrtxzh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2jxsjbcrs.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2uejqslvw.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2wvbonmki.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2aibcjepa.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2dprqymks.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2fgpunxzx.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2gfnnablx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2bipqxmtp.html


<!-- 参考信息 -->