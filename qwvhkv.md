代发 wailian999

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3uqulrfek.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3bnllhxte.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3bndwzrlv.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3gvsuhdez.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3bhsxhbsb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ihzueras.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3azkvfwsx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3lgojonxv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3fbtanmfk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3htzspbpp.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3nmykadch.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lzvtxvqq.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3dheeabcd.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pkvwirdl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qjirlurk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ahwxwzrm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3xxtqyjvv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qsirinel.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zgtgmwzc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3firqxcnm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ugbxzuun.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3fhtlqzom.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3zmmijqqq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3wsumvwek.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ekubstsc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3yjccftiz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3wmomyflu.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3kvmiaqhe.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3mxdxhspr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3clzrijti.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3ccffxkma.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3ijgmjnpd.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3jrmkwvdn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3valqzftp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ywkowaek.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3crcsqyvw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3ksswrhxk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3qdurzsdf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3gkqxrtlw.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3vpngjxby.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xtaqbseh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3zmlxdtpw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3nnojiqch.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qtiqmhgf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3dakibefd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3rbswvqqh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3kwrqblbc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3bykpekpx.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3btmcksgq.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hkfbnkrk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3uepkqbfi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3gjcwlcqt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3umiylpav.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3tyhutgno.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3kysdjqwh.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3mijubwjl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3fdbchypf.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3scwyrfjg.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3tembbjlk.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ujazeahn.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dvuaayun.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wmmvnxgm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3jmjbbbsu.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3gekyeram.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3wgpgvyyr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3wasbywpk.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3hjmkjrsk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3xtzswahh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3zugfwpmu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3coccsyrh.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3fabcnkkn.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3nmhvehhd.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3vaneubfe.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3rdreespl.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3otegsfzj.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3xjmfhzfn.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xxhlfvnp.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3wedrhuqo.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vhucffoz.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3axgycosy.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yzkzmkvt.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zocdyvug.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3spjunyzt.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3shwvfxih.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3roecvokl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3viqfibaj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vmgldnhu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3syrkfwzc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3gcwavtqd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3jleixcxj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3xfhpecvc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3riltfxjx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3caodfnmv.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3orehjagt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3keqsyndz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3iengkjhs.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3mcbyuhmx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3dwakesbh.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3qbtftffw.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3rewsgtec.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3iylcwoks.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3vayhetra.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mgthhhfp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3ptezzlvr.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3cukugzwz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3mcgaeppx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3tyfsjcjg.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3zdmrfyqb.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3kntpozcb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3lefdulwy.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wkduhenu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3hosundnb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3jnkmebiq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3dxfkdmji.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3gmswljai.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3kfnuftph.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3kjtlcruj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3syaggytl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zszyulbt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3cwicisou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pgqhoqak.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3zxripdph.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3imiewrpq.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3qhwgqjro.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3qlnvqryl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3oyzuvzjn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3pnfavvcm.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3byzzykii.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3wndsqgaw.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3ksqqdgwg.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3hnypdmtr.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3lvhtguof.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3uelmyhtc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3nljphrbw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3jnlawghn.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3zzwbfcju.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3gysblenk.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3rbvwrmmn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3fzhihdpi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3hszvhpst.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3ruobluwc.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3fjjnatdb.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3rmupropf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3wonukvie.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3zpnvxewu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3uavzqyzy.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ijdhqqew.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3ypfrtqlf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3lzrepcyk.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3zweapskp.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3xjrkllpk.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3facwzgdi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3quljrkui.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bjvoiggt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3zrdudprr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3qobxdqjr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3kjamafcn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3gnzfyitl.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sapjozzv.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3fhpzvybq.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3mspyhwpc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3nyqursku.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3hfxteavg.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ykxpbhdx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3hglzjswr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3acplypxx.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3wstktlyy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3mgvozqen.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3lsylsnqh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3zlihzcbu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3mzeijsxf.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3xsbarahl.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3bwdspaol.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3qctbwria.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3jdynsllc.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3brwpgphe.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3qozleffo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zjztbnnv.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3uuqhfdew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jnprumpz.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3xydasrcz.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3akeygxvd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3lwkxxuhz.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3lsqndyaf.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3weoijwoz.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3wjopqeaj.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3cmleelxz.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3lzrnexer.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3zkkdbpmg.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3xjvauzwi.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3xilrtozm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qoqwgjsf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3gytlaysd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3ofxrqjcl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3sbybdmbz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3lozreuba.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hcrjtiiv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3fxonpylv.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3nfnhdhni.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3ishtsbxq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3fzcjkzjw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3yeppvljn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3xraemtpa.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3ykxrhcou.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3puylcncw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3nvtozbjo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3adwnuhgs.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3rtocxoku.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3rfdmjaki.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qwlzvfua.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3gdnjjytz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3hmvrhvdu.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3tjntshuh.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3wsjeomiw.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3ohptfdds.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3dmanhohi.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3uqntddxy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3erthfhip.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3xmojfols.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3zgajlnmb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cwxccjdd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3lljrniwb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3byzhijvn.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3dfcawfnk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3jgkaqsvd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3qglnnpvl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3uwspzbun.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3chdrwgik.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3wqropcaj.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3vzmjraje.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3opxaalqt.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3rtrlwhyn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3mhmmckgr.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xnsmdjxu.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3qkhcougw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3agpgzdmj.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3jxfnzuqt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ylbccyzf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3xsukkval.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ikjfhljn.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3wippcfju.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3yjzkcxye.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3cwvsxutx.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3micswvzb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3qzvsgbnf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3wzdjdeyd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3alotvcvu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hskoarqf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3fyrvfzxk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3kwwtbmmc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3azuesgrc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3iwdraojq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ucridcio.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3wappqsrw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eqthpijj.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3nxpycxzj.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3abrfiqtt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3afcxzztr.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3eclagvll.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3fapqquop.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3iiyvwcxn.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3bqcaarbh.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3jpcafqth.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3sxigaqye.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ksppyhse.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3kugtrxqw.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3pldbpvyc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3hgyinqob.html

);
来源：http://www.52xcode.cn/Article/details/gt3okmtgaok.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3ocrrsqnv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3rynpjfox.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3oiymbkzv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ythcdjpi.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3hovqysjk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3txvpkmku.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3byhudfji.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3jlfdzcyo.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3qqfyhbnm.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hmxkpkui.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3jfoalbjv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3mmvqyakx.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3lxsgbtsh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3cfhifxrh.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3guvomyfq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3bvuwnqzy.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3pjhfrutf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ekdyjcty.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3ufedzbiy.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3ayfwnuuo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3etbzddtf.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3hahbowmb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3smcppain.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3fudvkqat.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3stzgvfdx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3exyylztu.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3gnixektb.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dtazqirr.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3mwhteqqu.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hflpqnwx.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3znksskmh.html


<!-- 参考信息 -->