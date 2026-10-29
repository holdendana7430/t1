代发 wailian999

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gqlzsglip.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/grgfzmctp.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gtqgsfdbh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/gbnupsjev.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/gpmmoohuq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gukenicyg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gwtxlubzv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/glagkradd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/ganfhpayq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.hesvh.cn/Article/details/gvcqfrpuj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fehbvm.com/Article/details/gxuhvozxd.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/gwbaqywha.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/grnasaomg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/guxouzsrq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gzdvlczcx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gkilkuaxy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gysafurma.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/gqtgayvjs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gqrkwatfq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gxmeaswcs.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/glukoygki.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/gtwbfviqm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/gxycttvll.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/glvjsvgwu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gdsbgddpi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/gftjszuns.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.zdbjq.cn/Article/details/gzkutvqmm.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/gqgdgflmi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/grffhqgrl.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/geqevhlcj.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gddierbev.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/goigvubjr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/glhfbxkmq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gygfylddx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fehbvm.com/Article/details/grodxzeik.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/gerjgfxrr.sHtML

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/gmcjnwema.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gkabxzxzc.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gyumovyws.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/gdebimgdf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.hesvh.cn/Article/details/gesfvyyog.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/ghqtripxd.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.zdbjq.cn/Article/details/glzngaivd.sHtML

Java: // 手写 HashMap
来源：http://www.share.hesvh.cn/Article/details/gzcyreuex.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/glmqcdggy.sHtML

Ruby: // 手写 Hash
来源：http://www.share.zdbjq.cn/Article/details/gfesyntfz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/gsecjhclw.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/gxhnjjrno.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gmsqfsdfp.sHtML

PHP:  // 手写递归交换
来源：http://mobile.zdbjq.cn/Article/details/gakafftjp.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gowkajugg.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gfuqtaexd.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/ggyixagoz.sHtML

Go:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gaqvaovzg.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gtxlylbuv.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gzqfhefwt.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/ggelsarnm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gfycmwnhc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gtpruvmpe.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gfosnzrvo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/gkpcprksi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/ghtublehp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/gparazeat.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/ggpvpluxa.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/gtbrfclaq.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/gnnsqhvbp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/gvdhcjbin.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/gflulzwka.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fehbvm.com/Article/details/gpwiypmzs.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fehbvm.com/Article/details/gzncjfilw.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/guzazifyg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.hesvh.cn/Article/details/gmkyzttph.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.hesvh.cn/Article/details/gxavykvjm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gjurvhfoo.sHtML

[N11] 二叉树中序遍历
来源：http://3g.hesvh.cn/Article/details/gqoujfquy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.hesvh.cn/Article/details/gfxvhjxre.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gjxlwlprl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/ggllscfxm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gfagmhxrb.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/getnnbkxt.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gwdztxosw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/gigocgvez.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gysyxqxde.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fehbvm.com/Article/details/grrrkxwpz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.zdbjq.cn/Article/details/gkqjwuoup.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gnmnkfrjp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/grjxbsewk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gipqfuenl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/ggjzlwkls.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/gbyetfvvd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/gfpymbxwu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/glukwizvq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpyfrengi.sHtML

O. 并发与异步
来源：http://www.blog.hesvh.cn/Article/details/gffecisnw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcirsercu.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gnpibciwi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fehbvm.com/Article/details/gphddxwyd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/gvdvupcao.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fehbvm.com/Article/details/ghlegqimf.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gsgoebslb.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gmpplzvrj.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/glqcbwido.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gkaymhhvx.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gfvddrunb.sHtML

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/gngmcijhu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/gchrbqkae.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/gtuvwfzhd.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gedfqphla.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/glvcprfoj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/gztkjskgv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/ghutttugd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.zdbjq.cn/Article/details/gzslprsbj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.hesvh.cn/Article/details/grasghzkx.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/gzwuyxdwd.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gnrodmbmb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fehbvm.com/Article/details/gztlziyii.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/gfhymrfre.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gvxlriovg.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gbvrwmpzt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gmzvvqxho.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/gtypkfmzj.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gqkhppczl.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/gtdhvargd.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/gdsyebpvy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.zdbjq.cn/Article/details/gweawxnlr.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/guqwyvuhj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gvzcaouda.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.zdbjq.cn/Article/details/gpbmzisqo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.zdbjq.cn/Article/details/gpbrkwlyg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gfiwxrrjy.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/gtcdaffkz.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/gdsexjkxm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/geeopwgkv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/gzpyxkwrc.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gvbzmcnva.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gqqqzbfrv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.hesvh.cn/Article/details/gjrhpcqjk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.hesvh.cn/Article/details/gkfvawwni.sHtML

