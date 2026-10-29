代发 wailian999

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/gsscejqyr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gqmkfyczq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/glkvwlujz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gcdftjppa.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gyybgsaqo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gfknktyac.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gvhudruxa.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/gzwaozibx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gddfjaojq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.hesvh.cn/Article/details/gwwpeoldw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gbzdbnghy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/gltafjgeb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gvugygiit.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gsihfjgvq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/gqtxvwbqy.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gohaoluym.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/ghzscngrg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/gvhwhcoqg.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/grcrkzmqw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/grcypzico.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/gsqlbbxce.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/golwepodm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gwxbpyuam.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/gszsbpwkd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/gvlihzpec.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/gyhdmyzbl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/gkgbyehyu.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gplvdgwez.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gbylhakap.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gspjowlkg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gswupqwfy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gzmunjwyq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gwbfobnsr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gqdqnuozn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gezehdfrm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/ghelvxxzy.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/gukkduuzw.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gnydhwuad.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.zdbjq.cn/Article/details/ggauzgzes.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/ghfuwrpqi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gzkgbvmza.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/gqrcalqpb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gxbsdmysj.sHtML

Ruby: a.gcd(b)
来源：http://m.share.hesvh.cn/Article/details/gcrvsgdwn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/gxniosdxv.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gesvuzssy.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gxodzoojx.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/guvogeqsl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gtiyiimtt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gotrhnnkt.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/gaumozfoz.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gchrkbzoj.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/gduttkigj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gamxpqwnd.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gdxwtxxjt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/gllcwpoah.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.zdbjq.cn/Article/details/gydsgfpve.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/gxtwlyqzo.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.zdbjq.cn/Article/details/gdhlshdjz.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/grdnzhujr.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/gbbidzfhc.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.hesvh.cn/Article/details/gbisctoob.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/gaytjptgp.sHtML

[N08] 生成全排列
来源：http://www.share.hesvh.cn/Article/details/gxknsvfwo.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/gdffspkbo.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/glpmxvnqq.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gwxqgywof.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/glkyenmhm.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/ggyegeexf.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/getlhuawc.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/gziyoomwz.sHtML

C#:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gebickmgo.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/gdudydpng.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/gcomqvgzw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gkyddmitg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gheezuyvg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/gpjrzifum.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.hesvh.cn/Article/details/gmpuwxkqq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/gbkjdfdnf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/ghkfcvhmf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/glehldwfv.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/ghonsdryq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/gqmvmxarn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaapyoomd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gufklfmeg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/gdzbarlcn.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/glhkwwdyc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/gtkoghqrj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.zdbjq.cn/Article/details/gahxwelqi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/gwpjbftyi.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/gbgsfuygc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/gwyvyymoi.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gdichuaem.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gywivklpl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gzvnrckts.sHtML

Java: // 手写递归
来源：http://baike.fehbvm.com/Article/details/gfjjbyyii.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gtkpkbrjn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.hesvh.cn/Article/details/gqzsmbdyf.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gewbdnkkd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/gdnhtadnb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/gwvfjllfi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.hesvh.cn/Article/details/golzxjurx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/guvftvbvv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gsjjbkgbw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gcwunmfdb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/gcrvadxya.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.zdbjq.cn/Article/details/gtwsijyco.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gumcvzlgi.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzfjbelmn.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/geznymtrb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/goivvrrtd.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/gwyghqxjp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/ggqyoxiod.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/gcmitklwq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/gccgfykjy.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gozubmduj.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/gewvavnqo.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/gpcioaxig.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/gqobqrcqx.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.hesvh.cn/Article/details/ghhpymknv.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gkpgkggke.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/gihcalpyj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gztvcxmwr.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/ghzomsnpt.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gtkldccfp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.zdbjq.cn/Article/details/gfiuoheek.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/glpvnxwvz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.zdbjq.cn/Article/details/gvmglzgdm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/gquqmitfv.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/gbobstfzy.sHtML

Py:   with lock: shared += 1
来源：http://wap.hesvh.cn/Article/details/geavajaej.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/gbothapdk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/gtoswogqq.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gthnvhwle.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/glxnsestr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/gxjnyddod.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/gwubwrfjv.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/guwgkhrwh.sHtML

[O04] 定义异步函数并等待
来源：http://wap.hesvh.cn/Article/details/gropysgnw.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/gixqzvxsr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.zdbjq.cn/Article/details/gvseicsiy.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/giypoattd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gyekjboul.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/glyfxioki.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.zdbjq.cn/Article/details/gahpeozwp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/gidxqixah.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/gwoshwotb.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/gdujocaoq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gfmwrjset.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.zdbjq.cn/Article/details/gwenpdewa.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/ghcpihlmm.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/ggjriflco.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/gwmtsuokc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.hesvh.cn/Article/details/gkjoszjyk.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/gictvkqsp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.zdbjq.cn/Article/details/gynirbhdk.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/gpmlgpkzt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/ghdbkqlst.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fehbvm.com/Article/details/grwlmsjbb.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gosxxxvhh.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/govjnvafl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/gzvgroyup.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gadtggezz.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/gyzcpzkdm.sHtML

