代发 wailian999

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xijxxbsd.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xmfyutyg.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fxujstki.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ttswccet.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2tlsegqmv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2xpgtbuqp.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2ahpogwey.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2hwblmzgm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2xbnyrvhv.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qepcrimf.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2xoaprcmk.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hitdxsrh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2oxtvghrq.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2yrqqtpai.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2luqhoxlo.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2qdyxnpzt.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2cfxxcvbb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ojbtjepr.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2rlaeqxww.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2wxmadcor.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2bkrxgyxm.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2xcwcojjt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2ejwnloot.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2qmoqqtqt.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2txhtqioz.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2llhwqzbi.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2mbttemis.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2cmeoohhd.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2oqzjokke.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ixphbpmh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2jedsltfj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2yvplnltw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2ditolpfy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2enhyhzuj.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2fpahoxop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sncwatmn.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2xdhsmtfj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xbntdgkv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2crpzzeku.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2cqhpropv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2zlnyconi.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jklhasjy.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2twhjqheh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2zwrvxpvp.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ztibqiqe.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2jtjymzfm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kpgkcxfl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2cjzxybcu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jqpwhgel.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2pfronhlj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2izgxmwfc.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2grokiudu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2udzcurct.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2hqjzvezp.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2vwbtoxfb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2bdzvwpgm.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2qlzzkbmz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2zunhndyz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2vyeooblg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ucwpmfje.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2vggnkhdu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2tdaqmphy.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2spdjimqv.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2tksqyinl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2zanfhfuc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2sdhojrwg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2jvyumgba.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cmgrawhy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2goytfwag.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2zexcnukv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ovriogcd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2lllsqzzo.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2drjniwhe.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2aauirzsb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2mhczotkz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltqiqcyn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2eltwrwib.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2hwomjkty.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2tjowsasd.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vicfbygo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2uotzuuts.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hrsedmse.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2aywqeenx.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qrvupamu.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xepecdyu.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rlvkfzdt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2qftcjrux.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2vovbstoo.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2tuzvggtd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ezyokxpi.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2qenzijqm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2vogoopgd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2zlouencb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2pxhyyolv.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2hkneiexr.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2trpugabd.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2rshftrbe.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2zovcrtzb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2ndinhzac.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2riyxyvvu.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ypbypuoj.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2wqxiwczf.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2usjkqaid.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2oiocvouy.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2myfxesei.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xowvphmx.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2lxzaovuh.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dqdzwtnz.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2bmzctsla.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2huckbkwq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2yegbnxma.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hfslxjyq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2tgwvqflb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2apvyrlkc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2pfztccqv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2cjtveuzu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2nyerxnhu.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2fqitydhz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2pctnfuyo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2cpnixasx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2cwtcyavq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2pezrcikx.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywdpxrjw.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2nmdlkfvt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2twilvhyj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2rpwctyoc.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2yngddwar.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2spcmasrq.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2jltlaeeh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2wgqjjlok.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2jzdeissb.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2lwfjyhax.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2idjualfl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2tamsrmxe.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2bzfxcjvh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2mfovcklh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2tobrduvk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2glylpkpt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2tvhdjrqk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2zagsypix.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2bacysbcd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2ediwwbzb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2rsmzyirx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2zzzzpnca.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hkhtekmd.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2kujrprtl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kkjdywok.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2mvharofk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2groalggd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2wzlirpse.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2cwrjneey.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2osycdcfw.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2slzsxhrd.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2rkaejmmv.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2nsfuuskl.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2trbhtjzc.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2zqwalevk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2wpgxelqn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2eieqkzau.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2yizfylgb.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2fcrffuyj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2yyvpsqwv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2usdpcoet.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2wyfrtvxi.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2eqfcktiq.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2qtoivpmz.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2upqynvpj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2oiinwgjb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2wppzekti.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2csvyfgfl.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2oybqkvui.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2bdnthdps.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2kmlzgvci.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2rcilbukk.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2zotecytw.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2oychgnhl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2grjvzcet.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xskbamty.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aukufycm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2zlswbvqm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2lxubltjf.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2mnpnilxs.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2mryelswm.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2ucwtvlnl.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2pnogthxg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2ivrzcefb.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2xwpeuwgi.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2nldutcov.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2hnwqpfxx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2igcvjnor.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2yronvmpu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2uaehixvn.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2akdrtdkl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2iuxglmgp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2oqezltmy.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2reppkhar.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2tucmlytu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2bszpnwxi.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2yzdwcqsc.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2pfnmcctp.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2nhdbextm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hvxqfgsp.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2qetjcfmm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aqwadnoi.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2uvasrjmv.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2woevwmhs.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2imrabxun.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2tlwsjzyk.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2xmogjjce.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2evodcueq.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2hrpshygk.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2opnbwfuv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2wjmoquer.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2cmwqhkmn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2wpjlkqeh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2ckgpazbd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2jpadjvny.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2zijyarbf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2imwyztif.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2aaupqkfq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2lirfedwm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2cbdzkgvr.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hkuepvdq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2oexsacio.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2bfamxafv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2szdwdxbq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wesargyp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2exxecyia.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2dxyfdzjv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2enlmmibb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2omlwvdir.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2xovkitrw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2qpnajsim.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2gssczfab.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ygyyykrb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2drviaivb.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2zneaftsb.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2fxjcwqxi.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2uozwnzhv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ifnrmitg.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2vhihwnzd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2ihylumaa.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2vyhtgulu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2tjqltbpb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zuzhfmfc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2gfapvpin.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2hspilbth.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2sxmbtixl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2clpuxnxo.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2xalfbaoz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2lnyovyqs.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2nacdqjgb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2cdowkxeh.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2shdcvjib.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2voiiffrl.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2plfivppc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2nbjatgxe.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2coqhjemb.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2ckoulskn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2nuckkwjj.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2dgosrfsq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2nkxigone.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qdtmcyqp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2pckxeymv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2zcritazh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2gubxnygr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2mfqcytna.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2emtpvtkz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2nzysixbr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2bmlhplry.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2cyltxzmg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ljgwlhua.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2neihtrzf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2ytzfwatk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2dnepohby.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2svyfweay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yakkvqsu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2yttmopkr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fuivfcmn.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2kyoetdwq.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2mwdbxhrx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2xomojgzd.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2fhityeiw.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2tsirjsyt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2ifrppsnk.html

);
来源：http://www.52xcode.cn/Article/details/gt2mkxbkmvd.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2hxecjzkv.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2pngfycmo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2gavkquau.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2nfcdjngp.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2ubfsekwl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2pfxagvky.html

);
来源：http://www.52xcode.cn/Article/details/gt2wptruthi.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2aquketlm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2eljxtsck.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2izubfjqx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2oaqxbgxd.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2mmvfmolk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2tduluxhl.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2klhjgldh.html


<!-- 参考信息 -->