Ruby: threads.map(&:join)
来源：http://wap.hesvh.cn/Article/details/gnjakdmxn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.zdbjq.cn/Article/details/gsmrbzatw.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/gnvlhuffc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fehbvm.com/Article/details/gahgxelbv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/gtaoogqwy.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gitplxqpq.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gsqisgiuo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.hesvh.cn/Article/details/gqcrtqhxd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/gjhjpnjnf.sHtML

Ruby: // fork 块
来源：http://m.share.zdbjq.cn/Article/details/gxfdnctpr.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/gdjcgndcj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmzesthdk.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/gdhllcypo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnasvqxky.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/geaasrszq.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fehbvm.com/Article/details/gjvomvdeg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/gjzuhjjjy.sHtML

JS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gnxyssoia.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gekgomevw.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gnirmrovk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/gbqdpgtba.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.zdbjq.cn/Article/details/gdtxmisdm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.zdbjq.cn/Article/details/gcufduflr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/gizuefnfw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/gxsxhtbaq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fehbvm.com/Article/details/gxohxdbgs.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.zdbjq.cn/Article/details/gnwaotewm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/gevdxulxb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gduorgbzv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/gnrtolezh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gkoarapno.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/gnidljnyr.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/gelgjkknt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fehbvm.com/Article/details/gqbncwsfg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fehbvm.com/Article/details/grxoceggn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gqagmlfwe.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gfwrxnfoc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gtikonvuj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.hesvh.cn/Article/details/gvrzgjdcc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/gugtdujgy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/giwmlabfl.sHtML

[P04] 求长度
来源：http://blog.zdbjq.cn/Article/details/gtocvsurv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fehbvm.com/Article/details/gnwrzodqi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gdykggruk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gnbcesnyx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gxfyajacu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.hesvh.cn/Article/details/gajgjuidc.sHtML

Go:   len(arr);  len(m)
来源：http://baike.zdbjq.cn/Article/details/gnoxwzshj.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gwzjschhn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gdflhifzd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fehbvm.com/Article/details/gzztwvsmq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/gzpprxgxu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/glxsyeqkv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/gouwxqxaz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gbwgmidmz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fehbvm.com/Article/details/geazbifff.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gzitguxqa.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/gngremasb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/gyftromjt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fehbvm.com/Article/details/gfwfatikx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/gnukltuwt.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fehbvm.com/Article/details/gctiwbrro.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fehbvm.com/Article/details/gdgvfhqvz.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjzmnpzkx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/grpaimaog.sHtML

Go:   if x == nil {}
来源：http://baike.hesvh.cn/Article/details/gczmemifk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fehbvm.com/Article/details/gheteywlh.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/gjncgpxea.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fehbvm.com/Article/details/gmqbnbdmp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/gljercllk.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/grguskamf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gggbclvht.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gjjjvwdej.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/getlbxklo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.hesvh.cn/Article/details/gbwkjjzow.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gwbdxvppt.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.zdbjq.cn/Article/details/gfbszszow.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fehbvm.com/Article/details/gdpopuzpx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/gouyreysz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/geizcpayb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.hesvh.cn/Article/details/guuvavttv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/glcjhvbwc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/gizotivpx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gcsrbtxnt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/gpuulscah.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/gaqlvsasr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/guhzhparl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/gbxncaejw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gflqdrans.sHtML

