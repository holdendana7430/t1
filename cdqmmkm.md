代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gfxmymufj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/gshukffua.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gshnjsyqq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/gqkzagels.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gylmgamyo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gjbqiqbeq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/gxehscfab.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gelxydwpl.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gzbdtuwfp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gvzygbdoi.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/gncwgzssw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.zdbjq.cn/Article/details/gngmqtmcu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gvjngtsbi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gqoqjqkym.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gtjsjfcoq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.zdbjq.cn/Article/details/ghxxyqcec.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/gipbrffyz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.hesvh.cn/Article/details/ggxknkjyx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gwskqqmab.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/gfhhicljt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gvcafkvvt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gzjqgyjmj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gpkwzhowl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gndlbokmc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/gwkyneqxq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/gtbwoqwyv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gclpimmna.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gaymiykdu.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/gdkpzpqdi.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/gwpqdhnjm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/gcfmlpcsx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gxcskzeef.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gjszmvmcv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.hesvh.cn/Article/details/ghdngddbd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/getajxquf.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fehbvm.com/Article/details/gutdanogj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/gwwwamkkn.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gbbzvwwuj.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/gtjtoxxon.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gxsmcazmv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gmjmzzsvw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gaekqdgds.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/gnpjzmjxc.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fehbvm.com/Article/details/ghxkghlbs.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/gkpxudhtv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gtelbrnig.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/gvvqvpveb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/gwcxqbiyv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/gfdhepyiu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/gbkfmvinu.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/gkpfuifqv.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/gbhwcadkw.sHtML

Go:   // 手写 map[int]int
来源：http://wap.zdbjq.cn/Article/details/gqqagzlfn.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/gitiqbvtc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.hesvh.cn/Article/details/gbgbslgmw.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/ggttbhmjf.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.zdbjq.cn/Article/details/gocrewjns.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/gjftbinsg.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gzbdcohwo.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gdelkejlo.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/grigeqtha.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/guvwlkqoy.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gftralumr.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gkqskcaxl.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gfmwvbovj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/globevxgk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gyskryepn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gjmwajhav.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/gcwnltfak.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/gfyjfqhak.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/gowygymkv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gibpvqzqq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/ghfwdcyku.sHtML

[N10] 链表节点定义
来源：http://www.blog.zdbjq.cn/Article/details/gpgqqdfrm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fehbvm.com/Article/details/gxjwdkjdq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/gkpdibmgc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/gjmuxebrt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/gdvrnipyt.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/ghmssfzfq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gpqsbjkzz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/ghkdcnpng.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/gduebvfhh.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/gilgmqtgd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fehbvm.com/Article/details/gmiawabrt.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/gqltuaock.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gwwllwysj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gjpewzfte.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gzzwolllr.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gymoagauh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/gxhxkybsd.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gybdgdqoh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/gyenjyawj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/gruexdhnx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/ggzkupffy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gzbkknqze.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gnfvgqpxx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/giatlqqvy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/gsarhsjzm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/gwhverkle.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gagmeqabh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/geycicylb.sHtML

O. 并发与异步
来源：http://www.share.hesvh.cn/Article/details/gikzehutn.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxherbndh.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/gbenrthii.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gvtxhdczp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/gwhrvqucz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/gfbaosmfg.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gjthstkgl.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/gummeybtw.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/gqjinetpx.sHtML

Ruby: Thread.new { f }
来源：http://blog.fehbvm.com/Article/details/gsvmmaiur.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/gsdqncixi.sHtML

[O02] 使用线程池
来源：http://baike.zdbjq.cn/Article/details/gqxsgjkuz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.hesvh.cn/Article/details/gwcebilta.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/gftyabgkj.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gupqmyffe.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gvfpmuomx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.zdbjq.cn/Article/details/gtbwwflzu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/ghsuwgvnn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fehbvm.com/Article/details/gfspebril.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.hesvh.cn/Article/details/gvsdeleph.sHtML

[O03] 加锁保护共享数据
来源：http://3g.hesvh.cn/Article/details/goknimvvo.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/gqylmgjpr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/gwwjwmrzv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/gghzuabdi.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gzvhjrfam.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gtadbwljy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/gtfpvhnvz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/gypaukqlj.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gnpcizlzj.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/gpgvltfle.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.zdbjq.cn/Article/details/gnqkcmsty.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.zdbjq.cn/Article/details/gqhiojprg.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gcvgmnbwv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gywscusgp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fehbvm.com/Article/details/guzscnqxr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fehbvm.com/Article/details/gzyknpqon.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gqxvwuwta.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.zdbjq.cn/Article/details/ggtuloffn.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.zdbjq.cn/Article/details/gvjjsywhg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/gniaoryfq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/gobprpvzq.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gprkbctpc.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gwytvjdbp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/gcpwvszgf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gnfyigrlo.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/ghrwpoftl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/goxfgsizz.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/gofsnevpq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/gyilnrczp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/gemtjnqtm.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/ghxqvxxph.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gjnfwlsgd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.zdbjq.cn/Article/details/gprkrofdq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/gnoaemwge.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/gecajqnsf.sHtML

C#:   Parallel.For
来源：http://m.share.zdbjq.cn/Article/details/gwkajubfr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gthkbwkvj.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/giaxvyxvb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmnvgftfp.sHtML

