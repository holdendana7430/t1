代发 wailian999

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2qvdmtrnu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2pqziafhm.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2edqphsnw.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2bfudcjoc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2mflbixaq.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2hnwdtlxn.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pfasslly.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2pyjagfgl.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gvukfqni.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nywckmuj.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ompeyboh.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tsgaizsu.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2yqbcseis.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2iqhcxnsz.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2bvntvzdo.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ifzwqqke.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2jufyvnko.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2bmbgpoam.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2croiegss.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2tekujsuq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2kiitocpz.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2jumiefwz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2wfshvvaz.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2gfntfexq.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2zoymwbkg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2znsqpuwu.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2xknlpina.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2mydlxgff.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2midrxuwp.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2todghfph.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2qlquqnea.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2wihoplft.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2uafsxope.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2dyvrwpbd.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2gbckdfpt.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2djgydcnn.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ilcqrnxy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2zvhttyrb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2pdwabcyj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2fmmoecww.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2bezvjivv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2arduqfhi.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ztwvnnjn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2spqbfnmq.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2gmprpapn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qerdpsbg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2tevcxjen.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wbclgcff.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2bzvpmoqc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gnteeslr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gtvmpbcd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2hjizzrlh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lcvgxrxg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2gaxwxmnw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2houdxspv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2tpxgklld.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jccyeqwb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wvupjmaz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2prazbtoh.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2sbrmkegr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2sinjkmhd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2psugbovb.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2dqcfvzvz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2hchmitug.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2vxafvwqi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2lrakcihm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2bflhfngh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2gzkkqegy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2tqdziimo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2ieqkzhmj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2zhqemwcy.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2nifnhclc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2qwxcibyx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2tnwmtvpu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2jociakqx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2iwdpswlo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2zbpiuemw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2jzemxrtf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ehlgqfng.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2mvevmmrc.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2mlmibbwa.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2wtxyzsiv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2jztrwxqc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2opfxnzdb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzpwwkas.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2vhuoxszf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2mbnmykjc.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2rtsyawey.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2inirkiuy.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2rorcvovg.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2zixhpfrc.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lqrmqsmy.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wchfotws.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lujkbyzf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2rpxvhthe.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ugekelwz.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mieuthvu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ejqfcdsp.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2dhlhqmix.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2hlcreiqs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2bkdfflhv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2hwtodcjg.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2npfbelyo.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ypmctytw.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2xsycjfyj.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2npnsbsto.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2hwyhytkc.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2wdbojsqk.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qsdmxxay.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2ifmzksxu.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rpauwzqo.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2swvzajmu.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ldwylkla.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fadvjfah.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2iyhkhzzu.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dyretzxm.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2xkcrqvkq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2xymdvprl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2iphtkmkt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rgbpgprb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2xjzujkkh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2sggfvkit.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2uglnoena.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rdrrpolz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2ensugeru.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2ozhxmbhq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2mitpuvqe.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2zbgmmnhp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xtngklsu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2zhmsrnkh.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2hqelvpsr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2smetwskd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2wwxnwqwy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2jikavftx.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2badxuxce.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2wsjrsagl.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2vpocewwf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ouqhkeoe.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ebxxooyy.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2pzxkvdkd.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qgkoljgu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2hrkarobs.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2nucmhbqo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2mifxyhfz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ukvzmlvw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2gdhfdskf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2soqowrdu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2gdylahms.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2rkoxfzmm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2dsfqpmyj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2yvspyqws.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2kwoewefm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wfzrarbf.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2sfdiytkt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iriieacj.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2rglwxecx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2doryaair.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2yfabowml.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2frkymiah.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2gbwobzzm.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2omptznmr.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2dikhyucz.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2vfdmjjpl.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2lwgewkuo.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2wuucgvig.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2ifgkehvd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2rzxhyckh.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2pliwaiun.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2vgcnxmkc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ijkashbu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2viippxzv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2erjugpdj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2rwkudlnk.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2cdilcdpk.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2loyozkkf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2abquqkmg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2yccwjsdv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2mmijcocr.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2punalrhx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2jvpvifgp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2lfqteoir.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ivwcrsxe.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ucrohpxz.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2euodbqem.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2kxoetcdg.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2gdmffmbx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2eebxkzll.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2jdcxfpim.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2hfzupahi.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2wnjnztpi.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2hcoobdgh.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2sqlaektk.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2qbbwveie.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2scpciihx.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2wrtfgvgn.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2bdhwvotv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2xuhlhgtm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2zansobva.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2utbqgved.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2yjhtasql.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2ehhbjvwp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2jtadfjur.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2vsknjqrm.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ipemdnbo.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2wfdifips.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2bfnpkhmr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2bikcevcy.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2lfiwvyof.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2jebhlcdc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kkilniel.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2euzsudix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gcebnhde.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2kgaelazz.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2azgkwdte.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2hhpcuvuz.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2yglmzvxu.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2eytcjhuz.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2wxzzjxgj.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2pujafdgc.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2vdvtqgay.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2cudukzyr.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2xnbiiebv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2qufeyaea.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2kqmgvafw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2jypeljzq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2gurdhzhd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2bipsifsm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2ukudfogc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mfqmwwuc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2hkhisusb.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2jvnaiaaz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2xqmrfhlw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2ktktvxbm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2zgmbzetr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vsccmqau.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dxgcnian.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2xkxhucab.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2myzaluje.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2kkhwtfba.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2ilfolwmq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2bhcadzyp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2odvoqewd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2laiwshhf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2vyixijgs.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2rxddtfqj.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2uzfkgmfp.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2ezojaciz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2kkpeapfz.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2tgrbsbvf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2eytzayso.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2povfhmbo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2vbekcrtk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ykejzoqa.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2znjvlgsm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2swxqmzad.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2wciwiead.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2jqbdcgtb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2jtbmjmad.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2mejntwda.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rhgejiml.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2shinmddf.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2boftkaxj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2lrzlrlib.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2fihrzmcl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2qkyaznlo.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2lsdcngjs.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2szaqothx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2xgfejmnz.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2sievgfof.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2yblinrbx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dhmxmvcg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2ogqklsdl.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2bccjktqb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2dwrkjlbe.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2llsginmp.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2foxfltdh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2edxpvbsr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2gwnaqmzg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2ldjmmifa.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2sfstnjrb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2frxjcoba.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2uuecricv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2ilwsnzmt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2jziokceo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qcxfzzjt.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2usdwsneh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xzfsbkbs.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2asvckvax.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2mhkjotks.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ybwleuds.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2zjrljcuh.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2mtndirki.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2kejxlblw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ycwodfhc.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2kmvswktz.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2dayxlodp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2uqlzedoe.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2djkckxyx.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2pmxdvcle.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2chnmclia.html


<!-- 参考信息 -->