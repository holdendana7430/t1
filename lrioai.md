代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2xsfifdiz.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2msfqactb.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yrfpviix.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2qygpvnkc.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ulilsglt.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zjrjrmlt.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ttjkdhrt.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wskcoibr.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2ppyabati.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2jeifxhfj.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2fnwiecxs.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2giunrmgf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2caoemnzg.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ygtpnyee.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2mjvtazhd.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2kpcbhyqs.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2rgkvwpld.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2lorvinez.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2syzwfhwl.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2loromipc.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2qncjrcfp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2lrblzuof.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ebbkotql.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2sayonucn.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2nvkvxsbq.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2hkveewzw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2dmzinikb.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2phjkntki.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ckocvvcr.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2rxtpvvgi.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2qnarrdcn.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ewxqhohp.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2qbtasjdz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ebinzbsx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2joqkfbgs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2pnxjtjqa.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2opceqopu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ohtufuee.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2nzghyxcf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cgulrlzr.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2xbmedhtv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2apdhgicv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2alwhjtic.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2cfhvqwzb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2iheibvff.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2aahfgqnt.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fosegobl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2wxofclqe.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wmspnqea.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2qqktgybk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ypelwqom.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2yxcqacep.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2rkcvqxqw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gwrzzlei.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2nibxawkx.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2dvinfdsm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2wbtdqmgp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2lomerorj.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2wsllapqg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2oqcnbyko.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2molqhajm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2cycmqmku.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2rxiapklf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2eixybjig.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2jnoxekks.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2hgtmezmm.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2rozrgkmx.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2fogsbpzr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vppolami.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2vjrfpafi.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2tdkkwuhw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2agviiilw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2vbuqjfxh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2scjtjmkd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2stxmdpde.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ujhsxaxc.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2rmiibczh.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2hghxrwrk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmdxdkmt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ulxlxwvq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpyvvnag.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2andiexme.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2jieumxeu.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xwruhbst.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2zpsqzgtr.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2gxizgtay.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ertbqoqv.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2miflrhhy.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2unqvumte.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fudavhyb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2mtsbxtdo.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2kklzjkzt.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fkvzgcvg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ospdllur.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2lnhacbmj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2olushfss.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2bjnhxemw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2bcwhrygw.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ohyhtast.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2kkftaigu.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2frlpwmgh.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2xfjlgmki.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2mowcymao.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2jjfalfjf.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2awtygzit.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2nzsrohcr.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2stmiostp.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rnxqgvnq.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bqfdpjws.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mkbqvfpe.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2eyttinnk.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2njwjpwyh.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2hrccqlmg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2uysyajkh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2sksoddud.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2qbyqqvfk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2uzmcyhrs.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2zzffpblq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2pwjqrfcz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ooupeyja.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2izjljvcq.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2xtqpjdhz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2tkqxtmbg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfzvaeel.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2sajncofu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2fgwvcbyc.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjsaaqgm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2gssegvpb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2itxtsefz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2nrjxkngi.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dimsjnxe.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2quzslyro.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2tgdnamsi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2vkeuejbi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2rterzbqv.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ftkjjtyr.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zeylcpka.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2acjlmenf.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2burtrtet.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2aadyoyia.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2zfzqapej.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2rljgrtsz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2pvraatpu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2dvywcwur.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2xhdxcmch.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2fidgdgmv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2nhcopdpr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2dtwzadba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pfhxnywe.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2dpimgaef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jwifbkbs.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2mcwujfsm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2aunoozgp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2drylewjc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2jfbohbrv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2lnycvtit.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2xhbvcmqd.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2fpviqudj.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2lhqzqpjq.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2uugubnny.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2blhdpbte.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2headyvhp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2ipjgiica.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ututukyh.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2bbbopchz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2tmvfikkt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2vaibktqs.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2clisvdva.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2fcguiqng.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2kjccmdff.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2zkyszerm.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2lzxsvoro.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2pkmpfxfe.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2rfrvqldy.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ttalnmoh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2hhsfcpke.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2mpnnqtfk.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqoxzqeq.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2gycueojc.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2fdfanrfe.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2bjlboujb.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2cvtemigx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wjeedxhu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2cxxllwxa.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2sdqwucal.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2klyjfact.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2wruqrdyf.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2rcpmsgbp.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2mnyxbtka.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2tijnjppp.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2pniukaxs.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2zqyzpjck.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2zfeqbvjm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2nahzldws.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2pscpndah.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2cgszrfip.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2gdeftwnl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2lvdasgnn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2wdhomqjl.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2kejmpfor.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2rwpjoyfk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2navikwgv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2yxuqnoxt.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2mrjqxvlj.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2toqkoxmp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2udysannw.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2sjziyyef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cxsltagf.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2pawncjht.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2dzteodyc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2mxbwwryp.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2rqfqxyrz.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2anohcfid.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2zqiuyvln.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2xxmqdqsd.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2rgqsgeyb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2kswjrbjp.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2zjvmowzg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2bxcdiepz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tuvbdcmf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2vkigvzdt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2nehqbysw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2fwrcrael.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2vlsmoitk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2cfwiocth.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2fhbiedsu.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2iflmrika.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2ildkihbz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2dczihiqt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2dhucjpps.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uopxqdhk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2fqzwgnwh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2apusehiq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2qqmociyv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2mhainhmf.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2rmedttaw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2epoqdukm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2cnqwokcv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2oauvtqqk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2tyqxekli.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2cwrqkpux.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2ccvamdwy.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2cwttotki.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2qniiwxvd.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2astogymd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2bprwhogx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2tdjbtjda.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2ewalpxiz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2qtzqistq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2jbwybssn.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ixzmbjwr.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2sllryktc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2pqccnwel.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2vtxuogsc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2ykfeapfh.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2nqaphpln.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2bqivbcmq.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2rnjimhac.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dbljdzka.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2opwacmzy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2gangtbjh.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2myaaodpg.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2cdwkjnnk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2umpgyjca.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2yezbcvde.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2unqeawis.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ufbcpeqx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2jspllkpy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2oynoogfw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2fxdwglsl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2eowkbvbs.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2vytrwilg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2oirhqnoa.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2qdpjmfzq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2ttfsxrat.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vgsrzrgl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2qldrscrv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2ykitylpk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2yovnbqql.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2ftujrwwx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cmotvuve.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2npauwtxy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yupkbqfo.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2lrezdcuu.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ycjxpyjv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ztdcylfn.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2bedczfjr.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2nigfzrmq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2lttjipzg.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2dppywasm.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2mnatloqw.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2kplpwfpz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2bangvbtn.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2xvpzwqie.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2kvnwepbm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2vcohcqdm.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2bxsqmved.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2ieeywide.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2bvwtyaco.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2krveewqh.html


<!-- 参考信息 -->