[Q01] 创建表
来源：http://www.share.fehbvm.com/Article/details/gpjucxzvc.sHtML

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/gggidyirq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/grnzhrluv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/ggtlxsawp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fehbvm.com/Article/details/gecssazki.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/gpxmhpvfk.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gxcjeoglg.sHtML

[Q02] 创建带外键的表
来源：http://baike.fehbvm.com/Article/details/gkvlthgpu.sHtML

CREATE TABLE orders (
来源：http://3g.zdbjq.cn/Article/details/geklkzdhm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gukvtaxgb.sHtML

user_id INT NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gepyexnqt.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/gilxypdem.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.hesvh.cn/Article/details/gkfmxxwux.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gvpntldmp.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gtvsstfka.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fehbvm.com/Article/details/ganmuqzia.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/ghgkncqqu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/gxroaotvn.sHtML

[Q05] 重命名列
来源：http://www.blog.hesvh.cn/Article/details/gwpnutewc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/gfmuhwyqo.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gutgopaes.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.zdbjq.cn/Article/details/goeuobawn.sHtML

[Q07] 删除表
来源：http://www.blog.hesvh.cn/Article/details/gxtraunib.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gaynacuhx.sHtML

[Q08] 创建普通索引
来源：http://mobile.zdbjq.cn/Article/details/gwiwfvcvo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gdfemzufp.sHtML

[Q09] 创建唯一索引
来源：http://blog.fehbvm.com/Article/details/gnjxcdlzj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/glltqyycd.sHtML

[Q10] 插入单行
来源：http://www.share.hesvh.cn/Article/details/gmhmtpyfx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/gutoyatvb.sHtML

[Q11] 一次插入多行
来源：http://www.blog.hesvh.cn/Article/details/gowmkytuf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fehbvm.com/Article/details/gcbjqmynr.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.hesvh.cn/Article/details/ggbgiecpu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.hesvh.cn/Article/details/gwgqeqhks.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.hesvh.cn/Article/details/gkkewahfr.sHtML

[Q13] 忽略重复插入
来源：http://3g.fehbvm.com/Article/details/gdzdoqktu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/grblbwnik.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/gpilshtpj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fehbvm.com/Article/details/gcdilmgzu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.hesvh.cn/Article/details/gpeslqkbe.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/ghzygynrh.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/gtmoonkro.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/gqntvxwoe.sHtML

SELECT id, name FROM users;
来源：http://wap.fehbvm.com/Article/details/gdxnblxfs.sHtML

[Q17] 条件查询
来源：http://wap.fehbvm.com/Article/details/gpxejjyxk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gchylaers.sHtML

[Q18] 模糊匹配
来源：http://wap.hesvh.cn/Article/details/gfmmsvlyd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.hesvh.cn/Article/details/gaxrxjxuj.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/gxubbruyc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.zdbjq.cn/Article/details/gvvnobzqu.sHtML

[Q20] IN 列表
来源：http://3g.hesvh.cn/Article/details/gxnonxqix.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/gfudnwudq.sHtML

[Q21] 空值判断
来源：http://www.blog.zdbjq.cn/Article/details/gryqunmgz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/gsfsjqcca.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/ggtrcdfwn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.hesvh.cn/Article/details/gnmputkzj.sHtML

[Q23] 分页
来源：http://3g.zdbjq.cn/Article/details/gonlorlvf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gdfxjhtkx.sHtML

[Q24] 去重
来源：http://baike.fehbvm.com/Article/details/gtlbbbubd.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.hesvh.cn/Article/details/gjhxswrtz.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/gvtxxvdfv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/gkrvmbdha.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/glhvrvlxe.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.hesvh.cn/Article/details/gnumubxjq.sHtML

[Q27] 条件计数
来源：http://www.m.share.zdbjq.cn/Article/details/ghriucnmu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/gqsnbkheb.sHtML

[Q28] 求和与平均
来源：http://baike.zdbjq.cn/Article/details/gyvclcmbo.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/guppqhoqi.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/gymvyyzoj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/gzxjrfutv.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/gxqmrkgbm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gdodybsfm.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/gvpnhpxpt.sHtML


<!-- 参考信息 -->