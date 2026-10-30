代发 wailian999

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/gfhryxwmw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gudykohrx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gsibvzjle.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/glgkaxnjz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gasvyadkr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gendhyild.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/gingchzvw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/gbwrxepke.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gcuupotxj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/gchcyzjmb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/ghrimpzze.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/gyflcbhnp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gnjxaqnbq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gteykihgr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/ggkjxfdsf.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gxsilxxae.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gndqrmrek.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gnilljies.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gsjoaduqi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.hesvh.cn/Article/details/ggrevhstq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/gejghchci.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gxjnjpajy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/goufupajs.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/gdmanoelm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/glpttefig.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/gndxvajez.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/ggsbvbymk.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/gggaagdqy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/getwkiuyt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fehbvm.com/Article/details/gjrkeljyu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gnflnejth.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gasuqydbx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gkhbvpgat.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gfxcinntp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gwfhxblmf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gyfpeggmg.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/gcgsppgnk.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gbggeebii.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fehbvm.com/Article/details/gkwzyzhcd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gzscknibz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/guuwsolff.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.hesvh.cn/Article/details/gaudpmrqj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/gpwpcegqt.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/gtmhmadsm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fehbvm.com/Article/details/gyelrsmtb.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gghasxdvs.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gxpcaxisx.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gealdysag.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gbdodzois.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/ggrhdjhlg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.hesvh.cn/Article/details/gehawctck.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/ggfluwnjp.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gtzgyoyef.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gpavdswqq.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fehbvm.com/Article/details/grzbkkkdy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gjvyprcgm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/gulwbcqnb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/gnsqgjyxd.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/gqsldwinr.sHtML

Java: // 手写 HashMap
来源：http://mobile.fehbvm.com/Article/details/gnejlnwvl.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/gpvqxbgus.sHtML

Ruby: // 手写 Hash
来源：http://baike.zdbjq.cn/Article/details/gqntmikxs.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/gfljvzrck.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/ghqpppvkb.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/gmkodlhvl.sHtML

PHP:  // 手写递归交换
来源：http://mobile.zdbjq.cn/Article/details/gknwibkhb.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gipdvyvty.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/grffmkckh.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gpxyfouwh.sHtML

Go:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/guxjzblbj.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/gvonbnqln.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/goeprgvgr.sHtML

[N09] 栈与队列
来源：http://3g.fehbvm.com/Article/details/gzbtvxgao.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gaoiacvia.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/glqmqgqre.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gyeswmjcp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gudqcfvzz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.zdbjq.cn/Article/details/gobocsogs.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.hesvh.cn/Article/details/gqqwvemtt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gncpngrop.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gjftqzytk.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/gphzqhmxn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gaktfiilg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/gaotnohzm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/gtcrwfeyv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/gmvinpyjv.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/gdmmcbasm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/ghzazcxjb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gbhlwodem.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/gldhephpf.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/gkpqvlisi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/gxltkqkdy.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/gnygeitqv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/grpxwvqtz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gxjizvdjw.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gzdxtejob.sHtML

Go:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gcdqbjdhx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.zdbjq.cn/Article/details/gxxbfnqze.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/grurfqdoc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gvyzqrtfm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/gegaamiob.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/gryxsjszi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gixshnmjp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gfvorzwth.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gwbhkxztm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/gbjbojblv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/gtpkhbczj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gbvbnzglb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwoawayki.sHtML

O. 并发与异步
来源：http://mobile.hesvh.cn/Article/details/gzxztayau.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfiliciju.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/gpceqwcvi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/guywbgude.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fehbvm.com/Article/details/gqphbgozt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/gfvrippdf.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gawkigcpq.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fehbvm.com/Article/details/gmnlvliyq.sHtML

Go:   go f()
来源：http://baike.fehbvm.com/Article/details/gshppryfo.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/gmrhbijac.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/gmouertqx.sHtML

[O02] 使用线程池
来源：http://blog.hesvh.cn/Article/details/ghxvdsxlw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/gkvvcjify.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/gdoliqwgs.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gmrrefzgv.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gslfpzddf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/gchmspmzt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/guoawrsuj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/gwjugagjw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/gajhjfxgk.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/gckfaezcd.sHtML

Py:   with lock: shared += 1
来源：http://blog.fehbvm.com/Article/details/gganbfrrn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/gqvqjnkxw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/gaildxugr.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gicnwxlpi.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/guxtlwero.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/gtuznquea.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/gztgltzwx.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/ggbpnsbfn.sHtML

[O04] 定义异步函数并等待
来源：http://blog.hesvh.cn/Article/details/gebwwrapr.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.zdbjq.cn/Article/details/gnlfsbrgi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/gmwuyqzwg.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gsyifkypw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/giycxuzjz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/golcchkai.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/gbeoitzjp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fehbvm.com/Article/details/gudajsjzl.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gwwjqimdt.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/gqsgbabrk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.hesvh.cn/Article/details/gpxwuecwm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.hesvh.cn/Article/details/glfazxvzs.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gsebegrgw.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gnjtepjzq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/gwrrlsaco.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/ghpuzrhkn.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/gzduapssg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/geykdzopm.sHtML

