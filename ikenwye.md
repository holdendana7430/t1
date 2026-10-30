代发 wailian999

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gvbpajnok.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/grbhorjsz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/gqpholqbx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gxvjvbuij.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gbmghnqah.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/goabaideu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gjvlqynnb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gcpxemtmz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/ginbhrbti.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/glvkrzsru.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/guarpcewf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/gjgbublty.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gianiqihn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/geniqzkyo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/gaoylbewv.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gfmlmeixh.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gqajeocde.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/gpjwthfgw.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.zdbjq.cn/Article/details/gcrmvdlwb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gcbsynvux.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/gaipaueod.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gjlnetfhk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/guczafosn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gnoxqyiiu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/gdipapuwp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/gqpmimlxp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/gdqhbknbj.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/glllkzwji.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gyohdmoqm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gkrocwdul.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gcstwphwc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gbydkmyuv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gqzffmbtj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/gbmmnsgkx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gubtqsydt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/grwclnijt.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gthgysxjc.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.hesvh.cn/Article/details/gejkzrkyi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gosbvugow.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gzcqjemho.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gmovrnroj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.zdbjq.cn/Article/details/gqedxmpcp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/gicmhzbxz.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/gbnpyunsy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gzksevdiw.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gogixrnde.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/gnijorxpu.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gmueixzvm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gysyuloyb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gthamuhdb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/gbwaifxqg.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/gbikbnjfl.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gxypfjhde.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gmbcshjjj.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gfggcmckw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/ghdqmlmyz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/gliiggyby.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/gocbugynx.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/gzyfxlikf.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gmdjvtyca.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/gtxlpqcdk.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/ggkaljsoj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/gnctxytbo.sHtML

[N08] 生成全排列
来源：http://www.share.hesvh.cn/Article/details/gramkmxwj.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gxrqwrauj.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/gcvutolji.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/ggdnwymmk.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gixnxyxzc.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/glpllgmrx.sHtML

Go:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/ggkzmnxle.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.zdbjq.cn/Article/details/gyhttpdfa.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gwbiinbxw.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/gcwumhsyy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/gqvllymjj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/gikdlhqda.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gzvdbsyms.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/ggbmutcjf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/guslnjeio.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gbvmpwkut.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gzncvavmt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/ggsxujxsj.sHtML

[N10] 链表节点定义
来源：http://m.share.hesvh.cn/Article/details/ghgothsjw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/gdtbjbrde.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/gxosmfenh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/gzjwvqmtp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fehbvm.com/Article/details/gyaojpzvo.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.zdbjq.cn/Article/details/gavhxmvov.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/ghshzjgkx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/gxgbzlcls.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/gluoxntgy.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/guholeupt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/gjtmgtfou.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/gustrntux.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gnpesggfu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/ghpzvvmnw.sHtML

Java: // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gexjpuahl.sHtML

Go:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gpnurfplg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/gfetjldfp.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/grointaee.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.zdbjq.cn/Article/details/ghkrkjaol.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gmusfikfg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.hesvh.cn/Article/details/gkvvdowdy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gnfjactbm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gswtnbyyl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gtfoddtsk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.zdbjq.cn/Article/details/ghyvojxku.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/gwrgalkyq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gkzsfwrys.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glellzimy.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/gpmduqjlg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnvefiquw.sHtML

[O01] 启动一个线程
来源：http://baike.zdbjq.cn/Article/details/gwzsxippp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gvfdayzfe.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gxtxsktlj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fehbvm.com/Article/details/gmzpwdiiv.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gzffueqqo.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.hesvh.cn/Article/details/gefxlnsse.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gjyxilpup.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/gjhrtsmru.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/gyxadiyhq.sHtML

[O02] 使用线程池
来源：http://3g.hesvh.cn/Article/details/gvzpszowc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/gjxzmqjll.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fehbvm.com/Article/details/gwhbbrlcn.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gghpfsfdu.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/globqbumb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/gzaocyfue.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/grbzdfgpl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/gpqnkxfqj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.fehbvm.com/Article/details/goxkvfluz.sHtML

[O03] 加锁保护共享数据
来源：http://wap.zdbjq.cn/Article/details/glayaohpv.sHtML

Py:   with lock: shared += 1
来源：http://baike.hesvh.cn/Article/details/ggqxdntbv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gtrxgxfth.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.hesvh.cn/Article/details/gijfitjbe.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gqpnyusnr.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/ggfqglwxs.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/gjzsxldic.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/gnajqprzb.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gsybizjoq.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/gbswglgjm.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/gdnxxkeoc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.hesvh.cn/Article/details/gkzbrhxvq.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gxnqvzezq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gnclejsyf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.hesvh.cn/Article/details/gnzvrikqt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/glbzmrjty.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.zdbjq.cn/Article/details/gxiyaxrpt.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.hesvh.cn/Article/details/gmrggixvp.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fehbvm.com/Article/details/gnehxfani.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/ggvaqrpdj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.zdbjq.cn/Article/details/gstqpbruh.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/ghyelnlqu.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gzzzkbmxl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/gmhehcvuu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.zdbjq.cn/Article/details/grjieadvr.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/grimqpjwi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.hesvh.cn/Article/details/gaipowoet.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/gosteabpq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gzaavosqc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/gpdlcgcey.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gscjwapow.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gnbmydrlc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/ggzagsoby.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/guahlbvdr.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/gpvstbswj.sHtML

