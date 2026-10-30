代发 wailian999

TS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gbwguttmi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gajgkynls.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/giwrouzqh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/gnhffvuwj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gzkfnbmmi.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/glaurvcdx.sHtML

N. 数据结构与算法
来源：http://m.share.fehbvm.com/Article/details/givqlhuok.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gercetpvg.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.zdbjq.cn/Article/details/gykayzjpl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gitnhmuxx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.zdbjq.cn/Article/details/gypbdzcbg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gepjzuaqo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gihflugar.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gkvrbfsjj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/grztosiwf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/gtwpxvcwk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gplplsnzn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/gpuqppedd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gnxylqzzj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/gxkcfgfju.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gxjzgsuju.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gasuchqft.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/gwnlsdfpp.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gthvjdzjx.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gblkrkrud.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.zdbjq.cn/Article/details/genyohovd.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/gxdxopmsl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/gfduxxlep.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/glvpcbhkm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gcigddkha.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gnbllmiuw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/gpmpzzkef.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gxffgnqoa.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gptdmmjxu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/gccptddju.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/gziomqxvd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gpenzpvtc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gvdjfhbvr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gskojrlnx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gpxrqduac.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/guqezdjrj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/gampcuqxa.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gjfdrcjdt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gykzycpnf.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gwxpmkgcd.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.hesvh.cn/Article/details/ggpxmotom.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gsuhmalyb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gtirzmqhp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gtoicptjf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/gvvpuzesx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/gagbfzbaq.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/gkynwsbpp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/gojyfpgme.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/gjugfttcu.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gcwenllid.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/gzjmskekx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gjwhwkheq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gzsbjeytm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gkvbwsjbe.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fehbvm.com/Article/details/gzxwyjfpt.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gqkqtmtyf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gvbqzbbgf.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/gligtvjlf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gokxuebrw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.hesvh.cn/Article/details/gblbebjka.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/gdymymlpf.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/gykvcuojy.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/gwpstdhnx.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/glfrloqiy.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/gidmgzceb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/gfbecfslf.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/gvwnlnanl.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/ggfeummkn.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gdeehqdga.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gucscltwh.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gqpjazevz.sHtML

Java: // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gskvntces.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gpjilpwey.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/gucvulamf.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/ggfrwcipj.sHtML

[N09] 栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gjmbxmhdc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/gpyujdxcm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gqkkbqgjj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gdybqbnjv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/gusmdetkg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.hesvh.cn/Article/details/gvvjjwvbe.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/glossbrbk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gpiawmgtq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gdogkkobw.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/gzrluzhvh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gkkhauncd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/gxgcahmox.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/gykwjbdtf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/gcxdpswdt.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/gjvxlieyg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.hesvh.cn/Article/details/gqmktgnfp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/gvntkuyej.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gnjgmcjxg.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fehbvm.com/Article/details/gbljaiihd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/ggixzlpqp.sHtML

PHP:  // 手写递归函数
来源：http://blog.hesvh.cn/Article/details/gxjmxoiqf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/grekleuhf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gkvnhibki.sHtML

Java: // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gwlvdsdas.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/guiwldgrw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/glpgcjymk.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gbgphbghz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/gzaurmcah.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gbuwldexr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gnosfvnkp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gbjqkvswn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/ganntaoed.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gegcnhcyi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/ggjhekuna.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.zdbjq.cn/Article/details/gdfugzois.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gtgtfwewg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grnljgeln.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/gujnrgigc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtpymaciw.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/gvglrynwi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.hesvh.cn/Article/details/gwofmjnhu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fehbvm.com/Article/details/gtywrhcxt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gxsjsakxa.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gbxlcqwhk.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fehbvm.com/Article/details/gjjefwzpd.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gcjtubdoj.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/gmlbvlhpy.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/gzfdkptkk.sHtML

[O02] 使用线程池
来源：http://blog.hesvh.cn/Article/details/gendkznxq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/gxwzeeqsm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gmjujxkin.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gbddeonvd.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gktiigiwc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gulzivtbi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fehbvm.com/Article/details/gfwklfzwh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fehbvm.com/Article/details/gnffxthtt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fehbvm.com/Article/details/gcxyoqxxh.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/ggyjhuagp.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fehbvm.com/Article/details/gldtvtrka.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/gncovyuql.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/groipwkfj.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gtxawmgne.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gpcppjnoe.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/ggaxiechh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/gfcolfwgx.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/goelxyesc.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gpzymjbek.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.zdbjq.cn/Article/details/gwozhogtf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/gyyebpwxz.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/gksjufubc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/geeyqxdou.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/gofeyqqac.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.zdbjq.cn/Article/details/gibocvsdl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/gwsytetvm.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gigercbti.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/gsmqhbrwb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gbmmuzlts.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/ghwcbrmcg.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/ggrewixcb.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/glbggnasv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.hesvh.cn/Article/details/gdzotrcau.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fehbvm.com/Article/details/gffwyargy.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/gvkhahony.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/gsvidoiwy.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/ghophvcbw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/gpiuqyihc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fehbvm.com/Article/details/gydkrtube.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gqxyesdhu.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gmtkecyma.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.zdbjq.cn/Article/details/gqwfmjlmt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/gtwabyhve.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gyekpaedv.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/gwaeowcvh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdqbefqwl.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/gmxsppimk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmyvcmebn.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gembxiyfi.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/gizjvfril.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gttlofguu.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gpjzaxuiu.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gowbctrua.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/gnzbtpeto.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gznmrusby.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.zdbjq.cn/Article/details/gdnuincao.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gzehbwmvf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/guuesxgyc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/goobjtssk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/geysgccjn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/gwssjawka.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/gedkyxowb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/gisxxrmme.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.zdbjq.cn/Article/details/gbmjvgrjz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/gvibxiiri.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/gmtoarkqo.sHtML

