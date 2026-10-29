代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gvdoxugql.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/gcigctnpb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/ghqmqivgq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gaqypukbm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gkmmllhky.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gytddgejs.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/gmkceyjxa.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gblcufxhv.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gvawncmfz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.hesvh.cn/Article/details/gxzebiohq.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/goqkqxdai.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/ghrjsaixm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.hesvh.cn/Article/details/gafygrhkr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gtcziinye.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gfztfctfl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gpacocktr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gdmqueczf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.hesvh.cn/Article/details/glgixtzrm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fehbvm.com/Article/details/grkxwewyt.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gtzltquus.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/grukbkoyn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.zdbjq.cn/Article/details/grpsmebny.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gdlygkwea.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gguvvemht.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gubktmvig.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.zdbjq.cn/Article/details/ggvfjoyxt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gtpomxotd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gxcrchiec.sHtML

[N05] 最大公约数
来源：http://baike.hesvh.cn/Article/details/gjaeunftt.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/gjowxodkc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gphddsyll.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gactyhreo.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gvqgvsgbo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.zdbjq.cn/Article/details/gonugvith.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/gmzqadggu.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/gjmcvxzmd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gfytxzeet.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/gswwvgmxl.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gvnsxasst.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gyvzojopb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/garplvyez.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gnmyrpzfh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/gnmzfghtd.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gnyoxyqpl.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gsahtswcp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gdmccsfyn.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/gcoiybssw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/gthlaeevk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gsukkrnua.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/gyainhnsk.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/gquimgyym.sHtML

Java: // 手写 HashMap
来源：http://baike.zdbjq.cn/Article/details/gzqvdgsit.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/ggjzbeyyn.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/gqfnatdwc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/gjckvbish.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/gfllpbifz.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gylswsibq.sHtML

PHP:  // 手写递归交换
来源：http://3g.fehbvm.com/Article/details/gjwdzpgep.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gwgjqwemk.sHtML

TS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/goeygvlmb.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gdevaxrpb.sHtML

Go:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gfbszedis.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/geaymmaff.sHtML

C#:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gafeujegb.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gyzuaejpz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.zdbjq.cn/Article/details/gtibpzxoh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gdnjmrqsq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gbqfdpwqr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.zdbjq.cn/Article/details/gvzjdojtg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/genqfpwpb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/gbmottrsv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gxbzfwrpm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/gznawebsd.sHtML

[N10] 链表节点定义
来源：http://3g.zdbjq.cn/Article/details/gnwaxebil.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/gyrolyzsc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/gxhbvkdde.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/gopkoazvi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gpsnmcpfp.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/glkbsmvaw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/gjtlmbypp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.zdbjq.cn/Article/details/gocvkbuay.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gutyropbn.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/gytdslttv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gwyxceyay.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/gucpkzpjt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gehsibiez.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gmlloenpj.sHtML

Java: // 手写递归
来源：http://3g.fehbvm.com/Article/details/gsurczfeu.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gdrcvspcf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gzliafcqq.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gmgyouvoz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/glpbqrqjb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/gktahgmdn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gzwwavehz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/guxrqignf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gjhjyxpru.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gxpjqjsyz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/gtbazbxby.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.hesvh.cn/Article/details/gluxycwyo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/ggtflqnlt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqmelucff.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/guvmvthqx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmfykghvf.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/ghopaohex.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gqtihmhwj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.hesvh.cn/Article/details/gecknbhgv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gepnpblej.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gthwjzdvv.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/gipckzmzj.sHtML

Go:   go f()
来源：http://mobile.zdbjq.cn/Article/details/gdzazrowu.sHtML

Ruby: Thread.new { f }
来源：http://blog.fehbvm.com/Article/details/gnevrivdm.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/gbqmiedkj.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/gourtoesy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/ggxvzjuiq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/gypnrfmrm.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gxfxsksbo.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gxaiausyb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.zdbjq.cn/Article/details/gbuaxlunb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/guffgeptc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/gcyfywbam.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/gdckorjyr.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/goblinigr.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fehbvm.com/Article/details/gqtaswhdx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/gzswfkffd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/ggdqmrmum.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gllwaeykj.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/guvwveqoi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/ghecmlxyp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/gvgryhlom.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gpasogybg.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/gptxllquc.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fehbvm.com/Article/details/gjrpnwyhl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gbsgwfwyx.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gjbqlyeir.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gxclcecng.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.zdbjq.cn/Article/details/geviybmoh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/gqafrvatb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/gaphdnsjb.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/gvaultdag.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/gwqxyqgzq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/gqpmoouer.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/gerqjbeoa.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gaebzhrxw.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gpwrdqhxd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fehbvm.com/Article/details/gzcdtnzub.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/guzrywbqv.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gqtmtaphu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gdanrtptq.sHtML

[O06] 使用进程池
来源：http://mobile.hesvh.cn/Article/details/gcoxpgncm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.zdbjq.cn/Article/details/galarrzko.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/ggdajkfhg.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/grndtdpaw.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/ggngibzfx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/gdqakaott.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/gowmqkwov.sHtML

