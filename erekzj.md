代发 wailian999

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2owukxyhz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lumjhger.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2tybesuzl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ulslnurc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2milsghhp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2snmklnua.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fdudylak.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2jrbtvplv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yzkiygst.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2fkurtqpc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2quvtmzeg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bzvmsbsr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2flihxktg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2uhxfzsmb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2mcampdia.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2grvhwvmv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2hsyfusfd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2jdclisae.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2ucbvmgex.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ooyurxta.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2fjdszguw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2lnleffet.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2mcxqtrbn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2gscmaida.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2gcbivfmo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2fdujitav.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2nnuohtgm.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2oixfvhtk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2mdxjcnzw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2yburtkmm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ixmqcgfs.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fvxxxtrt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2frvcushv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2oooqwsrd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2jfbqhwbh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lzeikxve.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2qjfrwuge.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ubemeatw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibtjjbrt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2vmrxcrao.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivlbbcun.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2cpfwksxk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2whzggzen.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2qpspqxmt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2fdvhqpeq.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jnslmhye.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2rdhuitaj.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2otiovqwi.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2tlwjuygu.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ijrxurfl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2louhwjnu.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2glguacyf.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2psdvmsqq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2duffpceb.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2ojeqnrrg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2agshzhdi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2scqdtlig.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2iatupfff.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2pnquznfr.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2fwoohswi.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2cjpofyyn.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2ccawtjol.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2vcfofevt.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2vzutmvym.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vnjjlhbc.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2vxddsowc.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xozgvkki.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tovffgga.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ybsjfzih.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2yrrvieof.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2lxqjnvsa.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jkxttnce.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ycvnjwyt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2ouvwnfcr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2uswngbzo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2diqamhgn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2rzghjzca.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2pgwkdxkr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2ntvbkpnl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ldsvovdk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2bfybghvw.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2yatnwrzu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2hogrcxcc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2tbuqwizz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2qwcnivpq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ictouoog.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2phoqvywr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2vltcptmx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2oiwxijcd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2xaorgqnz.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2inlmlprp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2nglolcwp.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2iulkycgi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2imlcxkov.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2yqufzkal.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2hljnvhoa.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2hbecbzlm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2zkfvdorn.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2nlxtnwdk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2zowytodv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2srbmqqbq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2qoobfkos.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2vbbmlndr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2eajajlyb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2klxnzmdg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2gxtrarov.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2mgkmfaik.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ysbilqqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ieaggyir.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2fxtbndvg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vtflejdj.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2bzanovxq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2fwjhbibg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2kchwglty.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2wqlvozpu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ugvbtiuf.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2beaomymg.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2yiynkbbo.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2vopziblq.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2sswsftmu.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2udmuhivs.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2whrtyxyx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2bzvzfxwa.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2oimfgdjw.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2bceqljjp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2exvepcsi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2mlfizxlz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2qpfrvsiu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2tnzhbyuo.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2hqzuqruz.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2wribaxqt.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2pxbtoprt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2anvhxtqo.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2pspkogjq.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2puevtefv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2pdenokdu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2rrmbxaii.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxczvkft.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2gbccbsoe.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2vstfqjur.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2mjrmlrcl.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2kjenljxg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yogchqmy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2tttqptgd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2bhtfthcv.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2ffwlrqyc.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2icddoolq.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2dnhcjetz.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2tsnvguka.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2dgecgxiz.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2bdfgtvom.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2irnuygxl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2addgahxr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2lpylswye.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2scngzerf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2bpeylqar.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2dlgwwmpp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2favrejgs.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2ydsmvemp.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2masuxlor.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2fdianvcb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2byvpfqlu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2figzrxzo.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2mlqhzsbz.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2zebuqiiq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gowucmrg.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2nmhebgdh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2owpnkzsc.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2cmvzbsfg.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2hcvlurcw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2psvsellq.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2wtbcypxp.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ptwdyemx.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2wowysmww.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2tbroydik.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2hfipmhjn.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2qloadvrt.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2umkxceoj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2euivogng.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2isjxlfdq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2ewisequv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ccippisd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2swgaqpeg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2pehlpdmq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2swmpuozv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2ztwpbftw.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tytysrtq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2ghppxlkp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2qgfbqumj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2bueictxo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pxfddrzh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2wejclqnb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2exyajslv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2etcjvdqr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2xoulcxqo.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2jknacvqh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2xjqxaqxd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2igpnbrwy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2wdlcasmi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2aywhboof.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2vtghokpf.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2pabvchol.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2cgriuire.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2nbsvjlhj.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2kdjzaawr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2yqzpkqfu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2ydeczlfl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2todoqqhc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2eednslww.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2ebamlkyi.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2terxnmma.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2utuwfyvs.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2mswfelop.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2swfshvkd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2ljytnuzt.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zzmmdwau.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2diurrnlm.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2thloyawy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2rwwphdme.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2iibxwatv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2udxpvbqq.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2nbmzhgbk.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2lseprwnn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2pxuunjsl.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2jbkkjwle.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tpfadinu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ocpixddo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2rkxdatyq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2gcjwrhls.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2kqyinszg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2bpqpxjsu.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2ebrgrbrn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2wralpxqq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vxjahuka.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2yvsyydrz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ltuppygd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2fryvtuyc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2fljnwgzb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2krlycclp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2evkjscbr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xrnsquid.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2abbrsqty.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2adcsvvru.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2vqmaljzt.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2wvpqveil.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2hhgybmpt.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2iomewvkk.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2caxvengu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2zbdnxrdc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ojuubskm.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2ktdozdei.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2qinywatg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2tisfldtc.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2fgysadil.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2yisznmks.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2glniwnln.html

);
来源：http://www.52xcode.cn/Article/details/gt2tdctffmg.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2vnnwjtgz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2afngcadj.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2rurnigwt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2qzoongsb.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2jvlzgefh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2fakjwgor.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2riqyzsfx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2irtmqsfw.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2fjxmermx.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xmziiynq.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2kuawuibx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2aydpxtbj.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2kmrtptnu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2bjbvrihw.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2efxozqjp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2mshvzlsz.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2zfgurisj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2divffmbl.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2pyxihvcx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2dgtxmozb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2sbweqdyx.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2bthjxpvz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2sdqvyeuy.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2fcovrvyx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2ynuzeryo.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2zxmajups.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2bawtaamh.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2owhzpqta.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2upbmczze.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tpbazvxs.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2rbpydxlu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2ucrwmwra.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2htstzazx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2qbuagkjg.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2gjozjdta.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2ahonviok.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ddhbicob.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sagjggrl.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2hfyqyfbp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2hfhymmow.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2tjsxgugh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2spinoith.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2gnuqufen.html


<!-- 参考信息 -->