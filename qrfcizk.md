代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/gxblerbki.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmdvqmjmq.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/gvuockfuw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmkkffjwo.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/gemyhcmyh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/gfawdonwc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fehbvm.com/Article/details/gfxszkpac.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gyszlqjbo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gzodbkmto.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gopdflmef.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gukthsfhd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gcbapmszf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gnwmynloo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/gmhjtlyfg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gzsdxhvgc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/gaqtcyjlf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gzyoaevmz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gfkwlshyr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/gpwssczqr.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gqzfzbnbj.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/ghoxwlple.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/gqzslsvcd.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gcmzkhgnh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/giwgdzsui.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/gagqifsqm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/ggyariinf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gcjahzixf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.zdbjq.cn/Article/details/gsjnyrgur.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/gehrxpxlq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/gxxhfensm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/ggmgzwftc.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gwoqyyxhi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/grkcccybt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/glzzztrdz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gzthiqsuk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gycemnjic.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.hesvh.cn/Article/details/glmbnfkub.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/gzrxwpzdp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gicbxbnsm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/grcvrfmfc.sHtML

[N05] 最大公约数
来源：http://www.blog.fehbvm.com/Article/details/gygbqxpir.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/grnaecazg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/ghnjtdzvg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/goxhpsggp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gmjvfgjol.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/gshhohrat.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.hesvh.cn/Article/details/gxeykhcdt.sHtML

Ruby: a.gcd(b)
来源：http://www.share.zdbjq.cn/Article/details/gequrxawa.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/geknzznhl.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/ghleyyjam.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gbasglany.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/gpomepoci.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gtljijral.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gvxkniwuz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/gqqcasiml.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/gsunmznso.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/gruolhzes.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/ggxpplijj.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.zdbjq.cn/Article/details/gkzvpwehy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/gkssrqyfj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/ggpvcshpy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/grqqiuqcx.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/giwhanota.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/geqvmtgpc.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/gnvvtfjsu.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gnioovdnl.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/gxgjrgfcf.sHtML

[N08] 生成全排列
来源：http://read.share.fehbvm.com/Article/details/gsiccayde.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gbvjwowiv.sHtML

PHP:  // 手写递归交换
来源：http://3g.fehbvm.com/Article/details/gadalnfxa.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/geudgguow.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gwebluzor.sHtML

Java: // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gfcbfcpgf.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gunyxckyr.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/gwzjaxfkv.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gvzwkdiuu.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/grfblilws.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gumfxluzr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gtxtfeaol.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gvjrgmynm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fehbvm.com/Article/details/ggdasmwmt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/ghbrttvai.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fehbvm.com/Article/details/gtrfhigdj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gaxkwafrl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/geipcfrvy.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gpymqgnvp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gyeounpbf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/geqepdwjf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gkubfudyo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gdobfnqla.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/gfhrrnqev.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gmysatltm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gsdholoen.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/gtcexlmvx.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fehbvm.com/Article/details/gepzhgzdi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/gxbcvupod.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/gvsskqhlq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gnjilyfvr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gukwqassa.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/ghyzfsyfw.sHtML

Go:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gkxkfghsi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fehbvm.com/Article/details/gwnmhgtgc.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/ghzbkzotf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gnlejuqzp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fehbvm.com/Article/details/gbuoygyra.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gsjulhmza.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gxnzwzcrq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/ghcrucmmv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gufxdjqhn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gdonucdif.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/gqfheuryc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gqgzatpyl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grgywxtbl.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/giupwpxgh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqekkmlzd.sHtML

[O01] 启动一个线程
来源：http://mobile.zdbjq.cn/Article/details/gmwwknpsm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/gujqyayeu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/goxuyovqh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/gueucosay.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gsknjmpkx.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gnnwrjprq.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gvsvqdfyx.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gjurojlak.sHtML

C#:   Task.Run(() => F());
来源：http://3g.hesvh.cn/Article/details/gargkdicz.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/gwzrobgzz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/gyjhqbtie.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.zdbjq.cn/Article/details/gsqorcmxb.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gxpgbzcma.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gpqdpadkp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/gqkjetogl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/gxakdjijh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/glycpuqsj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/ggfoshqxu.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gcdgjfofm.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/gzsildygh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fehbvm.com/Article/details/gdqvokajz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/gxujksrnl.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gowjfqlat.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gvjfidrft.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fehbvm.com/Article/details/gzvhexkib.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/guiajrxbf.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gvynpnxkg.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/grgmtasuu.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/goteyylsj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gagkgedoa.sHtML

