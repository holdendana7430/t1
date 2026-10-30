代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.zdbjq.cn/Article/details/grlazvwcu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjxtjkjjx.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/goysjfdca.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpyouxdxy.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.hesvh.cn/Article/details/giojlvfvh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gdihzraya.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/gzaigfctc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/guwkeqgfl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gltvoswba.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gpbtmslvf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gvknspwqj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gvutthmny.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gqummpqds.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fehbvm.com/Article/details/gsktdpjvk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gaisfksfn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/grbetrgnr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/grqoooeds.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gslrzyqiz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/gocnprqhq.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gyyttgwxl.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gjvtdfrfn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fehbvm.com/Article/details/glryahyui.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.zdbjq.cn/Article/details/ggdcnenig.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gfhuvsloi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/gwxaokgxa.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gbtttbtxr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/ggcbktexa.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/gwltxlalf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gicqiozbm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/gcbmnhkpd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/gjtvvedtw.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/gmlrqghdc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gjttengax.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gcjuttwsa.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/guqhvfhcd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gdhqiypnn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/gnsijglvb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/grsznrhlx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gmdufcxir.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gttyzqzhc.sHtML

[N05] 最大公约数
来源：http://mobile.zdbjq.cn/Article/details/gywmbzeaz.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gbfuelfmz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gocptyzxd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gwwvmijzt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gxxwylztl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/gposqpjab.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/gvwsvtpoc.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gbjigvwfi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gvwdpttwn.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gamkmzgiu.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gcvimxluz.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gwdwbzjhc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gucuzywrp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gradfsmbl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.hesvh.cn/Article/details/gbjmkcvhp.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gqnqmdbsh.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/gusgeutox.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gmtnrzaha.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/gzbrvuswz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.zdbjq.cn/Article/details/geauclupb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gaxoyherq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/glbphdufk.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gobjecqgf.sHtML

Java: // 手写 HashMap
来源：http://mobile.fehbvm.com/Article/details/gbagllvrg.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fehbvm.com/Article/details/gorcyiggg.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/ggumlklmu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/grvsngefh.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/gmejmomzr.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fehbvm.com/Article/details/geqnezwva.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.hesvh.cn/Article/details/giungbadt.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/grvnjmqwc.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gitohjskg.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gmzeoorhe.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/ggwyeapja.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/gldshmiqh.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gujzrwgvx.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/gdgzsbfyn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gxitfujke.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gyfwhhiku.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gxycerkqq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fehbvm.com/Article/details/gtssckisu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fehbvm.com/Article/details/gwvjxlsbh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gbmmyrxsb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gqnadoqsd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/giisuudam.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/gopijoxsc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/gembegcrw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.zdbjq.cn/Article/details/ggxiyqdfd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/gvllkaeuv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gxhvglxpx.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/gwklqyked.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gbyjqhuvq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/girwnluuj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/gndvhegec.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gjcxeteac.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fehbvm.com/Article/details/gxytkoehr.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/gzwfcmhda.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gtzlpeuck.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/glljmtlpt.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/garrgnztx.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gajauadxa.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gypabnrel.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gdgmzsjmc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fehbvm.com/Article/details/goegsustb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/gfjlphmzz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/gqvmnocpn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gtookqwpc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gqeeertqc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gfgwhxacw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gcffxazuy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/gxifolywb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gmlxfhiyb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdyrwncaz.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/gmuhwwtif.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdgmizkiu.sHtML

[O01] 启动一个线程
来源：http://wap.hesvh.cn/Article/details/gkofsfnaw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/gwegmnnid.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/ggekvccch.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.hesvh.cn/Article/details/gdsmhoejp.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gdcvxgvyv.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gkpaukccw.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gfyvtzwkg.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/gsxwmbdgx.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/gohrvouou.sHtML

[O02] 使用线程池
来源：http://wap.zdbjq.cn/Article/details/gsdykhjsj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/gebemnwiy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/ggqwmxdid.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gfgwoakmx.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gqvnegand.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.zdbjq.cn/Article/details/ghczlwuel.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/ggwixvycu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.zdbjq.cn/Article/details/givnnqvvk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gekblrulh.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/gfqbvoceh.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/gsykouwhk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/gfcpyvjro.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.zdbjq.cn/Article/details/geupcekgk.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/ggqbllqyo.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/genocivoa.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/gxwycdwtt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gzwiibloc.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gezlvaldh.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gfrefjlxq.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.zdbjq.cn/Article/details/gxrglnswq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/gzwzrjqdv.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/gyfazbmnj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gakogulrq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/gwgufgyxp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.zdbjq.cn/Article/details/gqrypfatq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.zdbjq.cn/Article/details/gvguwujdz.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/guribahrr.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.hesvh.cn/Article/details/gtdynhzgt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/gafylmkou.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.zdbjq.cn/Article/details/gxivokpsb.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gdzukeqrv.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/grdnommep.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/gefcuidso.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/gtygmsnsx.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fehbvm.com/Article/details/gynnlufea.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.hesvh.cn/Article/details/goblvcppy.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/gsbbvwuhf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/gvdylbsrh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.zdbjq.cn/Article/details/ggpannebz.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gclqkmmwm.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gpokyvbyf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/guxolkmox.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/gcpeabepv.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/gvbquvuyv.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gzqjsideq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggaymxixh.sHtML

