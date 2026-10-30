代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkphsobs.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/gtpomfsur.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmbkuost.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlhjfhjv.sHtML

Ruby: arr.sort
来源：http://blog.fanxiaobao.xyz/Article/details/gihwzlnbc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fanxiaobao.xyz/Article/details/gommisddg.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fanxiaobao.xyz/Article/details/gufkbndym.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fanxiaobao.xyz/Article/details/gyjsgvoel.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcgiyuci.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fanxiaobao.xyz/Article/details/gdztfmpjd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqlxvveo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvpjiure.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlmheuaz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fanxiaobao.xyz/Article/details/gedkieklu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fanxiaobao.xyz/Article/details/gfxdstbpl.sHtML

[N04] 斐波那契数列
来源：http://read.share.fanxiaobao.xyz/Article/details/gpspydhrd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/grgthdbop.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gimzmokgk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsaptxsd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fanxiaobao.xyz/Article/details/ghuwysnur.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gozdqyyjm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fanxiaobao.xyz/Article/details/gmrzmmodk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbxgxemi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gwybcjrqt.sHtML

[N05] 最大公约数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcmyrdeb.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fanxiaobao.xyz/Article/details/givdpfkwr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnggnsvgk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkebmxfkw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjldakmts.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fanxiaobao.xyz/Article/details/geggogaij.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gngidmlnz.sHtML

Ruby: a.gcd(b)
来源：http://baike.fanxiaobao.xyz/Article/details/gxqjxfkgc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fanxiaobao.xyz/Article/details/gmbepniwz.sHtML

[N06] 判断回文字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gkecbjwfy.sHtML

Py:   s == s[::-1]
来源：http://wap.fanxiaobao.xyz/Article/details/gomyozrja.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtopngmrk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqaxlcuu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gpquvtfyo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fanxiaobao.xyz/Article/details/gusehiprr.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyvgsauk.sHtML

Ruby: s == s.reverse
来源：http://read.share.fanxiaobao.xyz/Article/details/gmskpffhb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyusyktz.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fanxiaobao.xyz/Article/details/gzajzyktb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fanxiaobao.xyz/Article/details/ganbgeaiy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fanxiaobao.xyz/Article/details/ggpmjqofu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsavkelxy.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnfmvgzt.sHtML

Java: // 手写 HashMap
来源：http://wap.fanxiaobao.xyz/Article/details/gteanremn.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fanxiaobao.xyz/Article/details/gghhrekml.sHtML

Ruby: // 手写 Hash
来源：http://blog.fanxiaobao.xyz/Article/details/gddixjqfr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fanxiaobao.xyz/Article/details/ghadgrdyn.sHtML

[N08] 生成全排列
来源：http://blog.fanxiaobao.xyz/Article/details/grabynmju.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gaxbzkpfd.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihmmirqv.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gojczyews.sHtML

TS:   // 手写回溯递归
来源：http://baike.fanxiaobao.xyz/Article/details/gocimfdjl.sHtML

Java: // 手写回溯递归
来源：http://read.share.fanxiaobao.xyz/Article/details/grfhwdyka.sHtML

Go:   // 手写回溯递归
来源：http://blog.fanxiaobao.xyz/Article/details/gbyngkwse.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fanxiaobao.xyz/Article/details/grqdommik.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzxxagdg.sHtML

[N09] 栈与队列
来源：http://blog.fanxiaobao.xyz/Article/details/gnllekryf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkoovyqc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fanxiaobao.xyz/Article/details/gzewlzwvo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fanxiaobao.xyz/Article/details/gdjsytyww.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fanxiaobao.xyz/Article/details/gyzfusjaw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfifpsml.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fanxiaobao.xyz/Article/details/gxufdmhej.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fanxiaobao.xyz/Article/details/glcrewelo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkuepfwua.sHtML

