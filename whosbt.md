代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2lpfbrprb.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2yihnggcz.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2drjynwns.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2acbwwyud.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2nzbktvzu.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2mkzjtfxa.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cmwvovma.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2aqdxzzky.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2gohmwumf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2vaopmjtk.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2xokxnane.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2rtfpawpg.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2blnmnaxl.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2rsqpknkv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2zbdorefe.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2tnuutpyc.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2impxzzgf.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2cxefuevm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2cdyauoqc.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2mdlsjamo.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2vfizvydj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2vgkfzlvu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2mkcdmfyc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2xwcvgamt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2hlfavprf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fgamyqsh.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2qtvelysp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vlenqbxm.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2cvxdbkej.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xtppppyt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2tnjclyci.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2hffgdblw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qfqbzubq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kdcvtsos.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bcpqbifs.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2jcrdebrp.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tkhhmjjq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2ksxcjlkv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2aqryfzrm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ttxdvtep.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2dcjswiow.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wpwiokfb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2bsiiroct.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2stghuyfd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qvmjolyb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2pxihibrc.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2pcksohlt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2bmgqmmum.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2gygamznn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ajglhvxw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2uthuoqfp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2bkdpnxdg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2oqfuefcp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2hhiyjnle.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2qvebllwp.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2bfpmgrpy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2fvqdssoo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2fwodsudd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bxvjvnce.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qmzwmpcf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2qoelncjk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2xpncoybr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2muewjayk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qoisgerv.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2jyqtxorv.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2xmviypss.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2rtdnqezk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2lyrbyxfu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2cfqpaimt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2tootkixw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2xlcnainn.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kmrovohl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ypriepql.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2slpceqpv.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2obdmxavw.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2wxltetef.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ofsaawar.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fgfbydnk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2hnxonthz.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2xfpkecsg.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2sobiraht.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2rdothctg.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2nbrxzqow.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2eoptfjva.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2ijsbdycw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2xrrpjzcb.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2xqplpdoz.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2mxcahppi.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2etngrijh.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2wjuxewcw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2nadtwmje.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2kpegazpc.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wzrbaxob.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2smetovgv.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gnteufhe.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rxpfolzg.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tmmxhebg.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2eksxofcn.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2bwybcgkc.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wrstjjsb.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2lwgjuxyk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kqnijnrh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2bzhigkfj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2yjyteqcc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2dywdghqf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2bcnqdbht.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2vsqbtagf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ifldigyf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2uqfjvpja.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2rhbrpgki.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2hjtuouzh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2yhszdmov.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2txpyjtqj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2wtsbccrz.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2syjaltjb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2zeepowfs.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2vewbfkmf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2epaphxjh.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2djokrvyp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ipkvcchn.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2khnxxdto.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ghpciqtj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ualqkjtm.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2lwfdbxmg.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2fskcmkum.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2tukqhgvi.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2nfxtjuqy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2jayspqxd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ghwzyugo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2kyxxoojn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2iwgdvrgc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2mbiihjth.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2abbpygqx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2jjtfbfza.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2ursguthp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2akcoions.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2doglcsym.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2asibmdhq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hptkofrs.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2niaagnpl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2yieczvlq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2osueyixm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2qzjbtbsr.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2bslbocfw.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2sugwuuxa.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2zvxgwqtr.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2rwiaepeo.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2xwbaegph.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2ghdhbzxm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2naiwgeek.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2inufiuiz.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2qnuianog.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2akjrvaan.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2kqagrzrb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2xxxzstqv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2jtymmuxv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2pzvlrzih.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ymuclmhr.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2xlrillis.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2chpntasp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2ythvzrnd.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2mpxfnpdx.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2yuaujkpm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2ybaupjeo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2fwiqvhpu.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbfmujuv.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2algbhgpj.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2lcttuzww.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2kahnfydu.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2mlyzzwzx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2tzqauqiv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2dytfdcxa.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2wujaurke.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2gpqijdxf.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2huvhrwld.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ojdytpzg.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2cemxppgd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2vznucvgn.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2aeaukkim.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2mrsfqzzu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2qobxcqyg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2isilmvfc.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2lmtxmquy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2zdzjgiem.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2wndcadkt.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2qdjhsshu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2xhyuicse.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2wbhbzavx.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2jgpwtjth.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2oksjzayf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2ihesqpeo.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2lswkhkdc.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2rvitgcrw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yahojxcr.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2xheegdkc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xgsurtrj.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2hstrkuwp.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2pmzyzemm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2bcsaqfqn.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2vfwfxuri.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2zauohkrx.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2eladnruo.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2ltkdclbt.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2cftksmbt.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2omevbdfn.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2ldpncrdy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2tlzmxhad.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vvfbaatw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zxfewwvd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2pflukcvm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2aelgwhxx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2bqvdwssf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2yxudiasf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2jngpuida.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bdhkadgt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2jjsojzux.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2zgtmfqee.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2zufxsmop.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2gkwordax.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ixvlbtmx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2hhhylwsy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2zjwslyaz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2oftmbwme.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2nselxpol.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2cugaoakg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2deuqdrsk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2rjpnqfdr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2fexrfghs.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2cemccnjf.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2awsxgfry.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2oqomjuyr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2gkuoiauq.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2emsbfixu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2nfyxiwwb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2ucesgoya.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2sbwabndh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2plpkcijn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2gfzgbkfy.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2kyebbmfw.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2bthmrwts.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2hlkfgucj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2rznlfcps.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ojqojsew.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dkhwvqrr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2qyyxffbj.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2rdsbgoov.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qcmnombu.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2uwplfnoh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2zdoonalx.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2clrpgivg.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2dpzmwowj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2berjdypl.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2bjkydtez.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2amiwzbdh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xqcnsbem.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ssyymlwf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2bokhumlq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2uivzshqe.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2mrealkky.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2qkfrmsgh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2jkyvxcoh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2cxxnxrfn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2kqpwwbyg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2urlziipo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2pgtdjqjw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2gdjtqfpm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2reyfaugs.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2swgaaevm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ntojfkvm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2dtjesvkn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2onwuampe.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2aoacujud.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2miijkfxl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2qftwmmvy.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2odwamape.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2lrarugmu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2qmstnqob.html

);
来源：http://www.52xcode.cn/Article/details/gt2zmubwujm.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2fkbvfawg.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2zxafoljp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2vulphjjw.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2iehzmqnt.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2lgmxkkek.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2hxejgxcx.html

);
来源：http://www.52xcode.cn/Article/details/gt2halnlwpc.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2jwcxrean.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2uhlcwbeq.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2suulsyep.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2eubyshrb.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2znranuxf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2fpoddzas.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2mykqywjz.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2dnlczduf.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2fpobwial.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ugizszgi.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2qtepnthn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2wqbsgstt.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2zvfpkcra.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ptyldxjw.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2isxrlhem.html


<!-- 参考信息 -->