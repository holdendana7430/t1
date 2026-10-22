代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ppeuaieo.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2wouporfz.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2szjcxnmk.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2vhjbjaia.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2efgbkgop.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2evqkwypw.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2snncgdvo.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tgrkzprm.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2vmlpiftw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2crktqhxa.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2dtajgxna.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ucmheqba.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2wwvwkydy.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ijnmxdjy.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2xxisvjwp.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2ddiqwpsc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2rdppnmcx.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2mrlfnvio.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hfqpdapv.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2pzedfrjq.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2dkiwhfwm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2brkcmtfl.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2qfzpdykl.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ddefejiq.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2doqovjjs.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2yetpcdgg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2clfmrwdh.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2dglbuyak.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ifaaxifz.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2buefpdup.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2hziknjhh.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2mftlpjbn.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2hhlzemyz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ujnlxhty.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2qcnenmsy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2mwjltgvn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2gbpbbqlm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2egkwwgbf.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2tproxnhd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dmegzyeh.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2hbzskgpi.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gbzaeect.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jvtuxhaa.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2nbfqolfo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2yzusjarc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jplplgaf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fnihbcks.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2srjvjiup.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gsgysnrh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2pxfdvowo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2rwwzvdfh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2rjazqjdd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2xqkjzceb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2qutmzgay.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2xjlsonds.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2czyitkzu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2oxbmorow.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2mumyyttn.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2yvjipqqk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2gpxygldb.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2uqchoclt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ybteoiuq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2cynqxtkb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2mzalpjab.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2xmvevhaj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2gtywaarh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2yutjurxn.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2fvtgynqn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fihvnftb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2vfregaok.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cmwjjygi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2aufqbhik.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2gvfpbjmd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2bwkdufmz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nwlzktpt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qrxjcedy.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2gwsgtzvu.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qtyiwfho.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wsjylutv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2reypttyi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrxujsdi.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2vxolekbu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2fbqehhvj.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2evunqmag.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2dsktsapj.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2plhepcaz.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2zzukooli.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zyrjtsso.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gktmohhw.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qtudapgi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2gocgqpxe.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2jqeiebay.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2gscjzigo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2iaxxvvzn.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2dqlzrknj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2wsqthjns.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2curfazlr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2hirkkcku.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2uyjrjvgt.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2wfzhuydz.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2dujtgtkl.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2knzjnkck.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2klcfspxb.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2hthwhphr.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2njlqtzap.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2bwzvqgno.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vghrqasq.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tfyeczpx.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2finzpove.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gcohaaqd.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2czkstbjz.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ugcuaebp.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2wpengwgx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lweydwwt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jmizdhnn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nmxgzffl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2fniswwmr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2kbcvblfa.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2gvahmysd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2hrhknmdm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2sycbbhyg.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2frsvdlcd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2ynheyiod.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2wbbdtkwn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2cflysmkr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2nvswudnt.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2kckzomvc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ofuaicck.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2zykphwch.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ckogjgrd.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2jcaqptlz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ogrnfenr.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2dxdoudfw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2zstrokph.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2cplmggzc.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2kpexldlu.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2vtwhfjvg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2ehsubrkn.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ualxshsg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2jzyysrvw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2jfbjdkhw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2ocfmarii.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2cmhevmzu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2hrijwgws.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2waqmdijv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2nzagjtmj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2okvaolia.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2xraqkveg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2txihrxro.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2qgqwjjir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jmqigmep.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2ttkksvsc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2itajsvrh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2bdpqiqvz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2ypaaidto.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2aplfmcot.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2isteaqxj.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2yqsekman.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2funmfbud.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2hgglvwaq.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2jkblwaex.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2zjoyfmme.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2omauwwiv.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2sowyxqqo.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2psypjioc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2supztlmd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2okcefrfb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2zfqtiygh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2jrgzcgvk.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2fwwvuzua.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2qovgbsco.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2lbcggqzi.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2crbeaydz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2eeuhcqvj.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2goeddfrp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2pkhfywkg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2kcscdksj.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2zpatnaum.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2gxuesvbv.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2kdnwzztk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2xjfbaiil.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2lpmpyjgk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xdhzjncf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2uovwgiso.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2dohepsap.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2jpnyiytv.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xyuluysn.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ouxxugbl.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2crqmftuq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2eoyyvaam.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2htyxbrrj.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2hszpesfj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2ogmjdydm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2fqhbowam.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2xskyvceo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2wuubzybz.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2bybzocxi.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ysakjydv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2zucvcldb.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ckuctuzl.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2phtorslk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2imffbstc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2skyovacl.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2dkworhxj.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2ntobzvrt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ikkppebd.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2yixregui.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qtpgynwx.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2mbysenbh.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2xkxeddko.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2chhnrxcj.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2iviidzjg.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2jdafddwv.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2bhgdowjb.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2sfsmrlcy.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2eolppudw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2kyvfaray.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2mecoqlad.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2jlopgnck.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yfnenysh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2gzffvihk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2tlqzacii.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2zuhqhear.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2bwgzycsh.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2usuzadgb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2gbypecpe.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2stwptxit.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2rzybibyy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2xhavmgca.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2prjzjwva.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ilkvwizu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2tulhyhyj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2fsrzrxeg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2nznpfcah.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2lotkabqr.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2tqwvkdkk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2ztwnqbpl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vfhkjrce.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2eymfsewi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2vioxzhlz.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2lyrcoosu.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2rdbegivb.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2pokjjoav.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2dhagyrcm.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2xzfluztl.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2ozcivujr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2dmtxbzfp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2vgmrwdec.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jhubgqzs.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2qjzkzkim.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2annzjjqy.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2owfrldgr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2tubduipf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2tmzbdtcb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2btoooten.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ipbjkeuy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2bgojltsa.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2dqbecsde.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iftyivbz.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2vaquxvdk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2mwkzpema.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xzebnxim.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2xorxvtos.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2negapvhc.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2chgirdwp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hfeogiwb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2qkhhpxaw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2wiqdisbc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2tzwnlpip.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2usqtwjcp.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2wxlurxqh.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2xbgpauha.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2tadgqygg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pivnaaut.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2jdbaggqg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2viqqlbhu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2ywkorgmr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2vuqofiff.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2xgmxkszx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2rwaqffar.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2epwjkubc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2oguqjqva.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2psbgzgiq.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2ccjvdolm.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2eexlablq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2bbydudyh.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2olzcnywe.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2eowdmoqk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2eucudznq.html

);
来源：http://www.52xcode.cn/Article/details/gt2wxjulzhb.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2rfqqfoic.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2iygavavf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2sygfrede.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2lwieffca.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2vgbymvfx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2qsplyjlv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ohbyarqd.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2wkdcnhex.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2ecmyjszz.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2xuqqgfut.html


<!-- 参考信息 -->