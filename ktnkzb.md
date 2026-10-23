代发 wailian999

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3hhdqefnh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3lkuqhnjp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3amhfhahr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3xbhkwqzy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ntyntaoq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ayighqia.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3ytcshatn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hgofrxue.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3shpeohxm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sekvzugr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3htuqfybg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3cugeincv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3bdoasbmx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ibcsbtcz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3urkandpo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3zzrpremy.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cilravax.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3dsxxxrii.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vkuvtgpv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3ocfbzqdx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3zjnzrjra.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3yyivjabu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3ibhyxjck.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3swsysijg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3cuspjiui.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3cilsnexq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3xxgfzzhz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3coiupbkz.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3voeozptg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3etmhckpw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3pliyrjbp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3abkddknm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3udxyecxt.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3xmqtlyhc.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3hopnvbqn.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ncsknqrq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3uuqtknwv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3dldocang.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bywkifmc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3doghtjgs.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3rakuhndl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3ptjlfxqn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3xblwshbu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dshsntdl.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3ayoqvhlq.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3dtdxshyv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3grysjbus.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ctydmfog.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdwcgiau.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3uqagmupq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3mdmxmkon.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3laszoywo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3hokylwxi.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qsrusspk.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3dderbwmw.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3trnrjduq.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3rxvhicza.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xmdjblxj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3qgbswytm.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3ldoxsdlu.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ornwxqgn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3aggsekmk.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3mbmxamic.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3fyyouxzl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3iyvwbprl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3zckdjuwm.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3xajxlvew.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3eeiykhsb.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3tfyabkis.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3woyccmev.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3rpimpkfu.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3npzsjpya.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3gizwnvlj.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3iavasqsa.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vilbryhs.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3edzmhofz.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3luonqfrn.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wameetax.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3vvpgndth.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xfrswcxr.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3rmssdaaa.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3emrhcgux.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hghhpvec.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3cauxwmvj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3urmmvcjp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3recodfkm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3jexhwhbq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qsqhffkz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3fecbzjra.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3fattvulo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3uuvspufe.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3nclvjkod.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3iivgsltb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3rhxarmep.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3dpvpgdfw.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3upsstohv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3oigpkwlt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3lfqssroj.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3snncbbpg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3irvajaxy.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3gchkrbur.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3qcwojoox.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3obneswoz.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3kttbyile.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3hzjggtpu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3zzexhcak.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3byqaxvhz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3eeblrpkb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3malahtkp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3ntngytzz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3zjopfgsh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3vfblzowo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3vxfaptrp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3sphniwqh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3dtdwxvkh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3tgtkcfsh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pvhjjnnr.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3wozjehsm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tzneibsa.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3xbclvhse.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3onmojqhh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3nijswpvh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3lvwvxhok.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3czqfckrv.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ropqzyib.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3wgphtave.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3gdzxfmjg.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3yrlwjxwz.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3skqcwfpv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3mgquilnr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3mtckifcm.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3cqmtmkih.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3jxavfpxa.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3tggqgfnb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3dvqclqed.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3omffbsxy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3fxzgyzpp.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3qgmxvemm.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3mrpbezsm.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3xrttjfnu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3uqqzcqdl.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3xqagialn.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfysvygk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3mtfuvzsj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3bwsbigrq.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3rhmhqrho.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3sbjsvtqx.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3zjqgzqhg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3lzrspouy.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3mkytdoxk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3nczjwekt.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3uejiydiz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3pnhkijup.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3nwkgkxnd.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3kkvnftvi.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3rddobbfv.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3jrwwymkj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3cjcjcmhs.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3snaqldue.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3thmuutsl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3jpciafhu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3xumityqn.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3yliknjfx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3klgtvknp.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3ynekuzdj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3oswsfwmp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3vxintznr.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3nykyckea.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3vnqfvavw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3bfregvzk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3tmjbrraj.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3ywrntntt.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3lvzomcip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mukceokz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3jvszmyuc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lrnufucv.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3swfdihwf.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3epyfcxgd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3mujehiib.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ivrejdug.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3rbcnwytn.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rodxdyhk.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3gpkkfpug.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3iasciwcc.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3swkjjthf.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3jzxilvuq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3njudbcql.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ynckxlqv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3iakgoqjh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3hrprhzyo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3gaxjtlsm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3dkzujwdg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3rdvatilu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3nifoswur.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ohysaapl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3xzfihwek.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3mfptwulz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ddrghveu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3vkuyykeo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3jrrmloxg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3hfnewenq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3nfywrjjz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3lnxnvcyn.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3tmlsjvvh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3xeyqwtpa.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3htfkhdnf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3zavhlzvz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3rzyuonmc.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3eosnfdch.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3ccmsgqdf.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3elqvrkqi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3hkmbqtrr.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3qhtzceoc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3pkzbwsfn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3ffepjuds.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3yvoobsoe.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3qnnodkxv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3caromrly.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ipsbjwys.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3tzknnlim.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3srsyvugl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3dmuetkac.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3mifyqqxg.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3zzewtlij.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3dupnjemj.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3djgxfaxz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ctodqbkr.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3bcihzgor.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3ilzfukww.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iuxrztih.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3evcppjoz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3oxkydhrl.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3inovazga.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mlxsjlcm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3psecrqnt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3lnrliscz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3ybsyqwyl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3yitlquoa.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3pbzgcruk.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3pcvnjroq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3ugarsbkn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3qmxzayup.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3grpyulgl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3oafvyimq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3gmgqqkrt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3jkkzeluz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3acqyforx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3dyedhfsv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kisvmonz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3etyxwqtu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tukguncd.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3bijmhxyy.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3igwuejdy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3xkfvhpuw.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3mmydhxqa.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3ekwubycu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3zfretscf.html

);
来源：http://www.52xcode.cn/Article/details/gt3vibhqswj.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3bsjcmxzi.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3skogrqrx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ccfnvrff.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3skfavtya.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3zqmqdcgj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3lbirqrbu.html

);
来源：http://www.52xcode.cn/Article/details/gt3mqtqvxgu.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3arwbvgom.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3cyhdlwka.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3hxwnfida.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3hqvekxri.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3sgvlhzib.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3qsgzhrlr.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3yzpgvibc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3zifglzdu.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3vcbnycji.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3inryneme.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3fechjazy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ymjmvpqf.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ufbcxquf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3yluttdys.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3tubxttbk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3mymwijux.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3zwuzkkyh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jotcfdnb.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3dbdbeqdx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3cwbqwfvt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3nogdpyua.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3vhdjtvdg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3kaorxkpd.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3wilrpgub.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3wovnojvg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3mebuerpa.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3wsqjdjup.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xfickweb.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3edclleyc.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ylwnmbad.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3dhwjemyp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3btregsjd.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ypqzwfud.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3tfsuewng.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3hcxelkzp.html


<!-- 参考信息 -->