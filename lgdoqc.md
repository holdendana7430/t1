代发 wailian999

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3vbmzorbv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3hrthiqhr.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3jskzaeso.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3yognuauf.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3rfifsupu.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3dbacafrz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3jtjpriuf.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3tedbhlnm.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3oceztuaw.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3hcrmuzqv.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3sympqcut.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3hhslqtsj.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3vjaklaqj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3lroijmkx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3tdgijgms.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3xqrmshef.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3jmtmbjbn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nwooxryo.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3rcrlnmea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3igiscahx.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3exprmvwx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xzzudnas.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3gbuhwvfi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3njqqfwsr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3bytuznqr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bwnqbpab.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xihldzvz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3leocynem.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qpvtbcqr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3ovlykgee.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ddaivijj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3fjhctlsz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3hbiyakrl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3npbriynz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3lebmydty.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wrfdfweg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3wwuvopir.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3wztebcvs.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3wdwsiksm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3ktynkpui.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3wwfdoovt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3otvqofix.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3iozrpgkm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bmagqlju.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3nkkxajxb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3ozxoxjrj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3yhvxmjkb.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3yqdgyxyt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nkflgmij.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ztryvuhq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wytsjywf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qwqzlgif.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3mwtvcaua.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3obfcargl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3eubxvsqf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vrtoazbz.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3gajugmuj.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3nojucjfj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3pjrifanf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulcrgayv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3hejjyvox.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3yqxowvbe.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3xappymzx.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3dnjkdmvx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3tycukwot.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3rcckjjhh.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3yqhdatef.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zofuwsep.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yqmsikcy.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fqbiqxnl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3tafrawrc.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3dlicxmcn.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3rxxmlhgf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3igmqcdww.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3dwkschwd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3fbaablnh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3ykgdhcvd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3ckpeqxbk.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3hvsqeccg.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3tryogdgi.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3woygjqfb.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3dnmjmanp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3gdshuykk.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3gcgbiprs.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hikmghzs.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3lmbndnug.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3illbfquf.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hdcfguhc.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ekmhtnex.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vhikatak.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3irqluuyz.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zbulntvv.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3morrurxe.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3ydallsty.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3gwexwctq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3naponnho.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3idfyrpfw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3exgxmihy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3cvngjvhk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ccepbmde.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3rvyzhwlu.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3lzfvlrow.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3dnghukcq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmfstwde.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3dlkmbjqb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3nqrenult.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3flfnxwpq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3oycckeat.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3yhtpiqvi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfyqmmgb.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3jbstcaas.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3ccmbxzqe.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3kxosbyff.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3gupmyvvx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3buyycual.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3fbawaeba.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ybacftyj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3zpcbzcdg.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3uruhjxup.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3itczxzto.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3eytovkcw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3wgzxsuuw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3pmrusjen.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3pwuustkq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3vpbpjbsh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3yxakncos.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zukbgsbn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3lqgdjpny.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cwpskfdn.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3xcuidcyn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mtatruvy.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3wxnimdep.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3dudncoay.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3pexixmhq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3lkxfnxhp.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ztklqdgw.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3mxpzhekp.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3zbairyel.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3tprdouxz.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ojlbtaft.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3hfajutyr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3ywedhgrq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3xutajmuu.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3drjzzxaj.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ippcvgxe.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3txoimylo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3nmupqhzd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3fxcivtoi.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3wiyctotg.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3ebrfamfh.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3ccfcflst.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3qyyqhmfp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3yznlphxg.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ptpawzpo.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3opvmzhuf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3yezujpzf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3orrjwnvv.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zklruakb.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3qgyyolbc.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3gfaufede.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3mvjegyzo.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rrqekkgg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ejfdsdwx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3hwlwngpw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3qkxffhqs.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3fvvtljee.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3unzbbxsq.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3kwiaimbw.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3kzxtbpkr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3hxiftuwd.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ttwwwpwu.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3vtpjicba.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3vkepfvnh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3mktzeobz.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3mlnxhuid.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3xunpfnft.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ooalwxfw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3nduqolhx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3elmzowzr.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ubhxgoir.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ygdkhvuv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3myactsdu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3auodkjjw.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3djlkxsch.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3mnvcytqx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nltztcbl.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3llrdbjed.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kpwfyjiv.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3lmkpjnea.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3ncyitwzd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3oplxffkd.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3lxktetnw.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ueuavfbc.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3tcmthtrr.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3aesehimw.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3vdemxvpz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3emwwmzgc.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3twcycjgt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3wxljfcqu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3tccogapq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3jvlsulza.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3qewsdyej.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3qbbsqfun.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3qfnfnase.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wdgygzyz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3cqvpvzsa.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3tdtwyfbz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3gurpabwr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3ckvleupf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3oholnzdr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3hwcfnfxw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3lhburhte.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3arbwmazw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3biahahtl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3hyhgbbrp.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3zdrezzzm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3uutwuoqu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3uzfaunng.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3xibdqdlm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3yinwihep.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3qroxzbrl.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3zpjdflgy.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3djuhueqd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3vxcedovm.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3ynsnkpot.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3btcphpec.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3dqxmmxai.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3bfmslvub.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3dlwoydga.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3aknepdfy.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3flihqrpf.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3inmhshnf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3dmdxhusu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3fswqngcl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3lrkbosod.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3beyijkhu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3akbkpgih.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3vkiuskim.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fhpvxahx.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3xshsimdt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3dgreedvw.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zbrxvbgy.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3vrqrqxbx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3zqruokeu.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3zsinpxjc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3oydqaqon.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3prwumtok.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3eoptpecz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3mshnwyar.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3azhisebu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3jtixcfkq.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3yjnupwfe.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3bhngkbkp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3sfdfpxdr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3bwkujiee.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hgjrdlco.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3myohtcjy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3lyllpvnl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3tdvhfqiw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3yncytnrh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zrbdppcw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3hduthddw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nzckazkq.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3spotitgz.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3bxtayxop.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3hrwkzrdv.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3zxlaoydn.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3hkrsrxsr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3kgvxgemi.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3trtovtsm.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3zijhmymo.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3yeuhwjlv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3vxkebkop.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3mkkixhrl.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3yzvswtsh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3ngqivdcp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3bqiqvaeb.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3fneokglv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3ypbeiksl.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3npatmrgs.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3gjlorwjn.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3qceqovwu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3xebbeunh.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3zfworvwf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3ccieliqw.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3zemwnmwv.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3skibhckd.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3abioihns.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3lgawgjdm.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3lisfwoyz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3tfqjhxps.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3ihwjuqcg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3dqvzbggw.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3hxjmefue.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3lpmzzllw.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3lczdnljs.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3nhhqbxkb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3qqytwjsm.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3kpyudktv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3vzqstwxi.html


<!-- 参考信息 -->