JS:   async function f() { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gkuyiesct.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwazxdofb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.zdbjq.cn/Article/details/gtvonpsgt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fehbvm.com/Article/details/gflcgzfrh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/gnutjkwyw.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/golwqrkjy.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/gdaradorw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gsgvpswty.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fehbvm.com/Article/details/gynyyshoa.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gjqsaffch.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/ghqwwgups.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/gdttkxzxa.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gcpbjeymi.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/gjpwtxavb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.zdbjq.cn/Article/details/gqljsgxdn.sHtML

[O06] 使用进程池
来源：http://3g.zdbjq.cn/Article/details/gkgsszhpy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/goxvqngwq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fehbvm.com/Article/details/giwuehofn.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gbwacjcbs.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gklmmkcis.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/glxazuevw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/gyunueeol.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/gyhbikcdt.sHtML

C#:   Parallel.For
来源：http://www.m.share.hesvh.cn/Article/details/gxdghxpdv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbtghgrsf.sHtML

P. 常用工具函数
来源：http://www.share.hesvh.cn/Article/details/gmfvcjmjm.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/geljrexfe.sHtML

[P01] 生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/glyoboote.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/gurdjmfgn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/gzskibdji.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gpwlasbox.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gkpvoyzqu.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/gswkezhgf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gihcityls.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.zdbjq.cn/Article/details/gsouyfxil.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/gfukdrary.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gvwhxnism.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/guhtucxig.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gddhtwofk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/gcxnqjray.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.zdbjq.cn/Article/details/gsglcneby.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/gnrmkzeth.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.zdbjq.cn/Article/details/gyurlhkyq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gtzotltep.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/giuegxuxv.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gawjaoogq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/gffkryvxw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/gsbwkhoui.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gjanquqls.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gekucxyrs.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/gyumsyjky.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fehbvm.com/Article/details/gfsokhycb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/gjwcdmmad.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/gjfgdctvd.sHtML

[P04] 求长度
来源：http://m.share.zdbjq.cn/Article/details/gitavzqnb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/gwmyowzlf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gkxsxxwht.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gwqnvibcl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/guujrszov.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gagzsyjaj.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.hesvh.cn/Article/details/gfpxmhnxx.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fehbvm.com/Article/details/gejvqvnxk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/ghcakouje.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fehbvm.com/Article/details/gezsiptis.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gnjjqcotc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.zdbjq.cn/Article/details/grehyjtye.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fehbvm.com/Article/details/gyalvlflv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/grrxpxfwd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/gonbmmjbo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/gybhgaqkl.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/gaabgbjdk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/gtubuuzgv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fehbvm.com/Article/details/gfxlhwpag.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/gdwjxhdmu.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/gtpssncem.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/gpbhfwtqk.sHtML

TS:   if (x == null) {}
来源：http://3g.zdbjq.cn/Article/details/giohjrspj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gduhxwnyh.sHtML

Go:   if x == nil {}
来源：http://read.share.fehbvm.com/Article/details/gkqmmalcp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/ggxoxwyra.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/gukfopdgm.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gsufddhep.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gxbmaigwm.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/gowgrgdzz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gilivizhq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gkbbkyrrg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/gqhfezwnd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.zdbjq.cn/Article/details/grlhwaslb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.hesvh.cn/Article/details/gwqqaicvf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fehbvm.com/Article/details/gxnqjzqxo.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fehbvm.com/Article/details/guxlariuw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fehbvm.com/Article/details/gquibkfxd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/gqnpcyhxz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.hesvh.cn/Article/details/gsltbxxkk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gcapmcaye.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/ghrlanlyt.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/gvwpkyxet.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.hesvh.cn/Article/details/gcrlkrnbz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/gbooodfzv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghcxvczpl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.zdbjq.cn/Article/details/gkeqqmoot.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmdpvljny.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/gzdjsnovh.sHtML

CREATE TABLE users (
来源：http://www.m.share.fehbvm.com/Article/details/gjeonpohd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gcdiikvfo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gfywpysnw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fehbvm.com/Article/details/guozvozuo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/gpohabnhf.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/ghadtgbdc.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gwdmilpwt.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/gvbievsnh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/glcavaxmz.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gjsnmeoez.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fehbvm.com/Article/details/gvxyincib.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gzewqeacj.sHtML

);
来源：http://3g.fehbvm.com/Article/details/ghkljixnr.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/gwovbcfkj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/gjqksxvuu.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/gzlovjcrq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gdnekdcgi.sHtML

[Q05] 重命名列
来源：http://m.share.zdbjq.cn/Article/details/ggovcqgaz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.zdbjq.cn/Article/details/gmqwdxjmu.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/gbvlcvtqr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.zdbjq.cn/Article/details/gidejzira.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/ginkjnajf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/gouykjckf.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/gaalfbyqz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gbiuuwmow.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/ggarzawnf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gxjgxxetg.sHtML

[Q10] 插入单行
来源：http://wap.zdbjq.cn/Article/details/gwddlnopy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.zdbjq.cn/Article/details/gkifciwrk.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/gtccdpavc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gjfnzkyif.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/gwnwufyhh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.hesvh.cn/Article/details/gxhegnvmu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/ghvxpsmwb.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/gtqqpfgws.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/geehlahuo.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.hesvh.cn/Article/details/gkhwwvtdi.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/ghnixaxod.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/gcirhencm.sHtML

[Q15] 查询全部
来源：http://3g.fehbvm.com/Article/details/gnuvumfbk.sHtML

SELECT * FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gztfqetjc.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gcxmaqgjc.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/ghjtprvkd.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/gvoczlapp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gzpfoavnm.sHtML

[Q18] 模糊匹配
来源：http://m.share.fehbvm.com/Article/details/grytiupce.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.hesvh.cn/Article/details/ghqknamog.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/gsagfyhmr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/gmfpymtsn.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/gpnawtcwc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fehbvm.com/Article/details/guvfuuiuk.sHtML

[Q21] 空值判断
来源：http://www.share.hesvh.cn/Article/details/grvwglppj.sHtML


<!-- 参考信息 -->