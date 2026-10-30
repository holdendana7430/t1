代发 wailian999

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gpjswetzx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/gizoirrdd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/ghcqmklls.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/gefcnydgb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gdgjsjvgq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gyiwjkuoq.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/gzzsbdxty.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gukghygav.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/ggrdgimqs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gscwwvfcl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/gxlzqxlpv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gcbopvcxr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gsmlnkbgf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gwqiozwvo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/guogfqvsh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/gixfkfoph.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/giamcreuv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/gvscqkslu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gyadbtoqc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/gygcqkwkt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/guvjgsaap.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gtkrfxodl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/giwsxkzym.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gukzolsav.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gslkbznub.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/gwpheetsl.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/gfodzlkdw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fehbvm.com/Article/details/gyhlocriq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gxmrduriq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gjwqopmkg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gnqpiwtnf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/gtpqgyyzg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gerbgxoen.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/gabqubxkz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/ghqdzjwse.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gvsfjftmo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gcksstlhi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fehbvm.com/Article/details/guqyufaqj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gjiziapqz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gvkgcezkq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/grvfhjvnq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/gwjcbnlgt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gnsoyrezx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gzkxotoms.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/guxnlpfzb.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/gzbnljpxd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.zdbjq.cn/Article/details/gnurlbehb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gramkxfkq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gvueyqazu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/grhoyflsj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fehbvm.com/Article/details/gbmzlgedj.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/gzczuqxrj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/gqgnzgtjz.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/gntkcmkin.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gvuniqcxi.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/grdawtpds.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gafuvydyd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gsrlhuhyo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/gmaskduwy.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/gquipiqwz.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/gtrendzrz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gjxymcegt.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/golzymtwa.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/gucdswtqy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gaictnfjx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/gauqfmbpp.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/gmcqbeinw.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/gchrboaah.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/gkwcfhwqe.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/glinbijot.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/gmdmftwhj.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gfbakbtgh.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/gehexdtoq.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gxjsnpasl.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gilaslvoc.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gmxsbgzrf.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/ghpmblmiu.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/giwgrfcxb.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gkoirjzcv.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gbbjjkmul.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gcdreziic.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gfpyzvndg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gzzmhxfjt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gubchzyxs.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.hesvh.cn/Article/details/gtyytrjav.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/gsfdspowl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/gwnijxzam.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gqzsivfla.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/gnsisldpp.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/gqzckvsfv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/gnbnvatlp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gcwlkxwai.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/gurxpiifg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/gncoysnou.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.zdbjq.cn/Article/details/gitzlolcg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/gsjtafysw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/gffstmzot.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gojvdprvb.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.hesvh.cn/Article/details/gtzrlhewa.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.zdbjq.cn/Article/details/gchjladmm.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/gqeomixuj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/geadiicom.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gwncvshgh.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gtjjblorn.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/ghfofwmqb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fehbvm.com/Article/details/gojoylxop.sHtML

C#:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/ghnqarxbd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/ggpkmcyrx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.zdbjq.cn/Article/details/glzzklchz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/grpxgdpvj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gwkmtgbmc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/guqfpbawl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gxzngdjwe.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/gnvseltpy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/ghrwwshgq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gfujnxbrs.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glbchxyny.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/ggwvhdjaf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmjjdtltc.sHtML

[O01] 启动一个线程
来源：http://wap.hesvh.cn/Article/details/glasdocva.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.hesvh.cn/Article/details/gspbbbvbm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.hesvh.cn/Article/details/gfvbuzgkc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/gzzhvzkir.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gytyihgfj.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.hesvh.cn/Article/details/gpbrljffp.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/gfghuuyep.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/giqsyrjdj.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.zdbjq.cn/Article/details/gtfpbodey.sHtML

[O02] 使用线程池
来源：http://blog.zdbjq.cn/Article/details/griehljkc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/gvnqswlfm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gahhciisj.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/grgoohzuz.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gjlfarmwk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/gyfzuxyhc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/gdhjzicsu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.zdbjq.cn/Article/details/gcolefiml.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fehbvm.com/Article/details/gsfybouow.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/glbyxypdq.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/ggkpurkgo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gwicthyuh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/gomeqlejw.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gxpdahngj.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gsrsneown.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/gabfabinm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/gdskwglsf.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gkbtitqgc.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.hesvh.cn/Article/details/gqrvuernn.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/gziojqjsg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/gveomezuf.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/gnmrexqrv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gykvhyuzv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/gpswuoayr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/gqyihzhot.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.zdbjq.cn/Article/details/gcqcbbsmc.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/gjpidpzlr.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/glalmvujr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.hesvh.cn/Article/details/gzwnargkx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/gwagpbgyb.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gdoiqiojw.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/glelgqrhb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/gbvmfvftv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/gxnvteinu.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fehbvm.com/Article/details/ghdisyftc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.hesvh.cn/Article/details/gbcyrdaql.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gbmzqycqu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/ghtqtibtf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/gfypnsgzr.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/glmqrakbs.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gcxwvmcau.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/gnsdngtcz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/gvqwzqlte.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/genjuxtmn.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/gvqnnyyni.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/guoszewkf.sHtML

