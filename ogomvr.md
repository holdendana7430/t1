代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3rxqumcaa.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3sjptopkx.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kqhqwjek.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3kjjgplxz.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zwquzrnh.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ssjepyfr.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3motmdjnb.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dqdwlexi.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3miaomspm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3jlvkgkvd.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3qaqbkvfv.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ndnpnpao.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3iopfkrds.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3kjddwsrr.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3oqkrsfvo.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3sepmjznv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3edrhkxmu.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3mnztudyg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3okngycke.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3tdwhvdrk.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3vpclauea.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3slfqferz.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3qkgtrvgf.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3yrtliucl.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3rxyuigpo.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3pjyujmrh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3gdgdtrjt.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3nunninlg.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3vrqnbsex.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3rcadffub.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3cvddctof.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3pjkiatwt.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ozxnkbdy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3fcbtvebt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3lgfejult.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3fqfezqnq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3bjsfallt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aaxfduev.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3qvrpzwtp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ohajwmrp.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3wszsxqka.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gzwgcgky.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3dajozhsb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3muoixfbd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3vtrnrbfc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ymojgbky.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ekofzqfk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3ztbqfysg.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lrrwavzt.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3upwcxkrk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3pwnamspi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3dfdefpzz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3dmtmeovx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3dotklkhy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3wntscltz.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3kzvwpjmy.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3voazinio.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3pkwqlbyh.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3iolviapq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3ihewqyua.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3fepluhax.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3rdqvtqmp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3yvhdeuse.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3mvimjihd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3wvzkvvll.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3cvwxrfvh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3lpkhquyh.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3smwblawp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cyomlkfb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3qljsjctd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zunaytwv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hukptksb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ogivtyga.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3fvgzqpvi.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3jzplzbdp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ndcikxyd.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3wbskdkjs.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xtjngbbu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3oonvtpaj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3kbvdozxy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3xppmratm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3uwmjnbhp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3dilgtour.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3xvehdeay.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3jkpawbae.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3dmdwudxf.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3myrifxpe.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bbutmeqz.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3iuoaqexy.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rgtakpue.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3kauqvokn.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3nvazgpna.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3bfshtqhh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3dpvyogxv.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3voaicisl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3qyhgixvr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3qxtqztmm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3eevqcvwg.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3fivbjjcr.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3dctczemk.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3syimpatb.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3qaabqdnl.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3znlkiwhb.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3bcpmfifx.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xeffzmgn.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3kccndnac.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vulnxidy.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fzwfxemu.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cuyxenva.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ufenqozr.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3wgfograk.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ppkpcubq.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ckvfsnls.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3arqjrjze.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3yqvedonj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zgjdkjxr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3vftjveyl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3geiizynm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3rynxsmew.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3uglhgfng.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3qybiinyj.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3zvwsgnjg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3nmusubva.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3mjoijwuv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3avgvhvhy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3hbenzzfy.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrdzyffs.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3wnceosov.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3qwwqszaa.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3szwwcayj.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3oiilgqmj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3ymjxtnmi.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3izvvrkiv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3kvwtjxmc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3gjzbpdzw.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3evyomnlc.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wcswvhep.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3grgyfrtr.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3gapnxvir.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3irowigol.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3lzqcepeo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3uipgjpbz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3yqyfttsl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3cihnxamr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3yorrmtkl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3vigqheve.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3jywwstvt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3uihgjgvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3samvwugb.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3knfjsgnu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ysyvfabi.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3mvmioxlw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3hjfltpds.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3wagvtwsc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3qwwxssmc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3apiwxtpg.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3orplmpzc.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3zgtqjkye.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3febeotkg.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3exgdhihp.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3uzbunrkh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3ioghwujc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3qaeurkbz.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3kijicxme.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3xpvughpr.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3usjoegwb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3dfxsfnfa.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3dgaooqch.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3eqitxvuf.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3iecaskrg.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3lbcbwgmq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3hjpayrjg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3svnxzgtg.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3kakhvqbb.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3dreijiii.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3ikbczlue.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3pdcbmylj.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggeqxwgn.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3yxlbghcf.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3pvdkbodu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3pbnlipln.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3fzrpvpla.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ehdbmalf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3vvgxcaie.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3srzqergu.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3dxcnjkow.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kbsvmvtn.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3vikulcej.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3oflxplas.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3hmsndkck.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3krzjfwuf.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3xcmefzyi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3mgraajjd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3zffpctxu.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3rckwztnr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3bilyorxk.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3jkwfmsoa.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3syrfjyag.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3nrgjbsbv.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3zbkpbshb.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3tvfntmgm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3ufumabre.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3wuybyepy.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3aeqoxhhd.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3alnyinsd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wdxesdlq.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3nprpjcrz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fjrlyaxk.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3vwlfyldx.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3bvocwejd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3pacmfwee.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3kkbubjiy.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3mcakpogf.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3avjynxhz.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3mzulfnpe.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3vkljcsaq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3vscujdvu.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3mdwqfqwb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3xahwrhyi.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3wvsanwmf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3icmphlgp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3czzoyvwr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qebphabv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3ovixezxy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3zffqtlsm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3fnmklila.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3jgoyyjfo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3xuiddbyv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3kjjngqun.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kywljuyp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fhvorgar.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3moebzhgp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3ofycjvwq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3aekpiwsm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3gjsdawzn.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3karaajum.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3jllgetja.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3migshaio.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3qdjsdczd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3rcxdfkaf.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3uuayocdx.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3ifimffmj.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3rvzwwyva.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3qgqrjgil.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3wfcrmugf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3zgidslpy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3raojmkye.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3yhvjschm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3iiyojqkm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3sxpdnjae.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ainwmxjx.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3fiwtjids.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3hburgiqb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3vphjbanz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3lyjvslhx.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pwrbadpt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3opitjefd.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3jdlhkdpv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zhoajbdz.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3mvikyskv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3nubwizja.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rlxlwjpt.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3zxcjbgnt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3dslbggqk.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3bnauyudr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3zvketoyl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vfdazxsn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3imunckhv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3tlmzmxyd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3akihoynk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3gvgirniq.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3pyquuweh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3qeiyakqh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3hbgggcot.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3niojzfub.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ucsnzgfx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3wvuvabke.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3eacvrmxb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3ujlyltga.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3qpglzoam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3prdwezzp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3sexogbrp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3amjkqlne.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3evbwmlul.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3jtodttsc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3sllfrmmx.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ibzplgue.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3rarpqxab.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3bvvucezc.html

);
来源：http://www.52xcode.cn/Article/details/gt3wsrtrqma.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3wkxbjtes.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3bewaeskf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3jzvlnkhh.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3utcsxlor.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3ipfwabfp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3joebpmhe.html

);
来源：http://www.52xcode.cn/Article/details/gt3wpcqyplx.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3umlxmmbs.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3mksdzgtz.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3txhskkjq.html


<!-- 参考信息 -->