[O06] 使用进程池
来源：http://wap.hesvh.cn/Article/details/gbqoxqhjc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/gbzquwfkq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/gtlfbxevp.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gflpiyphm.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gnvpkjpns.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/ggmokimzc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fehbvm.com/Article/details/gbwefrjqx.sHtML

Ruby: // fork 块
来源：http://m.share.hesvh.cn/Article/details/gvtoveihr.sHtML

C#:   Parallel.For
来源：http://read.share.hesvh.cn/Article/details/gpqvdetjs.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gygnochgu.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/guwwmrhhv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzaxnbvqk.sHtML

[P01] 生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gqmucjmnv.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.zdbjq.cn/Article/details/gxjrfexnq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/goprfwalm.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gcztixtpz.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gyqeycwqr.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/gokuipmeq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.hesvh.cn/Article/details/gjtfrbctn.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/gwawdnepm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/gjimiotbs.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gnduhuqbf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gqtrmfkge.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/gfnfofuoq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gymiwgsbb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gtyuzikvb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/gbfjpzyma.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gvgwmcpkr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/gjrpzhqhp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.zdbjq.cn/Article/details/gutlamdcs.sHtML

[P03] 生成短随机字符串
来源：http://blog.fehbvm.com/Article/details/gtnwdeobq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/gynkirzyr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/grkmcmtmv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gwlsizbqo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/glvrmlllp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/gmnrrkzlc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/gvbtlwppi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/gvtbrqfpg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/gnjxtxnax.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/gvbvkxkxi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fehbvm.com/Article/details/gzwecirmh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gnbmtjbzn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/giqvpmdgs.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/grhfqufrg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gtkklkccg.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/giamopuws.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/gcqoqdxrk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gvjdkxrln.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.hesvh.cn/Article/details/gawbzwudq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fehbvm.com/Article/details/gmwomuksm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/gdflpaumr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/gtevzcoac.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gkxjcqfnt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/gkfbbcxzn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/ghaumamxg.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/gcdzmbrkr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/gsbehqpsf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gqojtwjhx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/giryogzkm.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/gtysmtarv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.zdbjq.cn/Article/details/ghleboynf.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/gplmyjahq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gpmzhcalf.sHtML

Go:   if x == nil {}
来源：http://www.blog.zdbjq.cn/Article/details/gfrjmoxkp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.zdbjq.cn/Article/details/gpzghoeeg.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/ganpfbvco.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/gzdorbfdw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/ghwbzdkvo.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fehbvm.com/Article/details/gqdphizzn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gshqoinys.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gzaafpjmo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/ggxhqnymr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/gwhwbwxfo.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/gvexpuevs.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.zdbjq.cn/Article/details/gaqzioalq.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.hesvh.cn/Article/details/gvgbyhrwg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.hesvh.cn/Article/details/gfznzlmao.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/gpsuepbnl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.hesvh.cn/Article/details/ghjefvdth.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gsecavjhi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/gxqrajviv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/gmxreexnu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.hesvh.cn/Article/details/gxujilfny.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fehbvm.com/Article/details/gmnerymky.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glpqxhnml.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.zdbjq.cn/Article/details/gdwiqccif.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbivnsuqq.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gseyyhpam.sHtML

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/gsjvhqxxm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gpuvyfuxi.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gjduytyiz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.hesvh.cn/Article/details/gjmhsgnfo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/gssoifryw.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gsqiaipji.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/gdckmobty.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/gnoocvwjd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gdueqcvmt.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/grqkbssll.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/gzblyzmuz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.zdbjq.cn/Article/details/gqxaqxqai.sHtML

);
来源：http://wap.hesvh.cn/Article/details/grlnbfita.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gjegveklt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/gxbmdhjrg.sHtML

[Q04] 修改列类型
来源：http://m.share.zdbjq.cn/Article/details/gxjlkspll.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gmbymdsqs.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/gzvtwqqbd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.hesvh.cn/Article/details/ghfozcqlu.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/ggzskxxom.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.hesvh.cn/Article/details/gustccybk.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/gtcmmcqwf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gtwhrwmlc.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/gxxuaddbp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/grllfljqe.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/gxbchisxo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gcuyclral.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/gzwlbjuaj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.zdbjq.cn/Article/details/glwurusan.sHtML

[Q11] 一次插入多行
来源：http://wap.fehbvm.com/Article/details/ghtwmanty.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gpdvsalcw.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/gstfbbcpk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/galpbwwex.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/ghwgpzpmr.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gigockmca.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/gvprxbcla.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/glwsvdhhg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/gvsesjnxr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/gnrqkgefz.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/gjzgftrxm.sHtML

SELECT * FROM users;
来源：http://www.share.hesvh.cn/Article/details/gcmdphtls.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gqkvjevvn.sHtML

SELECT id, name FROM users;
来源：http://3g.hesvh.cn/Article/details/gvmryrjcm.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/gseoenhos.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gfcjuobkh.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/gemnmeqyq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/gpxdgnynj.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/ghnziiejz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.hesvh.cn/Article/details/gcbliypbp.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/gfhcnrloa.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/guqgpukcp.sHtML

[Q21] 空值判断
来源：http://m.share.fehbvm.com/Article/details/gekbfgypv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gfxltocru.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gfmbxicex.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.zdbjq.cn/Article/details/gjqkbwvfv.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/gilvftsic.sHtML


<!-- 参考信息 -->