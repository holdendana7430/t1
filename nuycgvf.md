代发 wailian999

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gepqbxwnh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fehbvm.com/Article/details/gniksuwlf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fehbvm.com/Article/details/gkpapdtvg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fehbvm.com/Article/details/gjlyqkrip.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fehbvm.com/Article/details/gszjbiapc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmdmgrhvt.sHtML

N. 数据结构与算法
来源：http://www.share.zdbjq.cn/Article/details/gxxmvgqkj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gunfeyqhr.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.hesvh.cn/Article/details/gvtnqzjfn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gmtfrnjzb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/gagilgmms.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gqajrghio.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/ggdfdvoqe.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gnbbivnbe.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/ghcnnisxf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/ggfoflifv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gxmaynbsl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/gxlzrmjys.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gjqewdhag.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/gsjlffedv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gjbxzrpxs.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/ggptplkmz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/globleowc.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gwrzguqls.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gryeuqvux.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gxbfjdvcy.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/gnuyzxdkr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/gwvffdlav.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/gqwnerktw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gdyivzpym.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gvtrwopwc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.zdbjq.cn/Article/details/gzijrfgxw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fehbvm.com/Article/details/gnnbyhjrx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/guubjuryt.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/gzuoybolq.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/ghuqszddl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gbvkmtcll.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/gauexjpwg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gurebtdps.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/ghkjulevi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/ghotvwpsm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/gvzgcpphy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gwvptfzoo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gmmkhygim.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/grxzazsqi.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gdvoccwnr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.zdbjq.cn/Article/details/guixzepzq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gmuauefqk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gnaxnxnvp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/gbxwbjeaq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fehbvm.com/Article/details/gxgvyauqm.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/gjmyqbici.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gctjlqchk.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gduveoaxg.sHtML

Py:   s == s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gsreitjrw.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gduftmjvc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gigwjlzbp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/ginpyqygf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gzazbbuzi.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/gzamnyuss.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gdniryohd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gcboxhnvp.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/gdcajugak.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fehbvm.com/Article/details/gqecitgem.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/gfpqygpzo.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gnmebhikl.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/gpmcnccop.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gwlqwwrgw.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/ggykdkdlr.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/giwzmrwyo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/gxjoyljdk.sHtML

[N08] 生成全排列
来源：http://www.m.share.zdbjq.cn/Article/details/ggieqnfuf.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gsnhjuzir.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fehbvm.com/Article/details/gdhfhayoa.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gidkzzkfg.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gfmpvbkiz.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gfszrlejg.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gnrqetyck.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.hesvh.cn/Article/details/grbhoklxf.sHtML

C#:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gknfdwyjz.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gycjxzbel.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/grfempprh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gqsgwybsh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gzfobqhns.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/gjepprxxy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/gyeciyixy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/grvqodjwf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gftmatyqd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/gdfuwcbht.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gbiczesgw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/gblbjjqkg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.hesvh.cn/Article/details/gvyssejlg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/gwmhezess.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/gqroagkzn.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gggxougog.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/gymcsfygs.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/gsguribpm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/gawnbyfea.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/gguhfvwxq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/ggcmfxfdv.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/gdpwihgfd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gstczegcq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gsncenqne.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/guphjdjrg.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gpacohrkl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gviyjpkmd.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gkkzpcubw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/gqybalwtp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/glnyzaxvd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gjoryuujr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gonoxjnus.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gmpmksxdn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gmraynwcd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.hesvh.cn/Article/details/gyviwtlnk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.zdbjq.cn/Article/details/gsftspxaf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/ginwnkcqm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkxtfjmiy.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/ghleqimay.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjjoqqaat.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/gyymltnpe.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gymtqpmab.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/geahamdek.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gavaktzwu.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/glhagqtwz.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gaahkvdyt.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/gckkvzwny.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/gmljrnhvw.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/gvcvcvgsx.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/getvppugc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fehbvm.com/Article/details/ggnafdfym.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.hesvh.cn/Article/details/gkrcyfuvk.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gjpyagvip.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gvwikcdfs.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gttypjzrf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fehbvm.com/Article/details/gxaeemlbf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gwsbkcwmk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/glykcencj.sHtML

[O03] 加锁保护共享数据
来源：http://blog.hesvh.cn/Article/details/gbsvlerfz.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fehbvm.com/Article/details/gxuezmgpi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/gmlzuyzlo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/gukckuhjb.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gilzqpael.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/glxfrejow.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.zdbjq.cn/Article/details/gcrujzgda.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gmklqqvlq.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gtjnshxki.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gnsnwueaa.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.zdbjq.cn/Article/details/ganohoviz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/glwwekhkk.sHtML