[N10] 链表节点定义
来源：http://baike.fanxiaobao.xyz/Article/details/gpgwugzbg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fanxiaobao.xyz/Article/details/gguvvfkpc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjlwmodc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/giewpmnye.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gooypidsd.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkkgjhkrb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fanxiaobao.xyz/Article/details/gejeqqvai.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fanxiaobao.xyz/Article/details/gmxorrpnn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpwatoizp.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhhuuqcd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fanxiaobao.xyz/Article/details/gfscsudaf.sHtML

PHP:  // 手写递归函数
来源：http://wap.fanxiaobao.xyz/Article/details/gnsbtiurb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnxruuqf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbdzgplq.sHtML

Java: // 手写递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gseiihlaq.sHtML

Go:   // 手写递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunderebg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fanxiaobao.xyz/Article/details/gxkwhiqkf.sHtML

C#:   // 手写递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjzopjaj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fanxiaobao.xyz/Article/details/gmpapldxm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmggnxhop.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fanxiaobao.xyz/Article/details/glnqpbetf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fanxiaobao.xyz/Article/details/gzxucfotg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fanxiaobao.xyz/Article/details/gwwolccgk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fanxiaobao.xyz/Article/details/gcnzjwhyc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fanxiaobao.xyz/Article/details/gzqkrwonp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxodynwj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fanxiaobao.xyz/Article/details/gejnplrak.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gxizdjagd.sHtML

O. 并发与异步
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwktiyxd.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gjuyfymmg.sHtML

[O01] 启动一个线程
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhcfuoqu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwnrykiu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fanxiaobao.xyz/Article/details/gtklsiuwo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fanxiaobao.xyz/Article/details/gexhidkvg.sHtML

TS:   // 同 JS
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrywulst.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fanxiaobao.xyz/Article/details/grzgcfaxl.sHtML

Go:   go f()
来源：http://baike.fanxiaobao.xyz/Article/details/guvcgwbst.sHtML

Ruby: Thread.new { f }
来源：http://blog.fanxiaobao.xyz/Article/details/garefdhhl.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcqhlnot.sHtML

[O02] 使用线程池
来源：http://www.share.fanxiaobao.xyz/Article/details/gittmyztt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssypekxa.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fanxiaobao.xyz/Article/details/gimcvpjbs.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fanxiaobao.xyz/Article/details/garwhboky.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fanxiaobao.xyz/Article/details/gouzdoffz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gmwacenfn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcamwmpza.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvudckyx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fanxiaobao.xyz/Article/details/gonbgqklq.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fanxiaobao.xyz/Article/details/gyydesxtf.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gusjcjoas.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fanxiaobao.xyz/Article/details/gvslibhjc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fanxiaobao.xyz/Article/details/gryrzkjdq.sHtML

TS:   // 同 JS
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvzejnwf.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgalwfin.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fanxiaobao.xyz/Article/details/gskbhbxyo.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/gxjexdset.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdgmwkwn.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gfggmiiid.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstoakabu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fanxiaobao.xyz/Article/details/gisemntar.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkknltzc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gdnxehrmp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fanxiaobao.xyz/Article/details/gjaqqujgg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmrhrcbd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fanxiaobao.xyz/Article/details/gvivguquv.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/guqdsyqwv.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdgrrtve.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fanxiaobao.xyz/Article/details/gxbgojskb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavinwibp.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fanxiaobao.xyz/Article/details/gdfqvspxe.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfocqgsjk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fanxiaobao.xyz/Article/details/gcphecwut.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fanxiaobao.xyz/Article/details/gtxjtqqlf.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fanxiaobao.xyz/Article/details/gjwwrxicr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fanxiaobao.xyz/Article/details/giuukuimt.sHtML

[O06] 使用进程池
来源：http://blog.fanxiaobao.xyz/Article/details/gssipcdio.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fanxiaobao.xyz/Article/details/gobseqwvc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsvqwned.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fanxiaobao.xyz/Article/details/gaecongag.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fanxiaobao.xyz/Article/details/glcsugigd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegnpppmn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnhjmntp.sHtML

