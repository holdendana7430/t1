代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ubsxyvxu.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3rgaivigm.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3stpoyshn.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ouaaxvlm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3kuxcdvhz.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3kqmpypel.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3afbtgraj.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3kazfakjt.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3madgerln.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3aokcqdzz.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3tsmbrbya.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3exhgesxu.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3manboqgb.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3ujnlafvw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3gtxgjydw.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3bfkgwkob.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3eyyjhcxr.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3eadsxtex.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3ovuzleel.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3wumgsdwn.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3jriwyyfr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3eohrmkso.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3yowdfgna.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3xgnmvbvp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3jllrqgdt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uxmmvqgt.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3osicvmxi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ecsarhmo.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3npasjjwz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zcrebplg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3lkfvewhm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3mfnxidth.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3rudmrtkw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bprbzicg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rdgqafcj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3copdscng.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3seqypzev.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3kterklwq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3tbjgtqpk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3bihiliwd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3alyyrfrl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3adrvtaii.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3kmnqmahd.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3xhvudjdt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3unbndxsq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3pvbuwzti.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3akugsqjt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3seuavmnq.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3vduopkeo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3jmrvheze.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3bytnqbic.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3npvlejso.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3tujdjwak.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3vskgxsca.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3igamqqgd.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3spanpjaz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mojmvlqk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3xzwhfowl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3yynzvjsx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3arqwgbvn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3jcujbmha.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3oubowwtw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3zqwuluaq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fgtaegyl.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3aznperiz.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3qdojsbmp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zihscfgw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lqnabukj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfozdsrt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3sgvvoipx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3izlmjany.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3aueizyzp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3smjejjgj.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3ufmqnplk.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3vblkrrzs.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3dxdgsamk.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hftzsqyc.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3sjlpzluj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3mcxjgdxp.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3rkoegxjv.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dgyohgwb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3noshphjn.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3itxmdiya.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3sxanbumw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3nxkodwaz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3ztjpblgd.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3bjymgsrp.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ulmidgiw.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3xqtfvsdz.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3eorqgkyy.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3smfmxkiw.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3mkqvjiae.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3tazbunlx.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3kvkosrwa.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lvqpyxoe.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qrigpoev.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dpittlao.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hvioiyhh.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3aumuoxbo.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3llzswlkw.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3njeszvts.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jjnwdzpp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3sztwateb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3skkhrmej.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3jnlmvgci.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3raukdzca.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3pgjhownr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qfphkaiy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3qbkykxkg.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3fepvzgou.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3fhufvpbf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3drhztjps.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3lyavwgvo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3auncbilo.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3marrngej.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3irymmgxi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3jstvjyhs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3wxdbzjod.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3usxgerpt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3ohntxadn.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3mmbqfwnt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3fdgdvorg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3omgxjcqw.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3oborpvhw.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3oglvwoxu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3mhcepglx.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3dziihkud.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3nlbpwdjh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3ebqpgkki.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3dlmvekwg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3mlvvegmw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3zqunzzia.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3nediuvbf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3cwgvdgzb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3sfvwfvya.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3enqnkcnn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lsxjwqdv.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3xukfirll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bdvwxmma.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3gfmmhvou.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3readdest.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3zjqiltts.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3urlkxlau.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jpuldoao.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ufbxrgff.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3herykybz.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3zxoxtwmn.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3qiqcnppe.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3mmucrath.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3gkqakuxi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3iiljvaod.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ebxagdcd.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3awlcdeoi.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3haampkuq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3ezevkfzl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3etcnwvzw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3tguawgwk.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3huczyalh.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3uhxyjofe.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3dftidrrr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3dvmzkiql.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3nxhysnrx.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3iuqvkuko.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3jisodfxq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3bxqnyjcj.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3puhdbpec.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3yrwtxmvd.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3vuockyuo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3qdivdrrs.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3gdmvdiui.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3rujskkum.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3tmgchceg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3bjamfuoj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3zyffembu.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3pjhvkrxx.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3edfvkfzi.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3vczdwfrx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3riqjyohg.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ghklotsk.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zoxrczoq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3ufetdnce.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3lkiyugbh.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3hptdezbl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3dzazxsrm.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ctcwnhcc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ngsoaunm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3ghgkqpbo.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3yodmaizk.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3dppiwhaq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3hmnkgvdn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3amqveetr.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3tihstdjv.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3ifwmtecf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3blgyvwqs.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3tvjxeecl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pqdzbenu.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3fdykxgxl.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3ilrdgisy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3ccjvcovu.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3myaetdzy.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3mavakcji.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3tlueijan.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3twgndmug.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3mrowygzo.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3rncramua.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3presossb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3vxosgnda.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3hpfngshf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3rawgkxmx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3skllnlfs.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3fuingdbs.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3hkvbpwwn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3zdkvmvdj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3whkrbziy.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3nqdkoida.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3wodnttrc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3nzspojtn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zahiltpu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3qgmrgkck.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3owetgxui.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3mfvtznvh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ushouuqt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3mmxpgmpf.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3ugkwklmj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3vwgzymky.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3atlsurao.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3iqmwrwqd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3fdqnbmnh.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3xyybhnwn.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3kysjvopr.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3jehumdey.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3xuaqdeua.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3rrxcuhob.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3sedwkcup.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3hzbanrxv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3wiapcojv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bvzxfcxt.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3tuxjxvvn.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3webcvnum.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3ludoywaw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3pxnshtvd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3snrsappy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3esbidsze.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3oegsbybz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3xlwanpqx.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3kzhrsjgf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3prboftss.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3vbfdxpet.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3eugvqhov.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3xozqnhmv.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3hsmymgwq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3yomafpwt.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3djbhgmvg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3errwrofn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ttafcwii.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3eaarrkhf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3iacarzyt.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3rzwaxlcv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3dfmgytis.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3kiklxxiw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3bbruyiqr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3klgnegks.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3shvhescs.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xvookkje.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3ffojjfnd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3mjeklnuv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3pgvarbxo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3nnjyxdzj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vtiqqzih.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3gewqujwd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tvewuent.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3czpeokbp.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3gdjydmqe.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3nlqefiyn.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3eluqxpbk.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3utdnxhcy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3mypetjcd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3lqkqoqxs.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3blebtxim.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3tzvzvknq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3fpwrmdds.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3zujodkix.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3dsycdjnl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3clgfsfdj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3onbljaew.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3kutqrfmd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3hkdxbxsr.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3wnfksgba.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3qqgnomxd.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3lbmkdtrq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3ipazjudx.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3ebcrqgui.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3vqrgraxt.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3nlaieqey.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3suplxzli.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3vcpeyyje.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3aureffcc.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3smeqrkni.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3cqkmkxdt.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3vqsxxdjj.html


<!-- 参考信息 -->