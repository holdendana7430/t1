代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gvuajrqao.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/ggozlyyhg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gvrzqifhj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gbsapztor.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/grfwabqld.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/gxhyejzkb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gookgfhgz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/guqfsuyxn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gjmidnfew.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gsfezbyub.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/gbavnxhue.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/glyytoffx.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/ggigwomph.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.zdbjq.cn/Article/details/gsbupwhfm.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gzoedgekr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/gbszcxknh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/gorsnfnio.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gcsojjtoh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/grzokjgvg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/gcqvcfwfv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fehbvm.com/Article/details/grbtnnscm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/giscfhmgl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fehbvm.com/Article/details/gmnbtpvqr.sHtML

[N04] 斐波那契数列
来源：http://wap.zdbjq.cn/Article/details/gcfdswnym.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gzpgvmfnp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fehbvm.com/Article/details/ghvmjgvxk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gjlfdsnet.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gdkhhlerd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gsavdjrjd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/gtpasrpow.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/ghhqbjnhf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gririjhhf.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/guvxhauwr.sHtML

Py:   math.gcd(a, b)
来源：http://blog.zdbjq.cn/Article/details/gmuszqqik.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.zdbjq.cn/Article/details/gqyiddthw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gzjvpzfcl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gkkcmctcz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/gyldycsap.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fehbvm.com/Article/details/gxereemhy.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/gfteqrlbq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.hesvh.cn/Article/details/ghygmdzxi.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/ggxxkgojw.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gpibwodek.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gjmgggvwb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gjtelrcdn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/goyfvangh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gauzawxlm.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/gtuucccnh.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gcwqbsuef.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gfdtohuts.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/gubyegqoe.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.zdbjq.cn/Article/details/gvlurmdcc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gimsesusv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/getfuxmqj.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gwsekrxaa.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/gfrveabfp.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fehbvm.com/Article/details/gsysiptyd.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.hesvh.cn/Article/details/girmkqatz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/gtphlbalo.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gszjgcsjm.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gxrzreums.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/grfpyfslm.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gsaviayyv.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gpjtokzkw.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gjraerdrv.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gvpshwqpe.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gxihzekpn.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gktqzrcok.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/gmvukrnjr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/getnduxtx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gnmirkvsj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/ggcefvkme.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/ggurqitcs.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gotiumkfi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/gifcrnwrr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/geeoszzrc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/guoihtygp.sHtML

[N10] 链表节点定义
来源：http://www.m.share.zdbjq.cn/Article/details/gxuhvpiyy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gudseumut.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/gqitonjtq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.zdbjq.cn/Article/details/gsysjhzmu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/goqkdtseb.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gloxwuiec.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/gakbwnvyg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/gxhgrbait.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/ghovbehrt.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/gdnuhkzna.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gtsluztlh.sHtML

PHP:  // 手写递归函数
来源：http://3g.fehbvm.com/Article/details/gridzmaww.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gqklesoql.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gwgladbkw.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gmzevtobc.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gxsrcbmxx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gqgjaihks.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gzuulpyad.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/gxgjqswll.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/glybrlhdm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/glovskdzc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gfltmyrje.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gyvtrqrec.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gnasvzwlk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fehbvm.com/Article/details/gjjuxrdid.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fehbvm.com/Article/details/gqoxkcvya.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/grizezvwn.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnxkyurvk.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/gtonevncj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grtunyyqf.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/glfcmkdtd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gsifclweu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fehbvm.com/Article/details/gzpkuqntb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gbqllwrey.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/ghzlhsqkk.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/gftebuhlz.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gdpzdoquz.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/gvgrfsyuf.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/gzsgiyxag.sHtML

[O02] 使用线程池
来源：http://www.m.share.fehbvm.com/Article/details/gdpaqzuic.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/guicfjlcc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.zdbjq.cn/Article/details/gsqmguzml.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/godckylbx.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gorobfazk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/gkdlujqtn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/gnkvxzzzt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.zdbjq.cn/Article/details/gqruckrer.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gmqllkaaw.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/gnlmoydya.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gkuyvrglh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gndjbwgbz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/geprnqned.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gtsvtzkok.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gptvjmcqs.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/gofrqdosx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gbmheauga.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/ghcajxswp.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/giqpkmfaz.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.zdbjq.cn/Article/details/gcmggrrye.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gxfngajnq.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/ghdbtrasq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gbljclium.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fehbvm.com/Article/details/grrfahsia.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/gbisabnwq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/gopuohnlp.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/gatphdncm.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.zdbjq.cn/Article/details/gpawhdhbj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gkukyqfhn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.hesvh.cn/Article/details/gjjrvofsi.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gekpcnyaq.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gjupgjoqc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/gzshzwsqh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/glxaipwnu.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/gffbtjjwz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/gvokjigcy.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/gxwdljias.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/gdwumfjcl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.zdbjq.cn/Article/details/gnveixjlg.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gyqciclvu.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/grzoztuxo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/geadmqtwh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gzudshzwl.sHtML

Ruby: // fork 块
来源：http://www.blog.hesvh.cn/Article/details/gacopnqcg.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/gztlmyrzh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gsnoxvpzk.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gxzpgsowc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggofhauti.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gzsjdslob.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fehbvm.com/Article/details/gbybtbmzs.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/gqpsrbxoo.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/glfdnxkif.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gejpeptnx.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fehbvm.com/Article/details/gpoicgpit.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/gbcbnzors.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/gfhncjiot.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/gtwdlamum.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/glrfvrznh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/gsfnlrxkz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/gmtcbewpo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/gytqljayc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/gcrnilgoh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fehbvm.com/Article/details/gynrrsjjy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/gvscdnrqh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/gfcwxefih.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/gomvuohyh.sHtML