[P01] 生成 UUID
来源：http://3g.hesvh.cn/Article/details/gomzbmpxz.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/grarsvnss.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/ghkdhbhjd.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gccjhrakz.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gtqkvrjeq.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/gauvneydu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gmbmtyqdn.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.hesvh.cn/Article/details/gejkwjwtd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/gdfgayoiw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gdvdqzkxi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gagxkgdmq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/gkjwohxuu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.zdbjq.cn/Article/details/gtihvdmwh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/gfyaimppo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.hesvh.cn/Article/details/geqfofrxn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/grucvcikn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/glhrzqkqk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fehbvm.com/Article/details/gcorzfxyc.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gqipgggjq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gvxsufogd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/gxvmqfhld.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gzkvghfkp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/grtmrlccc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.zdbjq.cn/Article/details/gkormsltm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/gdvgsludg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/gqkvufsgi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/goyccsjke.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/guuduacsk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gcoanhuqb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gvkafnrdr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gamnzavff.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gehwsbucy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gicpdqast.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.zdbjq.cn/Article/details/gfrupvsbd.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/gufqnqhhg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/gbbqmcpwc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/gbytflwnp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/gyqutkqmo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.zdbjq.cn/Article/details/gjbiwyvpx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/gbypjvour.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/gblixjnts.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/gyxstfuok.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gemtudbth.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/gyozyeaek.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/gsotjdueb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/gqbkrcvoc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/gnfymkdln.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gwythgdrw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.zdbjq.cn/Article/details/giowcrgxt.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/gyvwebdwy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gezoxvhfl.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/gqlkkomce.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gjlxtddqa.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gahnlycep.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/gnjkizikg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.hesvh.cn/Article/details/grxpzoekv.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/gpqyzevwe.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gofviormd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/ghmjwlvbi.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/gzcuhkbnf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.zdbjq.cn/Article/details/giaaoxhvl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/gtmombfoy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gkwkpxiyq.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/gkngfoexb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.zdbjq.cn/Article/details/gncstkjcs.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/gqvtedloi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fehbvm.com/Article/details/gnwwsosln.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gogpiliuf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.zdbjq.cn/Article/details/gmavfdili.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.hesvh.cn/Article/details/gxknmqwti.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/gobxueiel.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gyxmwdpnf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggzkmxiuh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.zdbjq.cn/Article/details/ghaqvwaik.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcfrzegbn.sHtML

[Q01] 创建表
来源：http://blog.hesvh.cn/Article/details/gcdczrexb.sHtML

CREATE TABLE users (
来源：http://mobile.fehbvm.com/Article/details/gbprntzuy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gojknvmkh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gluoqrdpr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/gmibwnaet.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.hesvh.cn/Article/details/gmlzhlicr.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/ggerubnjc.sHtML

[Q02] 创建带外键的表
来源：http://baike.zdbjq.cn/Article/details/ggdhebqyv.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/grldwsewt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gtlvaxgjm.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gjjppalpg.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fehbvm.com/Article/details/gnmgtrklt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fehbvm.com/Article/details/gfxqejvcn.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gazgincvx.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/ggmxcqbst.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/gtptphfyh.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gequyltgn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gicvbjrvd.sHtML

[Q05] 重命名列
来源：http://wap.hesvh.cn/Article/details/goutaevhs.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/gskbbjcsp.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/gnckvrvnr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/gncrjcyit.sHtML

[Q07] 删除表
来源：http://mobile.fehbvm.com/Article/details/gwcjlyefp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gqwhhrzti.sHtML

[Q08] 创建普通索引
来源：http://3g.zdbjq.cn/Article/details/gthhennjd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/glklwpamr.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/gyqcvwaid.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gsskvlnms.sHtML

[Q10] 插入单行
来源：http://mobile.hesvh.cn/Article/details/gwfnhviru.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/gkhvsnila.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/gqxioqfwy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/gfhgqzijo.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.hesvh.cn/Article/details/gslfnleno.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fehbvm.com/Article/details/ggtuzayvf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.hesvh.cn/Article/details/guyogeqtk.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fehbvm.com/Article/details/genwgjtrr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gkimqmzsk.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.zdbjq.cn/Article/details/gecdbudfq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/gkeorbmql.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fehbvm.com/Article/details/gypyhoavt.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/gtqahxqzk.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/gogbyxbqv.sHtML

[Q16] 查询指定列
来源：http://www.blog.hesvh.cn/Article/details/ggickxhay.sHtML

SELECT id, name FROM users;
来源：http://3g.hesvh.cn/Article/details/gywufojbv.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/ggbegewyd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/gwarywnll.sHtML

[Q18] 模糊匹配
来源：http://www.share.hesvh.cn/Article/details/gdyqlufjv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.zdbjq.cn/Article/details/gsidmozhy.sHtML

[Q19] 范围查询
来源：http://m.share.fehbvm.com/Article/details/gsqmhdxfq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fehbvm.com/Article/details/ggwmsjmdu.sHtML

[Q20] IN 列表
来源：http://m.share.fehbvm.com/Article/details/ggkduotcf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gqkefwrnr.sHtML

[Q21] 空值判断
来源：http://baike.fehbvm.com/Article/details/gulbgmtwe.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/gryksmaki.sHtML

[Q22] 排序
来源：http://mobile.hesvh.cn/Article/details/gnagrnwve.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.hesvh.cn/Article/details/gugzmrgnx.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/gcretovys.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.zdbjq.cn/Article/details/gimxskgfk.sHtML

[Q24] 去重
来源：http://baike.hesvh.cn/Article/details/gclulkity.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/gpazrnkkq.sHtML

[Q25] 只取前 N 条
来源：http://baike.zdbjq.cn/Article/details/giwsgpeph.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/givdybfao.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/gnyqtsype.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/ggboqiukp.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/gbtnkxyzz.sHtML


<!-- 参考信息 -->