Ruby: // fork 块
来源：http://baike.fanxiaobao.xyz/Article/details/gtofoputa.sHtML

C#:   Parallel.For
来源：http://3g.fanxiaobao.xyz/Article/details/ghuhedmwd.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gkerltuwy.sHtML

P. 常用工具函数
来源：http://wap.fanxiaobao.xyz/Article/details/gmmqwbcwh.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gjvwamcxe.sHtML

[P01] 生成 UUID
来源：http://mobile.fanxiaobao.xyz/Article/details/govnnrnpw.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fanxiaobao.xyz/Article/details/gwhpvpzog.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbpuhpqa.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/ghksqihhs.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/goppsvdvl.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fanxiaobao.xyz/Article/details/gmhfwczge.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fanxiaobao.xyz/Article/details/gtmlreeje.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fanxiaobao.xyz/Article/details/gfbsuvssy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnvxcvia.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgqitgrv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnyrcsfdw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqehdjnzy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fanxiaobao.xyz/Article/details/gxggfuzgp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabafwdbj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcjwtkbd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgyfwqyx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/grpdtolve.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fanxiaobao.xyz/Article/details/ghbnebrkb.sHtML

[P03] 生成短随机字符串
来源：http://wap.fanxiaobao.xyz/Article/details/ggkaqhihc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fanxiaobao.xyz/Article/details/gqrdyngrh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdiziuynd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gtjzplnuz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhkdbdiq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glokspdvu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fanxiaobao.xyz/Article/details/grvbipoij.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fanxiaobao.xyz/Article/details/gletzbzal.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fanxiaobao.xyz/Article/details/gsrhkhkdw.sHtML

[P04] 求长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gercojqix.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fanxiaobao.xyz/Article/details/gpavwrkwn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fanxiaobao.xyz/Article/details/gdwfwkhze.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fanxiaobao.xyz/Article/details/gayxqlkyn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fanxiaobao.xyz/Article/details/ghegwrwng.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fanxiaobao.xyz/Article/details/gohbfxqif.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbuhmipzn.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fanxiaobao.xyz/Article/details/gkligsfyt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgvjvvzq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fanxiaobao.xyz/Article/details/gxacytlll.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gshxdtyca.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhxymiur.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fanxiaobao.xyz/Article/details/giproohqu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fanxiaobao.xyz/Article/details/gsozmkajb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqnmyusj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fanxiaobao.xyz/Article/details/govpayhbt.sHtML

Ruby: a == b
来源：http://3g.fanxiaobao.xyz/Article/details/gmqassebn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyvjmizs.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpkqessy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwvhkaow.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/godwxkrse.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrgashxp.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsrehsdn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbthucif.sHtML

Go:   if x == nil {}
来源：http://wap.fanxiaobao.xyz/Article/details/gwlgcjmgm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grprrubiv.sHtML

C#:   if (x is null) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbksfsdl.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwxcxviw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fanxiaobao.xyz/Article/details/gvkjdwgte.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fanxiaobao.xyz/Article/details/gzfvqmend.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gnatvvrpu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gydomszea.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafvkluag.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklmfjkag.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fanxiaobao.xyz/Article/details/gkcygvabi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrjrgwle.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpyjcnnf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fanxiaobao.xyz/Article/details/goqpiqvbg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fanxiaobao.xyz/Article/details/grvrzwhec.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqhogjja.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fanxiaobao.xyz/Article/details/gxnwruajz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fanxiaobao.xyz/Article/details/gwznddlmh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fanxiaobao.xyz/Article/details/glalivspa.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxjixwly.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fanxiaobao.xyz/Article/details/gqvggbaee.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmubeznxr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjevcevg.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmfyshsp.sHtML

[Q01] 创建表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpwrazco.sHtML

