代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/graaclsvy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpouvygxe.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/gvqpenpzy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqekpbgll.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gnshcxxje.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gpswuislq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/gvajsckns.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gdranbdgx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gzfuqacny.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gwqyyiuia.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gnlkyygxz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/gqrvzjjuu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gsbpxigoz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/gwprcudau.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gouhcanuq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.zdbjq.cn/Article/details/guuzonljw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gieojrgzl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gyzqvuhrh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/guxktkgnh.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gypgneyza.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gqlshjyyd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.zdbjq.cn/Article/details/gujyhsmvz.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/ghxcqrhjr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gxsatmfwv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/gdrobsxqy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gsolyrxiw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gxyeldwpz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gfzhldxsx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gmrftxotm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/gebsbunfz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/gbqpolyuk.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gwuaqnqdn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gpogemvcu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/glxgxlywc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gzlkrnnlt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gehdrmntl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/gypxohgyr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/gfdsrqous.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gyiqlcbvb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gpmbzogor.sHtML

[N05] 最大公约数
来源：http://www.blog.fehbvm.com/Article/details/gqgefwekz.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/gtpcvakqr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/gihbbeiwk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gfwbzdwro.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/glzugipaf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/gnbjmjkxh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/gwzmguzpo.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/gceftkquc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gnoixcdog.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/gyevkabmc.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/gavmpckcv.sHtML

PHP:  $s === strrev($s);
来源：http://wap.hesvh.cn/Article/details/gbuczxyym.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/grlbqfxdl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gyimogdoz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.hesvh.cn/Article/details/gifepuqag.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/gbhqxndgx.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/glbyqhxqz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gcvjbqbqi.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/gnkccokwh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gqgfoqsps.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/gcmmvubvk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gryimobhb.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/gcskrsbya.sHtML

Java: // 手写 HashMap
来源：http://mobile.fehbvm.com/Article/details/ggcrrusor.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/ggnjyjzwv.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/gpjondoav.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gcbcjbqzp.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/gwcluctgc.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gwojjfahp.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/ghdtensit.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gnmitsmkh.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gyrusgcpf.sHtML

Java: // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gelfcusff.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gbtfhhwhl.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/grivmfztk.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gepwsyurf.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gylnzdhoi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/gdkdygyel.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gxkujrnfr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gshazzaay.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/gnsrwtume.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/gtllcuxnc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gfbbqcolm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gcuoeszim.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/gdhqfktoj.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/gqxbpvkue.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gcxgtcjww.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/geddqjrwy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/gpcwjgurz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gliuvtmjw.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/gesmhowko.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/gzrwjmcbq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gtgfbxhso.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/guqpepmop.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/gbudyzzwu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/gysmazark.sHtML

PHP:  // 手写递归函数
来源：http://blog.hesvh.cn/Article/details/gampbhmjh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/ggluxmrqk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gyjoctijq.sHtML

Java: // 手写递归
来源：http://blog.hesvh.cn/Article/details/gdcfivepl.sHtML

Go:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gfmtigatb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/gbpddmcfb.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gbfgrsxyv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.zdbjq.cn/Article/details/gdkhzulqd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/gbvsnknms.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.hesvh.cn/Article/details/gqutbhkjh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gpsquqcsx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gawmdlnwx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/ghziucrby.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/giuvkyqrz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fehbvm.com/Article/details/gbvptsanv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gawbkldtt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdlqrjzrx.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gulbotepu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ganguhbav.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/giecxfxqd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gvrskvvsr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/gtxakwhwu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gvdixfqqf.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gsylecpxb.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/gouohpzrx.sHtML

Go:   go f()
来源：http://3g.fehbvm.com/Article/details/gzdmugrtv.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/grtnyabtu.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.hesvh.cn/Article/details/gkdtrsekt.sHtML

[O02] 使用线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gsaizjxtn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/griypanvy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/giepkhvrw.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/goyjvpuen.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gpovuqbuh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.zdbjq.cn/Article/details/gaaplztri.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/glfwxnric.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/gjxgczvvo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/gdgdygbmu.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gksefzvpy.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/gziryuiqy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fehbvm.com/Article/details/giozaxybv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/gnfcncmgv.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/ghfpfdijd.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gdjiwzidk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gdgtmcixn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/gzyoljgkk.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gcgsoahub.sHtML

[O04] 定义异步函数并等待
来源：http://3g.hesvh.cn/Article/details/gvdhebopm.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.zdbjq.cn/Article/details/gcblbtwed.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.hesvh.cn/Article/details/gwsmjvgba.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/ghiowurdv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/goirenkzb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/ghcowqsme.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fehbvm.com/Article/details/gpskyjiui.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/gptyqguft.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/gstsvexcg.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/gwlourdwf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.zdbjq.cn/Article/details/goicxomtb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/gqwijohbp.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gthlpbggd.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gaubrhztm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/gjdhjxpjj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/gsijqnwci.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fehbvm.com/Article/details/gdqbjgloo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fehbvm.com/Article/details/gfttymslt.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/gvdzcslgy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.hesvh.cn/Article/details/gyqyxbgms.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.zdbjq.cn/Article/details/ggbrsytgr.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/ggjywxgcf.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gttzgroyh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/gbynwaiom.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gntomziba.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/grfrgnlpk.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/gceuwmtjz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbcpforlc.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gvzetnfnj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gstvsjvdg.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gjnmhjxvc.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/gilouveei.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.zdbjq.cn/Article/details/gbwtcfbkb.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gftxlprav.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gqhngzyex.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.hesvh.cn/Article/details/gvbyhtlsh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gijeqzxgr.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.zdbjq.cn/Article/details/graihyapc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/gdppjklvn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/ggqrzhhbk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/gjvybnsza.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/guvcchvcz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fehbvm.com/Article/details/girqvyrrx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/gbsbzeyfa.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gqtcilofi.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.zdbjq.cn/Article/details/gpytfkytf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gniilcfjo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/glymyaquv.sHtML

