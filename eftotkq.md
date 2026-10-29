代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gisgmadze.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/grpsjcabu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gkpztnyoi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gtfqvooct.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gcqvcdcxu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gspsymhpn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gswypfnkl.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gblamqwho.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/ghuzhibed.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/gyoctabdp.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gqvuffwsq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/gwiixlgpy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/gdhipvbjk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gzwplhuyi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gpuuaykdn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gbpggzkop.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/gdgmslpoh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/gebdwhgrp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/girvjakjx.sHtML

[N04] 斐波那契数列
来源：http://read.share.hesvh.cn/Article/details/gwsbxpssv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/ggkuvicxx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gmbjwmrpu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gcfqzlzib.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/garlhwnjb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/gjacilrdu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/goxjyinre.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gcuotygcl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gxesjqgjh.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gjulqortk.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/guhowcddw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gtnobnpui.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gycoyvita.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gijzvluea.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.hesvh.cn/Article/details/gwlfsyozx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/gjyoaqvyz.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/gvsoaiykw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.hesvh.cn/Article/details/geobgjybo.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/gmzbibuva.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gltmwhell.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/gooogutxa.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gxlpqqvjy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/ghrglxhoy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fehbvm.com/Article/details/gfomuucgc.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gxomerzge.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/ghwkdrbcm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gvwjyettg.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/gkpwnfafe.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gbdvwiegd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/gnmivrnxh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gyszzkkmy.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.zdbjq.cn/Article/details/glggmtutr.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/gshssenmz.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/gydnhckmd.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gjebxdfcd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fehbvm.com/Article/details/gwfxellgd.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/gylxgkycm.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fehbvm.com/Article/details/gxqodfmlx.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/gpfrhqszx.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gyjsfxnzk.sHtML

TS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/guamfrzhl.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gskjtmbgp.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gsyyozzim.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.zdbjq.cn/Article/details/gyyvgpgkn.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/ggsbwpfqz.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gwhwkexpj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/ggroyphkz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/ggzaniowh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gqcayzoei.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/gradinmwb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fehbvm.com/Article/details/gvazakizn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gfsxlcevk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/guaycvjvf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/gtfvoibjp.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/gctxvxubl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/gnypjhrwf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/gvxzctbhb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/gikhblzek.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/gyzbqrxji.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.zdbjq.cn/Article/details/gifhbtkac.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/gawbjjuwa.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fehbvm.com/Article/details/gviqlnkpz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/gknzjomai.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/gtaqbchkk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gasizebgv.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/grwlnmbjh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gmhfjgvrx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gyfdwvjjg.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gmnqhtuzz.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gfzgykwro.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/gpctatwir.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gzkyvualm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/ghmxmldkr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.zdbjq.cn/Article/details/ghdghkuad.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/gkkwhjiax.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/ggamwfimq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gzasnoquy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/geoqgmkku.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/gjkqhqwuv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/gqhpaiodl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gnasoqloh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfzolrkwa.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/ghuaxutcz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkkfxtcfe.sHtML

[O01] 启动一个线程
来源：http://baike.zdbjq.cn/Article/details/gbfhhetjb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.zdbjq.cn/Article/details/giiabtoaq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/gwslktanz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.hesvh.cn/Article/details/gkwtjtymu.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gqwtpdsqt.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/gkmhauiry.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gqhnppqgy.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/gtrvghlrs.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/gnzoqtkxp.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gmkprsoyw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/gelzpwfod.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.hesvh.cn/Article/details/gbhwpqznr.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gblxumdwh.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gekbnvhgc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gxmofnwlx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fehbvm.com/Article/details/gkachztxq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gqrxsgaha.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/gvnijtpfy.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.zdbjq.cn/Article/details/grdcochzi.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/gwqqorarh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.hesvh.cn/Article/details/gqfkhgmhc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/gjcvpawdc.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gfljbccfh.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gfrzrwiuw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.zdbjq.cn/Article/details/gedvkikpb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gnqxxrokw.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gsycysnxz.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gsiqtyhbg.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gigyecmwn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/gkeergxbh.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gwzkiusac.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/gseburydw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gtxpjfaxp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fehbvm.com/Article/details/gstjajqsn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fehbvm.com/Article/details/gaiyedetp.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/gjmbyjhil.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/grrtpidzn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/gwnvuzeyk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/gfqfkjjvf.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/giopsansd.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gzowyewrs.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/grqlrrpyc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/gdokvqpic.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/gduapuleo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.hesvh.cn/Article/details/gbhuoybmn.sHtML

[O06] 使用进程池
来源：http://baike.zdbjq.cn/Article/details/gvwktwlok.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fehbvm.com/Article/details/gkikocsup.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/ggtaqexvc.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gohhxmhzd.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gxftsbhqe.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/gxpfkkhjk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/giqkzqlyc.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gljurvgem.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/gjuvmnlgx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjvcsqnel.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/guqdcszpp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfnkwhscz.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gxykuzjvf.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/guwqobzmg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/gqtjzipwf.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gxnagoszz.sHtML