CREATE TABLE users (
来源：http://blog.fanxiaobao.xyz/Article/details/gaamupmse.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fanxiaobao.xyz/Article/details/gzimlypza.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fanxiaobao.xyz/Article/details/gimtfadol.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fanxiaobao.xyz/Article/details/gczvttglk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfznfddum.sHtML

);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmspjstes.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fanxiaobao.xyz/Article/details/goeszlcad.sHtML

CREATE TABLE orders (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohcaeisw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fanxiaobao.xyz/Article/details/gagahzkxk.sHtML

user_id INT NOT NULL,
来源：http://read.share.fanxiaobao.xyz/Article/details/gypqffjht.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fanxiaobao.xyz/Article/details/gqtulgnkp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fanxiaobao.xyz/Article/details/gexkdxsbi.sHtML

);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsajkvghe.sHtML

[Q03] 增加列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemejjgxv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gmfvrhoaj.sHtML

[Q04] 修改列类型
来源：http://3g.fanxiaobao.xyz/Article/details/grmdtgcpz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fanxiaobao.xyz/Article/details/gygtbmtht.sHtML

[Q05] 重命名列
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbsksxuu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fanxiaobao.xyz/Article/details/gqwghjmnb.sHtML

[Q06] 删除列
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtwkgvqf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpntijrgy.sHtML

[Q07] 删除表
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyufeagu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gmpwmvisi.sHtML

[Q08] 创建普通索引
来源：http://3g.fanxiaobao.xyz/Article/details/gclulcwvw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyvagisz.sHtML

[Q09] 创建唯一索引
来源：http://wap.fanxiaobao.xyz/Article/details/gpgvpcxbt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsalvwoqo.sHtML

[Q10] 插入单行
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginbyponz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gdtmllnhv.sHtML

[Q11] 一次插入多行
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgtooyke.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gwqllcuwl.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grecrfaak.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrwzwaie.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fanxiaobao.xyz/Article/details/gwmrwiial.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fanxiaobao.xyz/Article/details/gfprymeek.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynmbjwcm.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvdxgcxe.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fanxiaobao.xyz/Article/details/gcqgdcfdr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fanxiaobao.xyz/Article/details/gvddlpvhk.sHtML

[Q15] 查询全部
来源：http://m.share.fanxiaobao.xyz/Article/details/girdercic.sHtML

SELECT * FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvdyhidj.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjjpqarz.sHtML

SELECT id, name FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gprhdxvos.sHtML

[Q17] 条件查询
来源：http://wap.fanxiaobao.xyz/Article/details/gdkiomlqx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghibdwsyu.sHtML

[Q18] 模糊匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gdagtqlxu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fanxiaobao.xyz/Article/details/gmegrxefu.sHtML

[Q19] 范围查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfftpmyh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fanxiaobao.xyz/Article/details/gmpusopod.sHtML

[Q20] IN 列表
来源：http://wap.fanxiaobao.xyz/Article/details/gcznoyyri.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmggyuoan.sHtML

[Q21] 空值判断
来源：http://3g.fanxiaobao.xyz/Article/details/gjxuybukj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtddgmwxn.sHtML

[Q22] 排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkrjjsmd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqcweuyx.sHtML

[Q23] 分页
来源：http://3g.fanxiaobao.xyz/Article/details/garqiuiad.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvpvnsmm.sHtML

[Q24] 去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpnqrgfu.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkafxqya.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/goalekrly.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fanxiaobao.xyz/Article/details/gsstoejkx.sHtML

[Q26] 计数
来源：http://m.share.fanxiaobao.xyz/Article/details/grunznbse.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gprkirknq.sHtML

[Q27] 条件计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkeusuupm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywktukjs.sHtML

[Q28] 求和与平均
来源：http://blog.fanxiaobao.xyz/Article/details/grrjyvdtl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gawzbufoe.sHtML

[Q29] 最大最小值
来源：http://wap.fanxiaobao.xyz/Article/details/ghpojkcjt.sHtML


<!-- 参考信息 -->