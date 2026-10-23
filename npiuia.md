代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3fdzyztnm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lkejnjnj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3txvicuyw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3mvjzjzsx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ndmncpvw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3oizcefdb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3zsrpryie.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3yhnhbixh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3touhmimm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3rgmwhcxl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3byncezzl.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3llmdwpty.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3kyuppqcs.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3zwlewlqc.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3cukgavnd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3mziwqhws.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3ilwwotqj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3csnrzctn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3bgdqajws.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3oewnszqn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3zxailhyn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3nekrbhmz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ivrsekkj.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3wxphbgck.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tjsxminc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3yuvfcxre.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dvjbiggg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lxweurtw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3tbbzhwfi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3iedclnun.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aektfpre.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3knitifkj.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3btvsbzth.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3cznsmils.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3cpcvmysp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zsxgtxls.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3iawgntsw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3atboussc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3spikxeig.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3vobzfycs.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3zrhnpjpp.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3imyszehv.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3azrrurcj.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3aoqnhjzm.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3twjfmxce.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wpplkbig.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3hjqmvzsk.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3nnhiiqhj.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ledcgvtq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3tnaecams.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3pdqstlpm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3cotjfmtp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3xtlvwgeo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3kagfhatg.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3moscygpx.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3czcrtojt.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3pgtvklnh.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3vxvcnxrw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3jlzphxuh.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3lqjnlfyi.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3xaeejlvy.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3rtshnqxm.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lughmyru.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wdwfuypt.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rnqxbcok.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pheofeez.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3hpbhlpyh.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3apfuvjts.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3qmmwuswt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3lcllioao.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3yiowfogy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3afiirlep.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3mtfoddoc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3oxfkfazf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3iqtuhtmw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3udlhrrqf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3eigypbmv.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3hjvgeaqt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3ntwgzleb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3lyhhhxet.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3tjtijvaz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3huzsgjxv.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3wzonsptq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3aasdtzcx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3qabonzbv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3jhxbuwkj.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3eoiurrvt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3sqsukrqc.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3bbeqvqrb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3gfyngsgu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3qpswxqer.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3sdsvxvgx.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3xlwvxjyu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3ofleykzh.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3rtlxhanh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3kgtdyicf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3yzhudnny.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3plenmynx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3qzwxhwze.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3xdlzpjgk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3nfpukohv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3yzdkjqmn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3dijgmrmy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3vzowxqyd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ndorlmon.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3mnlckbst.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ropmmtyj.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ybqwevrx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3hbvfrchu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3bvwfpvqj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3bbuxrluy.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3wwyxkgeg.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ewdkbiun.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3usttyyvc.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3kwgozimc.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3eodhiibx.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3aospxyxq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3rknsfmgr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3werhqgxb.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ivwtzfgr.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3wyfimvrk.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3fipiibnv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3ylsveaat.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3pekjvulu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3tlxpolcs.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3qkxdwitf.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3pyspodwi.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3gjynxjrk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3fuzirsha.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3bsmgjaiw.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3axckzwun.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3caernfrm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3zrhzeaao.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3otctgjkk.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3lhnokzto.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3hntjcgak.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3hvabfjai.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gbyeiglb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ldcglrqq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3ofrzqkpb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3pqrcwgkk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3dedxplqc.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lbvzbsgg.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3zlpncovf.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3ndmknjcz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3lbossvvd.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3cufyyihj.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ovvlwrvm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3zfgtasbs.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3wgamdevz.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3nsexiqzt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3oxfkzqmi.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3eilakyur.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3vcliwvcv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3yxagtmty.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3lwxcfhyg.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ipgenfhb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3usrngymc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3nylkaots.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3bjusgiec.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3qmxjergc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3evnpfiwd.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3vrskgamf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wzufofsj.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ntzsytcd.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3bgmnhmee.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3taqallkm.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3qjidexgx.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3xhzsiasn.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3eticnxlw.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3mzxzuuhk.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3muqfyand.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3hkaxyjtq.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3rbpmluub.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3zdwvwcyx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3kxdhawqi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3czvcnfbh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3ngtrlpzr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3arefgsch.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3edgsafdv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3smiakpun.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3kzxevjid.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jbaaqvln.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3aodpkqfo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3ldhgqwiv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3xjwbguwg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tcrurdfc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3dsabipkg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3thhhncee.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3uzervtys.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3ksdpjozd.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3hmvooyrm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3dcochacj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3iujysjgv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3djuuvmag.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ibjdrahb.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3tmwllyhf.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3prcjuvkg.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3wqaqeotj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3tnjthatb.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3zmatdczb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3bteafrob.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3dnhvzvgf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3xmmcdkun.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3unhbxddr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3srgbumsv.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3dtjibbvs.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3abplyght.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3krevlxnf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3sjsvciuu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3qmbgvsze.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ebmjyuzj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3eeunfbnn.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3enafqxym.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pzgtgytl.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3dctngriq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3zbzmgxty.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yrbwhchn.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3xrbalfgj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3hpsqvkng.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3hbkgazdd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3bvlhbbpy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ehoxorfs.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3oxbqsubm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3gynnouyc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3igzgvcuf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3ccywisdl.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3xwmllvfb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3wenislug.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ymzeoieh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3tpbtjbku.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3yjxndxtw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3yddulkcj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3mruidomt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3degrtoqq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3lebpcuwh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sljhrfkx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3xkwoctzt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jnqclhmx.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3nzbmhvrz.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3mzikakeu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3gxuwwmjc.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3yxgrzdtt.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3xxvharkr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3vykuarjg.html

);
来源：http://www.52xcode.cn/Article/details/gt3tbfumjef.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3swenlpic.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3hhmawkkk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3scrwuxdr.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ecgnavvz.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3vtmmxzrp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3pxhvifma.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3dtnxesqy.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3xyfjmskg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3mfhsnrel.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ktepikcu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3twjdgdau.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3udpfjnsm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3dausxrwu.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3rohuwurb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3ymgrehlg.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3prhunope.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vbnvlhcm.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3gwrhrjhn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3kxlpifhk.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3eqyngpzv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3oxuavhdi.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3fjdpqlhr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3wfvwklba.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3rnbhvlyp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3tlljrsdh.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3sgjassxp.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3ywszqdem.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3msbqlous.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3zyfekdmx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3vdikcrhj.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3iskhobdd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3jiffvrjk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3enmbxxre.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ecipahrt.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3trggldic.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3nsrrfjwq.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3knjluikt.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3eqbpzarj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3gzkzsejm.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3tamhchab.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3jvmrcfex.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3lyoqyxny.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3nepqszke.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ljbwyyum.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bmchhdac.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ztlfdnbl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3vgumkgdt.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3lohzjbmc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3crtstoou.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3nkteebtc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3cqcspkcg.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3rndqipdw.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hfijfhqx.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3dtlfoqsr.html


<!-- 参考信息 -->