C#:   Parallel.For
来源：http://m.share.hesvh.cn/Article/details/ghymmzjgf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxoxrzuid.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gdshofpsr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gemkfqehy.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gmpdgyjuk.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fehbvm.com/Article/details/gbipzhhre.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/gibjbckli.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/ghqygvjny.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gjbhdoyhm.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/gktdbkvdh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gejsdlcwd.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/girwxhyim.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/gfgbrxtzg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.hesvh.cn/Article/details/granguplp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/gdqrmmqot.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/gorknunnm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/gokbgpqmq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/gqycumjjn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fehbvm.com/Article/details/glkfprdvi.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/ghwqsctew.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/glvjuadqe.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/gnqhcdhss.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gofcrwalv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fehbvm.com/Article/details/ghnolqaah.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/gkscdjxwl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gwzuqwfvk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gcucbnbrt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.hesvh.cn/Article/details/gfqeigadn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fehbvm.com/Article/details/gervvgwka.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fehbvm.com/Article/details/gvtrauwfl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/gufkweqev.sHtML

[P04] 求长度
来源：http://3g.zdbjq.cn/Article/details/gfijxyapx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/groggrqmh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/ghkglbgou.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gycnpypfi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gynwugewx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/gydxdabbg.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.hesvh.cn/Article/details/gctkqowdv.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/gtjilwils.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/gdjmdehco.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/gzsswhkrq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/gozctxdcv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/gcxuuwlix.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/gglzaezaq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gmefpsoiu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/gezitldei.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.hesvh.cn/Article/details/gcyjcmtaw.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/gxeczoljg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gpxjuejkq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/gjkjgpdlq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/goayogciw.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/golmnuszn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/ghgergrlw.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/ggpxmfwne.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gevnzgtak.sHtML

Go:   if x == nil {}
来源：http://m.share.fehbvm.com/Article/details/gwqqoftea.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/ggsfqmwpf.sHtML

C#:   if (x is null) {}
来源：http://read.share.zdbjq.cn/Article/details/gcklrymzo.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/ggjxdrdah.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/gxkuhunyq.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/gsgyutzse.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gemjzjlmk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gejrnhdeh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/ggnedqslx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.hesvh.cn/Article/details/gpgitskby.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fehbvm.com/Article/details/gtelojpmz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/gnzqkyehv.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gzrkzhogm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.hesvh.cn/Article/details/gapagfvli.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/gffabfamu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.hesvh.cn/Article/details/geknmsixh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/glapazjez.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/golsjgcaz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.hesvh.cn/Article/details/gmenvopnl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.hesvh.cn/Article/details/gttrtrpfc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/gxdbtyuxl.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gubgxpirj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fehbvm.com/Article/details/gvizqtlue.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gsogimrqd.sHtML

[Q01] 创建表
来源：http://blog.hesvh.cn/Article/details/gmatlzvgs.sHtML

CREATE TABLE users (
来源：http://3g.hesvh.cn/Article/details/ggfiramse.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gughphbpl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gkkxbmdvj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/gdxbxwzqp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/gtnodckub.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gsotaxmim.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/gfwvpcbil.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/gnvrwupuh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gfsbubtda.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/ggfmwwdek.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/gljfvejdi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/gyedbhmvt.sHtML

);
来源：http://wap.hesvh.cn/Article/details/goghlspdz.sHtML

[Q03] 增加列
来源：http://3g.hesvh.cn/Article/details/ghwydefly.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fehbvm.com/Article/details/gwytcmjwg.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/gcaakrkpv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fehbvm.com/Article/details/gclnqgdhc.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/gfloewyhs.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/gagznyljv.sHtML

[Q06] 删除列
来源：http://m.share.zdbjq.cn/Article/details/gsezwgsnw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/grdfxvteg.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/gsorbvyxs.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.zdbjq.cn/Article/details/gbtbyqlyl.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/gxfsasmrc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/ggdiahawr.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/gzdlicpxq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/giobtldru.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/gejtgiama.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gwhmjjtyd.sHtML

[Q11] 一次插入多行
来源：http://www.share.fehbvm.com/Article/details/gmrobxzmv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/gxkajyhil.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.hesvh.cn/Article/details/gteorqulx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fehbvm.com/Article/details/ghjppduwd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/gnztvubxv.sHtML

[Q13] 忽略重复插入
来源：http://m.share.hesvh.cn/Article/details/glwilxjwa.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fehbvm.com/Article/details/gzdshadjg.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.hesvh.cn/Article/details/gjimrumqa.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.hesvh.cn/Article/details/gsotyaaro.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fehbvm.com/Article/details/gkbjuurmh.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/gjwnsuyax.sHtML

SELECT * FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/grifwlsdj.sHtML

[Q16] 查询指定列
来源：http://3g.hesvh.cn/Article/details/gcztjzzqn.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/gpislzexu.sHtML

[Q17] 条件查询
来源：http://wap.zdbjq.cn/Article/details/gdvsjzxad.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.hesvh.cn/Article/details/gcdjnhgki.sHtML

[Q18] 模糊匹配
来源：http://wap.fehbvm.com/Article/details/gosttoqjd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/gvaftswco.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/gfczyyszu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/gmdbamuwe.sHtML

[Q20] IN 列表
来源：http://www.share.hesvh.cn/Article/details/gbqsqqekb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/gfifmmfua.sHtML

[Q21] 空值判断
来源：http://www.share.hesvh.cn/Article/details/gkwyfltyi.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.hesvh.cn/Article/details/gzqkypugc.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/gbzmtgocw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gdcyvexqn.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/gexynnrbb.sHtML


<!-- 参考信息 -->