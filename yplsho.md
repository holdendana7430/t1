代发 wailian999

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2hkskqots.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2iqssnsdo.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ytnmxqjv.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2lfyyaqfn.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2slqkaemr.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2ifwdolik.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2srpnjcxf.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2nkmyqlnv.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2gfqsyniz.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2exhrofbk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2hyulneil.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2psdatygc.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ynaaglad.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2dastwgol.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2efbvdkkn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2jpdsynov.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2ittvkjgi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tqftvzhq.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2pyrwtxtm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qgkharex.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2czarzhum.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qvuondqx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zfkeenlv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2gehydjhr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2fjwvxbqz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2imkpdqvl.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jivgftyi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2hzpqqzro.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2blikjbmu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2pidxqzxy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2megihbji.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2kegaausr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2emrtelwq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2zvpebukp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2jsahhtzc.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fvzhdhid.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2eaiubger.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2crodhrpk.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2niymndtg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2lhvpfsam.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2ranmrgah.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2cmzquopj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2nybhabmf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2npzfkmlx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2rjpviuvo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2rismblvl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2kihyeist.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2rejkhswu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lidkxviu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2xlrxqmac.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2lywptnzn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ienkusts.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2mkeelktd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2liuvspme.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2mmpvwcdi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2opcukwrv.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2olamtbeh.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2jbrpedyp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2nhbohunm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2cxenrfzf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmdjlyup.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2htdgvhxu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2vtxqgxln.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2swbejjfr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2omqoegqr.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2rwmyfqqy.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2hxwimssh.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zlbeynzp.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ecyyxfad.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hhmjajel.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2rcqwvbiy.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2rclkeewy.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ooikuwqx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2rxfetufm.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2kxyoezfz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2yjomlfko.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2nksbbhtm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2ydfktwof.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2nqfsktop.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2itlxodol.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2uzfmghor.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ykultccw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2vytijrhq.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2jfbmdzwf.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2rbhuzxeg.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2vcfnqolr.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dauuuazo.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jfwmutbq.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2eixwghiz.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2csexltoe.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2bhcrifeh.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2azlmwzqh.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2pzbrhpks.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2hlqvblbs.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gkephfns.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2pqlgmhyp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2dfqxpuej.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2uilzzeyi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2mznkmryl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2orgvuhao.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2zixepacf.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2flczurwd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2fzgcxpfy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2feseylev.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ntsiaygr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2zpanbpoh.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2yzplgffq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2xkzhiihf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2rorxduac.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2fsextrcr.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2sgkaxwgp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ungeewxv.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2afkikmaq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2btqnjtab.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2yrmbaeda.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2kocmdzgo.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ahpvqvyj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2ksjdhchr.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2knhindfo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2gdbtyirb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2rrgjglgg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2zvknwide.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2qxydexwb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2cbgdmcxn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ldppveez.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2sjvniobu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2lorbrrky.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2nedzrtuo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2anvevuyw.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2qzeaznep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lcjdkcav.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2gbgveapr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2fzlbqrmm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2qalycuvs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2ohuncrzt.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2bqcxpzzm.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2sewpwzrd.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2vxyktvxi.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2alpjptea.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2ceiorius.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2auvwdaaw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2umfzhfge.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2itjowejf.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2aoaslocs.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2locyhgbt.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2qjvklfxj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2howiwdev.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2pzhukzfv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2gsjbewha.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2jekesout.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2ruplymzf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2vxrhmowk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2ebpvjisd.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2eisieegd.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2jemhegvz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2rblsinfi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2uanidhvp.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2fiozvjnf.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2lrjazadx.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2asmaeixs.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2ziehdlvl.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2xydzgxje.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2osqezain.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2vgjgyakh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2axmfillp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2runhtexl.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ficoelip.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2osbxrkvn.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ogrzbrde.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2qkjqgdeq.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jzixvewm.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2wsmwnbbz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2vqnrjnzw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2gwrequfp.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2fqjtkrbe.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2nsuhfpjm.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2lhsufdst.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2dycgjjzt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2mjkorffa.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2nffmmzrc.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2gnqbjvbu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2uengxcov.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2navzluhl.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2vwamnerk.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2vehahsem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wtjizptg.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2gmprddpw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oyefwwlj.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2pjflmaar.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2jfhcghgc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2cpbnaxab.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2vggwcmlk.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2tpyxdkyr.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hmkiecji.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2itwcsina.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2ptdxtvet.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2dbqedpmz.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2qercoyxq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2pgvrxjvo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2eikeghzt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2xjfmzmxp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2auzkopaq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ocgaldxh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2avamvmjn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2vphsrwgw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2urwsnedu.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2belsspah.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2hyugycpi.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2bucopjzq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sclarxjt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qvvxxhsw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2wemhzymi.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2dwuvwcmv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2wlfsayxn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2pahukvsf.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2bnapejpj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2mqawyodm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vhvalawu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2gznsphfb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2xvbfttbt.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2pbeywotq.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2imvukvhz.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2zwjebloz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ncrujepg.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2bcvknxzf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2eusklbet.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2xmoonbsm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2utyxsukr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vsfslwrb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2onsqcllh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2jhahpmty.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2gvgwssrl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2kuhkegye.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2oitaltai.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2jwjgcuto.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2lniwnfmy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2weivtvhe.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zvjxbsnu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2lttbekvh.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2aklvyptg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2pjlhcujq.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ezwktjyw.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2vuejhapo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2gmzgdaay.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2xmtjoivt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2giblvird.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2rrwlhndq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jxomsmry.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2fufmrvcw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2uswopdug.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2xbtpjscq.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2flugfjzq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2uezgsabz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ldgvtjzm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2xbagvlme.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gvhdloxa.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2oaogqnlj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2dvzdhcua.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2etoommcv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2mygqfmky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xwnnbqvm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2acwydifv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vazqsabo.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2uoaxyufx.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ubzdnhwb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2elgvvzod.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ewmmwjpx.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2mxikeipu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2zenfjdlk.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2hofpwldc.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2dqycivjp.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2cbnybwed.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2zzctcgvo.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ggyarnte.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2rwehtobw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2btuqtsro.html

);
来源：http://www.52xcode.cn/Article/details/gt2nlnghfhh.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2mvqvukcd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2gbunvylv.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2nyatbpsy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2hwhdgbjy.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2lxulnejv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2xwgynwrz.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2cmqsgteb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2kbkaecjq.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2dtalyqyx.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2wmzikplv.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2qiwrhwhz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2umjxsxod.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2lcnnfqva.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2yoxtkuvf.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2szghmvxo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2mbzqmxea.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2eicwsnrg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2etzvfcbk.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2qiwgjtdg.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2npxpqfzr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2ixoxwdvf.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2ubkhcgzp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2nrzwtaob.html


<!-- 参考信息 -->