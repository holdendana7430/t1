代发 wailian999

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3zsxhcbzo.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tcckahly.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jtjfwczr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3acrgfdgx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3knutpnys.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dmopuvgi.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wchmrfmv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3odfgeaqx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tcpuqkek.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3iqjpnvmo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ukwdqtvk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qwsjqzda.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3wplrujod.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3nxpyzeqx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3pthypnpy.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fviwycgl.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3eqflqxzm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jeijcyow.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3suotcryf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3wyminwyo.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3sedwvwol.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3dwoenhfn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3tjngwcso.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3mmwnvltl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3zyjpyeqm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3yjxpxtlc.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3jfelithn.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3ymksbwgn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3grpccfhd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3slajvuwn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3eooidnil.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3skzqnnic.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3zaprsirg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3vuggyclm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3utxxahxv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3sdaiclab.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3qztjvhfx.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vadjrfhl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3fckabibc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbtfaxck.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3oupfgnol.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3gzqytcsm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3ukrprxcj.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3zloqhtvy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3odvcvluk.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fvwsedmk.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ayexehqr.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3sugzvwxh.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3teppnbro.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3exjpfcjq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3zmxgllyd.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3qqbqfzpw.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xscsqtyi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ztcouebs.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3tkvhusye.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3klctvoxb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3vdznlrxf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3uaekjueb.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3bhhfeoqm.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3svblrckc.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3gqchhrax.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3yxqhzcsx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3iokzljcu.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3olnqezee.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3kwgdfuli.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3nqykfgfb.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dhsfuypc.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vvuncyeh.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mrvarawr.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cgtifksp.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3ovdukqtm.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3oonfpdfr.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3qcwsmflf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ykmorsqv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3fozupdsu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wdyrtioh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3rkgzvaed.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3sbjdohvr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3odnbmhmx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3gmxxpfux.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3cqjegxdp.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3xlsqycls.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3uxvatyrt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3buxjfgle.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3eihfqcqj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3ukekqypx.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ivzdmfme.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3ukssttgo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3dqzhffmc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3yzkabeer.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3sdvxcjpv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3syzzvhge.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3qvemyepa.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3xcqpoztm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3xgmhubau.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ejyidlxn.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ikwbspyy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3pxbjlbts.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3rqykysks.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3sbmlibxl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3aiisatpc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3nnermtjg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3fqfmyvsc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ezvpsilw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3lumobwtv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3snvqytol.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3jftpdtbo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3yrupekie.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lakiptit.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3sxwpuvvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3euafpmsy.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3yhjjqsmy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3thmwkurc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3dpdbguly.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3rpouymvq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ekdvevii.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3runmfsny.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3rcvfjsan.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3sbgqmlvd.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3gpbyulky.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3koinoglf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3yqawlqcp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3ssvercyp.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3icpsyibv.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3wzivrjot.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3jdrptele.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3wpncqhlz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3pvrxrwhy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3vqwwdyle.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3mncrdflq.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3mkxsakmj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3jhknbyof.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3exgjbwpw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3segkihcs.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3krnajcdi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3djptewey.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3mgmysybu.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fpqmeikd.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3gwysmtew.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3xkuxhpey.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3ezyhnqli.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rbznoemy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3vofnnmgd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3ylcvgraj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3ljzitsrd.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3hhasznhj.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eoqomlwv.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3qjbeljle.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3wgayeden.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3ezjrqfjl.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3kvklzpkk.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3llfuuluf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3wsgfzgfb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3trozpjxx.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3rrpqqvwl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3akugzieu.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ntymcvpz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3xsnomexl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3bylupcsa.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3bhzsfxbz.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3pmfrruef.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3mkhccnit.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3nuacpfbt.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3heplvdta.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3oryfoncb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dyerkiwu.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ccgnemeh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3urcjexmg.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3burvmmrd.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3phqymrdt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3edtatlfz.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3afogunav.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3lczdjxwx.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3fzlxnglh.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3xrldzltw.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3cbisdwog.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3tmoizgcu.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3amatbiaw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3woyxcwwg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3hrmgjzur.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3iutvczdo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3gdbfiiys.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3srwvwdzd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3wivhknep.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3fqsownnc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3yxqhvdxu.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vilpiucq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3bpbvjqzy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3cakxfpfy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3hqkzuhfe.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3vikodakb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3ralggeug.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3mxqajrae.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ywfkcgyp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3qfolpznq.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3hrxpabow.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3jkvfwuqo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xzneoaif.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3hiljrjgm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3oenaqmwc.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3urchbmog.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3vkhmpsrb.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3rkyplspu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3qwytpdue.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3vpdujupe.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3knyyxkcn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3udktojnn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3lurpaibl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3dixkacid.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3bmrjzihw.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ckcawrtu.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3ktankywz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3ehjjqrvr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3torgnlhr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3elgjtwbb.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3foouqcsl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3hzeconfc.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3yafwfxwf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3rjmcwyot.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3atexbzhd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3xwfxssal.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3bgobnesz.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3jjtbxrjw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3zwzppwqc.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3wnsgxwfu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jpurshxx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3wmfitkaw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lsaukadn.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3rgxvasfy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3veafxzdx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3pwpuhyuc.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3gblrevue.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3jrjseuvh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3icusfpyc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3cdkswuyt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3oujqffhu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3coboknpv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3yptbkqzq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3rlrgfckm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3osdqnmzm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aqiotbof.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3gpinpmhq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oltnmiwm.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3wnvswefl.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3aqukfkyb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3iopcclmz.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3xfjlpspi.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3vfkjcjkl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3ezxlepuy.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3wdieuqal.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3fwpeaggd.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3pjtcmovx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3yxpkaome.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3lyrrmpqs.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3dkvwodbv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3kpeqsgqc.html

);
来源：http://www.52xcode.cn/Article/details/gt3ixodvrsx.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3udjqjjau.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3lmktfbyb.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3fibpbkwp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3cznubdqr.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3cpeqepnp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3gaapzysk.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3otbnbnwb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3rjtttvju.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3itslnejd.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jsycyyui.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3vcwfgxpt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3dfkbgttm.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3hfltxybo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3jgzieluq.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3ayzonjwv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3mswgcyge.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3pimsmlvc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3eoffcgou.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3qsvysprq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3txsfztzj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3nrdcitno.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3oxejuhtv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3vjcqsysd.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3pprzepqb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3xyjiilqy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3zpbnagzu.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3iwwfsfzi.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vznyhyfm.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ycxtfdyg.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uklugndh.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3stlgkdky.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3zpwwtenf.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3yicqbvos.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3izzbtycn.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3lwoxaisz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3gdsmktco.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3emvqwyga.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fyhlrriu.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3hluxgwqv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3goyhsgpo.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3okkaedjs.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3xymefbth.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3jmzyvxpn.html


<!-- 参考信息 -->