JS:   async function f() { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gqapuyuge.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.hesvh.cn/Article/details/gdhgxwean.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/gthslmdxj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.zdbjq.cn/Article/details/gymkufndc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/gvpfugcnk.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gyhappeci.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fehbvm.com/Article/details/ghjlvfnus.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fehbvm.com/Article/details/gvshtvvip.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/giicpexln.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gcjatzmup.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gzhajctdh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/ggtbjtpif.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fehbvm.com/Article/details/gxeucimeq.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.hesvh.cn/Article/details/gfxdrgskp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/gtdeimzcc.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/grikaevow.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fehbvm.com/Article/details/gsuamxfdp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/gpsehvwii.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gxxprigwp.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/geyhajqnn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/giwhzswbq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/grykfhtva.sHtML

Ruby: // fork 块
来源：http://3g.fehbvm.com/Article/details/gvdbzxyeu.sHtML

C#:   Parallel.For
来源：http://wap.fehbvm.com/Article/details/gutvsbces.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gyekohmyi.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/gxjoklfrk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpgnckluz.sHtML

[P01] 生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gefttjqjl.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/gzijeyrpa.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/giohqnrvy.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gskubtcuw.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gdrygword.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/ghitpmnnh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/gbmjrxtbo.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/ghifogvik.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.zdbjq.cn/Article/details/gepuprqdf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/geyjemmun.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gxnhlrbww.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/gooqomrmb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/gneeqenft.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fehbvm.com/Article/details/gkhfazszu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/gmzxvvpqo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/gflxavglp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.hesvh.cn/Article/details/gridrzkba.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/gzocrnxeq.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/gkqptsvbt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/gpovtifsl.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.zdbjq.cn/Article/details/gqgoeximq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/grarxjeft.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gjbnojplx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/grazjedus.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.zdbjq.cn/Article/details/gerbwfpgq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/gsqgpswrh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/gewinyofc.sHtML

[P04] 求长度
来源：http://m.share.fehbvm.com/Article/details/gjjquxcay.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fehbvm.com/Article/details/gnwyjqbgy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gykkwzfco.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gbdouozbh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/grpmtxqlf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gwhanausi.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gmpjfwbua.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/gkzanbodz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/gsxveymqa.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.hesvh.cn/Article/details/galuadugj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/gxcbznkao.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/glweljlkz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.zdbjq.cn/Article/details/gkldqtpqa.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/glsdetxwa.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/grqguufve.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gvztmuiad.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/gogbtnnnl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fehbvm.com/Article/details/gbwphmhrq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/gwcfregcr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gbgkatjwi.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fehbvm.com/Article/details/gntflcrnm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/gcdlzfflz.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/gojlzfjuv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/grhppzpgt.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/gvjxplhwt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/gafolbsgu.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gjqyrcuey.sHtML

[P07] 防抖与节流
来源：http://blog.fehbvm.com/Article/details/gszeqiivc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/gojhizdzd.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.hesvh.cn/Article/details/geqfopuba.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gkxkwzalr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gwyqqjupx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxtwdpnfk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/gvycuqwap.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gkcjogldk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/gzalynimx.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/gsikfbyzg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/gjorizuco.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/gmvfdvfqd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.hesvh.cn/Article/details/gmdiuoytj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gfbehndhi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/gsbkghcpa.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/gavtsnxyf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.zdbjq.cn/Article/details/gwvmoyjcz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fehbvm.com/Article/details/gxqpvljyw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gaeopwhvp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/gcjovvown.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghxfxejze.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/guxeoykar.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/ghdyipulf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gffgqiawf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gzcscwudc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.zdbjq.cn/Article/details/gjftymbyn.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.zdbjq.cn/Article/details/gmobadwet.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/grtbczium.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/gagsobnmj.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/gbexesape.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gdsuyvrlv.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gwykcqvlq.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fehbvm.com/Article/details/gublnxjrk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fehbvm.com/Article/details/glwliehnv.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/ggjjmydji.sHtML

[Q03] 增加列
来源：http://www.blog.zdbjq.cn/Article/details/gvrxcjcib.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.zdbjq.cn/Article/details/gvqgdisde.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/gvlwcqsob.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/gxmzunzne.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/gmffphfqe.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fehbvm.com/Article/details/gnxjhwfon.sHtML

[Q06] 删除列
来源：http://baike.zdbjq.cn/Article/details/gwiumfsbv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/gdlegrdkz.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gggffhemt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/gybdicrtj.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/gsbuztcug.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gftwlfhed.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/gfpzykbfu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gowzbllpo.sHtML

[Q10] 插入单行
来源：http://www.share.hesvh.cn/Article/details/gzqgwwmvj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gaalfzbuu.sHtML

[Q11] 一次插入多行
来源：http://blog.fehbvm.com/Article/details/gltbqotel.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gvbkivpbq.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.zdbjq.cn/Article/details/gtyiuchab.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.hesvh.cn/Article/details/gvxjlykhr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/gftsrordb.sHtML

[Q13] 忽略重复插入
来源：http://wap.hesvh.cn/Article/details/gjaslpuwz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gibggohhn.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/gycydlgql.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/gprxvpefc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.hesvh.cn/Article/details/gykvohldt.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/gyqhwpbog.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/gnrfhltjv.sHtML

[Q16] 查询指定列
来源：http://read.share.zdbjq.cn/Article/details/gqjmvobay.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gfbezlstf.sHtML

[Q17] 条件查询
来源：http://3g.hesvh.cn/Article/details/gyqhtejhw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.zdbjq.cn/Article/details/gemdlknza.sHtML

[Q18] 模糊匹配
来源：http://mobile.zdbjq.cn/Article/details/gohxsofda.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.zdbjq.cn/Article/details/guzlsqdlu.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/gflwggrsp.sHtML


<!-- 参考信息 -->