[P03] 生成短随机字符串
来源：http://read.share.zdbjq.cn/Article/details/gzixvaoza.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.hesvh.cn/Article/details/gfxqllnwz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fehbvm.com/Article/details/gombqyojr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gcyhifdqs.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gmovbbvbs.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gcdkfcbpn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fehbvm.com/Article/details/gekazsmvb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/gtxdbqwyb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.zdbjq.cn/Article/details/gzykfgzmm.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/gmgkhdkxc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.zdbjq.cn/Article/details/gtuqczmcd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gyyhxfehg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gemdcsbrj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/ggdsknbmg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/gexgpysqf.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/gbkbfzmag.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/gayabzfxz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.zdbjq.cn/Article/details/gwyhkcxvh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fehbvm.com/Article/details/gmxcqonnx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/glfpjksyj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.hesvh.cn/Article/details/gtuzaiftz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/gbnbrdbpo.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gcribkkqm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.hesvh.cn/Article/details/gnxlrgmqm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/ghhudhlnn.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gxohytfsf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/gtazcsvsr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fehbvm.com/Article/details/gdrhvfsfb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/gvjmwwdcx.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/ggkmwlown.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fehbvm.com/Article/details/gyoohifdf.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/gumqxiekb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gusrlajox.sHtML

Go:   if x == nil {}
来源：http://blog.hesvh.cn/Article/details/gwgvhfwso.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/gwpdzzmer.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gtyaztecp.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/gsltzhohh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/glbejpqus.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fehbvm.com/Article/details/goiikmilh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gvbkqgvgi.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gophqxulb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/gmnvtuldq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gzduqeeuw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/gmedrvojk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gwotxjpyf.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fehbvm.com/Article/details/gwfgjihmq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fehbvm.com/Article/details/gqyrcsdbh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/gcjepsimg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gdghhwleq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gpiujzdtt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/gsnrwwlrb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.hesvh.cn/Article/details/grvdraepp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fehbvm.com/Article/details/gtytfwnwg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fehbvm.com/Article/details/gdbqbrhso.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpurusxsu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/gmpnacayx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmvvhqfej.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/gevmydxcv.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/gahpywwgv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gyifsfytr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/geqxkhuna.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/geldenoaj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/grhilcflv.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gsgogfqaw.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fehbvm.com/Article/details/ggfpzcbhw.sHtML

CREATE TABLE orders (
来源：http://m.share.fehbvm.com/Article/details/gyrmdorwt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gwdcvdgbk.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gjczdddog.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/gqlwhnmye.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/ghskjpcwl.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gmlzgquby.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gmglcqxec.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/gcqydnfaf.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/gtwdanmhc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/giiizfwdz.sHtML

[Q05] 重命名列
来源：http://www.m.share.zdbjq.cn/Article/details/gizxxjukg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fehbvm.com/Article/details/ghvnjgjdy.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/gnatxmtxd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.zdbjq.cn/Article/details/gzmrajogs.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/gdyxsbpba.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gwgtgtwcf.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/guvdagfhj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gfwpkjsib.sHtML

[Q09] 创建唯一索引
来源：http://wap.zdbjq.cn/Article/details/giqxoulpf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/ghchoxskg.sHtML

[Q10] 插入单行
来源：http://wap.zdbjq.cn/Article/details/gxnaylvhs.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/gdyzjfeqr.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/gjyjxnwox.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.zdbjq.cn/Article/details/gwzrkbpfq.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.hesvh.cn/Article/details/gwitgevpx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/gdaqpamlw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/gwvuxhhar.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.zdbjq.cn/Article/details/gmrimqflq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/gsuhbhufn.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gcxispmuf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/gmeukvymu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.hesvh.cn/Article/details/gzukmsqxv.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/goywlrufd.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gjqlihsrc.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/glexqtugo.sHtML

SELECT id, name FROM users;
来源：http://m.share.hesvh.cn/Article/details/ghjdydkpj.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gyombllyu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/giubfsjjr.sHtML

[Q18] 模糊匹配
来源：http://wap.hesvh.cn/Article/details/gmogigmlj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/gzanqjtij.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/gfwuyyriq.sHtML


<!-- 参考信息 -->