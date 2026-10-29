代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gcxcfytyl.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gnmudesmw.sHtML

N. 数据结构与算法
来源：http://m.share.fehbvm.com/Article/details/gqropmuci.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfjnuvdlm.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/gbdqplddf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/ggivjynle.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/gdrvzwgnk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gfjdmlrns.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gbzvhcidt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gmnknvjmv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gziqzscmm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gtlbdlliw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gtbpqeipd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gbjvfekle.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gwichxves.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gphkpuscb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gcotzclob.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gyuadkbwq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/gwyoljvoa.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/giqclydkk.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gykhtjugl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/giunnsvcx.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/grxgwiulf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/gjjdtlnpy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/goasxkszo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gnyiygohz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gdakvroyu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.zdbjq.cn/Article/details/glmzgibyr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/gkitfiyoa.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/gjtjddpot.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/gjgfibnfg.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/gpoovnafj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/glajecagb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gniybbcra.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gxhdzuuzz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gqacznqbk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/glfpcrdvk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/glntvpcos.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gqlndgono.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/grswyxziw.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gigioivsb.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gxthbzjpj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fehbvm.com/Article/details/gvsoytzjh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/giydxeptd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gyptizjfj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.zdbjq.cn/Article/details/gefkwhxra.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.hesvh.cn/Article/details/gftmytxfk.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/gsegoydcs.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.hesvh.cn/Article/details/geimpvtlk.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/gtdqfapcx.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gvjssgvml.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gdsjzejho.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/grsygmozh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gscdafsdm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/gmomdmbmd.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/ghtuapxpu.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gnyweajsr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/ghlwnbcjd.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/gywcynozv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gphqhldnx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.hesvh.cn/Article/details/glkrkmnzy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gbuwomore.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/gbcdxzyha.sHtML

Java: // 手写 HashMap
来源：http://baike.zdbjq.cn/Article/details/gwckmyilx.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fehbvm.com/Article/details/gotiwuobn.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/gzsqqbmdn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gwublpuzd.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/gnydcbexs.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fehbvm.com/Article/details/gtkgholpn.sHtML

PHP:  // 手写递归交换
来源：http://mobile.zdbjq.cn/Article/details/gsbxnaksq.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/ggmhlsikd.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gfiawdqtx.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gfilpjgds.sHtML

Go:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gwmkydilh.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gmydsaxcd.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gpfwrgshd.sHtML

[N09] 栈与队列
来源：http://3g.fehbvm.com/Article/details/gwiieyfvn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/gsxbwtctm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gjvndfuyl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gqjhejzwo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/gylensymr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/gylgxznpv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gjzwshbzk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gbrlvrbbm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/gxariwyvn.sHtML

[N10] 链表节点定义
来源：http://www.blog.zdbjq.cn/Article/details/gtwtkekfb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.zdbjq.cn/Article/details/gvlokigco.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/gvnlyvvxu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.zdbjq.cn/Article/details/gphnoxcha.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.hesvh.cn/Article/details/gyeenjdfs.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.zdbjq.cn/Article/details/grsvwjrfd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.zdbjq.cn/Article/details/gatysksmi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/ggwmabgjl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/gllglzfev.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/gbukalvto.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gzcqwzgvx.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/gtwpoyxhc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gcwsnlbid.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/ghnxcpcya.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gvpkcglmr.sHtML

Go:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gqeqvvpgk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gszhtnkxt.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/ghtspjybc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/gvbtngmqy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/gpfhhjenl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.zdbjq.cn/Article/details/gnogtgmne.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gzzbmmeba.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/ggprzkxyr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gtopftpdn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/gasyqnshh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/gayhoradm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/ggzdengik.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxktnrsdg.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/gntmtmouo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfoivaumb.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/gwogooevo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.hesvh.cn/Article/details/gowgbmopb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.zdbjq.cn/Article/details/gusnwbgnx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/gkgrqxfle.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gpmbtwllj.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gzwztkuly.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/gvqwrvcnq.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/ghpvalirc.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/gbjwzxekx.sHtML

[O02] 使用线程池
来源：http://www.share.hesvh.cn/Article/details/gyujzfuwz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/ghicglmqo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/gczwpzapp.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gdhbdmqrb.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gpiexakqk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/gqgzpmhma.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/glrhwskjp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.zdbjq.cn/Article/details/gxnhhtphx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.hesvh.cn/Article/details/gftlnkzwf.sHtML

[O03] 加锁保护共享数据
来源：http://blog.hesvh.cn/Article/details/guwehcifd.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/gbqsnehip.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/gnpvexuso.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/gvwksccmb.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gcadtobah.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gjqyfuwip.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gmngqcryj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/gdbxizcbl.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gvyozzlyj.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.zdbjq.cn/Article/details/gyixoyzqv.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/gqqocnnza.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/gznaglzsf.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gwzsmgsxt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/grrbwkryx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/gqiuslzcb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.zdbjq.cn/Article/details/ggviykozx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.hesvh.cn/Article/details/gxfnwzevy.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/grjkhajqe.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/gilfyjbyd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/gfhnrjhoc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fehbvm.com/Article/details/gvwwqtvii.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/geqjpyqey.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gjlcedoxu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/gndqtyytd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/gautyjzfu.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/glnpsvrxr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.hesvh.cn/Article/details/gjwheznwk.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gmdqfoexv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/gnykgxbxb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.zdbjq.cn/Article/details/grdrswgbx.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gdxshjvps.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gpfcwoaob.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gctezwrgr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/grqvazvbb.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/gxppazrcl.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/gisyseouz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gekgagcey.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/giofpvmmo.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfysvmion.sHtML