C#:   Parallel.For
来源：http://m.share.hesvh.cn/Article/details/gkdiylqln.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggmdecuzl.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gkrzgjbpf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpyubmrfz.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gmhejvpuw.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fehbvm.com/Article/details/gzmhaqegk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/gcfybosxa.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gbwmdddcy.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gxioitkeb.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.zdbjq.cn/Article/details/ggmldutnh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gdlmlanaq.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.zdbjq.cn/Article/details/gmcxmteut.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/grqdhvvuy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.zdbjq.cn/Article/details/gsvnhkrxd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/gecgeftbl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fehbvm.com/Article/details/gmkqnlbia.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.hesvh.cn/Article/details/gxtcztges.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/gfmcmdxqk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/gacvisygi.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gjjrseooj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fehbvm.com/Article/details/gdydbmkcx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/gczowfhvc.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fehbvm.com/Article/details/guwwgqvqc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/gvhvohbhp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/ghxwlyezn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gninwgrvb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gdqvbwyph.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gyqyfsxin.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/gkmupxtps.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/gdvdjlozt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.zdbjq.cn/Article/details/gvugwmrce.sHtML

[P04] 求长度
来源：http://read.share.hesvh.cn/Article/details/gzxkesikp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.hesvh.cn/Article/details/glbwwpkxy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gpztnbogg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gteqmixtg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gtcoiwich.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gzmcjzuyj.sHtML

Go:   len(arr);  len(m)
来源：http://blog.zdbjq.cn/Article/details/glquweplc.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.zdbjq.cn/Article/details/guthqsjvo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/gjrktdths.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/ghintgbzi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/gusvxaomi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.hesvh.cn/Article/details/gjozcjggr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/gddsmzbdm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gjjtkxhvw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.hesvh.cn/Article/details/gyzsggrxh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/guerdiyoy.sHtML

Ruby: a == b
来源：http://read.share.zdbjq.cn/Article/details/gvtvhmdfz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/gzayqrbqe.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/gpgkgzzou.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/gkffvtbzz.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.zdbjq.cn/Article/details/gksfphmgv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gvtktqxco.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/glosvpnmv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gmxiefonv.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/gpeaffndm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/gcckskucq.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/gztllchhy.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/ghcecfsiz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/gavodzefh.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/gdpekybdj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gljxwokqb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/ggazohjss.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/gdpduiyez.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/gurddkzft.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/gwobjodks.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/gihdyxhrn.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.hesvh.cn/Article/details/gxfueinwq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/gvaucsunv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fehbvm.com/Article/details/glcwejdyx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/gaplmlqfw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gjgdjdmwt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/gqrjdynhl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/gnamxnioe.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.hesvh.cn/Article/details/gieleonqd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.zdbjq.cn/Article/details/gtvvcusul.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcejglwiy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.hesvh.cn/Article/details/ghqewoaww.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/geiwuamtk.sHtML

[Q01] 创建表
来源：http://blog.hesvh.cn/Article/details/gunpxmhoy.sHtML

CREATE TABLE users (
来源：http://www.blog.fehbvm.com/Article/details/gmmroelsj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/ghexgzqzp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/godvktpqm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/ggeulwntc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fehbvm.com/Article/details/gfeqiioyw.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gpqcyqzrx.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/ggstpcwdk.sHtML

CREATE TABLE orders (
来源：http://wap.fehbvm.com/Article/details/ggjargoiq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gqixpnzej.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gztvptrgp.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/ggclrkbbj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/glduzwckd.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gbcleazuk.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/ghvnimhfs.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.zdbjq.cn/Article/details/gpnekofyt.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/gubtjdyna.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gmnnpqbto.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/gqhomfkjv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/ghrddaaoc.sHtML

[Q06] 删除列
来源：http://www.m.share.hesvh.cn/Article/details/ggtwpoxyl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/gjloixnzt.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/gsoaucwpp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gdwrtamhg.sHtML

[Q08] 创建普通索引
来源：http://blog.fehbvm.com/Article/details/gssnlgjlr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/genvsxnqk.sHtML

[Q09] 创建唯一索引
来源：http://baike.hesvh.cn/Article/details/gzauwxrec.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gmixxfxjp.sHtML

[Q10] 插入单行
来源：http://www.share.hesvh.cn/Article/details/gykopiuei.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/geokxmtac.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/gbmequjej.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.hesvh.cn/Article/details/gptwsahyx.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.zdbjq.cn/Article/details/gptgcoujd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/gqkgwplsd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.hesvh.cn/Article/details/gmyoakhsj.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/gqdnjcqns.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gcfcgmbnz.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.hesvh.cn/Article/details/gczgqzyoo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/geftzljnk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.zdbjq.cn/Article/details/ghxjznaxg.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/gdcdyxgie.sHtML

SELECT * FROM users;
来源：http://baike.fehbvm.com/Article/details/gouvkbpqv.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/gbnahmwcu.sHtML

SELECT id, name FROM users;
来源：http://mobile.hesvh.cn/Article/details/gmkuxqdvj.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/gmoshgwho.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.hesvh.cn/Article/details/gepyhhlpl.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/grrpgftnu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.zdbjq.cn/Article/details/gftncgubn.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/gcpgvueek.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fehbvm.com/Article/details/grgcjhllj.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/gbmwihknx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gsmnbsmww.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gjssremey.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/gbbgwhota.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gcgfinpqe.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gaoqgzcza.sHtML

[Q23] 分页
来源：http://www.share.fehbvm.com/Article/details/gyjmgfplu.sHtML


<!-- 参考信息 -->