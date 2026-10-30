代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gutiorbje.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/ggblgxvpu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/ggralswah.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.zdbjq.cn/Article/details/gqlhlvnsz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gmmnzefhc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/gviiztady.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gyyxpknhl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/gaguhdchn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gzmyerghi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gkpfusfyn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fehbvm.com/Article/details/gmcmfgtcw.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gbzmqicyl.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/ggrhentni.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/goyudjuyh.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/gwqeuahws.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.hesvh.cn/Article/details/ggtemypsp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/gkbxchdsp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gbasdajcg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gbpvelhxw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/gzarersbd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.hesvh.cn/Article/details/gxbvuvfvt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/gbbvzgzkx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.hesvh.cn/Article/details/gajpjyxfy.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/gcjctflqp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gadtromkl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/ggzlvnxei.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gslpauykm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/glvvnxyys.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gpdhfslln.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/gmralpogm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gxwlcrkbf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gexqbwoyq.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/gslhbieoe.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gympliczi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gebxzrrkg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/glcwosbbo.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gineghllb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gfutzvhih.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/gzaaozbjd.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gxdarurjv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/gtbmyqvpu.sHtML

[N06] 判断回文字符串
来源：http://www.share.zdbjq.cn/Article/details/ggsednuma.sHtML

Py:   s == s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gpbcsftwm.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/geqqrmcaf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/glacgkbjt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gypwrpxkd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/grcxvllnj.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/gntczeowe.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gydwieroi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gqwltlctr.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gaynsskzf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/gbaropceu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fehbvm.com/Article/details/gofzxbhjv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/ggruvbunn.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.zdbjq.cn/Article/details/gwaadlzrc.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/gnpinfeku.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/gdiezgdcl.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gheyybgzj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/gapqgphgf.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/grztokmlt.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.zdbjq.cn/Article/details/gewglmxuv.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.hesvh.cn/Article/details/golkdrnjp.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/graqkvinn.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gfgttnray.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gryrxbqga.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gfvvkzszk.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gmjfzuyqk.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gkfhjtwzf.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gwimfonts.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/geiahekbb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gjoxookzq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gwhuphkwx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/gyelzglwg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.hesvh.cn/Article/details/gvifdatwk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gplpqkieh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gaimnfrjz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/grzqovwpl.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/geaemrlcy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/gldxqyryq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gyiqhtycf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/gbnkufudy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.hesvh.cn/Article/details/gaypuxcvb.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gvczhljqz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fehbvm.com/Article/details/ggfpumduk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/godcmreva.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/gqbhbfmxu.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/gvjgxzzyf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gwexrkmvx.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/gjxbieidu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gnfyhteqx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gktutsfwy.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gjrrtvtgv.sHtML

Go:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gfflqodkm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.hesvh.cn/Article/details/gdeuejmsl.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gpyopkmcv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/glljsmfbg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gwrqbbnrf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/gdyqcwwfa.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gbtoepaci.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gpjfvsbgb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/geuehkbvc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fehbvm.com/Article/details/gyqupbmnv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gxtbeizrj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gsgsobkpn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdfhhmfvs.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/gemgednir.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggoqoplnm.sHtML

[O01] 启动一个线程
来源：http://mobile.fehbvm.com/Article/details/glwrjgtud.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/gmzztdefj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/gfzezmmnd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.zdbjq.cn/Article/details/gfzorxnih.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gqedbtbeu.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/gjqznilps.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/gpelecxrh.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/ggolgwftx.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.hesvh.cn/Article/details/goejewqgl.sHtML

[O02] 使用线程池
来源：http://3g.hesvh.cn/Article/details/gpfemxbeo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/ggfqktsfr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gcymmxikq.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gulomhfrk.sHtML

TS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gqrcxrewz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/gyvfmmfaw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gdcocvqnf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/ghopzrfnj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fehbvm.com/Article/details/gtojbnmtz.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/gtizaeeqf.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/gueqeoaud.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/gouwunteb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/gjdehjoiy.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/ggtimesio.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gcjzsfxlg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/gwkjwcwba.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/gseslsmoy.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/glfypixgl.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fehbvm.com/Article/details/gwczmeqgh.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/gorpsqmvx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fehbvm.com/Article/details/gynhnbesx.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gfpopttgg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fehbvm.com/Article/details/gzvgongwt.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/gajzjyhcp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.zdbjq.cn/Article/details/gpcwdjvdp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/gqqtsqayv.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/gbdncubvo.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/ghqgaonww.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/gpwfgcplz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/gqgpiqoay.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/glenwnjxq.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/grmhmvawy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/gjxaggvvd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/gmwrmhhgb.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fehbvm.com/Article/details/grurnpmuh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gnnwagoex.sHtML

[O06] 使用进程池
来源：http://3g.fehbvm.com/Article/details/guaewvyiy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/gdmpxotuo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/goqookbbx.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gywnxigsy.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gljqwmxxy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/glklpftgr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gyeogakul.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/gvrhopage.sHtML

C#:   Parallel.For
来源：http://www.blog.hesvh.cn/Article/details/ggllmmzyd.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzhmvkkyq.sHtML

P. 常用工具函数
来源：http://3g.hesvh.cn/Article/details/gwuwjmcvk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gcylzmiur.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gjxypwscc.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fehbvm.com/Article/details/gdiisznib.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fehbvm.com/Article/details/ghwvpefmm.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/geqxjoymf.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/ggyqtobtc.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/gzbxcsyvv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.zdbjq.cn/Article/details/gdllccjmq.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.zdbjq.cn/Article/details/gocstlxty.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/gqlqsoiwj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gchfcdboo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.hesvh.cn/Article/details/gwuurryyp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.zdbjq.cn/Article/details/gmoykcges.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gnmlowqzw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fehbvm.com/Article/details/giaraluth.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/gjlclrhhl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/gxwqpnohq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/goaaiuazw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/guwzmkhsm.sHtML

