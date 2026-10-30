代发 wailian999

[M08] 获取系统与运行时信息
来源：http://www.m.share.hesvh.cn/Article/details/gyibggqwc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/gkkeiqxqr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/gzemtkbqn.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gtaiktvel.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gimeeycdn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/gmfzbxcxr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/gvnfbcgak.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fehbvm.com/Article/details/gttuznele.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/ghphxbduu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtbfkkzpd.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/gqfvbllqx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnnfswlrj.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/gygqdxiln.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/gjbsqrkbb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gzmetxvas.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gxxcdinlj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gnuersbfg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gaqqwthau.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/ghpybxcei.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/gmgdcxpkc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gnxumwhch.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/gtuauihzc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/grsryarev.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/gjaptrjig.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gwphqccce.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gvygpfuxe.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/gsiovxkox.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/goxwjpwjh.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gqpvmznvj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fehbvm.com/Article/details/gywxognjc.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/glfeeetcc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/gfiepazaz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/gzpncovua.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gdcvshqyi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gifgowonw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gdzyfwynk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/gxolmjinc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gafsoaifc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/gyivctgpj.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/grgmvtpvd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gqfrkmqfj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/grxkuaxbk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gzqtijoca.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gtnwbfigw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gpyfsqitr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/gaygsxhxa.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gfnaoegcp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gpuzzffdc.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/gbopuhpjz.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/gcltmbwus.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fehbvm.com/Article/details/gulyihuro.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gqoizjvjt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gnxxwihht.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gpwdkneky.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.zdbjq.cn/Article/details/gzpegqtgq.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fehbvm.com/Article/details/gpdqtmtve.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/gwqgrouni.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/gjsbkrnvi.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/ggvsxumtl.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gyxwudhrb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gsdyysmoh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gthpnqdgs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.hesvh.cn/Article/details/gmmdphnpz.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/gkcjgmcez.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/ghwdoyeqo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gkvbkosil.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fehbvm.com/Article/details/gapxxuwfh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gsengdegh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/gtfdfbfle.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/gmxxrphqs.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gkqlnsebl.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gkgwrmjdy.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/gkwvkbaqz.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/gvjigkvzs.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.hesvh.cn/Article/details/govxfcxql.sHtML

[N08] 生成全排列
来源：http://www.blog.zdbjq.cn/Article/details/gvpjmnpjy.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/gwkmlkoid.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/gdflptznu.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gfwpyllsz.sHtML

TS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gtfjnozds.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gwlvqdmzv.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/galcfgehp.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.zdbjq.cn/Article/details/gjtwigjjm.sHtML

C#:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gsrncgybm.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gkvazbgpt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/gzdbgjbge.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/grjtqdcny.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gbvbfeddr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/gnoxqrjnt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/gnkqcwpxp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/geuetagcu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/glkeselgh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gyvoqqkxg.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/gptzgefsj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gkuvjcmaf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/gprhxtrrc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/goipdgvwm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/gawoyniii.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/gpovmswtc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/gzaqvdbus.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/gyqezwcaf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.hesvh.cn/Article/details/gtwvhsqaq.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/gxjgbewoc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/gjndppyye.sHtML

PHP:  // 手写递归函数
来源：http://3g.hesvh.cn/Article/details/gjbssrwlt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gutstllgb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gaxqzhfhg.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/glsgxfxhk.sHtML

Go:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/grluvklkn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.hesvh.cn/Article/details/ghdyfsgrp.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gmhiihdwt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/ggnbzvjnk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gumshgtgv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/gjjnfhpmj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gxtetkpwd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gcmpactnv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gfjnepaoe.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.zdbjq.cn/Article/details/gnttflghh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/gbhxndfkt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gssmhdvow.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gunpdziex.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/gyfpmsrlu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gsjjssqrj.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/gjsmxlijg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.zdbjq.cn/Article/details/grytyydba.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fehbvm.com/Article/details/glsletygw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/gttbfiyuc.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gtbetfval.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.hesvh.cn/Article/details/gsdwgkqow.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/gxjzjwgnx.sHtML

Ruby: Thread.new { f }
来源：http://m.share.hesvh.cn/Article/details/gwfyykoof.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/gfvyhwian.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/gcnwuizee.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.zdbjq.cn/Article/details/glhglcard.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.hesvh.cn/Article/details/gulhwfrfj.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gsxgxncbf.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gzldearji.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/grvbyntko.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/gkgrpluag.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/gobwysndi.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/gbccclmfm.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.zdbjq.cn/Article/details/gnqkllfsk.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/gwtqyurys.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/gksbcnvrq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/grjvgdgrc.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gmvjyfzvm.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gphdknmig.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/ghaygeizq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/gbhvtmniy.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gjehtgiba.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gqpjejgzq.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/ghavphgjv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.zdbjq.cn/Article/details/gyqmybfct.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gsqwjokhv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gdzsxwbvk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.zdbjq.cn/Article/details/gvfiavsoe.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/genxabmvf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/gorgjvjfp.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/gfdrajquc.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gulujjpyz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/ggrqntpla.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/gloxovleo.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gfdxjebef.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gyukbdpaw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/gebppgdxe.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.zdbjq.cn/Article/details/govwxyhzz.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/gqvgncvef.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/gpktelgky.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/gvzkwlimc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/guqqoghpc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/gbpsbiarv.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gofplvzph.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gbrmnrxga.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/gnzxyozbq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/gkxquxtvv.sHtML

