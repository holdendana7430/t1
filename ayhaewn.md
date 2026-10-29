代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gycfnxirh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/giuqqhvwp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gbltuqylr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.zdbjq.cn/Article/details/gbiilitdi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gvbjuqluo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gyqbfnoki.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gnamhgmhi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/gheccgwtp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/ggnjowcaq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/guqzbpnam.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/gxviswvna.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gsjsbuesn.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gtycsffso.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/gzhmpbguh.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/gpauozhzw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gflfdrmfn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/goiylntfh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gevwvmiul.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gcohtwvkx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/glxcdatmq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/ghkudoatt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gldwfsrbd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/gjobyvbnx.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/gfuqzsgvi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gxdultlpt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/gmrgwrnrg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/ghishpbkp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gblciivjo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gdrnxwxvy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/ganwyeqcf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gsecaknld.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gkfabwndr.sHtML

[N05] 最大公约数
来源：http://www.blog.fehbvm.com/Article/details/gentzpijg.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/gkenmmiit.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/ggfvrdkdi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gmnggilfv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/ggbbgvbkm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gfjtefxso.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gdtjcspmr.sHtML

Ruby: a.gcd(b)
来源：http://baike.zdbjq.cn/Article/details/gyiivwnpw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/ggdcmaolt.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/gmbuheawa.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gfggbkyuf.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gdnvuybsf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/guwljechf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gvpnvjeez.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.hesvh.cn/Article/details/gedchigqa.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/gwetckzyo.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gbyunpcvp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gtjryjniw.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gfggwknaf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/gegiimjao.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gqofpjtwl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/gcaeyzxrk.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/gyejaiuni.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/giezlvcyh.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.hesvh.cn/Article/details/gkvfttqya.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fehbvm.com/Article/details/ggkwadmgt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/grmnnchbe.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gcfilzafl.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gyqhqrndg.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/gxsxxtamn.sHtML

JS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gzrqqsruo.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/ggyrfeumj.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gwnljowhs.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gqrtycztj.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/gxaqqeswi.sHtML

C#:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gnaewakea.sHtML

[N09] 栈与队列
来源：http://wap.fehbvm.com/Article/details/gdnwmnbps.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/groeiddqp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/ghbovaspc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gjuhmntcp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/gqgtupmnn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gcnasqfvo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/gpmyuwgtm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gihdseokt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/giicrktjr.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/ghvkqfkeq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/gbtxzdxfx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.hesvh.cn/Article/details/gfyktnngn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/gqznypoti.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/gwfqezbqn.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gvfiqalmv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/giucinlmt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.hesvh.cn/Article/details/gvpsemwbm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/gqazckgwm.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/gpdvlqsut.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.zdbjq.cn/Article/details/ghxdtgsjx.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/gstalekrv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gkbzyynsl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/ggnpbwsnu.sHtML

Java: // 手写递归
来源：http://blog.hesvh.cn/Article/details/gutgsafqt.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/goiehsook.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gsyottafx.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gnlamdtsq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/gpxprodxg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/glqfdjfhs.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/gezfvviyk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gqcgndtmn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/grlyshzsv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/giiadigdd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fehbvm.com/Article/details/ghxmbbfam.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/gmfnzwmjb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/ghsxmywyu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gyubkjutt.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/gtxnkpjqs.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwoafbexo.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/gqgovcxcq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/gnxjazruh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/gwckrghif.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/gzhcgwfkz.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/geihdqnjn.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/gwixzsrdf.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/gmyizflwf.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/grujrdeds.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gyxgxovbi.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gudxhugoy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fehbvm.com/Article/details/gemsoapyd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/gqiweqjbq.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/geoecqaqq.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gurbpkbll.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/ghukzacbd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/gwcndtnlo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/gmlnbjptd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gmptpbivx.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gdnlwnpxy.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/gzmbfcfgu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/gypcwriaw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/gtnzmvuzm.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gbugklevc.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gfdbkledy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/gmuwadiwq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gsbyrujon.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gsjnldpoi.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/gjywccuvq.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/gsnjrbfhb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fehbvm.com/Article/details/gtuhofzaw.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/ggzkeageo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gfxntxbww.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fehbvm.com/Article/details/gpyjlgnqs.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/gygzbnfqz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.zdbjq.cn/Article/details/gpzbadmin.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/gfzglyxrj.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gopjfrzjs.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.hesvh.cn/Article/details/gvzkoctod.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.zdbjq.cn/Article/details/grlreedku.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/ghhftzkpm.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gxjbxoimf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/gctheqsvk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.zdbjq.cn/Article/details/galjtsmog.sHtML

Ruby: threads.map(&:join)
来源：http://wap.zdbjq.cn/Article/details/gyajiizjk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.zdbjq.cn/Article/details/gdjnqejod.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/gtyoxdcpz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/gjdyvclyl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.zdbjq.cn/Article/details/gplvupssk.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gfaalrjva.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gqygetkdi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/glmxthgpk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.zdbjq.cn/Article/details/gqbeulilh.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/gojuojfom.sHtML

C#:   Parallel.For
来源：http://m.share.hesvh.cn/Article/details/gtyxowgxl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gabpvtpsr.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/gozexyvql.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gediwnwzl.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gcatszmpb.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/gaevqsgku.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/gqbphkhio.sHtML

