代发 wailian999

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3xtlyupan.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xnzfdwvd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3csrbsyxw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zqsqgwgj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ngresxzh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dmidxkyf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qdzucjan.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3tqcfvhwy.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qktcsipv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3kozgsmdy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3dzigtcel.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3wqcwgsuh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3hqtckivs.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3gfatcnwq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3eovlvqkw.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3vozvlyuv.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3woytcuko.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3xgriryug.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3gckvixrs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3ukhqlvvg.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3pdtjhjou.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3olejszuo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3iksovypg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3hwmtauej.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3roiaubab.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3zwafwywq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3oiyloivf.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3cdgetpfq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3fvlfsmpn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3fprjyevt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rvgfvtpj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hfsatiim.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3usthsvmh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3xyjbsnrr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3gwnuvjnc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rwzviuuq.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3fpdynhtl.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jecozvlk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3cgavsggi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohgcfowi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdlwqscr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3xftqcwjo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3mwqhuhgg.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vdjseeab.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3buxujqdv.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qfsrppac.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3vsarbrfi.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3syvohjit.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3adglitfn.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3swbyjrhg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3pcwisvsk.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3umntzlal.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3sxvmlmyr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3yajwnsit.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3ennfarsi.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3taluhfxi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3yygfcqpb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3pvvgzzwy.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3dzptajnl.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3fzrttjxc.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3ynukdwul.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3whmcxddt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3feeipxja.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3qmyautkm.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3easdeorj.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3qzhfinlz.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zmcgimqv.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3imoovsba.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qtpfabzb.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ynybyrpn.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3rkvdquar.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3bsvldnra.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3vxumylfl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3ltbqhghl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ptuvjsnm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3nzjmiwfa.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3esmbzyca.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3lqkcruaz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3juhlobfm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wiczqwyr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3rmjtzwtf.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3wmzynptc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3qeuehidk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3iuttdjkh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xxczngzt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3hyiooeuc.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3qfmhbpab.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3bciohqmw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3qaneelze.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ivgjdszf.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bpeddadz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3fovbocuq.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3toovfmgu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3dzyyhyqz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3pkhzxari.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3nskjqraq.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3emwhmreq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3memumipi.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3rlzxmnfg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3dhuaecpd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3qsraugnx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3kpzqekoj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3vfzdwxym.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3pbkaiizc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3mhggqlov.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3vzyhnirf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3rlvclpao.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3fobbdxsm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dyibmxej.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3uashgvtx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3schjssfr.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3tugcypbq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3xobnbwuz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3zeuftkbg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3qmmdijff.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3tiblfivf.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3hngrjras.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3olnkbqkt.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3iyxgnlpt.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3wwbhspcl.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3tsxvckir.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3xkflkron.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3ptgfontz.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3fitugegt.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3xuvhrnht.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3ecbvrgtr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3lmtctoms.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3tqjeqrbk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3iouzrhgg.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3scytlgil.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3nmarsyxj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3mnyhbpor.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3yzytxzaf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3bzdujcxe.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3lkcdynot.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3cvitpuio.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3pxqxogub.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3btvnxrix.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3rgzyrvzs.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3pqwumlrn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3ujkzgoev.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yfmhmspw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3uouiarwq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3gqyuqddy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3vekohozn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3ffeyvtth.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pyjhloqo.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3ryrjvnvr.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3xgbuimfy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3juebkkui.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3rkxduhcq.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3qwgoevhb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3bcbnyojo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3nqadxxlb.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3mwzuffzx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3uhozhxxm.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3xsfghmwl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3cpmfwskg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3mwuluzmt.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3efbqtlrk.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3xepcalgs.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3ocehgdld.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3ixtknvjt.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3vcacyomg.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3ajipvnbo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rwjbdmod.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3zdfsrhpi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fzfyhkcz.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3gklqhqey.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3atwisdjm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3scyyobui.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3swvwokqy.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3nnrlsskv.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3hkkblgwb.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3dewvwfwj.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ammzsubm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3uqqekire.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3zasntadc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3daihchva.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3knssudoc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3eqkltzvu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3udccklca.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3zdlrjvyz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3qwobkmpd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3umqiatsa.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3xejqmsdb.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3zpfmkwoi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3xnzuinvb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3jjnhuaya.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3vraqpsjl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bnzpditr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3aattpduh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3yznappop.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3wsdnmbxq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3pyacprae.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3zdelojce.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3ylcjbdcg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3tubxcqqs.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3rfypbsxk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3rpohqgxq.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3xbvoqoat.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3awixlnyj.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ythbwnlm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3gkhiglwg.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3lnhwohyy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3sxzyrmfr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3vvevuefl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3pnqujjep.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3hfnyutuq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3mqovabae.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3eisgajvm.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3dqjuukod.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3veevttxb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3ucwktibx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3rbwpbmdb.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fmndynfq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3tiyelaso.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3asbldhgr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lorlriuc.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3wtuktino.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3ejpnetje.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3wetsjixu.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3jejfjvpp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3hkibvdis.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3zwygqvyz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3bqebgiye.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3tfbynipl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3tzjqebfi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3eistjtac.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3jljjfvqi.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3tflpomwe.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3vtikenoj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3mnostaby.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nczixssi.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3drkwhhei.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3blgukksv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3vjzkargk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3aqzqwrkd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3tgzidgex.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3llcmfvqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mntsuomi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3sbhfimmv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vepsfkqb.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3npdmsdpy.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3uwziypre.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3xqrsozli.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ulomhwcv.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3cjzpqlcr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3sdagnsns.html

);
来源：http://www.52xcode.cn/Article/details/gt3zomwcwmy.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3wrobgqua.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3txchnjxf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ikgunuwb.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3vwcgsulk.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3lppimxic.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3urlezodl.html

);
来源：http://www.52xcode.cn/Article/details/gt3pjpexjsd.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3zvxaxzky.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3xbpxmpqu.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3xqherkpo.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3joffedci.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3djffkztd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3jcgxfxrr.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3wlmqhbuo.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3mxoxyrbw.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3fxgwusiv.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3rbworceo.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3xqvugtwm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3fbfpohfo.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3deyvddne.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3gckawnmo.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3ijegdpmz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3wrxoqifu.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3lyruybbd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ycefynma.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3eqqeheuz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3vyugqyak.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3uqiqxeph.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3kqyjnezg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ytvzyiio.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3hggmvuan.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3ctvpxkez.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3uetmavhu.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3jdrzxvmg.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ydcagprs.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3gipzpdhc.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oommvibe.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3mvsqawfq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3atuzjhsa.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3cdpqlfbq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3dnpaqvdx.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3duvhiciv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3vcmcyfov.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3lmxacbkt.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3eiraxrie.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3lssalkpe.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3eiqqcjdl.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3fsfahrqz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3nktehcsc.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3amvwcfpi.html


<!-- 参考信息 -->