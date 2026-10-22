代发 wailian999

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2sygqnats.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vdqghbpb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2iqedwbxm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xajarefc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2mbvcqujg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2npvfzxne.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ccjvxjss.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2uzwwtwxy.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lpfewosc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2jsiuimxp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2wborlekh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2msprkftr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2hquyhomd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ufecwmlo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2cfsrivqc.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2kgjvhfmm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2epykfplq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2holqvtkz.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2ymmtpurp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2ubfvfzbz.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2skvmhpda.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2gdsaqbre.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ukjrnjfb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2yapcavgj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2yefndqxn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2snsctzts.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2hqaraele.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2hrrxjret.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hhbejgod.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2gaddxdbz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rtrjhzxo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2lyvpoedz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2baaaouyr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2ugijrchp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fyowfddq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ubvilcwo.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2tavsftzl.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2cbpuqbbp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2azytgcfm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2dcyipwzz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2yehfrwqt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2bwkaqjzk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2qhllgipp.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rlojroek.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2zjutsnyw.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2dvsqdhyx.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2qvzgkxpl.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2karizljm.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bumzujxb.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vgpgksys.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2ogydxhgl.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ugtdhjnn.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wzcqnrut.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2pumqnspo.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2fpenzowd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2gfmgyqmf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2wyfmwqur.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2ybjbggzw.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2blxiteib.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2vynjlelq.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2kcxnfpag.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2slmfiqzt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2evvnwkde.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2jcuhdxyy.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2llrerpxt.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2mnkxwfsq.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2medqvvuz.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2epchdnsx.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zwqsurdf.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lfmgfopa.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2tlevache.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mxmhebpz.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2hymtudvv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2wlqvoseq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2plcavvio.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2dfwolnlz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2gfevqtzv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2qbgxnamm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2bjdlgvah.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2rfukujff.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2ascwehpu.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2ofuakamz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2ptqiiurk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2yaueyvcu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2gjbgmaqe.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2yfqqyzyv.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwacnfmu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2agbrgdqd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2zymncxza.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2mijzeauf.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2toxcmnon.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ekjrmetx.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2dxwrjrth.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2nsesakoy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2shvefwwq.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zkvwkplb.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ymgumbre.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2itgoyycx.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zoqqentc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2iifenjme.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ucmtcvkl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2ujhjriwl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ubihefhe.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2tspqthho.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2yjdntetq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2utrclbyx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2opyejnqe.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2mwqlxflj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qjurrxpw.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2aissfaze.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mnbqeidi.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2xtypzjel.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ziuzhjgz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2rmfaaubo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2patsejvb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2oijnqdnm.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ndshadsh.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2hpkuzeru.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ijlnvouv.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2tluloyyt.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2bsqatewo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2dtbebaau.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2unaeunfn.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2tezogxzn.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2riryosbq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2wozyiyvt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2ikjdedec.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2cbmaiexs.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2cezerlda.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2fyvvvncp.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2qthubhfe.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2kddngtti.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2owveppzc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2xrnlclrv.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2seriztef.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2wvyowblx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2dcfektys.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2cqvhmlec.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2xavdhvme.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2kcxueshq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2gxwjmove.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2vfbdjuib.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wevthplk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2umllpmyv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2xotdravw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ybgwjmqx.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hrtepwii.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2vzgvfyhd.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2aqgtpatr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2qzszzlzx.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2hsrtyrwy.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2pjsyhlgo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2mfqjdsig.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2trlxfrer.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ubrmrdda.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2yfcaebno.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2cmyvbdgu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2fmxjemde.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2vsbinipv.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2hibeffqi.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2pysplppy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ddvlaeew.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2dvybihjk.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2agqgbuju.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2feocfxbk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2keylaeoi.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2zctexndr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aahpmxwx.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2nybmyyxh.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2vkkqxhaz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2mgpetvpq.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2wbdoygtp.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2nhzxtaeu.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2sresbhiy.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2bwpfxxmn.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2qvnjbasd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2ucxfiguo.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2eoyabnor.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2bgkqpqza.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jmliklum.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2fbxpczkr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ojclpmvh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2risbneuw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2dkcdjpzn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2tmphxkqi.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2mmdgrrmg.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lzgjvwcb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2gvarubvo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2tjzrdnsx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ntovokay.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2flzovwua.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2wisezprw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2okqvabai.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2fgeeerpc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2obwlsdmt.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2szncwwwa.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2nknvlrbc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2terswwse.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2hhatmhfy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2xkatebts.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2puebslro.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2swtprfsn.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2byuhckkg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2jzldmifh.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2tezajyoi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2myisifyy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2jpqrdekt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2kdcncjci.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xrlkxpdy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2wznrdspc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2dhrprvje.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2ldljjxio.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2kbambaeb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2zwzgylop.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2gdbohbka.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2vgjarsma.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2gwzzkgwi.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2rosyvunk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2zxkvmnva.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2lfgdjhgv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2shxhdvkw.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uvuycvfv.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2moghwogp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2vxsagqpg.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2ikaypomx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2knznshpp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2athrnxrf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2chtidbdl.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2nqsrzsbw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2vlhdctls.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2yraxskvu.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2ivtphekc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2htatuswg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2pnjpfcrb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2pahwjwcq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2pfxpbajr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2nqlyhznh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2sxfpmnph.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2eenkvjkr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2wfaifxoe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cyaiqvql.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2ubrxujoc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nsiyvldg.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2cfscmlli.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2vdzeakcg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2crfcvlnm.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2xmgldhgg.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2qfvaixxp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2livhhqye.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ysupxout.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2tasckuon.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2blhtwpug.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2tzslecam.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ongcblng.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2uvkqpuzl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2xlllcfbr.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2pdlpgrbt.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2vaxlrwlq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2khnjhsmn.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2ovqgjcfr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2jnpucyav.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2rchcqksr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2zmysmjxa.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2omasvexy.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2nxkojgxy.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2orljrwxe.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2dowsrjtt.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2lrliotdw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2gdnvqatu.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2vzpjhdrk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2yclhzyhz.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2uojoubay.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2jrhkrdlg.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2dxyjclvv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2wilazhss.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2xhsinzau.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2cmctxlmm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2euvwmiok.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2mmgqjgic.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2pgerirts.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2afcaggkm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2mudnvzdx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2niqpytvz.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2syamfzhf.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lzhqpexf.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2todwychq.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2awaassfv.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2wcepbgkr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2xvdrkecy.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wfbwjsbz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2abtlqrut.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2ddojodhv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2yibnbkkv.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2mcytvevx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2axwuvnbk.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2ppgjtzgr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2ksphjpnp.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2aljjhkcc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2bcrpkoyg.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2epgagnil.html


<!-- 参考信息 -->