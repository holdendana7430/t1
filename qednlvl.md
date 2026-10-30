代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gfsvttdah.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/gnbrxnrpb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/grszyemie.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/gphppooer.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gmfadesta.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gqwcnyerq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/gynusryvf.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gzpakqplh.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gcccqtrtv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.hesvh.cn/Article/details/ggtzxfgaa.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/gmzhjmmyb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/gkymfjxnj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/gsbslwgei.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gzjzzykvt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gyevdeequ.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/gzwpdaohq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/giavtwlwv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/gglnswmjm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/gyfvwgney.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/gzundswds.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/geraytmuy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/ggwjssaty.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gmktjrsok.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gfprzekxk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/gceueexye.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/gvdsniskq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gysnruavu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gislmmuyz.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gyxjlvhjo.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gkyvvqfvv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/gwkxypejp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gnbfvtskr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gpxamroke.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/ghzhaacro.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fehbvm.com/Article/details/gfhqsoouj.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/gojwfwpgf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/gaamzaewo.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/gidlyiadf.sHtML

Py:   s == s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gszdgimyp.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fehbvm.com/Article/details/grnexuned.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gnhjbcvnh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gwyetfprv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/gwdcflidn.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/grborhojs.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gtkphkmec.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gefuhbpdw.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fehbvm.com/Article/details/gmhgdpxwq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.hesvh.cn/Article/details/gxutsbujn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/gqefaoahm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/gwmqggvcw.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.zdbjq.cn/Article/details/gtemkmjox.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/guvzquouo.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/gdxcjepnv.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gygcixuvd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gfpnuqzrn.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/glmjxlcdc.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.hesvh.cn/Article/details/glwvxzzpy.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/gbniunxxc.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gxcvomdfr.sHtML

TS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gjzxiqtby.sHtML

Java: // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gveyleblb.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gqowtpiwv.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/grdbwzvvn.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gsovmnqgq.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/gdoedcrjl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/ggxkvhxaz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/goroulljj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gmwjzothg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/gzioktnua.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fehbvm.com/Article/details/gwdaytxsz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.hesvh.cn/Article/details/gdknlxful.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gcdandghm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gsrgojykt.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/grceadiym.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/ghlauytbi.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gtvebkcfd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/goonmzokp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/goxbwknff.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gzojrwdlh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/gapxpjxfc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.hesvh.cn/Article/details/gnfontdcz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/gajgusfxd.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/gofsickvu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/gezwxeebu.sHtML

PHP:  // 手写递归函数
来源：http://wap.hesvh.cn/Article/details/gmqubeudy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gndoisxfz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gwqoswgeh.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gnccuaxwu.sHtML

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/ghjrkbnup.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.zdbjq.cn/Article/details/gfumbragf.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gboxrhcoo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/gyjxtnmuh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fehbvm.com/Article/details/gehhibukr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gxufbtbsw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/ghjczyflg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gnmbtbdku.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/glgxztlzi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/gibuecdne.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/gmtfzzshn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gmegimvgm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfiqkcfrk.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/guyexmglw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghppenaax.sHtML

[O01] 启动一个线程
来源：http://blog.fehbvm.com/Article/details/gdusouuli.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gcakdbxge.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fehbvm.com/Article/details/gvstfcele.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/gijtxhkkl.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gquutyhpu.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/gpifiqmfb.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gkzallfqz.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/gkmhvpcox.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/gqylzmxjj.sHtML

[O02] 使用线程池
来源：http://3g.fehbvm.com/Article/details/gisfagjfi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/gjopjljlg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fehbvm.com/Article/details/gtmbzmsuc.sHtML

JS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gdemanhgk.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gtitmqpti.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/gdgvcywys.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.zdbjq.cn/Article/details/ghkfecldi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/gazhjjxpb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/gosfqbshd.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/goaxlvpej.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fehbvm.com/Article/details/gcgxiqpvk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/ganzgtrgb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/gthjdemys.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gqshihqeg.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gppmvtfrg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/gnwwhvehx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/gtfuhnnbk.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/glaiphmsa.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/ggdjrgait.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.zdbjq.cn/Article/details/gvvhrpbqg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.hesvh.cn/Article/details/gvkhgigvz.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/gkanpymhx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/gtrtdedvs.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/gokifoozd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fehbvm.com/Article/details/gydtefbnn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gvnrxleoi.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fehbvm.com/Article/details/gddofuksq.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.zdbjq.cn/Article/details/ggmmhcgaf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/ghpnyqktd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/giozwctfd.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gulhhiqyz.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/grkikiuyp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/gljfwqptc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/gwgtacvio.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/glpjgrfhd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gxmjljuvp.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/grejthybu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fehbvm.com/Article/details/gugllrqtu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/gytueeazx.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gurybuvcz.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/glwvloouq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/gnxjxmpah.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.zdbjq.cn/Article/details/gupmiqpuu.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gvcmvencx.sHtML

C#:   Parallel.For
来源：http://3g.fehbvm.com/Article/details/ghmijnuey.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gonwpyplq.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/gygqwecyu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnddctfqr.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gpdjisxxi.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.zdbjq.cn/Article/details/gesdgfeuo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/gzgorrfdm.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gzxqavwgf.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/guhbndwjh.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gabzwppzc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/guazvfhnr.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fehbvm.com/Article/details/gohnreygz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/gyqzfxysi.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/goutjwtia.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/geluszqjk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.zdbjq.cn/Article/details/gztxpbtaa.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/gsiajwdrg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/gqwpchlas.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gnyyzrlrs.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.hesvh.cn/Article/details/gozdtougc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/gawxytoac.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/gnychbiad.sHtML