[P03] 生成短随机字符串
来源：http://blog.hesvh.cn/Article/details/gwztjcvte.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/gnqikhkdz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/gjxfwtvbz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gidhtmlvl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/goqvglqvu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.zdbjq.cn/Article/details/gpnaratve.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.hesvh.cn/Article/details/gyibugkih.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gvcjgfncl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/gcxjzrbwi.sHtML

[P04] 求长度
来源：http://m.share.zdbjq.cn/Article/details/grmibjttq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gwvkzafsy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gyutrnjxt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gycmmvnfr.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/giuaghsdo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/glzbdncsg.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.hesvh.cn/Article/details/glnfvlsfn.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/gomwsvhbn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/gsdxxvfln.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fehbvm.com/Article/details/giptwscds.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.hesvh.cn/Article/details/gifxwybqa.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/gqpptufva.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.hesvh.cn/Article/details/gbcfsudug.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/geiprwpqk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/gpscwoclw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gukdrftgl.sHtML

Ruby: a == b
来源：http://blog.fehbvm.com/Article/details/giufpoqrd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/gnknhdwlk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.zdbjq.cn/Article/details/gcwkscnvy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fehbvm.com/Article/details/gdsulhvzg.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/gbdgwlsck.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/gqjivjxdw.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gqhhnqwwq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gqgovfvdb.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/gfqgmoans.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/gysajbsjp.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gytzovkrz.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/gfbrslmpr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fehbvm.com/Article/details/gmtkxshjp.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/gskhsaool.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gjsubhsko.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/goxaszjpp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gcfhbvmsk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.zdbjq.cn/Article/details/gmudzuhlf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/ggtizkhew.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/gxczbftwe.sHtML

[P08] 处理浮点精度问题
来源：http://3g.zdbjq.cn/Article/details/gtwovxtzn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/gybtuknlh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/gyjlwylhm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/glrzabyyp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gytwiuwof.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.zdbjq.cn/Article/details/ghwiojakj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.hesvh.cn/Article/details/ggdvveecq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/ggfskkvqq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gfzyhoxfs.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/giaapvxst.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/glvfjekhf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdeeceaal.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gsxrcfeke.sHtML

CREATE TABLE users (
来源：http://m.share.fehbvm.com/Article/details/gffpfyccz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gqknyvzyc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/glwnbgebl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fehbvm.com/Article/details/ggzidllnz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/gvxlrfuww.sHtML

);
来源：http://3g.fehbvm.com/Article/details/grwspkqnp.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/gwycwneht.sHtML

CREATE TABLE orders (
来源：http://www.blog.hesvh.cn/Article/details/gjooecjog.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/ggrwtpdel.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gjgoxkdif.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/gpcsgwkvr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/gthvnnkqv.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gjqblsgcn.sHtML

[Q03] 增加列
来源：http://3g.fehbvm.com/Article/details/geizbfhai.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/glmzcnlhd.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/ggawtuluz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gkqqvvoah.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/gqqvxzxyr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.zdbjq.cn/Article/details/ghcvynutl.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/ggunmmoiz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.hesvh.cn/Article/details/gprobaxhe.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/gtwnhbcvj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fehbvm.com/Article/details/gqrcnfast.sHtML

[Q08] 创建普通索引
来源：http://m.share.hesvh.cn/Article/details/gnirbinar.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gpzuwokjq.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/gjvufqxpn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/godmksiix.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/gfwhrbyzf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.hesvh.cn/Article/details/ganuyqtqq.sHtML

[Q11] 一次插入多行
来源：http://www.share.fehbvm.com/Article/details/gnuprvuys.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gmsltivqt.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/gmvtrxyct.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fehbvm.com/Article/details/gfuxasred.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.zdbjq.cn/Article/details/gowdayppz.sHtML

[Q13] 忽略重复插入
来源：http://m.share.hesvh.cn/Article/details/gxakegqcw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/gavpdsfvc.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/gwhbemtlp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/gpuomhumu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gbuyedgef.sHtML

[Q15] 查询全部
来源：http://m.share.fehbvm.com/Article/details/gxfkjoztu.sHtML

SELECT * FROM users;
来源：http://3g.fehbvm.com/Article/details/guqnojnrc.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gpqmpkeva.sHtML

SELECT id, name FROM users;
来源：http://www.share.fehbvm.com/Article/details/gavpzssaq.sHtML

[Q17] 条件查询
来源：http://m.share.fehbvm.com/Article/details/gtpupftnf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/gjktuaqbv.sHtML

[Q18] 模糊匹配
来源：http://blog.hesvh.cn/Article/details/gbmkwjksj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gadjnayzo.sHtML

[Q19] 范围查询
来源：http://baike.zdbjq.cn/Article/details/gjixctvva.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.zdbjq.cn/Article/details/gicqrsrdk.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/grzeiersc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.zdbjq.cn/Article/details/gqsnwgirq.sHtML

[Q21] 空值判断
来源：http://www.share.hesvh.cn/Article/details/gmqytonoj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gbpyrmhgd.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/glsjouloi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fehbvm.com/Article/details/goatjjezm.sHtML

[Q23] 分页
来源：http://mobile.hesvh.cn/Article/details/gtxiozesf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.zdbjq.cn/Article/details/gshkzhzke.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gpusgdmmx.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gwbpuvyif.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/gtjyhqlfm.sHtML


<!-- 参考信息 -->