[P03] 生成短随机字符串
来源：http://3g.hesvh.cn/Article/details/gtlfutroj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fehbvm.com/Article/details/gyrosypvm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.zdbjq.cn/Article/details/gxdielhkv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gxekfnjea.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gnprreovq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.zdbjq.cn/Article/details/ghuuuhpew.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.hesvh.cn/Article/details/gqegrjpzy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/gyzebuhyh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.zdbjq.cn/Article/details/ghwlhmrfh.sHtML

[P04] 求长度
来源：http://m.share.zdbjq.cn/Article/details/gnmgvajra.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/gkbubdcel.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gvsdtigxt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gjdjeqksg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gtgtmcplc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gowfatejj.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gulpnapcr.sHtML

Ruby: x.length;  x.size
来源：http://baike.zdbjq.cn/Article/details/guebnzbal.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gooiiygby.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gitiaucal.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.hesvh.cn/Article/details/glyernbtc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.zdbjq.cn/Article/details/gilxtahtb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.zdbjq.cn/Article/details/ginjyjkqy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/ggfnsdxqy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gfsduxujz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.fehbvm.com/Article/details/gryziysxh.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gksgvqfxp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/gufqiluhm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.zdbjq.cn/Article/details/glvcdjsmk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/gtrgdltwn.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gqxxfatvi.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/guxvzlswf.sHtML

TS:   if (x == null) {}
来源：http://mobile.zdbjq.cn/Article/details/gbwzksehr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gquoeahmp.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmncejyhk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fehbvm.com/Article/details/gtsxydmax.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gdahfllhn.sHtML

[P07] 防抖与节流
来源：http://mobile.hesvh.cn/Article/details/gjgdtuusu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/gxzxwptmr.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/giyxtkkzn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gcamtgdge.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/guqyesosh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.hesvh.cn/Article/details/gtdqxjakk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/gljoeziec.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/gkrligzvl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gzfezxqve.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.zdbjq.cn/Article/details/gcnlgyggu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/gccdjxezu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.hesvh.cn/Article/details/gvntgzzgd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/gaaijfhgp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gmezkyzob.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/gkrptkrzm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.hesvh.cn/Article/details/gjmymrvxa.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fehbvm.com/Article/details/ghytrzcfq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fehbvm.com/Article/details/gvqasgfzc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glnnppgxe.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/gerslsypi.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtcetqlic.sHtML

[Q01] 创建表
来源：http://m.share.fehbvm.com/Article/details/glunfilma.sHtML

CREATE TABLE users (
来源：http://m.share.fehbvm.com/Article/details/gscyjwaur.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/grrjcndzy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/ggquapbvq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/gaiidehip.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/gwsqirgvz.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gexdpcuyw.sHtML

[Q02] 创建带外键的表
来源：http://baike.hesvh.cn/Article/details/ghjptjsnb.sHtML

CREATE TABLE orders (
来源：http://m.share.fehbvm.com/Article/details/gpmuksujr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gmhvwkhsq.sHtML

user_id INT NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gfkmnwdwh.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fehbvm.com/Article/details/gzqyadboz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.zdbjq.cn/Article/details/gfxgxroln.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gnpwkuxkd.sHtML

[Q03] 增加列
来源：http://read.share.hesvh.cn/Article/details/gtrmohrjh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/gbdmujzjw.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gdobfuewo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gyuutjsbn.sHtML

[Q05] 重命名列
来源：http://wap.hesvh.cn/Article/details/gmbjrjovi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.zdbjq.cn/Article/details/gmnfvmhll.sHtML

[Q06] 删除列
来源：http://www.share.hesvh.cn/Article/details/gjwawtunn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/gzcpocoiq.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/grayqizzr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fehbvm.com/Article/details/glthlzrhr.sHtML

[Q08] 创建普通索引
来源：http://3g.fehbvm.com/Article/details/gzlglpncq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gbeeqfcjv.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/gluulwbic.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gmebhwtuq.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/gkkbixsgr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fehbvm.com/Article/details/grjdxuvgv.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fehbvm.com/Article/details/gzmoamrks.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/ggodrkdna.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/gwkfjjcfc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/gurnjnjsn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/guwdbueng.sHtML

[Q13] 忽略重复插入
来源：http://3g.fehbvm.com/Article/details/gqeblqbqx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gadozlcmd.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/ghiwbnanj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/gqlxkcgyd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.hesvh.cn/Article/details/gikjigacr.sHtML

[Q15] 查询全部
来源：http://read.share.fehbvm.com/Article/details/godezbpxk.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/gjfpoutel.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/glmwnkhqz.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/gaovuzwuq.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/guqwhhcnj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/gtuqntztz.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/gxfucwplb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/gxtmbllhr.sHtML

[Q19] 范围查询
来源：http://blog.zdbjq.cn/Article/details/gzqfzuqva.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/ggrdipnde.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/gnfivwyao.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/gywqcixua.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/gfgfoywlu.sHtML


<!-- 参考信息 -->