代发 wailian999

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ngvhyceg.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3onwturtj.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3xakheiwa.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3eemkcvrg.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ocdqkrco.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3jocyzeoh.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3mbhcqxjz.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3fkvibsoy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3amjdoslj.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3dtphihvn.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cdcoklsk.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3mntcggxp.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zlfnwmur.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eeypjpps.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3omhwuezh.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xxyuapgb.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3gsjwwxgb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ehksqoxr.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3jxkqtqyq.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3bwgdiagz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ygjqgvbx.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ctgpifbl.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3oalnkjgx.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3kmtynlvl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3qcipstkd.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3pkwwiotj.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zpgpfcak.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3jtnhkvqo.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3yraeehth.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3rljsmxmg.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3epepmast.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3bwdzoubh.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3lpuqejcv.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3jvsllzhf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3fopsafhk.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3xssujopa.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3cuffwoxx.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3qkpemagd.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3lkyzvdtx.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3eltcsiho.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3qlrwupng.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3qtrmvgmr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3lodqrodk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3yushbiyc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3obhsthrf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tatnugsb.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3qhnwofgd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3omhubwmf.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3idvlqlvt.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gqqqlsls.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3xzlkudix.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zmlrijys.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3dyyzmkae.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bthzqqiq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vynymcuv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3kircodah.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yxckdnin.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3efmnvvlw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3oiiylsey.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3ccugpgqi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3xoffvcri.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qnaqlvry.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3mysyqnfr.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xpevycbo.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3bltxstcw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3qvucuuam.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3xexqkvas.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3vjlsbbrg.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3gqrjlhns.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3bwuxzzwu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ddepemeh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3kcufilfz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3wddrhkfq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3gzzlwpnz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3sntcwwvb.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3cbbkwtoj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ayyzvxgy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3jlocdfnj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3drvvusmn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3cdiamfrr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3flzofgpp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3lbufbncu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3xspyascu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3isjocqvg.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3xoblxoad.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3laeakhvt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3gylzxhlb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3qupdueeo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3lswofrei.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3jaljczpb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3dvlmmfea.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3vihktscf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3rbsucjvs.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gogdctye.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3mfrojhau.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ngohcrun.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3retowesn.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qcwdqdvu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3meallyzg.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3nvllbqkn.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3bgnvwdyp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ddjaxtso.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3cahadeng.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3yroxafgs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3qxijgxzr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3zomcqmot.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3zwajlrhe.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3fkmmxkjw.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3xcbipktt.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3oqtjkilm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3qjxvbrgh.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3rndvgztl.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3hnjxkiui.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3rsuciuup.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rbaklaub.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dipspwng.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dubcvnuh.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ekgbcaus.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3wkbvbthk.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ygcaxoso.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3uqtkbybw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wmdgtvmp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3uftxhnbd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3asrkovjv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3upcxvmti.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3gdliuklc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3itejfqja.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zagusllw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3pzknldkf.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3hfpwmbxl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3nwmjvzsv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqqrcnqx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3gmhohbqn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3bpwkprfa.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdbhlnrx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3lewqvyqc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3ijogtdvo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3auloauxe.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3irdkcbyz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3remmxrly.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3zqnocetl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3brrledjx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3cgodynaj.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3relektad.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3nmjxuqze.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3dzbzqnzb.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xagzxiqz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3vjrbqryo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3srluvfdm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3jgqnhbdk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3tpyyqavc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ubiuqygu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3rsrpsewz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3vksufhaf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3wjtenlac.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3remogfle.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vfeglcmi.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3hcujfyvr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tovxfcmx.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3bnxbckay.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3jfmdzcic.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3jvrwipdr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3dibqzhea.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3wpuicmxt.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3kzojsefr.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3edrypuor.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3qniuqnvl.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3xayngpwz.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3papdpstz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3lqxmtcrk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3wsugqlqq.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3awyvmdwp.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ydpwtxli.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3zvuivsbm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3lqxyyhao.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3mxdzmzhk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3axnmehas.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3gcrspzot.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3tjuqdoef.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3duthmuaj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3zmlcfiwh.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3byebaakk.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bnyodfvv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3mnwspdeu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3zttyuxwc.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3isgnugai.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3dzulfqra.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3oujrgegw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3zvrsyndn.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3itvwebmx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3vuxfozxn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3gphwohhn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3efwpnlim.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3jpicdymj.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3rawihoth.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3hhedozhx.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3bqbkainn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3ibriapxx.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3udbqddrh.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kosfrhgl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3iwrqmhqb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3gmxeqlma.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3webciyng.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3pzfscfoi.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3fflotutf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3smiaxvyi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3zhjnhhpp.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3gkhclzcl.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ytgmlpvw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3fspcvjjs.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3sxwemdap.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3eygdrovr.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3qchgoopl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qawipbnd.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3nnldzrfu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xdllyhhj.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3fezzswjf.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3aovqofok.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3zhqincpk.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ymroxhfo.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3dzddzmog.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3kmnsdtfd.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3teapkmnt.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3bxkokbql.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3yswxumhh.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3ftpjrtjb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3tuqoiqbw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ystwnvsx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3auqpgeco.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3drcldkmb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lsmvgxda.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3ybaezipy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3mxayqvlp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3mnnlauxs.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3flarnbcb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3hbisvlcw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3pkwtmoqy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3zhyagkky.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3zivdfpzr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wpicyvle.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3qazfcqsb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3juyvaibv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3tskljzol.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3yiiybmqj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3icepphtq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xqukholh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3hmiktqej.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3cgggoohr.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3otemjawz.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3reffkxhz.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3pydlfnkt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3nviymbwy.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3zoxegoul.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3ironpodn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3xugzsmil.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3sopwcqlw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3kdyepiug.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3tynyuhid.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3cajxqulo.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3kxsbevev.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3sgmcytxn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3obtbjxau.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3tsgilsnx.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gcghlhgv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3medtscrl.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bdqszotq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3fwfmodct.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3hmijqryl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3myjuppqb.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lcrhrhuo.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3fmaduydn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3omymbgnt.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3gwalnaaq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ptexsmgg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3xuntgsph.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3odhsbbqj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3bfppdknm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3xlfbrwzx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3ywwbmrgn.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3ockoytis.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3gpdqccxo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3iqtrwcdu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3repwxfhq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3szhloieg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3pphrjufc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3bttofxdw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3qbhwgujc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3xklbxzyf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jwoobkat.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3dnmlohel.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3juveciey.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3atyweslq.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3nnpiwxaz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ajvnzwmw.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3bfysfhiu.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3vagywazz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3njluplzk.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3mrrackyc.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3yacmyprl.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3opysuzan.html


<!-- 参考信息 -->