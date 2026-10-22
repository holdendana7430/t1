代发 wailian999

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2niqxmvnw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2ksjfrxap.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2jqrzyghz.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2cpjmrhsc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2aorxaoes.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ifslhygn.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ymqhcokw.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2nnnhwpdu.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qmjncwls.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ajphvchb.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2afakdtbo.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xrjncuso.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2pxqlymsw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2dyrznnba.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2ixfkuybv.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2tqesgmxl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2anjtzayv.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hztozblg.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2uqsyuwev.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2cumpqnpi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2ftyxjigr.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2wmasbrjf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2xbkghrpr.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2vacvtxjv.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2tnjxglyt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2vcyedmrl.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ixwszsyn.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2nznwmpif.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2tnvxhzqg.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2uwuqjodl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2ksnfbhac.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2pmdurgco.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2fjcpufyo.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2veeovadm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2nubideyj.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2qmobtxoy.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2idbanhog.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2uupgbpdc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2anetevft.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2gbiemokz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2ubshzyiw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2muawvfrb.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2jdehbudu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mlveinlg.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2qxroxqeu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2komhwqjq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2sazwzuhf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ruqcaxur.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2oagrsqcf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ikkwzezx.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vzpxazbo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2hrduzfvg.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2agjlhwwo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2jlqylymb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2cdwqyloq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2wetqvyqb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2vvfsuqno.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2efxvndei.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2ikfalzpq.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ccvugzny.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2jzikaznf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2xbtpexdq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2pvgyeenw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2viwpsjpl.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2rtuwhvuh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2hvxqcoci.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2hykhpajt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2bechwitt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2ilpuiojv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2pvexxudc.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2dxzddoeh.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2rqepviev.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ydulyngo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2mbexhljb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2euktvdae.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qsotmwet.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2mymukecl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2mxvqapll.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xwqbtqvy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2lnbhkbkv.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2qlbckrwl.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2tvmyqpuj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2fzrogger.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zexchbzf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2xjqwcmez.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2qlquqgwq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2cngccfux.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2fvoitlqt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2avccwvci.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wvkogdfe.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2aopkvymm.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xxlgkwtr.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2aqlyzdzc.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mkwxppnk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2rdxbprte.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2azpwqyjr.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2jnhywxev.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2mbzdvawp.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2ycunjmlm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2xxsqzugn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2wooraydn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2zkoxsvzp.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2friwvirc.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ffsxhctu.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2dfimjpsh.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2nisxakym.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2ejsvyzvb.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2dwxeylim.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xwayylfy.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2xlsubbou.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2uagwwwju.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ufwojyhy.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xwconzfm.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nfqahygo.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2ghwpqyod.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2njsngiln.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2fzquuzmn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2almwmpuy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jvydzsva.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2viainccq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2pwlzwjal.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2roqnqgev.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2oymbnpgx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2lcdnssvx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2nwzsdcee.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2wesmskkr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2vawiudme.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2ghrszwkx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2aaszicqz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2fbuzzhwy.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ecqliqbl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2hnhloxdp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2yuerimej.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2cztrihct.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2jaodnuxj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2nbrdlrdm.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2stbqygrt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2qmebonjg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2wkoyajeo.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2anlladgi.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qqtwrxoy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2lovspzny.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2tsppnqez.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2dheyalcp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ehwwortq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2sztxhocw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2pbzglnyk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ygcmpnyb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2wodzvpsx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2qzezqysr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xxkxduei.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2zdesfyrj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uyuyiqth.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2jzxarrlf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mnnrjeic.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2gbzcalul.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2paywpelp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2pxlciamt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2qwbmrzdn.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2asuprvfa.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2vcpyuylb.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2prcynmxu.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2norttqxl.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2kjegfkfs.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2wvvovqmz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2iqeelhfv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2txbgteou.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2skjkfnit.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2vzgrrwer.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2cxfygtok.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2popnxucs.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2qecvwqrn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2hikvkaal.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2aicafrda.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2safzmjnh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2rxbymoto.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2buthpujr.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2gmzwrtrq.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2oxbjlxoj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2tetcmxrj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2zwwycssr.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2illgexku.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2raynwvhh.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2ofovxcfs.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2wassrpch.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2lwoyixjo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2dfyllleo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2rrmfxurs.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2qlgjelwd.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2gdswvieh.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yuopiuzs.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ncxlqqtk.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2lmjsfsod.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2kvmgolly.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2ozpeeqja.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2tnvwqcyn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2iahyvfol.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2huikebcg.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2thszesxm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2bzersnau.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2sreinvtv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2louazzue.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2zvyoerae.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2yjlxyysf.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2tgaifwzl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2crzjgblc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2rnabiznr.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2wwisugic.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2wyeimmno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uxafygbe.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2vwiiougk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lujcyrwl.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2vngggxez.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2revfgiyl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2akzcweae.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2irqumvtj.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2gipdemwo.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xiauavty.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2vtmynjhz.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2uifxtyie.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2gprkicgz.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2swcpdjjf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2mpswtksa.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mmanotli.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2vfipglse.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2trxavlhx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2nabqvcal.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2rpemmwnq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2noovmtxe.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2yegdqfbm.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ylfmvmjh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2bwiknmcy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2wimfqsux.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mbnlsyoj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rbktmsbw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2uralbexj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2hnuflauy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ceblnxaw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2qojirzga.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2qzfvacep.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2wzsvpyzr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qwgggyzr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2lipjgqmx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ryisnlpg.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2emogdmeo.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2nxazapce.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2mbjwrgrg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ucurqxxk.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2shzlgurb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2ojlxgrbw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2dhozegmd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2oqwwxrnw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2frrkbkfs.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2nsavyohw.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qaczcjnx.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2vldvfqjw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2cyzsilfi.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2rhuihoyz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2xbajbyhd.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yqlmzati.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2wbsknrvw.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cgrzyizc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hzqouofi.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2fotzbzyw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2diblnbxq.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wsgjbasu.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2bvaqdlqz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2mlrtmjxe.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2wvolqqoz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2coldpoui.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2cwerbqdv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2yuqdsymh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2mztzfvfm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2fddiqcqs.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2wulqokzw.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2wztbzqbq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2jvbzxluk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gqhkppde.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2efkxqoyc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hqejejwm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2dmluvatk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2jchgjlvj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2tvrumxnw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2qyqusgkf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2acpuhjbt.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2eufobfvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kmrcjpsh.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2vfojpati.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2xahnwbsu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2lkbaxuiv.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ajkuibba.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2zzmgtlha.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2xatypezp.html

);
来源：http://www.52xcode.cn/Article/details/gt2kgitjlkd.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2xpjylfun.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2bsqqzarx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2wuftluao.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2rjtljvmu.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2bfdgolld.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2xwzcifhh.html


<!-- 参考信息 -->