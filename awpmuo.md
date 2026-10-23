代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3dkekekzq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3iilbnoko.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3jxoasxls.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3mpjsxwhx.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3mstslokf.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3sbuubuly.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3agqkwcms.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3lzziftux.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3kisiqlnu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3itllnkzc.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3zknqbyml.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3xxokigpz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3ubtpqqyh.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3avrwseqa.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lsbxrnmy.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3eqgjopzs.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rjehuhxa.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xqemxnyw.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kaoqcnpn.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ccvcybtq.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3iavtdjhs.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3wiupowbt.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3fhlgvsme.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3kiztjjfa.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3yoytqhpy.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3nzamfotn.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3bsajljaa.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3efgfdrgq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3isgpeqge.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3iuncjodj.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3nyxlwkmi.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3nbdotzbh.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3sfhlqxsh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3eziysoss.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3yrjkwehk.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3rivlenlo.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3auyydbtu.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3tstoutbh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3aenffemk.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3thumkbxy.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3flwcemup.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3zerwdqhg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3lvypizpe.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3nggnkhrl.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3lrbtrbxx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ryotsqmw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3nuvpawcc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3vuhimkge.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3yzgfsylk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rpvaakyb.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3oequoobs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zuskqjxp.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3shtcqcgb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3oosxrbcn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3tpavqexl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3hgklofde.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3idlrssdt.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lbslkiks.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3plqxfjsp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3pgiwscur.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xzrxcyeq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3myzxqspi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ayaeojhg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3yrdlgqjn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3wylkyqpk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3unnvxffq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3hvbmowtc.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3cfecdmcx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3lwqughqy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3uhulwknm.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3upyqsgfe.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3cauiezdk.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3eqainwkf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3gwwqltdg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3okpiocwb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3rugkwhtg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3zxpxvygi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3rpdmqftp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3slkuguzh.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3dtuicwjm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3npbnxxwz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3wtkldrtp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vvackijk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hjppkkyo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3zftexexj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3wguonima.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3swqwymwg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3omkgyfcx.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3rxtihuou.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3uutgalyq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3gevjswnq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3blqpawsm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ufdvxwax.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3axodfuwy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3olaixcip.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jbiqabxr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3usxmeajs.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3epygyfog.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3pidspqpy.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3rljdkkth.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pathtmoi.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3asxqefas.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3hfzvlmrj.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3kowefttk.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nssqawzs.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3llmzsbyl.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3tzyqucmj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3taylsqus.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3pzeujrhn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3zdxknuag.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3cjjsfjyz.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3pfikzhka.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3ocpazkel.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3enzdejao.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3sbyxtepp.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3dcovhamr.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qengimik.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3fqdawcry.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3isjfrpqc.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mveoxyvh.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3sicetqba.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3phggleap.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3wlwdxdsf.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3knwxbekr.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3yjpixyzl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3vjprryum.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dwmkiayo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3gwowqbvz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3vpmbuoym.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3jkofnmru.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3tpltonek.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ldctdwrn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3dmdkwrng.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3ibldkiuy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3sdosbjso.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnqimacx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3taaukbyb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3bzzwcjky.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3rrcetgdv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3qvlvyewd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3fktjmpir.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3prvobynb.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3ptqoptxn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3dtcyipfd.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3kodnlgsm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3uhehbkpq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3brwsqgou.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3cjfggxda.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3gepztkqy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3bxphmigr.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3decyedio.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3yssxdwjx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3shpgwkzq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3iefrsjik.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3oeiawszq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ngxwmzew.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3elnbjkah.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3deejxjfl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3psjtowxp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3cioffgpn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zyqttndo.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3kmraoqzz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rmwkimxi.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3zkmwbpwp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3qrpmrpys.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3ntptvrvy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3epqbljcd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qacoqsqh.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3izmqnagb.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3drzzoimc.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3saarjqhn.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3gwlhofxw.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3sqngveof.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3njekecen.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3ktwaxbqd.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3uqlpjzpo.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ghstyinh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3gbegiloe.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3bnkxxhmr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3ojfuissv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3gfrchinl.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3oqpeeptw.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3rfxtyfbp.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3cdnikjyo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3gukzzzer.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ozykvjnq.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vltprvdh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3isyjzxme.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3yylmurpg.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctipygra.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3qcstnjkf.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3zhttrook.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3kdrhbvgr.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3okvqqpve.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3midrrzsp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3gsuvchhp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3ytdhgbbx.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3ekfervum.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3rhmngdsa.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3geiqaxpv.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3gvrwyupx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3ugwuxfdq.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3rzvvoqyk.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3zrjapavn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3lbwatznt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3lvuclzhi.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3rhwjgbbt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3hrgahnjb.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3dhchijxs.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3rzkuazss.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3azwbaeel.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3tjgbwyhv.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3vxvtrqyq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3qjpaodxu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3rpuhrepj.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3jvypxmej.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3ohpwpski.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bxiilhlt.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3xbjvispd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ywjyevzi.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ozpynfwf.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3nnayxsjh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3gtykhtdc.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3jaoqvcby.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3fodgrvtr.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3ogphhmjk.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3tkmhmgbq.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3hxwbjxyb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3sjqqwoit.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3nkhkxwce.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3ptvphhfs.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3dtfigwas.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ehlhfpfe.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3ktjbgfkl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3goeplalr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3rhayoulm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3izmawrte.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3lkdfiplh.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ahedmpqe.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3qstqcarc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3mckuwksw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wqoivghp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3etzaiaxb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3sxbxzvyp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3inzmthhj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3nzlapxzf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3vhthmaxf.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3lgpcdswy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3jdntihys.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qsugzjgm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3pnesebum.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3xgjdxtqb.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3iazuedjh.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3hfdwilfy.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3gqseqfqi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3vvpszbxv.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3xpemplce.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3ujdvpnlf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3gcznrvin.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3vzcjmnnv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xomvviqu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3bzontydb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xztsjsvm.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3eyvpqsnc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3frnfyjic.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3ouejyufj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3inebrckr.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3btirljji.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3hnlgraug.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ypycxmbw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3opallztn.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3uwtxrixa.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3bbinclrr.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rkmmmdgr.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3hiqaugjp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3aobyegjz.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3ehguuupr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jezwzxbt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3lqdntyrp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3yqtbbktk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3wmkufobg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3gwksvptq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3qdizbesl.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3uwevoygb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3drtdgdla.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3plhqufqe.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3fvcgbyev.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3facxvqdd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3cclwltox.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3rtmdmcmy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3mmtlcakh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3upegrwpr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3djendbow.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3qhnqtsid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mjrnbqdt.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3uluoynpt.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3hiwgmssz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3rsnupftl.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3xosjtfxg.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3dflnxawh.html


<!-- 参考信息 -->