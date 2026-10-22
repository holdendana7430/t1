代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2oqkgrlvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sldocmgn.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ezsryxhx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2esyzbhhy.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2shxwdrfp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gwwfmmen.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2puizfmcr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2xbdchhgx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2pxdyebds.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2sphrwvcl.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lflvghvd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2yvuzijoq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zppjkuey.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2zwlmzfuv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ptxbvuch.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2kwdalleg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2mjyalsmc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2lnybblax.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2vzpkveer.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ciqqvyra.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2tsiwshxx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2haqotlxa.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2chexpwss.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2tafwcpbq.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2ahcqdpyq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2lrzdihlo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2pfymfzry.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2otnlbyfx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2kbxzwlyo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2sgkwrjzq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2uzsirqkk.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2yeiuuqgv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ulkrbrnn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ydpxjmua.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2elduxloo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ijwcdczc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2zsjvmcax.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2gaphympq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2xqftbkgp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ykuzuldu.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2tqvwakse.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2gqlifemt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2edquqzyh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgpjzjmk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2xdiqufja.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2oxfzdnpj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2oeqifrsv.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2blipzcdg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2vpmgijck.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ptypbyzq.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ylvsqsht.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2rxwjibal.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vfmnnbvv.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ihejnxvw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2jqdeffsq.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2djkxwhmi.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ihhebqkx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2lwhepsaf.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2aufvizmm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2lcusjblg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2aeuibtcl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2tvkelhjq.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2wscktrkb.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2rymhmagu.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2karwhwws.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2rzfyymru.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2sbfqmdbb.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2cuefwwjr.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dmijxojz.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2zrentsmm.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vasoxvkc.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ajgkfmpf.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2padvyadd.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mkbrpfoe.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2odynyzzb.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vhuacmgs.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2xycosuso.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2grzsmonu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2uaynxngm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2nbopbora.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2tjoiqogs.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2iwcbxcuq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2dzxoyqie.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2mcmmdprf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2aietpzdn.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2rgljbqhe.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2ynavwxqv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2byhwfcym.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2dpgmrusy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2vzteqett.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhwepgsn.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2irdtyttx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2kbifgoex.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnhfvvrh.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qnwouzpn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2txjoqwtf.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2uzbgebca.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2arqzbufb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2weatztml.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2goartapj.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ovhaornq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2gmwucrjg.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jllnpeyk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2iuoebioi.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2dgjbwmqi.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2yghikqqv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2diatfadl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2cddcmeeb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2gkjoszmh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2kcgcurcw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2msrfssov.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2unfwatbe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2phbhkhdl.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2fdqfefou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dzztyzpm.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2lmjzzsuv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2yvvgecff.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2umaofabo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2vcohcfhb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2bcqaixkh.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2wtjplngx.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2jnckjfjx.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2nqpjepmg.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2uyyfutxt.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2jagqniha.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2qupukfbi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2ktotkybk.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2wksqrrus.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2didxzzar.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2bbtxydyu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2skdfobtd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2npdpktrg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2hhsjzevj.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2guroliza.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2dbvmbvar.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2lbwgjjhf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2vrvzmxik.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2nxekbxvn.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2tjgquhwb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2ubguxdxs.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2hmbkszqs.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2pwerilsm.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2eoixbazt.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2zgnhosln.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2zejizrix.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2plcvbmjg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2esvdomss.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2tgoxzdyq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2pxjloddo.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2icmiwskg.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2vlsmwfmt.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2sczmfkff.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2piafqngj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2sybijxhv.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2negrzstg.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jvokmrnv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2rtzqdtgz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2bbwpldww.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ljfwrjsc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2lsgdtkvo.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2jmiclfwo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2lwvsrucc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2gchzngbf.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2lbgexkbz.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2rbbnzlfa.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2tilebhlz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2xcbssewp.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2wwucucbq.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2kalseyix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2huhynnpr.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2czvhkqnm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2royeolnm.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2snhaicyn.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2glhfwvib.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2hcomwlap.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2kiwaxltd.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bpnckjqu.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2aynldzji.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2bqqcanhz.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2cnfetrnd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2cyavqyhl.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2cywatsyp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2dxgywzts.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2zazufutp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2gtrotbfr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2hdezleis.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2esofkysv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2qtefrkta.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2xhdlevjb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2yefqvztu.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vtkjvlgh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2iexlgdla.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2zrxtgmax.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2doyfskux.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ufqzogmk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hubgwymw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2magvshyk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2wocbhwfe.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2bdpsfmwg.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2izjwjsgs.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2ckymsfbj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ssdohjod.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2xcosagfj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2qbvwdecq.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2xavgxhle.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2lmxxqyky.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2qecpbcec.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2tulhgayy.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2ivklihot.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2lvjogips.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2cabwvoiz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2ndhfivmg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2bopmpzqo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2kvhlszcm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2qzzetfqu.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2crenpyxh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2tuxjiktv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2zwuhrlsf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2qfkgzgyr.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2qpnhiful.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2ciolvxfy.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2lgdccjcx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2eaxszrhs.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2imovjxme.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2yumnzkee.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2isigpqgt.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2hhjzasfb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2wgpnorzx.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2zsnwuzmd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2nkuqaooy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2owkwyqzh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ozmdwand.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2czbqfjwm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ttwmqdva.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2rwluiogi.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2ptsgddnz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2bmtoftzb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qndlvzrh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2eazvsdvo.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2hafribsf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2uirqinvc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2stckyzrs.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2vcdvvclz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2omqrtqpn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tjlvshlq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2dlerzsll.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2epvybcov.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2nzyrofkb.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2dgaavirr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ivesekoi.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2nofpdnbt.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2inojuicf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2txafkscx.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2loiaaauv.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2wejyqxor.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2eohkqdyl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2htxylofw.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2nbrcibww.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2eeiwuxcb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2dptnbrhi.html

);
来源：http://www.52xcode.cn/Article/details/gt2wotzyejf.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2llefegip.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2tlhpiouv.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2cdfwwhxp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2yrirngpa.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2qfaagkcz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2ebujuygz.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2rddwsawb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2kskcqikc.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2gtpasajc.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2spprpzss.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2kjfeitzc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2pgkqbjdp.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2ngbywbmk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2agwxatpk.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2frzvbeeo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ljichlqa.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2xjbylavw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2pkowyopw.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2kprjaubg.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2ixskxxfh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2gtdzqubu.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2qfbrlhou.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2zprauobt.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2xhqxrqwt.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2gbmmwked.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2twxelrph.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2qlvcntkh.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hnjjmuld.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2xcaferxp.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ooxgcldb.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2twuapjag.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zwkbssyi.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2qytrozaz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2sxsxxczk.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2jrshmsdx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2swsoidst.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2fzpuyamm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2hwajfnul.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2sdukqrql.html


<!-- 参考信息 -->