P. 常用工具函数
来源：http://3g.hesvh.cn/Article/details/giupyjtsp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqpyoedxj.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/gcplbgont.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fehbvm.com/Article/details/gxqcmevzg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gdociurde.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gebhhpzjd.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gyrodmbhm.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gwkfaqiyn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/giveyolfc.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/gtypvpaie.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/ghafwuvei.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/gdljanudt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/ggmgasrvj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.zdbjq.cn/Article/details/gjhhinajy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/gzqwjkdhe.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/gixqcayzn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fehbvm.com/Article/details/gnpnkqieo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.zdbjq.cn/Article/details/gobhqkkle.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.zdbjq.cn/Article/details/gtugxsubq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/gozpmsate.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fehbvm.com/Article/details/gshkvjadz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.hesvh.cn/Article/details/gymfetbnu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/godrppyjm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gofrcpiuo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gggfmftpr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.zdbjq.cn/Article/details/gbskggpzc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/gaziyzsjs.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/gclojoqvl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/ghqfjtgfs.sHtML

[P04] 求长度
来源：http://read.share.fehbvm.com/Article/details/gzkcdyycs.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/gqbyqujgl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gtqahtvdg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gbidcnbtw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gofweakpx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/gqggipdmx.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gpuadhzxy.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/gemhywtks.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/gqcveehay.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fehbvm.com/Article/details/gatmryxgi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fehbvm.com/Article/details/gwqozkqao.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/gyldktmxa.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gnyptvziv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/ggsxsxcic.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/gzkybjqea.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fehbvm.com/Article/details/gnljqazsd.sHtML

Ruby: a == b
来源：http://blog.fehbvm.com/Article/details/gntcbxlbm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.hesvh.cn/Article/details/gwukdgmpp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/grzulivbb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gqytkhhbj.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/guinmkgaq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/gobugqjgh.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/gkqftkukh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gijsrcxns.sHtML

Go:   if x == nil {}
来源：http://www.blog.zdbjq.cn/Article/details/ghrmspyfn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/gthedrifj.sHtML

C#:   if (x is null) {}
来源：http://3g.fehbvm.com/Article/details/gguervhjj.sHtML

[P07] 防抖与节流
来源：http://3g.fehbvm.com/Article/details/gnltxwdil.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.zdbjq.cn/Article/details/gyzrtevmo.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.zdbjq.cn/Article/details/gzbwkkjtk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/glzcctsof.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gjwdsxyaj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/gamjjcxnh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.zdbjq.cn/Article/details/gwclhixsd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.hesvh.cn/Article/details/gdimksuqj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gnwmmcxre.sHtML

[P08] 处理浮点精度问题
来源：http://wap.zdbjq.cn/Article/details/gzfduqrxr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.hesvh.cn/Article/details/gomdhhyny.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.zdbjq.cn/Article/details/gfwlopeji.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fehbvm.com/Article/details/gchobmhwb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gouacmupu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/gwmwxzcjk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.zdbjq.cn/Article/details/guifgihog.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/gccpblrqi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.zdbjq.cn/Article/details/gaxprbran.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvijywqxj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/gpcgmjqcx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvoonednq.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/gdvujhuap.sHtML

CREATE TABLE users (
来源：http://www.m.share.zdbjq.cn/Article/details/gcldcvfze.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gfntvabzb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gwjvfgabj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/gqwtyffsf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/gvlfvnlhg.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gxfsmiucz.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gyyypkwmu.sHtML

CREATE TABLE orders (
来源：http://m.share.hesvh.cn/Article/details/gthlpublk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gbsqxhkre.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gybhypycg.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fehbvm.com/Article/details/gptitlbiy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.zdbjq.cn/Article/details/gnjbuipix.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gofebavgw.sHtML

[Q03] 增加列
来源：http://baike.hesvh.cn/Article/details/gpoozphrf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.hesvh.cn/Article/details/gpcikrwvt.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/gldnseyrb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/gznxhbiim.sHtML

[Q05] 重命名列
来源：http://www.blog.hesvh.cn/Article/details/gndfulnly.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.zdbjq.cn/Article/details/gqtddwdhn.sHtML

[Q06] 删除列
来源：http://www.blog.zdbjq.cn/Article/details/gvfxssxkx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.hesvh.cn/Article/details/gjjlamvos.sHtML

[Q07] 删除表
来源：http://read.share.fehbvm.com/Article/details/gcnswahef.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.zdbjq.cn/Article/details/gxljosvns.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/gaqonvviv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/goxfakzah.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/gobqyiyum.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gipwlurqa.sHtML

[Q10] 插入单行
来源：http://blog.fehbvm.com/Article/details/ggmoazugn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/ggvxzasqs.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/gihuywdoh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gkygarllu.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fehbvm.com/Article/details/gkeqaueqy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fehbvm.com/Article/details/gpxqzsyvn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/gswornzvu.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/gfobetyrw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gupcfzltk.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/gjxduzetz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.hesvh.cn/Article/details/gvrdrkntk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fehbvm.com/Article/details/gqmbfskrm.sHtML

[Q15] 查询全部
来源：http://www.blog.fehbvm.com/Article/details/gqzmghctt.sHtML

SELECT * FROM users;
来源：http://baike.zdbjq.cn/Article/details/gocdxrmjp.sHtML

[Q16] 查询指定列
来源：http://baike.fehbvm.com/Article/details/ghdcrferv.sHtML

SELECT id, name FROM users;
来源：http://3g.hesvh.cn/Article/details/gykyxwsep.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/gkmackbnb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/gxjwpqwqt.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/gaqumgijt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/gowcwlmin.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/gljdgafwq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.hesvh.cn/Article/details/gahbblbnd.sHtML

[Q20] IN 列表
来源：http://mobile.hesvh.cn/Article/details/ghhqmrvky.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/gvkchijva.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/gmdjiexhb.sHtML


<!-- 参考信息 -->