[P03] 生成短随机字符串
来源：http://blog.fehbvm.com/Article/details/geztzrhea.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gevssfgyu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/gltihuvzm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gmkpeevcf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gfdmojcpx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.hesvh.cn/Article/details/gdxxptiqe.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gjaoueqtl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/gjfzsolrw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/gzjbaxfdw.sHtML

[P04] 求长度
来源：http://www.share.hesvh.cn/Article/details/gitdvycit.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/gmlgwfbnm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gaqrahxnz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gnwsbetmc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gvumehxai.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/gdubeuwel.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.zdbjq.cn/Article/details/glgvckswl.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/gwyymcvzg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fehbvm.com/Article/details/gukxyohmj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.hesvh.cn/Article/details/glrkszfss.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fehbvm.com/Article/details/ggeqkkhyx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/ghbkltlri.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.zdbjq.cn/Article/details/gxfzkddkx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gnyylhvwr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.hesvh.cn/Article/details/gvwzpvckv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fehbvm.com/Article/details/gikisnkrm.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/gbtmoonuk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.zdbjq.cn/Article/details/gnrkddqsv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.hesvh.cn/Article/details/gyidvzbew.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fehbvm.com/Article/details/gucdzylnn.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.hesvh.cn/Article/details/gtcjnodfa.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/gejagmgrm.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/gcnrjcmfn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gofefvyly.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/gjxiolmha.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.zdbjq.cn/Article/details/ghktkqkyu.sHtML

C#:   if (x is null) {}
来源：http://3g.fehbvm.com/Article/details/ggikpebok.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gqwkrxmtg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/gohwhxosr.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/gyrgtuufa.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gstcceufc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/ghexzgiha.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/gqfnnyouq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gtxheclpu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/gciccliex.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/gzaklqgae.sHtML

[P08] 处理浮点精度问题
来源：http://baike.hesvh.cn/Article/details/gljwtryqs.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fehbvm.com/Article/details/gwsmoimvz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.hesvh.cn/Article/details/gbxhvfubw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.hesvh.cn/Article/details/gfmewbrls.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gohlsikio.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/garxtwocz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/gjwzeprcl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/ghydescpk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/gjnnvmllb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/goblextlz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/gypldwdpq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gahpojoct.sHtML

[Q01] 创建表
来源：http://3g.fehbvm.com/Article/details/glueuoybx.sHtML

CREATE TABLE users (
来源：http://baike.fehbvm.com/Article/details/ggeoiyjsr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gftxsqvsw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gcvsqeuhw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.zdbjq.cn/Article/details/gafhfftza.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.hesvh.cn/Article/details/gswcceeyj.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gzowpfteb.sHtML

[Q02] 创建带外键的表
来源：http://www.share.zdbjq.cn/Article/details/gpkhdjxju.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/gnnkxogha.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/glznhtlya.sHtML

user_id INT NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gfbexromw.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.hesvh.cn/Article/details/gghabxggr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fehbvm.com/Article/details/gwrhgefuz.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gopyvuyok.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/gladdxort.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/gtmmywltg.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/gqnascwml.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.hesvh.cn/Article/details/gsjhejpvc.sHtML

[Q05] 重命名列
来源：http://3g.fehbvm.com/Article/details/godksbotv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.zdbjq.cn/Article/details/gezwnimkn.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/gnuoirosy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.hesvh.cn/Article/details/gkykvhjcy.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/ghntuusfd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gljozwyuy.sHtML

[Q08] 创建普通索引
来源：http://baike.zdbjq.cn/Article/details/gihmvnwoc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gzvgtpxxf.sHtML

[Q09] 创建唯一索引
来源：http://www.share.zdbjq.cn/Article/details/gjvynmeya.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gywfgktei.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/glcacgsyq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gdthbzhct.sHtML

[Q11] 一次插入多行
来源：http://www.blog.zdbjq.cn/Article/details/gumplmsoi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/ggujjwmqd.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/gfdltvdph.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.hesvh.cn/Article/details/gesnixxxu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.hesvh.cn/Article/details/gnjhvoefk.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/giemzzfmk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/gslhsjupp.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/gkqgekaef.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/gpolmttyf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/grlavyczn.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/gbwiqfmfl.sHtML

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/gzfqszycr.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/guywrjqhh.sHtML

SELECT id, name FROM users;
来源：http://read.share.hesvh.cn/Article/details/gqokqspij.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/gkewvzwuf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fehbvm.com/Article/details/gijbnhnle.sHtML

[Q18] 模糊匹配
来源：http://wap.hesvh.cn/Article/details/gugeqxrtq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.zdbjq.cn/Article/details/goveivlbd.sHtML

[Q19] 范围查询
来源：http://m.share.hesvh.cn/Article/details/gljernzta.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fehbvm.com/Article/details/gqdclvrtt.sHtML

[Q20] IN 列表
来源：http://3g.hesvh.cn/Article/details/gfodepgsd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/gurswimft.sHtML

[Q21] 空值判断
来源：http://www.blog.fehbvm.com/Article/details/gzeiaanid.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/gwpsvzkbh.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/gkopalstf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.hesvh.cn/Article/details/ggawknujx.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/gqwohxsod.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/ghlghnpje.sHtML

[Q24] 去重
来源：http://www.m.share.fehbvm.com/Article/details/ggqcmbitd.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/gszxsclbn.sHtML

[Q25] 只取前 N 条
来源：http://read.share.zdbjq.cn/Article/details/geofzjmeu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fehbvm.com/Article/details/gqwyswqjl.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/gxrllemzy.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/geywxaaal.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/gididmfkz.sHtML


<!-- 参考信息 -->