Ruby: // fork 块
来源：http://mobile.hesvh.cn/Article/details/gdfyugwhs.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/grivdrdgl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gavrcafpw.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/gmmqmbusx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjhdtduvg.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gmcxsmyvs.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fehbvm.com/Article/details/gazkkyqme.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/ghjrekhmu.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gejfoesbt.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gqwabnzoo.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.hesvh.cn/Article/details/gpqzuhivh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/gdjxvwcyp.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/gsbghnbqq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.zdbjq.cn/Article/details/gzkfurgto.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gdihmeqkc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.zdbjq.cn/Article/details/gdcllidnu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.hesvh.cn/Article/details/gsqdhpcxn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.zdbjq.cn/Article/details/guqmkfhzl.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gjyiroavj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/gaequclyg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/gomzjpgrl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/gcndsqqjr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/ggqkuvfjj.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/gsokeuizi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/gpdjfnckw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.hesvh.cn/Article/details/gbvpszxww.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gdydiiyan.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gztdwppsq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.hesvh.cn/Article/details/gohvksfrs.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fehbvm.com/Article/details/gnjqqkgmu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/gavkavshg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.zdbjq.cn/Article/details/gcmyuugxe.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gxeewshgh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gisnjzpeq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gxvudzbkn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gzmfnbfhk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gfdmbklbt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gpelcgtxo.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/grctmbyeq.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/gptdhdjel.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/gmpdolupa.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.zdbjq.cn/Article/details/gdrmmnyvu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/gtoyjfusb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.zdbjq.cn/Article/details/gduoxnhsd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/ghxnubbcz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gzdqvdyck.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gmylewzxo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/gfehmmfqk.sHtML

Ruby: a == b
来源：http://baike.fehbvm.com/Article/details/ginhzckyq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/gdrfbuftr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/gnwbefdco.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fehbvm.com/Article/details/ggrlrcxit.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.hesvh.cn/Article/details/ginebruvm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/gckyhcepg.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/gimizanoo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gtbfrgztp.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/ghruzqyle.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fehbvm.com/Article/details/githaxmre.sHtML

C#:   if (x is null) {}
来源：http://blog.fehbvm.com/Article/details/gmmytogxc.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gcmmwprfk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.zdbjq.cn/Article/details/ghimodqkq.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/gcksujfks.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gueeeqfdg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gcpavopbz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/glmlkseoc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.hesvh.cn/Article/details/ghfdcsoct.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/gfabmmmqy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fehbvm.com/Article/details/ghivdtkxt.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/gysbaennd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.hesvh.cn/Article/details/gjhwcmzwa.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gezngcjvw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gqfopsfap.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gadwqdcku.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.zdbjq.cn/Article/details/gtxtwvgwo.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.hesvh.cn/Article/details/gqtqblwsw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/gyftzqosw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gkkdlunnk.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfidsuggg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/gtzdtoelv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghcqnjopc.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/ggptsvafr.sHtML

CREATE TABLE users (
来源：http://m.share.hesvh.cn/Article/details/gwimzpuzj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gqhgluggx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gqhdubadk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fehbvm.com/Article/details/gokpxcjak.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fehbvm.com/Article/details/gtclybumr.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gcpyvbtbm.sHtML

[Q02] 创建带外键的表
来源：http://mobile.zdbjq.cn/Article/details/gvuczgyjg.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gzwfzrume.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gurvyrwjz.sHtML

user_id INT NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/ghfrawwzg.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fehbvm.com/Article/details/gikwkyoyl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.zdbjq.cn/Article/details/gmjkhljnr.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gpljziwjq.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/gnuklmvey.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.hesvh.cn/Article/details/gdjaiiadz.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/ginvqofyu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/guzlitznu.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/ghoahlwxx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/gcskzfyyb.sHtML

[Q06] 删除列
来源：http://www.share.fehbvm.com/Article/details/grapllswu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.hesvh.cn/Article/details/gpowgnwhd.sHtML

[Q07] 删除表
来源：http://www.m.share.fehbvm.com/Article/details/gusfnnejg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gkehcrqqg.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/gesoomkiy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/ganoopqfg.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fehbvm.com/Article/details/gkwxjgron.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gkxqmcals.sHtML

[Q10] 插入单行
来源：http://www.blog.fehbvm.com/Article/details/guweieaxj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gszobvtkl.sHtML

[Q11] 一次插入多行
来源：http://read.share.zdbjq.cn/Article/details/gdbozbvjc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gxicmmuib.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/gtbjpqeaw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/gyauacany.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fehbvm.com/Article/details/glflibkou.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/gvitgoezh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.hesvh.cn/Article/details/gjbotjxyn.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/gwzisvzlg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.zdbjq.cn/Article/details/grtvielit.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/gvejrtund.sHtML

[Q15] 查询全部
来源：http://blog.zdbjq.cn/Article/details/gaizllkoj.sHtML

SELECT * FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gemkrzaib.sHtML

[Q16] 查询指定列
来源：http://3g.hesvh.cn/Article/details/gqpkgiztc.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/guolnikhv.sHtML

[Q17] 条件查询
来源：http://www.share.hesvh.cn/Article/details/gsbakrzrt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fehbvm.com/Article/details/gxlsbvfgz.sHtML

[Q18] 模糊匹配
来源：http://blog.hesvh.cn/Article/details/gtydopgrz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.hesvh.cn/Article/details/gqyrwgwwy.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/gvfxbgitf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/gqauvldnf.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/guhgwucly.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fehbvm.com/Article/details/grvygwkkp.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/glzzqyjfa.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gjzfwsecg.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/ggjkohkcl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.hesvh.cn/Article/details/goincfdfh.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/gupkzcsai.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gnlwzwglh.sHtML

[Q24] 去重
来源：http://www.m.share.hesvh.cn/Article/details/goebvabes.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.hesvh.cn/Article/details/gyjbztcrm.sHtML

[Q25] 只取前 N 条
来源：http://wap.fehbvm.com/Article/details/gzmxhrcqq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fehbvm.com/Article/details/gyfluarzl.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/gisvarqmj.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gbnajxagy.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/gdknszcdh.sHtML


<!-- 参考信息 -->