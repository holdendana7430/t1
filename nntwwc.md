代发 wailian999

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2pdibexmy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2diknswla.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2rxyfxazi.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2yqpfjxmd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2odjuskap.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2qaidytjh.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jxlmqqdv.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mgxeyzlw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2kluoztea.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2nfunxpap.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2yqfozzjd.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2whcrszqz.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ovidpotj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2eqydoftd.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2dnmksyaz.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2xcjvrlpu.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2jkngqmky.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2rrbsibuf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2lfrcdugu.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2qbmaahpz.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2qbiznrrn.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2ibmvoihb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2dsoddmri.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2cavwtccq.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2nnjninbc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2gmqavxpx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2kppulyhs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2qozugvzn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2tahstcub.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iicxwitp.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2igtaabzm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2asqflyze.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2swmtqozv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kajgswjv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wrnunxkd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ckwejrde.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wgkypkgm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wnbbjdon.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ruwzyscj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2cnpxazxa.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hwqmjiyw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2hupmnohq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2nuububty.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2asxpunfb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2qgsurfkd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gtohtrfr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2lawapdiu.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2acdwfwrb.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2jmcgdqsb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2fxujuypf.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2mdmridub.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2rhfutbyq.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2efhjblsm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2bhhejdjz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2dindxnef.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2iydtklly.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2jbdaprsm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2glvozuyq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2arkngdqv.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2hfqekixd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ryaivwtp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2auytvwrf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2dkufcpbq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xyewvbqo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2mpqlhaae.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2rhkdwlby.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mcrxeqzo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2aamqrrlp.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2bjkdzhwd.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2tepbctyq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ooniuaxg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2soqjnzvu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2rgqxuapp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2rkibidtr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2cwunpbce.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2thuyjybf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2nemcxezl.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ndultntx.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2cofhgsul.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2lrapbqrc.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wczdwgpw.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xbvdsujg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2pxxmzgys.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2urllimhv.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2eomotdea.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2tmypldzc.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2dmmyzudk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2uiwsenlm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2jannyabh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2phuodtpe.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2cajhlgyn.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2nqetixsx.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2iutkzhhy.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2orupyozm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2comgjxqa.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2hgnuiyzf.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2abhznmzv.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2jsesbwyz.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ofmzwlvb.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xgubiigi.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zifpqvvj.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hadglwef.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2dpooqhvm.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2abdkeyjv.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2nyoxgrch.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2zywievgg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2pjjimhbh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pwckbube.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2lkxmvguf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2mcibfzum.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2uictirbf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xbkmetkb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2izfrfqrf.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2mfwjlpzh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2meearrvh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2iiceosxz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2fxccrueg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2zymvlxmf.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2gcuvqaob.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2iuzxukjf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2ndvcouox.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2afmadnww.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hwytcfug.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2aamcqidu.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2rtdmsdeu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ewpnvwsi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2iaxxzamo.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2mqiguaye.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2wxmnnrwd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2eznuhrtn.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2aqlzylqc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2kehxdtsz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2pppkpepi.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2jqgjyjrk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2zqpadtcc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ysbgzpaa.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2xaouojdo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2dzqxpxey.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2fwozarth.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2yyiseohn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lbbgoqzr.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2zowdgbvz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sdbkkaxi.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2futthzjb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2barocisx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2bwotbzwe.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2rvdkruff.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ksafifce.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2jebmpfox.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2wovgudcm.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2yehbvwmf.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2clbnmsxt.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2fwekvuqe.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2okvnpqix.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2iwcnxkzn.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2awhukloe.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2vrqrovix.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2zmsdylrq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2dsyzzzfe.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2qhgtgluw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2zhezrqyh.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2nwookkir.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2yijyeyzm.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2zkrtnggo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2mflacfga.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2jvqsnjxb.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2pjqpnqhd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2zcyayvdm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2jtdpqcfd.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2zsudcccq.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2wttaklvl.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2funfbcti.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2gqoofnyk.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2nrpsgktg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2oqynkmbe.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2byooqpwh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2vwtrlhxv.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2hhbaqpcy.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2guztdiht.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2cofdbuuf.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2ehvtutrt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2unzjdqxt.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2yeybfixd.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2njenyfae.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2svurnqye.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2vhmmvwlu.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2dhjrgnme.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2upyzdblk.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2fuswohxn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2cjhzfkqh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2awwnssws.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2dlygqekj.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2igekdlbe.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2affagqye.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2xufydqig.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2xxxphcff.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2onldmkic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pmpltbzp.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2qmurbaae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wrqdoghy.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2muntjxcq.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2zgyagskp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2lcoegpsf.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ekxqzybh.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2upjraipt.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2lvonmjuj.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2bqcuguwg.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ynunhqmw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2aqbxcmwm.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2ikqepvwi.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2kctmwvjs.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2bxpynamt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2nnbfqyty.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2tnyvfych.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2bgjjdeou.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2qxcpbaoa.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nbtdrxmo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2mubbcezb.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aolibscu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2xwgikmyd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2zcmxinbm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2aujaaudn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mnagrude.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2afisdxjn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2uzaigxxt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2pwgfmtme.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2dgxwjvzd.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2lfkiytlm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2rpyanhst.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2pxrpirej.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2cyhjvrri.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2tvtmduwq.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2quiqfhar.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2amqwmkiu.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2pvdcthgy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ngqbpyyd.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2vvuetslv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2oyskcdbm.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2jgoionhc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2vshwytua.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2zsbcggri.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2ztdkhlbw.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2usjqthhq.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2vmalgwri.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2curustni.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2itedrukw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2hosybigb.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2binxikfu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2xoojjfms.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ustmoejy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bdfwnjuz.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2gmrtocgp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2asnxnoye.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yclutlox.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2mbrbbroi.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2kelikujw.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2lamxxxeu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2akwfiggd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2kflcbpqe.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2gnivtpfd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2mzlwcbrl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2kyswhjkn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2ybfuwlfm.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2lohnsilq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2jzxwyilm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2fznbuvab.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2bymbwalu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2lkjeoxul.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2jvzlntvz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2ikreurox.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2qoizsiwm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2kpyccfkt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ukchwngv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2munjvztm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qzotoktw.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2fvfaprck.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2rzzuujdm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ewcwvwfl.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2xqevvucz.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2qtxigkqs.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2jigtuutk.html

);
来源：http://www.52xcode.cn/Article/details/gt2bzskzymb.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2lwyvoomr.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2zfbvataw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2fvaicxgq.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2zummgxnc.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2upreyxdo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2kqvekfqf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2fmvzomsh.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2grdxrduq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2dikkscxu.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2vxjfvlyy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2wlerllwq.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2duxzgquc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2rpsdjfiv.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2osgtkzdm.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2qulxdqmn.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2ctngdobw.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vqfdgljx.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2fmkuatoj.html


<!-- 参考信息 -->