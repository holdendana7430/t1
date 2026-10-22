代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2bbcuwmpk.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2fpjehwfv.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jyhvhaoj.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2jcotwppo.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zkgwdxkx.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zgfauibx.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2migvmwhs.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2clmyefax.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2wtwwnugb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2rekgpfgb.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2dljvgzoq.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2dxwgdjzk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2bauowmdq.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dqgjzlch.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2sekzjssf.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jzttsner.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2kzhnwagq.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2hzhyfusc.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2ofywuqoq.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2btobqnmf.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2kkjwkhpp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ykgjufqb.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2jxkeaswb.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2zbjbzzdd.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2sdehhgcr.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2gflixcty.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2aabuzlfq.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ybqygaxe.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2zgknelfx.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2wnaajtfo.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2uzhvejvc.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2zcifbrhm.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2hipytsxd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2guykaqrv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2tdnpdhkr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ulhhftmg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2qqmslsth.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gpgqcemm.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2qfmxpixe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dcoyrspg.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2qntpwycr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2khguboaq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2kkhwpual.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ivfsdkjm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2pospaqbz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ndnlzecv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mxzbucwz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2hjkzxbob.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fhvvdyyt.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2kfdodrjw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jlyrzxrf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2pxplygwp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2mcgoabcf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2bpjrzoqo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2ttnbrudt.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ugbbtbke.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2rqshzxzc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2fkmhntlf.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2kbstomam.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ogufrefg.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2anqgaepv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2snslpiyn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2zrfljami.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2bjbgbajj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2ztgjpgvi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2agujykhl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2zfblfofo.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2sueolqos.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wgftfsag.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2brgussqt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bmlpmhfl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vpkijhrs.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2qpppkufz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2ddelzapq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kwxhmrhq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2clhjjmhf.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2rbawqwbv.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2okkgunko.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zsobkrit.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2kapzjdoo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhazyvju.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2kqdfovbt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2gfhlyywl.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dupxabni.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2tfrekqxi.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2wncbnzbm.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ocxbyqqf.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pcelfzdn.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jublwium.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mpymjnxi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2sjvrwbxh.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2fidweejd.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2gyopwflp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2omsjtuij.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2rqupvtrv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2jazisvrp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2atrxdfkz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2zbtvtruj.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2jfyjelck.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2wdwtnuxd.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2ehrniuhc.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2belawrel.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2aiyusabi.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2wmwhwsvs.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2shnjnins.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2miqnqvww.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nenanxqf.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qfvvhycx.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zqnyeljy.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hoygxxop.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2qtfhhbry.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2oepvkzqm.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2atjhsbvi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2enioljib.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2lxzrefns.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2zdvelzwz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2esrvywnq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2vcuxgtfu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2waeoywqz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2dkxsxtgb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2zkvqbpxu.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2oxgahsso.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2pygncdum.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2chgnrfmj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2hoyujloc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2sdwmgzfg.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjuuwidp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2jvpzglrl.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2tfqzzkqp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtwfkfbo.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wygyxefh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2fjvuqfev.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2jzitjmxu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2wuqneicv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2trzimype.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2bjewifkh.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ufwilhua.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2sjscgrcs.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2tmrkxequ.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2ypzugixt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2paeraenr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2aqsbdjzz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2jvuxybjb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2cugjungu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2tidxvtxy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2hfyapncp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ujzvkwhv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2lejmgsea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rndhtwjo.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2papkmwix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nddoddwm.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2miyazvpd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2hbtagget.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2yyonlrqq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2smajtyuf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2tbvboepx.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2hjmmhiti.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2jsiytqtq.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2hqrypoyp.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2ftdxltfh.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2vbobgcqb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2bdsswsiw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2plrooesb.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2lfiwywbn.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2pqhsztkv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2rjlalomu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2hyupndxa.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2inklrsng.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2lybitizf.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2lgatcnou.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2svkrkmmn.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2jcdieicc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2adqtqxxz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vxzzniav.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxibfbpt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2mcipgzlk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2wlowprbr.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2gvkxuefc.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2rufzymse.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2otgpcnen.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2lmlxyxet.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lkvdtftv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2exwwbzrb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2uxomhmzo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2zuwkpjvo.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ybnfnhbh.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2tiurbtca.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2fuhedhms.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2fdqvlyzi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2egllcfoo.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2buwklpmg.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2gnqrieqq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2hsdnqrzz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2jfpctqqk.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2beqhkzrj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2pmppkxrw.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2bvrxfidr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2gjurefqj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2nnfnmtkn.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2wwlgbbgk.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ybufhiqs.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2zkolcquy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2uiilssha.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2uanrhjks.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2qutpahmw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qwulchxq.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2fnvttyln.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ttocwmin.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2dyxfvfkz.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2updohvca.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2xagddame.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2lzbugrzv.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2brosrcou.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ilwtakct.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2nlbhuehm.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ajambhyk.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2moimploi.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2owaykfkd.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2zbepmtav.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2xbgywrkm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ljykzwqw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2xbamfnfh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2afavoiqe.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2aqmhxjta.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2perdloai.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2aydyswww.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hawjayyt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2ijanvria.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2prjirtxo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ggpbhprf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2famfiujf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2akqopvzb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2xpnqsesd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2engodevb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2krqxvsiv.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2qjjylowh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2qecssspr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2tbopfdws.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2uqznqffe.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2dcdjrvsa.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2esmnpapg.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2qmigvrlh.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2jzhelwoz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2tidbwohc.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2upferggt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2mqsybtct.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2lqbphhtc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2spuawilf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2luogztzu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2nhbvnvtj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2tiwajylw.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2elhdakqq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2prydeyvo.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2nunyubij.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2laodglah.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2imijqntm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2hwkwleze.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2tbbvkjdr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2urjmjvoc.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2nhvreivw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2hnrdcody.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2guteamzb.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2udffsdel.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2lysgvdfh.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2cxnzjzae.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2lqynjsnh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2uentmdzj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2esndwpuh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2kkblrgik.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2pyjebkle.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2wzehhapb.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2vegjferr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2fvgkxlxs.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2qnvtvdct.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2xgmjfoxp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2yqgqkagi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2vqkexyew.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2zsgiyzab.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2itcsanak.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2uppjwgnz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lduisxwp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2gsgviagh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gzylgvap.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2btpoyufu.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2jcrbvahg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2idpgpces.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2dtuhscsh.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2ybsbhckh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2cjcowvbh.html

);
来源：http://www.52xcode.cn/Article/details/gt2shqwxitf.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2ellhfqvh.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2ziclmuzw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2nmuxkrmy.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2suzkvojx.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2mkloswng.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2lpulqjep.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2hirjsnzk.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2xhcbxueh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2wegrpuel.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2mknpwnjc.html


<!-- 参考信息 -->