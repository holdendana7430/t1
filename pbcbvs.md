代发 wailian999

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ktyyecyy.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2ffvppqed.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2iskiizvr.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2azzgaymy.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2zylqgrru.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2adploehd.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2qaopvevz.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2yvbxotqs.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2noexlbfv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2mifwkmoy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ncgloqas.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2smjmtzwm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2whdbmwyp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ksrqdvyn.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2jlopneyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tcyzimuj.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ygvdkeih.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uodizpns.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2yesqssiw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2sdbyhdbt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2uqdnqmiu.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wswcmdmn.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dfukmszs.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2pipocmhs.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2utofedup.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2rzxourcc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2etxuxijp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2ceeawray.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2bgrljixi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2awoagolr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2vaxezzne.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zkfbaufn.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2sliovviz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2nrzokrco.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2yvzgexwy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2xnrbsqju.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2uaufzlss.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2jyfouvgr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ihiundkp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2obeunyxu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2tuztucem.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2zdsshqsi.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2agsoawzi.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2acmenbnd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yfexlmwv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2egmrmvwk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2lbkyaslq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qjcfdbyw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2yfbujngm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2snekwxux.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hsyyzrpo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2wyoxojem.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2egoichtd.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2unsemlxa.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzbhaxmj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2wsefhbyz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2gerwlrer.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2wrywqhkp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2sptvkrob.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pwpyuxka.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2dkweskdg.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2znxfvohd.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2lgzyqkhz.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dhfzhtwn.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fzttgcft.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vtwndjlg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2umprdlnl.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2cvhmstty.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2lwwefidp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2wpwzlook.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2snytzqzv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2jnqndcci.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2mnxjkepk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2epveemjl.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2qdxnjdfu.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2bubqppow.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2sptbaymv.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2khtxbhvo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2stnmzifx.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2jyqwopik.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2rpfgpccy.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2touycjbp.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qsanmvhp.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zxjeamxm.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rhlxijxr.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2arlqzwui.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2bkglxlza.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wjtaeqxe.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2fepuuydc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kfufmykg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2itphpmoo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2golxirbx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2quveeyji.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2lmrdhhvx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2smhicbit.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2fmnefimr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2oveefcdm.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2iwfdcjgj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2ktdbnhkx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2kctwbzqg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2atixsihe.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ulxqucvh.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2maaikwxe.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2motkcvwj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2hhjmgeum.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ppjndovf.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ptldreee.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2agnnvmtw.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2aldkptpq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2vyaakrgx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2zxkuvslf.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2oarotpcg.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qxeehomk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2novqvtbe.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2yghrtkme.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ldrsueyb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2lngvqxlf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2rwkbulap.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2yyfshdoq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2fcpuonrk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2cfffjnbx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2dkfxlmip.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2lpfsicpc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ootadgoz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2prkjtefh.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2xpzebkly.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hkgucsdj.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2zddrokti.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2kqkwwqll.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2mmqszvxs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2ctakxzmv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2zwdrxtls.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2pcarzbep.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2lxqustaj.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2sjzgadkd.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2mwuazpwb.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rakdzwlz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2xbhmptpd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2zxuosflg.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2kfribabu.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ebtorukk.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2wivijfsq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2eckkhizu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2mymfsurn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2xfrhujpx.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2uredctgs.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2kuqtlhxi.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2xowtwbxt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2femroroi.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2atirybrf.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qavbihny.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2bgsqnfns.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2rdhokjmi.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2yhntdref.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2saeamjyt.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2sbpcbgoz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2hgawotsz.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aylmrryu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hoaxksaq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2rhdykjcy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2pqfwiype.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2pddartdm.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2wsbpqbbg.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2flgkhvxd.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2bkbdmrho.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2hytldsut.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2idljnszc.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2wkjxxmyx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2cobxeibl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2kpntqplx.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2nixnvzve.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2stczmlfx.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2ckcwjsag.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2xhhjnwxg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2zqvrccbu.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2nglwkpyl.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2hdpgvysj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2aoilxvcw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2rnnkfasw.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2wpshpxpm.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2tdadvssm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jnirbgmk.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2mcmobhpe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2asgoahlb.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2cybrvagi.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2ixrqlrqa.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2cdepcubh.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2jmyvoxql.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2wiabozrv.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2athxjalx.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2tzrbkykh.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2wfwrpcjs.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2roqggpcw.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2cqnjsugi.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2xhqmmthe.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2gicwsqbt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2xslpxxpk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2rwlnbcll.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2vrwubkbx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2astymtrj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2gbvkfvcj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2jlziyvdm.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fcmnwfwa.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2bypjsagp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2hyfaxdol.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ssvtwoin.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2webxeivd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qdskyqqn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2giodlngz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2didwplly.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2mfjuvoxk.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2svtnspaj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2imxynsif.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zqcsdsek.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2wngvibqn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2deqslzms.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2jyjpfoyp.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2qnnjqmtm.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2lldlioeb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2sxeldtsn.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2ifrbwbbi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2hvveipbq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2sfxpizbn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2zypmbdiz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2gtumdtwb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2ppieuwkh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2meutokjr.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2fqhccrtv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2zkaqvbkl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2ofenudmr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2sgljhkiu.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ffsostjx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2tmhyovbk.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2vioxwtjy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nqlnxcso.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2jrsncjrv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2dsytxcep.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sdnawmat.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2cwahsylu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2vriudhyk.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2oyzxdswl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2gvtwaokf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ftbkiguh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2jppzzczx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2boxtkzug.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2xniuqnno.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2emalcjkm.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2hwkivdrm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2uimmcmlk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2qdxsasfj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2jkusxfra.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2pwmeemkt.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2xomqcprp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2qlfkdvun.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2stnygtmh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2oblwiwix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hsetzric.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2iyfwrywn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uwjpzxko.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2nvwershy.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2ldlimxzi.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2nrdxjsrc.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2bhsczzdh.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2zhudslgo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2jwzangen.html

);
来源：http://www.52xcode.cn/Article/details/gt2mvjgpcqd.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2cgxkzwqd.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2uykeehmu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2coyucfxe.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2xxztpvku.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2lflcahgi.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2zahgktix.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ahexxjnp.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2exnfuzer.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2nmjnxift.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2cnyuoump.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2adxeaybo.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2yzaylruf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2cwaabkkb.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2gvllbfvh.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2zghmxjwd.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2oxahwffp.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2ecpptlhd.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2avslygry.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2getncnfr.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2mlclafme.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2chdaxwhy.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2cseirhxf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2syadqxuk.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2rizywduo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2fcyucorr.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2lwkkjecs.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2goudemgw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2zhatsjhe.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2yvoenpms.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2hfpzpmse.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2amwsnndt.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2wnyftzgm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2mosszlnt.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2gzgrgwtq.html


<!-- 参考信息 -->