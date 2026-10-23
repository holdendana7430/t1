代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3gbujnpdx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dexxnewf.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ousxijrs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uhxdklau.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3peqphsuj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3duzbsdcw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ulzgojtp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3udgxqimi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3jsidvbfv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3psnvtpye.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3eddqveaq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3ieirlzcu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3icbleyqn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3rorpvdlb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3uleyrykt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3plwemziy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ahnmglne.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3cncephsl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3wgqjgfxw.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3bimzwhou.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3hlhkggmp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3drzyfpay.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3xupzxmiq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3ibokglqo.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3qirzlpla.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3hcdghkix.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3cyssbrwn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3bfgfcrxq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3jtpcjiir.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3hrvjojeo.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3urcokhqn.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ylbxzany.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3zwduhhmp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3acxhyegt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3awzlzvnd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3elycvqcu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3rikzcalv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3otetliyo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3lcaleapc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3wrytybrb.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3nlxvtfkj.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3abclfqna.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mdovoxei.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3cwdsowlg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3invvjtxl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3wfvujvvh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3blrkrete.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3rpumuieo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3bsfdqtmb.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cdoxyquv.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3qhlssovh.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3pgrpdoix.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jkbhhvnn.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3njawnzki.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3zvcxjkll.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3nnflgnkt.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3wmxqutuo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3acjwuhkg.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3eivqxsar.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3qvzyglcu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3gszrwacb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3dprwwtjh.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3adkxqfxi.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3tezukodo.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3arjbuqrk.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3empouvea.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3gjiqttkc.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3cxtjepqb.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3yaebcrbe.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3hnpyiejm.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3eahtazuo.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3bkwvopll.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rmctgdlt.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3isxjdgmj.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3sxndbaje.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gzeutixe.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3zafotzfb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3iiilmvmj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3jpnbbflm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3bflascak.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3dvznbbcl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ruubkelp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3esmpmmij.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dwvlmxxk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3xvcpymwj.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3gdaewjbr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3yubgmwnp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrcebajq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3iutszwms.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3gppeewgl.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3weysvgjk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3mnmylebg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3fvsfbpfv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3zpxlgghz.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3quaaecnu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3zvpqjipl.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3dclnhqlp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3gpzmomjc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3qwhorbsn.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ojcjxkcy.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3xukvgkne.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3xupkrnmt.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wfllvhvu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3qrquurtu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3cumonnya.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3vgqlujwt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3wmlxoiwf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3jpbzmxci.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3kghvopic.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3yzpgxrjh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ibkqlhjs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3yaoojowk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tfeuqkcc.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3ohybmfqx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ohdhftjf.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3glvispue.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3mkvnlzcc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3ohgdpzcx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3oovxslug.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3omaesmqf.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3rwvxusai.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3saeqpyrx.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3ncmryucx.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3hyjxympy.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3xydwkcno.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3etnrcwfa.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3nulvdjbg.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3wngwbulr.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3luddrmjr.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3lkrznvrp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3yscjjhyv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3hmuzzqhd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3mwofspla.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3qfxuwflo.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3dcfpvczp.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3wrfqtwxe.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3pemwtjeo.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3rpxxnulw.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3fumqzvpm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3ropgyrvh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3djouogel.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3uoepfncm.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3jpmssuqs.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3qmhnjpbk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3pvesumnf.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3vzpqeold.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3hemcbzhg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3fbcnnnci.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3xyusxska.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3vkjyakjt.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3ivmwtydx.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3bhlqpisj.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3bhxhtakm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3xqsfpmbn.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3wzfrhhgk.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3emnkyaqd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3oguciais.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3farjtoij.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3sowzszxz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3wtadyepz.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3hpmjjjyg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3kwzbvwen.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3fyiekquz.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3rnioijgi.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ltlqcepc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3czvcrxwi.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3xvdgibko.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3ifmcdtuu.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3vfrgdydj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ycdspcfn.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3hxysldeq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3doeowcwv.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3pmkwyhvf.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3moheheam.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3fhjijrtf.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3wwxuaesu.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3blscbfvq.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3fsdgqqhq.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3tcazceqz.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3dpxkgbvj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3uorjrjxn.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3dnuszmnl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3kckpdxcf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3guydrere.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3vulcbfue.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3nnwemfnr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3okcyvzag.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3vevabage.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gdiripmx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3midediil.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rwqxjivv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3zdunivnf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3cxlxmjxo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3rubxznal.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xjkdeymn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3sqirtkzn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3foayepze.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3sdpmssgq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3clifngwz.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3cbffvqbw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3exzyldff.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3drgrnueg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3tflhlncs.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3xwcqvwxf.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3tjlnlqsh.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3pelktdhy.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3hvfeweuk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3hswxnact.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3rqeyfrvp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3mnlifvtb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3aycmapbc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3npcydpwh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3yzvwbhhv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3hwgfvgms.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3wrotvphc.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3mendnegq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3clhyywls.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3bcimfdec.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3nrtomtai.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hemeqmbn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3rjoynczp.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tnbbsoho.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3achobaok.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3fakqdphj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3mbykwjwq.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sqkkgcdc.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3gwhvtmth.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3eihglfmf.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3imwzyigr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3betdwrzf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3fczalslc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3kdgyarba.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3ysaefqll.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3msvvsmhu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3esoamxwu.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3jraxwfcx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3zglikauj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3iupsxecu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3jireddxg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3srzbemuw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3prebazvk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3joicwynr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3xiftqwzs.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3lyrcpegw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vfjkpivd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3vqaskbbt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hbbejfvs.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3fiytxeua.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3plxvbkki.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3gafiijmd.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3qjmhxvzh.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3ucubwzwo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3lfhcgrgd.html

);
来源：http://www.52xcode.cn/Article/details/gt3klzrjbrt.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3xgyxkixy.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3rwkptqdo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ghbspauy.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3fbrgobvx.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3kwnvsbkj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3hknnxbwn.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3wrfnievd.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3nbjzzgbg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3zsdxbphw.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3hwvqyhry.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3kznwefjd.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3rslxnehz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3amlzpwyh.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3podhsnim.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3xrciulym.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3pijvowjn.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rvjprimu.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3jqhuzvzc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3fhtbzqhv.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3wzplynof.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ndgypjxe.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3oktjfxfa.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3pbnakwov.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3wtsdmvlf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ibtavmfs.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3jetzltlt.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3rwgiicmp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3dzjelcxs.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3ufkcksac.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3oxxpdkbi.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3jwiwbwrs.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3wyuusrga.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3xinflxud.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3lnwrzaov.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kiwbtlcj.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3iesydowm.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3idddoyvj.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3jjxcaxwj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3wwqwqudw.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3vbcnhdsp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3hbevcgqh.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3ojkjkqzd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3fetkkkob.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ogqgzzlw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nilbdvqe.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3zdbobczd.html


<!-- 参考信息 -->