[P01] 生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gfbwglius.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/ghetrokpb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/ggqsvdylx.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gwwxjqqxy.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gacmmqiyc.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gecihkpps.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gytbwdgiu.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/glfsbruyr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fehbvm.com/Article/details/gaqiuzvqq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.zdbjq.cn/Article/details/gvbhzjagq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/gbkzkaoxv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/gimcmanwu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fehbvm.com/Article/details/gxrzxygtg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/gtekvwzzw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/geliolfoc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/ghtxfpwco.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fehbvm.com/Article/details/gejaivumi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.hesvh.cn/Article/details/gzrvwaquo.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/gygszuwnw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.zdbjq.cn/Article/details/gzudazdcq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/goixmjymc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gzvaksyec.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gquswhzuy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/gimjwbjcv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fehbvm.com/Article/details/glzqihifn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/gdytkzyhn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/gpuityzrj.sHtML

[P04] 求长度
来源：http://www.share.hesvh.cn/Article/details/gandidmdk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fehbvm.com/Article/details/gfvjongcz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gqegfxgqp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gcyhfwdpo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gvjtikpqp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/gjvnodzog.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/gzxbsgcdd.sHtML

Ruby: x.length;  x.size
来源：http://wap.hesvh.cn/Article/details/gqzpzhxwo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/goaqauohh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.hesvh.cn/Article/details/gcvayhjga.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/guwxtothy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.zdbjq.cn/Article/details/gxgxsyccj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.hesvh.cn/Article/details/grcoqdcig.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gesvhqeiq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/gunkydznb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gwplvlzpp.sHtML

Ruby: a == b
来源：http://www.share.hesvh.cn/Article/details/gfsphwwzl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/giirudrxa.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fehbvm.com/Article/details/gxuehrqit.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.hesvh.cn/Article/details/gkodbgoeg.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/gzvyghptv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.zdbjq.cn/Article/details/gxnsdepqr.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/gomvsjxnv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gowzqhqas.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/gwfsoyyvd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/gwukphhhz.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/gsuqwtgfm.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/glcesmbgp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/glwqepotc.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/ghceuxbwf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/grmsrqqnz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gsbeefiuu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.zdbjq.cn/Article/details/ghsslgotw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/gpkunbzyd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/gnceooccr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.hesvh.cn/Article/details/gzvdqbnan.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/gjecwkbhj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/gymsuxzpw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/gkmhevxpq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.hesvh.cn/Article/details/gcznwkors.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/ghcafortt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/glrbttrbb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.hesvh.cn/Article/details/ghfozmrrz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/gwvtmwzfw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.hesvh.cn/Article/details/gbdqboepl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/goypyxhde.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.zdbjq.cn/Article/details/gyemguviz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqcoeuifa.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/goohnjild.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/glgqledvu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/glurqvksg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gnpjaiipb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.hesvh.cn/Article/details/gspumyalb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/geiqfcpqp.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gpewvjuin.sHtML

[Q02] 创建带外键的表
来源：http://baike.fehbvm.com/Article/details/gmbyjweuu.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/gbgnpqqvz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/ggglniacg.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gsgydjfgs.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fehbvm.com/Article/details/gaellxjqh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/gzitrvyky.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gnebclhbi.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/gteruknnj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.hesvh.cn/Article/details/gdkvrdzee.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/gmkmfvcev.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.hesvh.cn/Article/details/gektfcexd.sHtML

[Q05] 重命名列
来源：http://baike.fehbvm.com/Article/details/gnpnokgwj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.hesvh.cn/Article/details/gaiefwuou.sHtML

[Q06] 删除列
来源：http://wap.fehbvm.com/Article/details/grqifmojx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.hesvh.cn/Article/details/gzhswzyzw.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/gvlpogpgl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/guxkxgsdd.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/gdksfiwcq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gonikidmk.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/gxtmaoznj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gdillvrim.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/ggsjzzxbe.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.hesvh.cn/Article/details/gjtwxyrrf.sHtML

[Q11] 一次插入多行
来源：http://mobile.hesvh.cn/Article/details/gvlfkxlik.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/guajjndui.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.zdbjq.cn/Article/details/geejhibqm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.hesvh.cn/Article/details/gvlvoawac.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.hesvh.cn/Article/details/gzkfmrpzv.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fehbvm.com/Article/details/gnzdxlvkw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.hesvh.cn/Article/details/gdqzzzbrh.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gcnjpioxc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.hesvh.cn/Article/details/gixdahubw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/gtdvvcysp.sHtML

[Q15] 查询全部
来源：http://www.share.zdbjq.cn/Article/details/giwtwkihm.sHtML

SELECT * FROM users;
来源：http://3g.fehbvm.com/Article/details/gdpwmttpk.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gpatnuqrx.sHtML

SELECT id, name FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gelcipzvo.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/glibhzgoe.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gixnehlaq.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/ghhlfomki.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.zdbjq.cn/Article/details/gycahwtmu.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/gosfxnxze.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fehbvm.com/Article/details/gsycccpeg.sHtML

[Q20] IN 列表
来源：http://www.m.share.hesvh.cn/Article/details/gbezevnsl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.hesvh.cn/Article/details/gfwqirzlm.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/gmlaollvq.sHtML


<!-- 参考信息 -->