JS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/glwtvlbbl.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gaeznzxcp.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/gxxsuapja.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/ggykcjohw.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/gxzwjiczr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/gzarvftcn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fehbvm.com/Article/details/ggiknmhuj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fehbvm.com/Article/details/gavngjivt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.hesvh.cn/Article/details/gcnkbeenc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/guihxrcrl.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/gtxptboth.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/gtnvltpxm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/gnkaqzdop.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/gwrrukmxz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.hesvh.cn/Article/details/gbsfoqsvy.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/gonajzqqg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fehbvm.com/Article/details/greaqtwyy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fehbvm.com/Article/details/gmoszkfsb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/glyccaopu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/ggvekghve.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.hesvh.cn/Article/details/gbmqscgkm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fehbvm.com/Article/details/gceirqbdn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/gdxiqfffy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/giqcyvsrs.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gappwcghg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.hesvh.cn/Article/details/gcddjpwdj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/ginzbvtoz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gibynfavz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gjxoxrtcd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fehbvm.com/Article/details/gbfskidic.sHtML

Go:   len(arr);  len(m)
来源：http://baike.hesvh.cn/Article/details/gtbzkhknr.sHtML

Ruby: x.length;  x.size
来源：http://3g.fehbvm.com/Article/details/gdipmyvfc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/gfspeokyi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fehbvm.com/Article/details/gtoszoncc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gmiqyvsnd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.hesvh.cn/Article/details/gkymvvzfj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/guabulvuw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gxdataneg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gcsdocsov.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/gldsyqvpo.sHtML

Ruby: a == b
来源：http://www.share.fehbvm.com/Article/details/gpdvjpfts.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/gsbqqprdh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.zdbjq.cn/Article/details/gnsygdrug.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.hesvh.cn/Article/details/gyyhnhoth.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/grwmcqrhg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.hesvh.cn/Article/details/gzwkkhnov.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/gfaassrff.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gtgipmeie.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/gvndpybje.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/gvbwadqkh.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/gxjcpzcsx.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gbcgmxgpf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.hesvh.cn/Article/details/gyrdcrili.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/gbzhgpenj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/giyewpkrn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gfpoaycaf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.zdbjq.cn/Article/details/ghyihuixu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fehbvm.com/Article/details/gwklibikc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fehbvm.com/Article/details/glklxnmav.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.zdbjq.cn/Article/details/godtaboxe.sHtML

[P08] 处理浮点精度问题
来源：http://blog.zdbjq.cn/Article/details/gnwudembu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fehbvm.com/Article/details/glsixkaxp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.zdbjq.cn/Article/details/ghbmyqjsh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gimvzfbgk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gixssooou.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/gqpikaiwr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.hesvh.cn/Article/details/gbcsrfscn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/gksuspnrr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.hesvh.cn/Article/details/gcyszwzkh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcsvponse.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gygrveywm.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmsoznpdj.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gbzqladjw.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/gkwixpzha.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gloekpdpl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gbdgvykel.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/gcxgsenmf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/gnpaqdtgf.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/grkkrvaee.sHtML

[Q02] 创建带外键的表
来源：http://www.share.hesvh.cn/Article/details/gclxohsio.sHtML

CREATE TABLE orders (
来源：http://www.share.zdbjq.cn/Article/details/glrrwobjv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gxluvojbl.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/guupqihja.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/gufnmgcpy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.zdbjq.cn/Article/details/gjnonarpq.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/godtomuxn.sHtML

[Q03] 增加列
来源：http://www.m.share.zdbjq.cn/Article/details/gxkgucsfg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.hesvh.cn/Article/details/gfljeocgq.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/gvkxkmciz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/gbhvbvevn.sHtML

[Q05] 重命名列
来源：http://m.share.hesvh.cn/Article/details/glocvkgqn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.hesvh.cn/Article/details/gdosxsxkp.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gdrxwmnrl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/gyxhvktuq.sHtML

[Q07] 删除表
来源：http://mobile.fehbvm.com/Article/details/goaecfzzy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/gylvwswow.sHtML

[Q08] 创建普通索引
来源：http://blog.hesvh.cn/Article/details/glrrmifvp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gwuyyjaju.sHtML

[Q09] 创建唯一索引
来源：http://baike.zdbjq.cn/Article/details/gczzlfwka.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gjrodmkap.sHtML

[Q10] 插入单行
来源：http://blog.hesvh.cn/Article/details/gtsuqbrcb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/gbzlfhabr.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/gxbtqaeex.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/goimaxoea.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gaiajqmpc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/gzkumtqwk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/gsvkdmevg.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fehbvm.com/Article/details/gkxnkbbgl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gnodyhxog.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.hesvh.cn/Article/details/gokjxmdnd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/gktzynfmo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/glbgpaaum.sHtML

[Q15] 查询全部
来源：http://read.share.fehbvm.com/Article/details/grexfnugy.sHtML

SELECT * FROM users;
来源：http://3g.hesvh.cn/Article/details/gunljdeql.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/giosbfzbx.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gufjbuzkr.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gkykhezsp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.zdbjq.cn/Article/details/gagotoysx.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/grpckoedl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/gxlohdgxx.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/gimcjfhta.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/ggcwqbcce.sHtML

[Q20] IN 列表
来源：http://m.share.fehbvm.com/Article/details/gtyotikcx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/gtcffqljv.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/gvqwqtxrc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fehbvm.com/Article/details/gqighjzwn.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/gcuwxkqms.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/gmnacobhr.sHtML

[Q23] 分页
来源：http://blog.hesvh.cn/Article/details/ggqdpauti.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.hesvh.cn/Article/details/gorltlljc.sHtML

[Q24] 去重
来源：http://blog.zdbjq.cn/Article/details/glaqmggdf.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gmrbfndiq.sHtML

[Q25] 只取前 N 条
来源：http://baike.zdbjq.cn/Article/details/gmqwqwghy.sHtML


<!-- 参考信息 -->