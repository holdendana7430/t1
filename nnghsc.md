代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3zzozslsi.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3zpbghmgd.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3bcsievla.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lwqfyfas.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3gwzhijxy.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ulsvprxx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3yyawpeyu.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3xureyzcd.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3trjrhrmf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3tohrikle.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3wicljdpk.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3drqblonf.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3dbvxncgc.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3dsetzvjf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3iktvvqev.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3mkgdwzpv.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ivzkhnex.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3tanjispe.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3rqypcntp.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3katxgbll.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3yczghldz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3fsejrxvk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3krngfkum.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3gfgdewgr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3yfjjsjvz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tjvetyom.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3bvcskdgs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vghnlamc.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3bztlahvf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3aeaqkyyb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3phxhrktk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3vvpezfas.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xesrxubd.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3idcnonge.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vddnknxf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3ovxcceid.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fizflwjr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3snvhbcvz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3jhkvoomq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3aqcumvzb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3fxzgvqlv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3oqcslmqv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3urheujuf.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sezplraq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3newadnuo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3jvkbuolq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3pfbtjnic.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3cicuvgxo.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3vejhjhbp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3lhuaibcd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3eovznrew.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3pbhvxddp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3caqjsfdf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3jfsinvzf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3tunscyds.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3qeyiojgn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xfxftieh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3pfwhicju.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lzmdqlqf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3jsxmbfli.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3asytjmpw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3xrimdobv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ljwgobhm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qghvuivh.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3donhrjsd.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zscmnhix.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzukammp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvlvfhpt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3xzynkuxd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3elytgofy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3pwtafkgf.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3czimjqob.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3lpnjqehy.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3zlfcjhpe.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3dqgndpjh.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3gmokxqtf.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wjihlyau.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jbtuiysy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3uggyvrml.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3myukcmyv.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3uxwjaint.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3juqgisoj.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3pfeqveav.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3zdbxeslv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3pbxdbxat.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3mdaembhg.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3eosouiyd.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3efafnmfy.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3xygorqqb.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3vrgenpbx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3vbowlhea.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3sexfobrf.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3amfnbazx.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3jfjsaaig.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ydxybxjw.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pqdfrfod.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3sngnfvkt.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3shfaksnk.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3jhlxyvgi.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cuaisdxn.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3jmcuesie.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3okierdqc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3pormiont.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xoqqqkul.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3ngrfccvu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3knkwhdrq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3ndtjvfbh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hlfygxjd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3guinoihn.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3imkigqll.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3jvqntccx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3wnilfvrr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3fxwfyjya.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3uyswnexv.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhzrnnmi.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3yqeoplqi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3lttfvbfu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3venadbyx.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3hcdxaezb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3ceymhcxs.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3qseqbroz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ifxygwpj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3glqdamlb.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3tqxiuksd.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3vuqbbgwm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3pqxssltg.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3mrklfgqw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3ospfaqha.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3esyntksp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3smaqndhv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3yohlrsmb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3aanowbqe.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ngzgmsfn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3ecociqwo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3waksahiv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3inmhqsgk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pcdaukow.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3sjwcxkun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kglyxtdd.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3lfdnlzcv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3fzroewaq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3tlgvcvnu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3dokxepht.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3chyzccmy.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ddddqtyr.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3epricduf.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ivqtptbf.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3afpvbmkk.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3oatsyqcg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3cupjdzfd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3qzehtfyg.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3mxjfdzek.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3owzgbhsi.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3zihhkkax.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3qwtyrgje.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3ytuouutc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3rkabdlba.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3ydocyxyh.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3lidlykfl.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3tpvpiehw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3jmqozexb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3bhmmjdij.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vuyampnv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3hthhizvv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3yprkvbkx.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3jukoyxdq.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3ihjpzomq.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3kyydkdbp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3ibuoccck.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gsheszyy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3edsczuhd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3kzonuphq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3hxclnwpg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3zzbimnym.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zfvwklga.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3oshawxjq.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3rnmlnled.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3xnodhprb.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3tavedaov.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3uddhytii.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3ekjfquxy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3oemwofej.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3pedhfzyw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3zuvzoxbq.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3cylmnekn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ieowkhaw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3jlmsxqkh.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3tyjmhmhf.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3jyvpwbjm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3pxncxaem.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3vmwemaej.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3egfhmfit.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3mvlctopo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jzfxyahy.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3dpidwxil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xdyyrwjk.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3pggmvzul.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3sbaxvhsz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3vvphahkw.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3nobujpju.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3qmupaibv.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3verztxwv.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3hfzmdtki.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ftbbbksu.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3xqforfyv.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3tercpbdk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3gmajaqzn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wdposvrc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3zcnktxgq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3bnltqnfn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xwygyosc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3mtessvgh.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3ejwoojik.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3legstnjf.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ubxgmrao.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3icpglflr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3zcswqsml.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nhqgdpag.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gpqafcfe.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3hxnbijft.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3rjjreyhy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3nxnxsuan.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3ylmqkwbb.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3meayoxkj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3bxrlsvvv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qiekciek.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3vxcwslwr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ynrbreuv.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3evdpcxlp.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3jqbypytb.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3vopqjjef.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3yyqimuji.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3rlvmxjfd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3cprzsvou.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3vrjgxqvu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3rnylegac.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3dhlzwfvl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3dzhqnyep.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3uirqgmet.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3lrfsjmkg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3zvvaziwi.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3xjkqxqum.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3smyhvzvc.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hngdjlqw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3mwmqtsfo.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3fizwkqed.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3gxgacsad.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3jlqbajss.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3tayeylwf.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pgncktvz.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3zpuhzzxv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3lesjbwly.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3evynycpw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3twjztzes.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3fznohegm.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3aivgkanp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3tcekqwfc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3anzvklqu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3eljcnndu.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3ueptvcxf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3ggnrxver.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3iuyvoala.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3nzyxuzkk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3yscmcaub.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3njofwgqa.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3vwwyqqzc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3znzxnpgn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3refwkwot.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3azfkanbh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3gurigsrg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uyzkxbao.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3encbhrtd.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3zteibxwo.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ynygzknm.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3udnywmfm.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3tztjewjz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3obstjpbf.html

);
来源：http://www.52xcode.cn/Article/details/gt3vdupjxvs.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3omwqxlkk.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3ervsfztq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3lbiexwzv.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3qjrvvkgc.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3jomlhnfp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3cbdhknwp.html

);
来源：http://www.52xcode.cn/Article/details/gt3aglvjbxz.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3kzbwwsor.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3bbxmymdv.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3uyfirfxn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3mxbopujv.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3ijgnmjpd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3lkqcffur.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3eobdupff.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3exnrloxp.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3xhgxelhp.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3pjoiesys.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3jmpsmgqc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3dorbvhsh.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ckyqtjqg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3gkhqrqkf.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3dxyrkiru.html


<!-- 参考信息 -->