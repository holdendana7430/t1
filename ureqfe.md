代发 wailian999

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2oyebtkce.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jqepslci.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bjnnydeu.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2effbbxab.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2alorpnqx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2zsyykeeu.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2mbmutagg.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2vvekmrlg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2nkjztwof.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2jgxtoxps.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gplbgxbt.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mjafmewv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2kdmhqhwx.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2kinviuhh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2trnvonoc.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2lxncrgil.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2qqduqsdf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2yypvgbxd.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2koqbvsmn.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2lxomsuqu.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2yxiiagvs.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2kkrqgwnu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2lyubydwn.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2eyuqoyme.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2azfxaxae.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2dohjagqk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2spxczlqq.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xrhhsklw.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2amfbqqyc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2hddktysl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2tlboibtw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2pnrqfatp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2hrqgpilg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cvujhopm.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2udtzmnbe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2afmrnzld.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2mozcpfru.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ewuhbzok.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2aflgfdwq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hzlkqkuv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2oiuxddgz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dqaxsqyj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hkymntee.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2mkgygwyx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jlqzxieu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2gjlzzssr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2uuizvghu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2gwfvjles.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2peipyufi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2isrxstqb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2euulcfbq.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2vffbrwtc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ibjqpves.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2xlcnpkws.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2lphcxzzq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2qtllzszw.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2kjfdtzgm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2inanerto.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2tqvwxqqm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2kvalaauv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2criplfpv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2apkvamqb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2ziyvanwv.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2xwjuzfgt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2bgsyeixr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2pyyjnwii.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ottjxtel.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2liholsvg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2kqetzojv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2eaifqrfs.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pffhcsel.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pmqqoiir.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2lxsqogrx.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ovhjrwgu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmgqganc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2lzmjeynn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dofowuvk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2dpytybph.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2uptksqfl.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2psqrdkul.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2felqlqra.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2llcgnztm.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2hxaegixy.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2mbnqjqhm.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rrnvftot.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uwwserts.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2aifamuie.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2wgiirrsj.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2beiwyrcg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2qfibogwg.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2bjvnrjca.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2prakzqzo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2dqjjcxku.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2dkhpoahc.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ssrgxblp.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2psdycykp.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2nwwrcpee.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2zdusyqrm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2cknpyojq.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2rhlpxmsg.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2ffhiaeyc.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2jtgolyad.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2oftuoerh.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pcuabakj.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xbanmspi.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pkzolktb.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2irjhjvxq.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tofwuwej.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2lsdqmlkj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2tydwooyk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2nqzgctdj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2fxnfkemk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2cwobdtcn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2gbactjgm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2uxyzdqsx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xnfonfyt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2kqsipleb.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2zfsyborl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2iiyqsvmz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2maxqywmn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ejgemeqe.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2tktcyqey.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwjnjswp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2ldelwyzh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2cyzlryue.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2vihnzqqa.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2ouoginvs.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2fejyyarq.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2goyyqtgi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2lonfipcn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2wwputlwy.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zmmnepfc.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2uodwknym.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2fylaxiqx.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2hpfpszdv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ssixtmnf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2zoxyjxqq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2zhmqhjuc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2fhymnppd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ykvvngwj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2tnazdkvm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2qcdxsslv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2bujsbski.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2qauuqtzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xazhcjnm.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2nxqnahbp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ouvknevm.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2hussbjwj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2lupnvtsy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2grsdeynz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2hcjqjthj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2pgzetpin.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2winyvqml.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2datzynny.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2bmbexdbv.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2hblotzmp.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ktxhhotl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2tsziuycx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2gnqeqdwn.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2oesbyqjp.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mbrrfmyj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2mznxcmgp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2mvltqegz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2cmawizez.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2irvqxviq.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2kpuwgisw.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2unaaquqy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2trykmmvd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2ifrsclrn.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2mkbgfbjp.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2kckyjdoo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2hbqpxkde.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2wsedgbya.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2pbutppeg.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2whtbnnfx.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2iptobnnd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2oephysmb.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jbozkumg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gejawhbq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2gsvurshu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2nbinskfi.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2pytlwehq.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2gctsxsxo.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2vgoomocs.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2styqllri.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2qtwguxkv.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2aqygiidc.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2fydsoilu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2mijcbzjl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2lramvgtc.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2thbihhpu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2poglycti.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2sbttlxlr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2koqdjprp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2qcymadyg.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2gawurfus.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2xgyfcnfn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2dwfaxucq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2rkkejovw.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2yasjtozx.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2nosujcdo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eiyssakw.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2jmimgmfa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cbcobeej.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2qzufsnie.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2bdufevru.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2sxnyisul.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2lqwdmwhk.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2uzyfpabg.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qsiamwec.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2zcnxerrz.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2gilidoqv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2uoguqydj.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2yeniwogj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2mnrzimwa.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bwcenpdd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2cxlqqxdx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2grmqviik.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2tycuhixl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2uwufknik.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2clqrsqxx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2xvdvldqi.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2plxhapba.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2rsmrjavh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2fxykijpn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bfcajygt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2bjijalsu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zppscrhw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2txkeulmk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2lgzbaaga.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2jzndyafu.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2zwvmqyrn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2unijlicg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ccofcnkw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2nwqldzbr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2rvapoabh.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2zlugfhhr.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2lfcqusdv.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2nbdrnkfc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2argxsqml.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2flhkpvpz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2rbpyngit.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2hfmjcxfl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2jiiqobjr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2cntluhcl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2uajrutfb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ddpymlxe.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2krbjujyo.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2dyfnagfd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2uldmrryi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2hxwgpyhx.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2cunnnnbt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2snzyqoct.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zxysmxof.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2yrbpxddf.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2qhjsshgo.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2ufvzptdj.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2jnyndgbs.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2hsqirywu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2fmbjthsd.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2parjmflh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2owojgreu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2frzeammr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nwtknhyh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2eyihcdqz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2rsfsumnf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2ytwjnymx.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2vcrwtpjn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2rirqzmkz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2igxiwtan.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2bzxukkaj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qymfhbyn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2owdiehcv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2mmpelvbp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2druawggj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2ejrzsgbe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oxgmulbk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2acpnhnrk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sihofqwa.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2ttjzxtyr.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2xqowedhq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2qqafpzvn.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2wfotfpfv.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2yzdhoqbh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2aqnmvifd.html

);
来源：http://www.52xcode.cn/Article/details/gt2rdapjtdf.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2qsnwyvqh.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2moxhkimb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2jdjxlmii.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2icialpza.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2jnrbsqsu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2zejcqzgg.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2wdflbzsn.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2hxjlgafw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2hytsupmo.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2xzmwtush.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2jmofgysb.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2vurpwicq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2srlzbeqk.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2dtjmevsc.html


<!-- 参考信息 -->