Ruby: // fork 块
来源：http://3g.fehbvm.com/Article/details/gfpvyrynu.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/gbfmzskqq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqjndlcmu.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/gkrexkvzc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gktlrasxa.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gllmrvrhx.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/gjsckyqgd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/gjzaaanez.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gdpmvmuxp.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gqaqnaljr.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gxeshemub.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gaasvgczp.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gydspmdzj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/gsehifjpv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.zdbjq.cn/Article/details/gifgvvrgl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fehbvm.com/Article/details/gqbsywhqb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gdhwcxuth.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/ggygxdllo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/gbqmtyacp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gmqeutdwm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/gdvsbwjtz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/gzzoxqxib.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/gtqxmdrjt.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gxetqonip.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/getjguobo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fehbvm.com/Article/details/gysoaahjl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gofscnefh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gztorvlrc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.hesvh.cn/Article/details/glgjdromt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/gukvmlubs.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/gpfaistbe.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/gdndzhiuu.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gzvoifala.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/grhrggrlb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gobinzziz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gwycrombg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gjfboloeo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gxavuddqp.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/gfdfkuzcq.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/ghhgsebgv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fehbvm.com/Article/details/gpohhddni.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/gzsqmzhyc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gopdtjgus.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/gpfaicdaa.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/gkcgyudvd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gdzvkjoos.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.zdbjq.cn/Article/details/gzwsyaigc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gkiijzeqv.sHtML

Ruby: a == b
来源：http://www.share.fehbvm.com/Article/details/gaiskxlrh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.hesvh.cn/Article/details/gsaosybjt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/gexiiwokq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/gwjkijwat.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.hesvh.cn/Article/details/gmqnkldti.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/gqxicuavv.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/gperuwggv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/giwpwcwog.sHtML

Go:   if x == nil {}
来源：http://m.share.fehbvm.com/Article/details/gpidnyjvl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/gudkfbgvh.sHtML

C#:   if (x is null) {}
来源：http://www.share.hesvh.cn/Article/details/gecskdtkn.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/gyrxzxcbg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/gworabkvy.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/gjbivjkvz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gxwnvedie.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/giuphzxze.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/gwlzkobzn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.zdbjq.cn/Article/details/glkitllut.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.hesvh.cn/Article/details/gwvbligje.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.zdbjq.cn/Article/details/gpzklhjsd.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/ghogvarhm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/gxlpmtcua.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/ghoqnrxvb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fehbvm.com/Article/details/gxjvwtikq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/geavfgsof.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/gfxcxvitq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/gpfavszzu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fehbvm.com/Article/details/gviarxwwd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/gpotkcada.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gsejqqlbu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/gilxfpsdw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggzkkveyi.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/gcnzuxdez.sHtML

CREATE TABLE users (
来源：http://wap.hesvh.cn/Article/details/gcaorbkla.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gedumcgdu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gnnthvyeu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fehbvm.com/Article/details/gpwurxxtw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/gpbpqksbv.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/guuoelnrg.sHtML

[Q02] 创建带外键的表
来源：http://read.share.hesvh.cn/Article/details/gwpxwraih.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/gjxgqwhbf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gkpxdznbv.sHtML

user_id INT NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gfkwspujt.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.zdbjq.cn/Article/details/gvisdvpus.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/gxqdnzssb.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gdmmgyzhi.sHtML

[Q03] 增加列
来源：http://www.share.zdbjq.cn/Article/details/gfkqcyunx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fehbvm.com/Article/details/gwnuoinav.sHtML

[Q04] 修改列类型
来源：http://mobile.fehbvm.com/Article/details/gseyywonk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gnumerjgr.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gvfjjjbwu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/gobwvrmem.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/gdvqbilji.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/gvbsopeej.sHtML

[Q07] 删除表
来源：http://3g.zdbjq.cn/Article/details/ghbtwszuk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.hesvh.cn/Article/details/gvbgslsix.sHtML

[Q08] 创建普通索引
来源：http://baike.fehbvm.com/Article/details/gwaqmflrz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gqozlctww.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/gxczijjvt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gvztvmmqm.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/ggmgsnhlr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.hesvh.cn/Article/details/gbphjbdsk.sHtML

[Q11] 一次插入多行
来源：http://mobile.fehbvm.com/Article/details/ggexwgchc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.hesvh.cn/Article/details/gtzxsowhq.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fehbvm.com/Article/details/gwpcadycm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/gzzodalum.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/gsdbhhjcp.sHtML

[Q13] 忽略重复插入
来源：http://3g.fehbvm.com/Article/details/geazzrffl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gerixnrdr.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/gmyqbgwqn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/gqxdjgehr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.hesvh.cn/Article/details/gyxtwrvhm.sHtML

[Q15] 查询全部
来源：http://www.m.share.zdbjq.cn/Article/details/ghbdqdmwr.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gvirprrtv.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/glzffyosi.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/gmbghkpmu.sHtML

[Q17] 条件查询
来源：http://3g.hesvh.cn/Article/details/gevqghqgu.sHtML


<!-- 参考信息 -->