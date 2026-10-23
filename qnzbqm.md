代发 wailian999

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ggaedlrk.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3natjmket.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3wlvnrdov.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ildbmhxv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3uhtamplc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3ysrkmflv.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aujqgpyj.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3rodosntp.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xoobrtbx.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rnypofwe.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vospjcha.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hdkygjfp.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3cidgwsvg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3owiyjdcn.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3kcpgqkcs.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3wqrbwzmt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3bfbyidsm.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3yzbqvcfs.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3boscdgbb.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ziidopsv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3uiidkmgh.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3gqvbvwya.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3otfglnql.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3dlvdjgne.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3xtrbbuie.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3klgrdmkj.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3faborftt.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3wadfbrju.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3edvjjczz.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3hniwjpru.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3efzeeczs.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3rvtgigxo.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3eywtuyfg.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3cswlutkn.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3chnscktr.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3cmlohlni.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3zamfdtmt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3faoxdvdy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3anhxrvre.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3klngpqbr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3rxtzsgnf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vwaafdby.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3htolqnpa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zkvnvuff.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3xyrhyksj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3glxeantt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jlfvyknn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3snudleph.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3odnwvhmo.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dltcxmqt.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pdbgqtay.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3svytwuds.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pehsoatg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3mcecmkbo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3vwmqyaon.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3slgninyy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3jxmjkumy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3linkuebp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3buyeglhp.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3enquroxj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3jcqjohxq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ylzgmlei.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3hhikwogx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3jmzrhdsw.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3tgubbiqf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3sbinkiid.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3howxjvhb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3dztufrxb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3rsggordf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3ixxdwlwi.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3tiyplhip.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3tdcpyikg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kyryoacp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3wkahryme.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3txnfeihy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3eqjshdmw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3bzobjgil.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3falhdcds.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ycvzckny.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hvporapw.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3hlkxdmcl.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3acketbax.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3oxtoowav.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3hovahepw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohmxwknt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3gwjgtwtx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3aqzyaxuv.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3dspngdmf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3kbdhpyeu.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nydutgam.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3qhdkjvdr.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3qiearluy.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xlqreoyj.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bvsfsxli.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3fgtuxrls.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3ghgrvgit.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3epjxmfge.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3bnquybzx.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3ezalclag.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3yyrwjvxg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3msbaqdpr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3nwxlxhbu.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3igojkcda.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3empvfwho.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3aavbhbzf.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3erhxclyd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3hwbksjvf.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3xgecwfct.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3kphhsivz.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3hcllxqsj.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ovphesoj.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zehyfwil.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3bengfjoe.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pjkkmkpf.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3vrmksdig.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gwcjcikn.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ugpbscnu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3pcerzydd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vvdkumtd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wleeaquv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3kclvdlch.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3zagwyssa.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3woutrezg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ttzzpoeo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3cleothzp.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3czbmkdex.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3zohrwqhg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3drgmzlmb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3icnlqntw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3awgxjtlx.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljjmzluj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3ltamuyow.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3opnqfupd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3yygcjnfw.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3igzcobpr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3xzebsfdx.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3dfuibfrp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3pdzjofnl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ucsnjvxu.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3zpfakked.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3exlbwfbp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3abtsczey.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3kusiibpp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3greutjmk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3bbwpjbyx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3frdlmnum.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3qfpatqtt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3gvfefcfg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3vzjljcsh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3cwbeqnah.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3qrqxexud.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3dvkprlck.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ygdnxbtg.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3ojbdabsq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rqgltmvs.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3sbwnnpwx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3mvriadfu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3uagackrn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3uvkvuagc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3zrunebtv.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ddoxgvvs.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3cacojabo.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3qyaejwla.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3fgdepkmy.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3gnuqcxxb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3hjrulipp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3qgsbuzer.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3zlrggwod.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3nywqtmtp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3lkwroipp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3rkwwjmsp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3rvkfqjik.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3vejxgvsn.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3hujswoal.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3gglmnqfo.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3ztigghue.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3igfjupmp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3bseftyde.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3qiwrypys.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3kadhvdiy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3savyudin.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tircusgj.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3spxxuhix.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3pbhqaqrh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3fycxatpv.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qlnxznhq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3yjvrkzdw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3uunyvvwp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3fdsloyse.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3xgomxttu.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ddjniasw.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3mkzjspee.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3bkqdakrv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3rwliksop.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3unnseosn.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3oqteaeqz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3sdvcecos.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3wwpnttzb.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3sgnbzyjo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3iohczsdc.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3eeeumpmu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3edceuufx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3olruaarv.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3pvvqojwu.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3qjpzubxf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3qkasvtrv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3wlrsojcs.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3lxvkqied.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3hkeziotu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ulrnnozf.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3dxbagmec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ycrvdkjc.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3zjhflnlc.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3mdsyzytt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3yfrxmzvf.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3rmpkbutc.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3nhejxnvk.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3vxemssne.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3buozuixq.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3hpcqnsnx.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ygspenoa.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3ydxmyxjk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3cmehwuin.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3evxelvwi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3zyeckcni.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3useqedhb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3kzgijitt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3xlubnxmx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3dnaxxxmb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3jexpuokh.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vfzkgrvq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3tpqqktpc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3wpifbikr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ewxoijwo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3twrlzikx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dfmnfvem.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3rtxfyist.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3pgmaeguk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3rgetpffr.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3xclqasdx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3ehravrvq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3avetmscc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3wddpdbvd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3yoszzwpb.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3xqsjfeim.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3pkegsgjs.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3muoyoiup.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3tjyrvlld.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3fcnwoivm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3vddmulki.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3sffcbrsf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3krbmmkzp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pznhsypo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3wuhlodbu.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3rmgxaqsg.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3egyhqhii.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3busgvrtt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3hgyauwfl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3dqsuuamj.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cbcejazx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3bzpibthv.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3syjwnojg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3avmwliaw.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3wvykktpe.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3gedbwxbr.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3jilvdeho.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3qxqvofll.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3hcoyxlkp.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3hmxfqcsq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ipimzlco.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3cadjnfyg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tfyynoxm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3jqhchytz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3jcuaayjk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3gcrgpbec.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3mzqksrmx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3ncmvaufm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3oycejnsb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3baehtvyp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3mpolusfv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3pqjhtraj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3wfzkxztj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3jrwywvqr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3hldbrvpb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3reahvhtm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3kjkcxgid.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sacoqxyg.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3nedabdap.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3rqnomjmf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3aoolmbmr.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3pxmsbpsu.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3kqinluot.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3vmucfhzm.html

);
来源：http://www.52xcode.cn/Article/details/gt3utcxwikz.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3typqnfsg.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3senmgbsl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3qczhjlrv.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3hakbbvmp.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3sgfivgal.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3jvedigps.html


<!-- 参考信息 -->