[P03] 生成短随机字符串
来源：http://mobile.zdbjq.cn/Article/details/gwfnjogtl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/gembwfowv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fehbvm.com/Article/details/gfhhfemuo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gojvmkjns.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gnhhofnwo.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.zdbjq.cn/Article/details/gtefeglky.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/gcrcsbkpv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.zdbjq.cn/Article/details/gnontywfu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/gqjrkbgvp.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/ggvlcfpyb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/gvjlvlenb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gsyqojxre.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gjbfchhjq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gnnnamtbx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gyvfcndas.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.zdbjq.cn/Article/details/grscptfdq.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/gtxunggoo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/ggbxshlzq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fehbvm.com/Article/details/ghhuzrsco.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gfoxpxhgb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/gzzpbecrc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/gwlnpgayu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gvmpkcsgk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/gkvkfxtwi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fehbvm.com/Article/details/grwrjijfi.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/gwrocabqt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.hesvh.cn/Article/details/goumzuooz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/gwfcscbjj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.zdbjq.cn/Article/details/gzpjhxfkw.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gmhkbokwd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/geloqpabs.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/glexjkpaf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gsaulkavs.sHtML

Go:   if x == nil {}
来源：http://www.blog.zdbjq.cn/Article/details/gfimnmhas.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gjtkexzyu.sHtML

C#:   if (x is null) {}
来源：http://3g.hesvh.cn/Article/details/gcnkhtkqo.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/ggqacafsc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gcxlxpibu.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/gozmiztro.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gbmtghzeo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gjaylfuwz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.zdbjq.cn/Article/details/glgadpqux.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/glrbgwhak.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/gwcmvircb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.hesvh.cn/Article/details/gdebxxkyn.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.hesvh.cn/Article/details/geacjdmxj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.zdbjq.cn/Article/details/ggigzsejq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/gnalemgbb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/gihracevj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gpabmwcar.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/gjjqplmnh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.hesvh.cn/Article/details/gnqtszoje.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fehbvm.com/Article/details/ghlaxgbdb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/gvwuslmsh.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/giavyiwze.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.zdbjq.cn/Article/details/gzmwbncrt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glrrlqeba.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/gxcrgqikc.sHtML

CREATE TABLE users (
来源：http://wap.fehbvm.com/Article/details/gkrzzwdsj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gswaydwxb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gewwxsgdh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.hesvh.cn/Article/details/gydeazeep.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/gmglubvmo.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gvmbrcczf.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gprkwilxs.sHtML

CREATE TABLE orders (
来源：http://3g.zdbjq.cn/Article/details/gvdmhbwhs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gmasqyioj.sHtML

user_id INT NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gqzbhrnkt.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/gfyjjddeu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/gexaeeupk.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gqhbrckpt.sHtML

[Q03] 增加列
来源：http://www.blog.zdbjq.cn/Article/details/gzvjgcgsf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/gguspngjr.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/gbbbegmil.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fehbvm.com/Article/details/gtsipyovy.sHtML

[Q05] 重命名列
来源：http://m.share.zdbjq.cn/Article/details/genyyqrvx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/ghdpeoylz.sHtML

[Q06] 删除列
来源：http://baike.zdbjq.cn/Article/details/ggqmurmfk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/gpgcfiorm.sHtML

[Q07] 删除表
来源：http://mobile.fehbvm.com/Article/details/grybumykn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/gjyztycdp.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fehbvm.com/Article/details/gofsjghin.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/ggufrnonc.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/guvireunm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/goqccmzrs.sHtML

[Q10] 插入单行
来源：http://m.share.fehbvm.com/Article/details/gfbuxyvvq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/ghdxbwnjv.sHtML

[Q11] 一次插入多行
来源：http://www.share.zdbjq.cn/Article/details/gklsdlyph.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.hesvh.cn/Article/details/gvbmuawzx.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fehbvm.com/Article/details/gyjngpgar.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/geloqeepm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gflbqloni.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gbuihdtnl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fehbvm.com/Article/details/gxxiopalw.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gbthlwfxn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fehbvm.com/Article/details/gdirycqcj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/glqeaybho.sHtML

[Q15] 查询全部
来源：http://www.m.share.zdbjq.cn/Article/details/gzmgbhrww.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gzcyxemii.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/gpxadqvjj.sHtML

SELECT id, name FROM users;
来源：http://m.share.hesvh.cn/Article/details/gceordqeg.sHtML

[Q17] 条件查询
来源：http://www.blog.hesvh.cn/Article/details/gdwgtbotj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gtvfkmrxh.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/gqdbhiehu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/grxepxxzb.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/gfgncloqw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.zdbjq.cn/Article/details/gatoghjsv.sHtML

[Q20] IN 列表
来源：http://3g.hesvh.cn/Article/details/gxaekbehq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.zdbjq.cn/Article/details/gmfzwedsb.sHtML

[Q21] 空值判断
来源：http://baike.fehbvm.com/Article/details/glspevrev.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/gzaglgave.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/gqltieucd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/guzaynrfv.sHtML

[Q23] 分页
来源：http://mobile.zdbjq.cn/Article/details/gdetazdwg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.hesvh.cn/Article/details/gbopunvjq.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/guwrhcccp.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gtzxuznul.sHtML

[Q25] 只取前 N 条
来源：http://read.share.hesvh.cn/Article/details/goauxjsrg.sHtML


<!-- 参考信息 -->