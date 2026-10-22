代发 wailian999

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xozrutmw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2ghbuymyf.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2avnslbio.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2hnonucgi.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2toslrljr.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2fdowvqdo.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nevwevzc.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2kszwvgux.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yxfsjijd.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hcdaisuy.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lirauduj.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2twfifrcp.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2njpzzmtq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2auuaeznx.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2crimqzox.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ivkvjyaf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2nyrjrplb.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ngphiqvu.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2opczwbsd.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wroduddm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2bvizlukm.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2uospnnac.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2ikdrkgip.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2lfnvyhhd.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2hhbqdkfq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2khocjwjs.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ihiaaizr.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2pfjacmka.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2ypwrkufq.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2xljtivcc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2gzqlzcnq.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2kfanpaed.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2jigayqtp.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2xzpntczl.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ivnygdus.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2cvknjzvq.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2rwwkckwr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2soitnsdz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2qwjjbqfr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ttneajmt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2jxdpzzso.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mgdnbfgs.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ymwegbcd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fbccitqy.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2wvifvujk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lhrdsvzt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2tktwhhqn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2byiydmlm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2cwryfqyd.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wsgripsp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nuombssl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2jkxjvyfb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hdtxfdxz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2fxggsxnl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lflydkxq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2ocqsnnve.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wxhdjfcw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ffadbdui.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2suhhpkfr.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rdwytxpl.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2aswgqrdk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2swwzdqat.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2eyspyeim.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2tqfillfd.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2hlehqbga.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2yghxxzgo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2hoqfbafb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2yvobalvo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2comigzho.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2avxtwrsh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2amczecof.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2xtnheyvl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2houqzsdb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2pqviaasz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2osexeckx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qftplcil.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2rgoyxucr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2lnagyeto.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2eqlgaton.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hajvxchn.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2zsioretw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2prnsfwln.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpxxrswy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnivrxpi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2rycwuufr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2zlyxmhlc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2oxngnizg.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tehftqgr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2loqnczsr.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ycraiyfv.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2cysjfjoi.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2gycyqfrr.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mdlmvnec.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tpnexfmi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2onxvzffu.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2qduyqitj.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vhovenoi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2qdjiqslz.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2kiyuuogw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2kmuroovg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2whnzimdc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2gontdzlu.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2fzqvaanf.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2mdkniqge.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2lmwjynyi.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2vzliuavv.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2hncdfmkm.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2yvqzztgl.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2egkgaipq.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2frmguomr.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rpguxnxl.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cvpclxnz.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zommgcth.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2skuosqfo.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2dwuszput.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rcwycwrt.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2jcxuptvo.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2yiiprqvy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2mfsmvrqo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lvmpfkho.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2bkhyhcub.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2djzgaczm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2uolykesl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2slhuvpet.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2klexszlt.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2yinxodug.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2zhgskfju.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2idpgmmjv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2ylakepeh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2ylnrklzt.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2hpxjxgwj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ekeuwhnv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2rkskvcys.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2zinmjymz.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2kxwkffeu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2koymuhsx.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2zzgtyrqy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2dgivzqch.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2qicknoix.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2nghffyan.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ataevona.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2pfzqmlrs.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xqygcqvw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2etijcraq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2bimalaty.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2dyygcsth.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ftrjviop.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2qgrebcns.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2raqqvezo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2atljywxh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2aeksbsvx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2uvjydojz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2atnlmvaf.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2klqjijtf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aksqhalb.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2gfkktqxb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2tyzbeujk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2wdkpquix.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2inieycdb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2prgkkfdh.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2wasumrbz.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2andawjeo.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2rsonugfj.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2axkucoes.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2yuuwiedb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2iodqrrcs.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2avafihps.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2jlvwmnty.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2kgjvglmh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2awihrdhv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2qmqwpdsp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2umcvlsqm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2xiqolouy.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2ytgoracg.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2vjdjdiqr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2wfxlsogw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2xkkjrezr.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2aksqfwzj.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjkunjnq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2vttyvgcu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2brqpvcuc.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2hgtqtarx.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2hmpqsrnv.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2ittmrcvb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2qnwnpnpq.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cqiiitum.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ozntudps.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2sztwrdwi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2baxqbioj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2hwbzbsqf.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ckefiyzh.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2qcmyhsxq.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2idipdbdn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2urewfoso.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2mchjorrg.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2aovbnbgc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2cvldvgvp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2qlkixlvr.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2bmlovhtf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2rpdomqix.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2tguklklf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2nsdmalow.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2mpwvxadj.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2zdcuiqov.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2yxmgpbvt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2vhebyhuu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2yyktfvve.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2nceyaexa.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2tgkmrgaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kkylqscv.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2ootqtyws.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uxnjpzmz.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2mufsriim.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2nwesrfzq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2brawwcsp.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2cfoasahd.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2edqigpwm.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2sgdiozkb.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2lebcamok.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2hbmiirau.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2nesyfgnh.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2allbmsea.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2ozhnvbua.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zmbmznbh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2pzqnworp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2rpdzujcj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2gtqhfwgb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2klyzbyvi.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2vuxrzdwv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2zbysareb.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2ijibttaw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2tpfkcttg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2enobzahw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pxzvmtoh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2zxjqsfqd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xhontscf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2mvsvbpmj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2dapkxduc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2irkfujmo.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2nfnzzdtl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2fdnqzfij.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2brriutfy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2afuohbwa.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2sxorvgmw.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2pkdncvhx.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2wutsxrcq.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2ssselwny.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2kklwdigy.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2ibcbxukt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2bxplgdez.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2jaxwhywh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2txjxpppd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2uszjnltz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2aummuqdb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2hlnhdnie.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2hguefwjf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2mbjckpab.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2qdjuxkrk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2lwebjkkg.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ysssmnej.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2scpdmdhs.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2hzflseot.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cbihozxx.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2ejmspayr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2bndhmjjm.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ittfrpzo.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2nhvdplzh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2rkykvnvn.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2wlxkxnwv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2jdkdxqvi.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2zxkgmbpw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2ajxzeioa.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2cdtlhlkc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2ascgsxsu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2wurvldip.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2ccsmiplm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2aduayzvy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jkxfmayr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2sepcuyeu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2nrsxghmq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2pwelstfp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2gujxwwup.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2qqmhyfpg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2hyhniucb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2akytovuz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2nmvporgw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ozompvfy.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2uitotkyf.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ezjrlhvj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2koshklhr.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2rmvyspoq.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2edqklxsz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2fclprkrd.html

);
来源：http://www.52xcode.cn/Article/details/gt2xgkmqqod.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2vbuuacaz.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2xsxyrfbm.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2tqtjrgnl.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2jvvaojfl.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2icxrrxah.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2pykejsys.html


<!-- 参考信息 -->