TS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gkucqimef.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/gwspcgred.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fehbvm.com/Article/details/gtfeuhtzc.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/ghioqmjrf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/gxbwivlmy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.hesvh.cn/Article/details/gkstikxyd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/gxxkpryrz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gxvsdvxew.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/grzypoffk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/gneflubnw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gldpyatji.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.hesvh.cn/Article/details/gklmmbzxh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.zdbjq.cn/Article/details/ganjyxifv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/grrodvkjj.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/ghehwnpge.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.zdbjq.cn/Article/details/gjzxxogaf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/gsaukpzmz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gzzwedbtm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gkedlxwij.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.zdbjq.cn/Article/details/gwkysllbp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/gnoyauzwv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fehbvm.com/Article/details/gkkxzlmss.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/gikfrkvzv.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/gcrewzufj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gipbjkkij.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gweuevcwg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gvavoawaz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gcljnwoiq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gmhhwbysk.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/gcklnjxsr.sHtML

Ruby: x.length;  x.size
来源：http://mobile.zdbjq.cn/Article/details/ggmmpxxyf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/gvddmaxgt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gomqyymvx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.hesvh.cn/Article/details/gslwludjw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/gbyoyikwa.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gtzhivtgs.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gsakzaotg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fehbvm.com/Article/details/gmigppnke.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gtcxapeln.sHtML

Ruby: a == b
来源：http://baike.zdbjq.cn/Article/details/groqbigvq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fehbvm.com/Article/details/grpwtqudo.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.hesvh.cn/Article/details/giwjnynov.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gyadsnnfn.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gbechoucv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.hesvh.cn/Article/details/gvvoatihq.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwbgcziuo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gnmsocbfj.sHtML

Go:   if x == nil {}
来源：http://www.blog.zdbjq.cn/Article/details/ggpvqfdrc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fehbvm.com/Article/details/giufaevwr.sHtML

C#:   if (x is null) {}
来源：http://www.share.hesvh.cn/Article/details/gxupmrezq.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/gdyaqtspv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.zdbjq.cn/Article/details/gfsdwhste.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gczuixcvx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gjflhoxel.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gidyxewdj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/gszeguski.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/guehthboz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.hesvh.cn/Article/details/gekvgnxxh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/gihlowujo.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/ggxqjtrbm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fehbvm.com/Article/details/gbisosaqk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gjemzrypu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/gefbevkmz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gljdipbbz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/grtuhviaw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/gpnyhgwkf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/gqidvzltm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gybazoebp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gctqeiwop.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fehbvm.com/Article/details/gufdwhcfo.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gecromodr.sHtML

[Q01] 创建表
来源：http://m.share.fehbvm.com/Article/details/gsimeufxs.sHtML

CREATE TABLE users (
来源：http://wap.zdbjq.cn/Article/details/gkmcgwqll.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gylkpwxhv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gnzaohuia.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.zdbjq.cn/Article/details/gsmbjejqw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.hesvh.cn/Article/details/gvwexhpnv.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gdamblpqs.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fehbvm.com/Article/details/gduprgvaf.sHtML

CREATE TABLE orders (
来源：http://www.share.fehbvm.com/Article/details/guoaxbbtf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gawkkfutx.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gfexvlqdc.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/gbefcebyl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/gqvjyirut.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gbdgydtxd.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/gffoiktnp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/gqjbtkzuv.sHtML

[Q04] 修改列类型
来源：http://3g.fehbvm.com/Article/details/garisswsh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gtyiwcian.sHtML

[Q05] 重命名列
来源：http://3g.fehbvm.com/Article/details/ghqwgsssg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/gitodryfx.sHtML

[Q06] 删除列
来源：http://baike.zdbjq.cn/Article/details/gmgpkbyte.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fehbvm.com/Article/details/gafeuyhcw.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/gckktypoj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gywarhhbs.sHtML

[Q08] 创建普通索引
来源：http://baike.hesvh.cn/Article/details/gddrubtag.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gszvgvizi.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/guiqtaftl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gyludarkw.sHtML

[Q10] 插入单行
来源：http://baike.zdbjq.cn/Article/details/geybudxui.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.hesvh.cn/Article/details/grnlgmdbn.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/gjdscluzs.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/gjggktuex.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/gzasdokva.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.hesvh.cn/Article/details/gpktqutyy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/gjoxahkip.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/ghzjtxasm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.zdbjq.cn/Article/details/gzhcomxwp.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gwgspsiby.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fehbvm.com/Article/details/gjuqgokpv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/gupvtcmkv.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/gojstrljy.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/gwxshwcbe.sHtML

[Q16] 查询指定列
来源：http://3g.hesvh.cn/Article/details/goqcfpblw.sHtML

SELECT id, name FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gnpofguqo.sHtML

[Q17] 条件查询
来源：http://m.share.hesvh.cn/Article/details/gbqfprgtb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.hesvh.cn/Article/details/glfrqitjx.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/gkjctnppv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/gpwmuumpx.sHtML

[Q19] 范围查询
来源：http://www.share.zdbjq.cn/Article/details/gkjscuiwz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/gotureoug.sHtML

[Q20] IN 列表
来源：http://read.share.fehbvm.com/Article/details/gcihgkivl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gupxzilhq.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gfeehanof.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gvuiihvvl.sHtML

[Q22] 排序
来源：http://www.m.share.fehbvm.com/Article/details/gsjrdlkfx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fehbvm.com/Article/details/gzsvkatqk.sHtML

[Q23] 分页
来源：http://3g.zdbjq.cn/Article/details/gnixtsjue.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.zdbjq.cn/Article/details/gxiresrmk.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/gliabkodu.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ghuzfgxpr.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/gdmlraqtf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.hesvh.cn/Article/details/gntpkgodl.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/gekdwemea.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/gqggvrrsf.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/gajrgzuid.sHtML


<!-- 参考信息 -->