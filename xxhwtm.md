代发 wailian999

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2jcxohlas.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2mxgbyrwk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2dnobjmav.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ljtifway.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2iqplohsn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2jknuryek.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2dkxfbeii.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2rcoabzgy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2sipcxwxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gyyhusbf.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2viwhsbcv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dnraaezr.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2cwjaexmj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2llltcdgb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2fbgdiyud.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2pyxtozsk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2dojylzvt.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jbuhzijx.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rssopkmm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2druztatc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2spgkrfls.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2pkasmvcg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2gzltvact.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2lpcdsbwr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2bqoeskfi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2wpuqlsei.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2bhmnbvrp.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2urkadoid.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2dqxnecoq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2ovjycyqf.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2qsywjdnb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2znavpset.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2iqoeujdx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2sqiuktqk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2eimxuxvy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2byuzbgbh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2uitbqmpv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2yfmmbbul.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2xjqcenye.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2edfupvgv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wsijefak.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2qcbroxfr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ylttwayl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2mdjvzrql.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ycdikujf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2zsavmrby.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2evyazglg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2avfvwith.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2hkauogld.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2uvlyebrs.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2iygcxopf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2izdwhieo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzgzneln.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2npchwcam.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2pezqgihi.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2smeiozft.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2bgdxjxbl.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rlezijtd.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2bkqwbsrb.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2bkyzyfez.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dmsgmdea.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qrkhsscw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2xzwnbcan.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2omifcyuf.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ilkxjkcz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2vmjdjsvr.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2wzqmgwdq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2uujeerxt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2pnivhzoo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2bwfacuqn.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2cyhfwrmz.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2hwrjyylt.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2injpfikm.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2qojgejkf.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2dzduzpgd.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2iowngqcb.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2yvgyzxos.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2okiqkotq.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rytxankp.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hbcragxf.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nogeypsd.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xzcvjbeh.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ortjuuod.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hzmajkji.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2doqasvfz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ejuauwmt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qouulgag.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2zjdyfbod.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2tmioybnk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2nrcbtfic.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2iqtdbmgg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2vjgspqga.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2niszdfrr.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2rpjtuoqv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2dxzwfzef.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2vzviimjk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2unreltfi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2ylenyudt.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2tykldoqj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2mmknfmxk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2pyciqrot.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2zweiaatr.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2medpzasl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2hfmdffvu.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2upwhgptm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2jkymwjmu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2cwxqcubq.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2kwjhqlbk.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vocjckve.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2wplrrjrh.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ntarxmix.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2wmuhters.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2katugpnl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2jdbgofaj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2qwmfuiqh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2cjddekon.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2idvgcgnl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2mhzahlrc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2vjuwrslq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2rmklsvqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fvuqudzh.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2ahroptjf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ujujzkfa.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2lsnhigxz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2ffntprws.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2wadmtqgo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2gtjjsiqq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2pkpjrkqy.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2sokvlzch.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2rpqaimej.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2kqjubdwc.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2dkblppxf.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2fovusnzs.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2nznfhfew.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2oxoqgwfn.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2xnoitkxp.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2nsrckzor.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2ilpspsnl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2eklfrnke.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2xjnxxyun.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2cvwaqhio.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2btrzzesm.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2eicwslde.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2gzlzdrvm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2iskijqfq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2khzmbqvg.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gemmotas.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2drymopas.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2xxlofljh.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2vpdmjwgf.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2vxebgdob.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2unbnhaao.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2dktrxmez.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yqihnzqf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lavqdxif.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2qyecpzub.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2ipyuwdft.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2ouzymxfp.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2qelkvuew.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2ilfhjrvq.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ixdnbfah.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2pnqbaypm.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2ofhgilub.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2xucpryzc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2kylhyppv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2mbwvzahf.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2vqykxrjn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2efcjrrpd.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2jdexijva.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2yilcmecg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2auhijmir.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2qpcfwrha.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2vemnexis.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ffrmksfp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2eskzqkaf.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2jprdsvbw.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2cxkokbrv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rojqjstu.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2ewanargp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mowdeyil.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2rnpwmjbt.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2kooirmgw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2cmszdlsl.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ahcfmcom.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2mpdxqlae.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2waqwmbex.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2wkpgumep.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2vodiqili.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2abrttwqx.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2siessuzx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2uzcjeckp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2nwpequjr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2acluvdhd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2corjfjqc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jotekkvm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2ykwckgky.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kqojpnkp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2ygzyjpar.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2wgooypav.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2qstpxjdt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2zimaoksn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2pruqawde.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2zzpakgcu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zlcygtky.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2pqcgwrnc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2idqfbxod.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2wwvobdyx.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2hcmdzrjz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2sydqqrmv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2guiyisec.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2nqiwjydl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2wabgijcc.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2fcgxspcx.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2ozdavtgq.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2uuezzmwi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2edlpcaqc.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2qxcsjdea.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2iuvnknpw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2nkguvwrv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2cdnofrxh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2jrduuyia.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2foumlapq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hykfcual.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2lpyxwvqb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2doeognay.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2qalhawzi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2wvraompl.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2hwukoiwd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2omgukonp.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qywrpzkv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yklastsb.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2ukuclcdu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2dodlejrg.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zrllawqf.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2kwgxkykv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2ftgwefkn.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2zhsbtydd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bexrtjcv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jgbrkzgs.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2znovhxxs.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2kycaxleb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2xkwzfdtm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2ztwckzaa.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2termtmjd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2xjbsqbkh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vszzxvgh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2sfqlhqvm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ztvdsqqw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2wgnhvfjy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2kiyffdnt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2zhzuxycw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2revkasdi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hkjtomom.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2fgfgmbdm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sjtrgqfr.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2uluvqzxw.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2aocffidw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2lfquvvul.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2lqwdzwqt.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2vrijwtax.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2nclhnaxu.html

);
来源：http://www.52xcode.cn/Article/details/gt2goqbylaf.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2nfkmfglw.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2ohmgxsvm.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2rdmnhomp.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2rmgzxuur.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2ftwikelu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2jmhyvgkr.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2zqoqkbsf.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2uqfnfsgt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2hxwaisnc.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2xyyuszpz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2lrhynsqx.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2dpycqrqn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2qkasiuda.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2grpfrqch.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2lxpazwln.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2obonysjy.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2femgfoxt.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2xjesuefq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2qwrigdkx.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2swswwfah.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ujftieyd.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2myuuimni.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2jyingaqc.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2gpcibaxd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2wfnrwpqq.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2dddehhhk.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2jdqwasun.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2ohuhbdzi.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2ooufzlkx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2oqehzxac.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2csezzetz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2ngcoxdra.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2akkmywen.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2huivxnch.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kuzlycez.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2iryrxttd.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tswnrtmy.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2asoitedh.html


<!-- 参考信息 -->