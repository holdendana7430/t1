代发 wailian999

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2jdetwcda.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2phygksiy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2paktofgg.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2uqkkmdfm.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2yvyrhsbt.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2dwvxlzek.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2plvvthim.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2aatjhueo.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2cquimpte.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2dnvvqqxq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2gncymuct.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2svigrwew.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2adssskvy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tgpslwzp.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2jbigkzjk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nruergod.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2dnrzbyup.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qwuvlrox.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wpcrqqaf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2zevzjlnh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2odtadnaw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cldojsnw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pdabciqu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2vodvnzow.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wpyvcpfq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2fedczvyc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2mwwytzca.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2hstjjjfh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ptccadux.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2fkciictj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2rtmcjuox.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dalotoql.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2kkcvdtfe.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2sfhupkeh.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2vwatpirk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2stzyicyt.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2veturajf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ebtixkcn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2zejrqyjo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2turqyrqg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2hzzvkjga.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2csxjfquj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2ecqhnrwf.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2kgjdmexk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fislanic.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2egeackbe.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2skuheygw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rfvrggny.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2gugzyscw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2dyigsjrw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2uchmdgbv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mmsqzasx.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2puplmbov.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2zvlbbpka.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2qijmozum.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ejztgyil.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qfitldye.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2zohwzfms.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2dqukjbab.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2wkhssagl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ktmgefck.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kpcagrvp.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2hmnznbkw.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2lkmoftos.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2aalmxdbf.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pqtjelrb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2adoazirb.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2fmzscasy.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ahureuqj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2fsxxjyfa.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2ukxctmme.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2xkzkijwj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2dfdofeig.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2pmwzuohp.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2nyoxdklr.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2xbmpwrex.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2sishtodf.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2uesdjbom.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2oejiefuh.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2vllndnuq.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uxxryxty.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2krzriooj.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2woaylcst.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zuchlmvj.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2opxjxfhd.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fehblcwn.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2crmzszhx.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ttwjctzw.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ekeyisow.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2dlkjwdoe.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gzngrhvq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ipwvdltx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2zfzqazox.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2oxkeveiz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2nnmfyqzp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2qgmduttk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2fittrbkz.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2surlsrck.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2rrgyvhok.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2jkjlobit.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2okqchvri.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2dmzeglys.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2efypllgd.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2zantyfjt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2roypckiu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ooiaokzk.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sdevrwlo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2fatuybll.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2snrfntbe.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2wuipcqqj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2tewxdwqi.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2sjlafhey.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2okxizshm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2vzsxnlas.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2uajyqlck.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2nnafhekt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2qkfwqmyv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2jhnjizdk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2mipysdgb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2wzplknml.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2tohtfkpd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2mtokdius.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2sgcesijp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2podyxitm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ndvpphti.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2fvryawsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vehwpdgm.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2bhgeudje.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2ngkmvowi.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2zkdaipix.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2ipbzyxqq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2aileaglr.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ribeuktd.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2kybujlza.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2tojwavkc.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2awvaokkc.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2ijzneriq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2narjwgjo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ctlusdiz.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2nkusrdte.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2cqflzbpi.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2pbipdzbn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2ojzjrfrl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2xeyewizf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2uaqmsytf.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2upsivncl.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2ipzdrlyz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2hhxzfmmv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2smevanuw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2gfsslyts.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykrnrfuk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2ifkqpqhp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2howpsjvm.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fuvxrupc.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2inwkdagd.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2cdvakqnh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2rxsxucxs.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2widehvdh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2buzwwmzt.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2rauixxja.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2mmwldxya.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2fdtougsw.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2szrupasi.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2rwjkufya.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2tsinpfis.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2afpsbxis.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2psqtaeul.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2koffrmrn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2uubcsbcp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2fzjemybv.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ktdupjpa.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2ufzodxgm.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2rxouxzke.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2hysbhual.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2nmdldyqe.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2dhegdfrj.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2igvjppst.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2tiymyzsp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2xpcoopto.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2xfseepof.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2ezavekcr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2josnfhhp.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2qwmmypdj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2arzmpgwc.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2mshgdgly.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2xugalmfh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2rlzvmseo.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2eoxfyyhu.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2uwysazgv.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2kqiwstig.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2egascoin.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2ogqvnsgc.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2vizlmgjv.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2ywpbdycl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2wwwwvdkp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cnudigyy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2uhnxkcmq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2rdwupbpy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2zpgfpobx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2tjslerfl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kcrbzrut.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2yaqgbqrz.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2bmkeqitn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2ynuvsssl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2kmqavjyp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2jsjkgvxg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2fyckcofa.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2iahbpkmo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2jmyejjsp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ttayehff.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2anprfaiw.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2krtjamjt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2gkwvdzjc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ddjjhhhz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2nnopnmsc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2gpkqvums.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2vsujhvrg.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2wtjupwwx.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2ftyqmygu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2iqmfgnls.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2tpzsjtll.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2gzzcrefb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2rqsizaea.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2cianwocw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zvhulyqc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2qmciiknz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2oevilsfm.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2rsrttjrs.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2sqroyfml.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2hfscsjwf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2xijmznio.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2niqmalbx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2vqkphves.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2bgyalymm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2slzfsurw.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2ohdcfbja.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2mvdkuoyi.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2loljjlix.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2oojfxlyg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2lpcnaitk.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2kvpnwgob.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ecpoecvg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2comnjcbu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2wsligobg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2tjqcwwdz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2kwiifrwe.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2jyjwwznu.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2mrivnkjn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2eoljdvar.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2xjbfzmem.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2tkjtyjek.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2bkmijvvx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2dfeflxcc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2psucxmww.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2nuiuybmd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2naeyplnb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rxigyjzp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2tlunfmwq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jtzihydj.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2bplqnryr.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2pxrvfhpr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2mcbiiyok.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2wqfaskjz.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2klygmqof.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2dixhclkw.html

);
来源：http://www.52xcode.cn/Article/details/gt2irrwvvnu.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2ovooamjj.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2ccstbnbs.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2qutdbjgf.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2xtlyjtuy.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2cqgvlktc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2winxhxdk.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2rqhzorfj.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2trpnjnve.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2vearxdbp.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2bvlvhjhc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2spvxlgfd.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2xoaebuno.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2hlleyfim.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2igyecyrc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2ectpmeds.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2uvtnkbpi.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2bvjraitp.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2rnqdtsbw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2xolwkwpw.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2lexcjffs.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2pbnebuyu.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2pbdylseq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2zrjxdmcg.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2nlxudyys.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2qwrslwna.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2bihbttfc.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2mntrrehw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2qukvkolj.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2sqbmrexc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2etvgwflw.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2ttosjxej.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2byegksme.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2bgfvnded.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2loebdcxq.html


<!-- 参考信息 -->