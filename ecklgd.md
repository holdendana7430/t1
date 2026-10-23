代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3czkousno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gdfdurhj.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3hyesyyxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3unzeezvt.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3cshpxcbu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bzkjfftj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3vtgkitsr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3uubioflz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3wbvqyitt.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hatimbys.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zrsqwawg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3uqphuwrw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zljjcynd.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3lhliuebs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ofqwwgrk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3pxqjmmgj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3agbuimau.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3fmrmxgpb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3kvrteshe.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3zubpuohi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3hffgbqvf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3gqkczrcp.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3rortnqvh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3sqkgehtw.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3hcpgxmec.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3gwkpknkp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3sbxbdeum.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3lpbbjykc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3nbuwytzm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3hmofwued.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3tayqeuzm.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3bcajggqz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3prbmcmdc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3mbfihqix.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fywhlfmb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oajdvjrc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3rpzavqkz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3edivaffz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3qghtynlz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3wartjdyi.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3fwizruyg.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3umkzkviz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3lhdaccpz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3fivmgqca.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3stqwzppy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3kzbokusx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3cqidmkhx.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3sgdnnayi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3hsrajvsg.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hlgodnfj.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3zprdejzr.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bfjfzzpk.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lzkvmcup.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sbuqctzw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3eecykpej.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3womsvugz.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lrnxnnwk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3fuswobic.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3dsvajwex.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3nuflnbaw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3ujitxfcr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3vwfrvtle.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3jdkfntsq.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3rfpktahi.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3uswzobwl.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3xeygmain.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3zagdwrds.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3dfvaxetj.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3msnvnvxv.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3yayexefl.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cltxeokm.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ukuvtzov.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wwksnkmo.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3onfcxybf.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3haveinon.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ulehcrni.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3hrdkrjyr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3yssfgqli.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zwbbahvd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fiprxixy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3lyytvuhx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3zdzsrxxl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3lqjbxcxm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jllhyima.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3utoldqmw.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3vodwyeie.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3vbmkqttv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvapixve.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3wrgqkikp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3arfmoszt.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3cdfbltjg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3zevwgfnx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3txkiclpe.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3glpdbodn.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hnbuemjp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3kwgbuwkp.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3tirfcshj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3quukomew.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3zhjvxktj.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3vefuqtdn.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3womrrqmh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3dglonxhs.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3nfuaiong.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3yacxkmrz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3ntrqwfaf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3ygkcpult.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3zjfozmqe.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3fxdgfebq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3mlffstje.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3xqtzybge.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zifmqomd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3yyykbski.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ctycbnqk.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3miqwmkfo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rzybtahb.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3ylxnlzci.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3olldgipg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3zkdoqgaf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3yqvpimtj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3banndpzv.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3heevkffw.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3lgxuflsp.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3hhhwmywg.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3lqhghqms.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3zzkmoixj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3dxzwecuh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3zliytyby.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3odrddwrm.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3kilbsjjb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3jwrotrzi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3nkdlrlmw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3tsydbdqe.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3pujzfaot.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3lihtdgck.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3mzeoiybz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3hsdsytwy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3zfrjcgnl.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3dqlbpqqy.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3wzxkrfdl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3mavyrcvr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3wbiqbejc.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3msllkrif.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3fqmgqjvq.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3umyziiih.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3mlaiegni.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3blarvesf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3lmoxqrwu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3xzfwxdem.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3iqbvlfgc.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3imxugtqv.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3trewssye.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3bqpscmoe.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3rwxkmpbo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3jgyezfgo.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ngxxbqrj.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ffxlqbjm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3betinzdy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3vbjuxkmc.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3psaaluyk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3admmxtbp.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3eypacgcj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3yqlnizun.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3cqinsafg.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3qpgacsla.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ceglrwhb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3uswqcjzf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3jgezlqro.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3qvrbdbsx.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3sctxsafy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lopatfzd.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3ypahgynh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rgirqpai.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ellwspyc.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3zihrtyht.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3iqsbogss.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3jqyvskyf.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3lizgktrd.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ildscgct.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3nrpoderr.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3jzjymoss.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3deibqtor.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3fcyvqvip.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3auntvwtu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3jpgibwdl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3qpuujcay.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3lfdwyetc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3zpqpqeld.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3babsohwh.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3owwqtipz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3phpghvte.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3mtcrwfgn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3maxedvbw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3uzkcwzeh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3fhljidbm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3hpgvsdvy.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3begcqxez.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3roeskjow.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3qyhqjcpg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3gqotmuhu.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3numhzpad.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3alhpxxbc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jyqlvkrt.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3nfcleird.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3zjmryfny.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ppjhbpsc.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3lqfmvdup.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3fyiczezt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3bqhsontq.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3ydqtuegz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3xdkpyqxx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3rhwovbul.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3odkledne.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fpquciwg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3swbotlxc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3kkgzgxgg.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3sqsjrmdn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3frnltzpz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3kgdrxcfx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3tkwqxxfn.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ggtflmor.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3raapinlf.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jcktqxul.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3wppziqca.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3qywxtbla.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3lxnyuejw.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3cvtixacj.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3crforqyh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3omggondy.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3gdnifjdx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3oovhlmnx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3dlugfsog.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3lfcahccs.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3imlbidrr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3tzjmtwyc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3mavkovxp.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3tkjqxhfl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3fiufhtjw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3njwzibbf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3izidglkm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lsrndaif.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3tvyxzncz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3snskpyht.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3csvlntss.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3mpjwsywr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rcufxkax.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3mcvhxlhu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rtnlgepo.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3mlbwetjs.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3lsqsufcp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3rffrrrmf.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3lrvmvvfj.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3mqkmzffo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3njcjgqnp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3orzzvhba.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3kyaqhesw.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3ypgzjeqi.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3mwmwauea.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3umaguyja.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3dksavhet.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3yyuizhdx.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3bmhfuibv.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3jhbtufmt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3nihfnqmq.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3qddnsdpa.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3jfliideq.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3xegygvag.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3atdchqve.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3qtgpnmnz.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3ccdtymrb.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3thwhigef.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3kmdhmxrq.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3sacpssic.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3sldnoxgx.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3mhojiujm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3pljijuya.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3drddnubc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3oytgxdwa.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3kultkxze.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jalgposj.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3ubrlmorj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3kthygyhj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3wnbajuoy.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3yjgijmst.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3snayvbzu.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3mdxxyayg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3qzyipnqw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3krwhllqa.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3hljntaqp.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gugvkzsl.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3bakattbf.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dsbjjfcj.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3uytkrtph.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jjkfbtbk.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3seyinybp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3ljcqnyki.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3qlwccmwo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3lcuozruy.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3mxqmdyje.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3lxujcdtd.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3ygvscwet.html


<!-- 参考信息 -->