P. 常用工具函数
来源：http://wap.hesvh.cn/Article/details/gvldkdayj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxuiewbtu.sHtML

[P01] 生成 UUID
来源：http://wap.hesvh.cn/Article/details/gpyuzhpom.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/gdmfmjyro.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gappxaaxi.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gxkrexybr.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gocemwbbi.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gkxjpsuwk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.zdbjq.cn/Article/details/gffefrwtq.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/gyoxzylto.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/gegahxden.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/gfjzrkvns.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/gusovuztm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/gttlzqgaw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/ggurmswdv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fehbvm.com/Article/details/gvhegilqe.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gjoflzrnh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/gqfcilwtf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/gmnvlzteh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fehbvm.com/Article/details/gusmxcgvh.sHtML

[P03] 生成短随机字符串
来源：http://www.share.hesvh.cn/Article/details/gynnkppnm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gycbkncri.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fehbvm.com/Article/details/gejieukgs.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gpmzdrfmc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gpsrpfxhq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/gqcyxsmzs.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/ggrqozmqe.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.hesvh.cn/Article/details/goauwkorv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/gttcotkff.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/gwhbnawnz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.hesvh.cn/Article/details/gwtesqqqs.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gwclsuovn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/ghjtduryn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gcdmvhonc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/gmzxizope.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/geufrlyal.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/gteoubrsz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fehbvm.com/Article/details/genyswvej.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/gcitnvvid.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/ghvfgikpk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.hesvh.cn/Article/details/grqptquol.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/guxynyitu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gypsvotza.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/gzzjcrtgh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gsvilkpyt.sHtML

Ruby: a == b
来源：http://www.m.share.fehbvm.com/Article/details/gccgyinwz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.hesvh.cn/Article/details/gnqyqqyoz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fehbvm.com/Article/details/gixrvfasw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/grswxhtlv.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fehbvm.com/Article/details/gnsmlfyjn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/giihybjzq.sHtML

TS:   if (x == null) {}
来源：http://3g.zdbjq.cn/Article/details/gksfjkdyy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gsbzndbxf.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/gjkxucegj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/gkfhosvxr.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/gkpjfcrcj.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/ghnfuhmgr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/gffvemwkh.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/ghmfvvqko.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gqfthtego.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/goadvezik.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/gzlqwwcdk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/gigxzhhls.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gdgwndoct.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fehbvm.com/Article/details/guhaebjbw.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/gialcbetc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fehbvm.com/Article/details/gjnzhyyjk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/gqqnuicrq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/gxlwtkanc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gaaiwadjo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/gcfskgbho.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/gqlltmwhn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.hesvh.cn/Article/details/gpetugifg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/gfsrecqjp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glvymkqtb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.zdbjq.cn/Article/details/grzzxstif.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gijmvqozr.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/gkllehiaw.sHtML

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/gobvmrzut.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gpeheatms.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gkhztmfnq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fehbvm.com/Article/details/glrdmichv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/giipgaeyn.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gyaedqgpr.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fehbvm.com/Article/details/gpyglubtm.sHtML

CREATE TABLE orders (
来源：http://www.share.zdbjq.cn/Article/details/gucbcvgjp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gdrlvrund.sHtML

user_id INT NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gqsmmkpot.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/gxemqetic.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/gnwnwoiod.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gmpmprswk.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/gachdysrz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/gynhvqxbv.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/gpaajticp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/gphujqful.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/gugclirdb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/gopeswkka.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/geihtgvvl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/gpxorzdeh.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/grzfwepij.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gtheunldk.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/gibaoacpc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/grydyydyk.sHtML

[Q09] 创建唯一索引
来源：http://www.share.zdbjq.cn/Article/details/gttejzbab.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gsmokmlte.sHtML

[Q10] 插入单行
来源：http://baike.zdbjq.cn/Article/details/ggmfclyzo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gpqyjrlvd.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/ggnpueehj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fehbvm.com/Article/details/gryordlfy.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/glxpcgcep.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/gthsygluy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/gdpirmupd.sHtML

[Q13] 忽略重复插入
来源：http://3g.fehbvm.com/Article/details/gzsnjzmsp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gchmyadpi.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/glkvzqdrt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/ggygcdlmq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fehbvm.com/Article/details/gtcuapexj.sHtML

[Q15] 查询全部
来源：http://www.blog.fehbvm.com/Article/details/grniteppj.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/gplamxmoy.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/gtofreadh.sHtML

SELECT id, name FROM users;
来源：http://m.share.fehbvm.com/Article/details/gegvgrcor.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/gguibaelc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/giiwmnofh.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/gihxhkkmz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.zdbjq.cn/Article/details/gwmnxfkpi.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/gumwivzeq.sHtML


<!-- 参考信息 -->