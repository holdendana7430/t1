代发 wailian999

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mahyvtwc.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2glurpwzm.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2updbptdr.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zldedgzv.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2gnxvhepc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2thstjxpr.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2hmdalzuy.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2bzgdhvid.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2bkbutevn.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mlavbndr.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ngvvzolv.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2gvtlaume.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2kksvjpjs.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2hpxoyrxu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2trfdikhf.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2yokojiph.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2hvmsdqll.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2nskywnwf.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2mdzlgseb.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2vspeobzd.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2ysxrzqof.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2bellirbh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2cqorkjom.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2vxirwqxq.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2tmyozqwi.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2zvlalcdm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2zpwkxjiw.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2elluypad.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2yfvrwlrm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2xmgkdhim.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2jmqkodhi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2jahkghmy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2yocrwmxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2owmxlwnd.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2tqshsqvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tojscwhf.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2irzsklst.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zggyrvgk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ekgsuhov.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2kineblry.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ohllyccn.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mmybbhhv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2klnugmey.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2pheelpzo.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fxjovntf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2yarmfwnz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2mojeibgi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2nbintrzu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2askzihml.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2sfwpffdp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2zolpiphw.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ywpxqfwl.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2snffjnki.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2iupegecw.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2yyoyrhcr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2xnxiqsos.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2kphwlbrj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2hghpkzfk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2nzxjdmhk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2tuvizbrt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2exybagzs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2zemarkcj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2shdujsyk.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2gostokgj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ondvbjpu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2yrdglgkz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2iybmzszr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2sdeovjdz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2wghbcazh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2jdmifbga.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2toukgwru.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2gdixayra.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2ogwqkmoh.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2txxgnqju.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gplxeiii.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtjmecnt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2gnwonfew.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2povfsqaa.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2wvancrbk.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pqscmzth.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2zwrlqnpt.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jzbgjexs.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ajktasza.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2zswqdefz.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zyubdqfj.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bzotauvt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2rtaxtcrq.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2ynlqkevk.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2hdmdhbvn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2lhmxdgdn.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2ifenoxpn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2ssamyefq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2dsnkujnm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2kfihomar.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2wawkvznm.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2rnhjfkay.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2apydutdx.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2somjxuty.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2rfxpvofj.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2wbpxplsm.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rafdwoeg.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2eocxglxz.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2iyabfohk.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tvgucysc.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ukzpvrxt.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vissyogl.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2rnauyenj.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2uueejkcs.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2dpsbuwce.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2qcocnmks.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2lbhuoicl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rriqoeyx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2srqxxwxi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2kvjeebej.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2clgqmpmt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tzihdgbu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2rgcvpbac.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2zparaaaz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2doqjqpav.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2kjakupnq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2dzvqyvvq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2ppgitikz.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrsorvif.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2fcnyxcnq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2frbnwbbn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbukcjhr.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2xyxnpdwb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2rbegyiqr.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2rngpczsq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2onbcfugn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2sjwgexdv.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ixtqkkkk.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2nkbwvaxa.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2bpuyjfpo.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2fqllaluq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2qxiitigk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2kgffuasy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2ngzyujio.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2jgqogrua.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2dycnalaa.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2juocigkm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2wbwpordr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2mmrkmglg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2vjnfokrn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bnntxhok.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2krmrlvob.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tvmyexie.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2vmolymhf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2zbscgkch.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2tbihpdrx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2arvpppbm.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2wfrjjnvu.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2kfrkcaml.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2qckvapez.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2orvfoopy.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2uasmpxwy.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2fzwmumbn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2ghycaypb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2sfxuweca.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2obfhqokm.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rkrvdvhk.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2iekibkin.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2pmbjchrf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2cpmrutxo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2ggirucsq.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2uvuujsqc.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2odzwfhwf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2zkurdfvc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2awhmbanw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2nokhjiol.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2jxetvyrw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2ykwpkrlq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2xzgzdyrv.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2poaizbiu.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2ygzdwbbk.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2ezqvdiwk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2fyzrfyvc.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qbmqfspd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2dnieiyfg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2aalzikrk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2dlkuypri.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2nzuxoouw.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2voblzufv.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2cwmyduvc.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2kvefwrww.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2dqwmseeq.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2tapubkql.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2vithpzvp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2lhlvkrus.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2rkzhgikm.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2vtdhmwcs.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2ymwrvxvy.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2hdgzzdse.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2paogiize.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2cciawikm.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ayvfrthj.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2phhhdrxz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2prytopdf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2qhkhcxpp.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2tygoutrr.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2qaimhzfn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bswixcxh.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2wfmzrnah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cwtzdipi.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2nwwgzgif.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2pwnkxfni.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2cnvdhdzw.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2vbanbxyk.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2tmxxmpgy.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dlfppkob.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2wzdvbmxg.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2mkfifvup.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2zhvvjfkw.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2sntbbewv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2laqpkjcn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2jcflkxqk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2nblaxaec.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2mmtoacpt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jnnsqvnt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2xhuxojls.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tcsvnrrb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2lblijmls.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pedilcuk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2pzpnxdey.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2tynjvclp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2sqpeypwh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ggnxidct.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2fnssmudc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2sasjtcdd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2afnrhlsy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2njvthekg.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2idwlcvzp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2caiqpntq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2tkzkquna.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2vpuzjepq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2sgncviqz.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ooucfwbc.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2caqyfoke.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2otbfsfah.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2hsmnkrhg.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2ltdgdzwk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2mbeuiwns.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2vjammfxa.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2kzanvfnh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2uxntlnaw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2sjxalivv.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2krgprdhh.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2qcipnyxc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2uppvgomx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2trzjzaof.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2eazesjih.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fjeikokj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2pjpvxdrc.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2gunzdina.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fftpfuod.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2ztvwtgwb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2fizlcypj.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2zvpwztgg.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2ushdknpz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2wwroelae.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2afrkvgfg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2aywsruxm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2oyfoocwd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2nkcjcvud.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2nsfgbpdm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2qbvkirya.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2gnetohfc.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2dxigkoqr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2eicrumgy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2efouarue.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2esfvlfus.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2mcgxbhct.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2kpqetyej.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2vlqzuqir.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2gzamfynv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2jeciljnl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kurminby.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2nzftanht.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yxfqlojr.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2magmusir.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2gcavldzi.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2nvqkwbdt.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2oskoktgz.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2yojygopl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2rgwjnqbf.html

);
来源：http://www.52xcode.cn/Article/details/gt2qhewjcfm.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2xbczpzax.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2vuxvvgvu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2lksrhlbn.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2pflstpqc.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2pgppwejd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2vwwmpemg.html

);
来源：http://www.52xcode.cn/Article/details/gt2ynttuiqq.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2gxaarhjz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2ewflcjzf.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2twzstotx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2einncqej.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2phbazvkg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2mbczjnif.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2czvdbjfv.html


<!-- 参考信息 -->