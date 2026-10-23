代发 wailian999

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3jrgassdp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ntuqtecl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3mrohngrk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wruszber.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3bzocpjzv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sxaopqnl.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3onzlqevz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3cfxbrfnk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pjortxto.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3jfdwulrf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3lrkswjlz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3qcvymzix.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3evfcmhaj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3anqcekex.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3rirjlfiw.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3zxpnuokz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3btpnaomb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3wsqycbel.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3glwbvlku.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3ovraucra.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3eagoeonx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3pthzwixc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3aooktjcy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qttcwjkw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3ybhsalds.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3uhtflkhm.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3agwuuojl.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3clwbmakt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3yknxvpav.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ynwkmolq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3bmcnxelj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3jnmgncyu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3dqdwleyn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3apzrqcqt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tvfqecyy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3kmzoubxf.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3azhwnlqn.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3quhxrjma.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3esybwmew.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3axuxvfuc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3lfecscjh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3hyzvrvgr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3mqxvgfts.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3slnvzumn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3bhoyfaym.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3hodpxttz.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3kkuxpxsl.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3jwnjkgxy.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3deaaxiyo.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dlhjaedw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3fdybinxa.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3pmbppyie.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3lsmalohj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3lyzwyzoi.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3urmtbhei.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3bppbhlai.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3xhyoqvpa.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3htljjxen.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3qizbkgtk.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3adibicmx.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3fhbzvvrl.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3emlcvokn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3wvjbrrms.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3fepjohvl.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ndddspgi.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3tbjyteeq.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ssxyfjuw.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3oihdzpex.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ptplmlvw.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jysfctiz.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3acjvpnts.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cripfupt.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3bfgfpvwk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3nfaenbve.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ahvxxiij.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3duyayvud.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3lqyirvxw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3pdyaoahh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ehzzpcug.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3xlmpvvyv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3owelrukc.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3hfnyovwl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3cnjcgbfp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3xfpzawkg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3udmvewyq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3nwwzkydi.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3nhhxaips.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3kbebggat.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3piimssbz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3lsdzesak.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3arapitgs.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3bqcnrqfs.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3htxfkjev.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3mmbgtqck.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3weoktmkl.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3tgusrwsw.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3iqjtfjto.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3mdqtdlqf.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3uuxzpybh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3tcwcbnis.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3xtzaiwfm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3vfswzttq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3fjjcopnl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3hchycbmt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ogalfjla.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3rppzwrew.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3iyysfvrw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ifklhaps.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wewogeiz.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3whrxdalx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mjpvbxfz.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3iuoonrwp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3bdjzhrco.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3tlegibzk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3klaozcbq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3quvrwiuj.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3kvmemupe.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3cbccothm.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3obyearwc.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3rdxulwvz.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3qjogxwwu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3zygyjqxh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3gbekwxig.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3adffgvxs.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3btmepwll.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3sckxxvgg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3vezuixgn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3hweqrdch.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3gbemldrj.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3vpchcxxq.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3ujxkoxhx.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3rnxpthan.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3qluwrdly.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3mjkdjukn.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3jjvzyxik.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3ffirrgob.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3qopeaugj.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3spkmchjm.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3letwojmq.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3rafffmys.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3xzztkhgt.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mkzlcfqj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3aghllqtk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3imccpetm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3exqaoxit.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3ppezruoq.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ajgeaola.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3rsjmdwbb.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3mkibhtrn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3ojqleobo.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zkllysjt.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3phidhykz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3pyxhksad.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3rcqnwdmj.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3wqbngclp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3mtcqdasi.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3yqcckyrr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3iiwgfgmc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3pptcqmif.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ucbebhbt.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3llffqmpa.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3sbdcifqh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3eremxozp.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3xtzymuuh.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3dfobdprb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tyvxnltb.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3bjerscbp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3olscwrnc.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3orfrokjf.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3vxerodtz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3urdjtwrx.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3zrzrxvot.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3qcvnizje.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3ppcvgjro.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3mlwdiblc.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qgzbrgai.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3xrimebtd.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3uilwaopu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3dozbcych.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3klcdulzq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3hcltibcr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3noytvauy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3cydrbavg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3wwcvlszr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3bofutyaj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3azdowoqa.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vvtrapfm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3zmbklpgg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3kmpxcekl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ynafjwkf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3cqodjveg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3bhukukjl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3hyamohkc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3bqzicskj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3ffvkxchq.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3lfzsqavr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3gfatbtsb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3pefuuovo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3jgfajuwr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3wygyabgk.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3nxduzjob.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3dcjgugnz.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3zlkglhpa.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ydtmivxe.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3axdrfmyf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3jhgktbfq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3rpeepcvs.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3wczijsxh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qvbojfli.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3xtadlhgs.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ncocvnob.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3eysbhpts.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3seliwcas.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3hchzaaiy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3upoijjit.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wjmszojm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3excrclfw.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3grarbdxw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lprhjbxt.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3thwxojun.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3lwtxpiot.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mxgxbczv.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3qmbwfuyx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3auwnvsst.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3hmwajnbc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3znriavtm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3uweglxad.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pvcwtzgs.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3kcurcfen.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3dylsnwqg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3yvdvtpzw.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3uxakitwm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3rvdfoxzl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3gelbamzw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3dkusqafg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3stzauihw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3fiunhpro.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3ykyxdtwu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3lncttoxt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3beoiohti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bsmeukns.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3bvqmrrff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rscmzvnk.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3nqxgpeww.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3kqowjdpg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3uorncbsc.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3axgmchup.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3mnsbrbgq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3vxpgflyw.html

);
来源：http://www.52xcode.cn/Article/details/gt3ysjvchjv.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3oimaoduv.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3qbnwxerf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3cgnynnms.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3xgcvucmg.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3ydyfceyz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3vkxtowfj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ecseekfg.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ynahmjdz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3bonovobo.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3tdlaowkh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3cfwxltyi.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3mibusuxj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3ticqrejl.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3vrdwuvzo.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3cwmxegjm.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3dstjokog.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3zhnwheif.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3gpjaibpf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3bxjvjmsc.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3ppsfgogg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3jchcawrd.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3iouvyvfw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3hoacbrgk.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3mhsfdtko.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ndwfdsoe.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3ifrjxveu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3ptkyjzer.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3iwqoqwog.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3vagdbqvw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3megbesfn.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3qqrnshqx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3sfnqkmkl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3ekuyrrvf.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ngxfaqrc.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uvatvyrh.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3hzwesatu.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rnneapiz.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3unpvgakn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nezamgin.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3dtyyqkcl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3xkexhubr.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3ofqtxsbp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3ogwnhouu.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3bqfxtttm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tbjcqfds.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3rmjygned.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ztnsvika.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3ienzyzhk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3slvzjlnd.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3undbwyzn.html


<!-- 参考信息 -->