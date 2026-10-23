代发 wailian999

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3jawpaeie.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3noysiudr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3sybdsrfi.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ihxbrvlm.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3xexlgpjo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3gdlbbtpt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3sjbkbjbv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3usnjfgdg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3axotlgqj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hlzknugp.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3zuobzlym.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ysykhzfk.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3bzngragg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3azwiyyhe.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3wobzmiwg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3clljjjhx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3klonqtsq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ptiqidsb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gzxepsvw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3ytlvcrue.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3swghmjdo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3tdfinaxs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ttckhpiy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3dqdwrzgp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3idabdqkj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3wlesaeln.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3gzgbzzwg.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3helxpeow.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3vjktdqrc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3bkbpxvgd.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3byhonnrq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3rygatbym.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3qcxifmvo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3oruuuntg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3bwufyenq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3trwcexib.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3lhmhexjr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3umttibot.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3pkunecvk.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3uqlslhtk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zjvmtdrw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3pkvcwzzu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xamzoxcg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jypevksp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3pnslfobc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3kmainwzn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bwaxiqrr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3hcfnjyiu.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3abwxywvq.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ptoscjyb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zbqlvswx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3zfaxutel.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3cskafdyn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3cxwfywzb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3rkzvhejs.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3gsevjjpp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3bgaztsdx.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wafbbzeh.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3fznlpnvl.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zayealkx.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dsatidwb.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ogihydxl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3yuyzdapb.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3eqqpcrjo.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3rvlwpgcp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ihtmomik.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3qepiveax.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3xgehkhmk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3ljowhiyb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3yowqdybf.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3hwuwmkmh.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3chomjgwa.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3fzypbcvt.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3uzfejjju.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3klnxcsvx.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3zpneldqk.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3eheetejx.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3axqwptzn.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vwlsdpcf.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3owtzolxs.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3eeicdxyc.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pmwqxqjv.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3idogjtfb.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3logbayfy.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3jwojghcu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dwyfbnsc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3xtwwrmky.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hdddobxr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3enumhxfu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3deebxuvm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3bsljrcem.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qgipdsds.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3occdbpuw.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3vzoaxhkl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3ewjwbelg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3lnbnubal.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3eyfsbfnq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3vcoqgdhj.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3gzoeeyfc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3mowtwrhi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3lkairxrr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltnnwtev.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3jjlaflau.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3ujrmepsg.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3pskilpan.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3sgfoegxd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3hksixfxt.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3emyiytxf.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xyxakaeo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3evcuwmmv.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3lzowwury.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3ohikgooz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3zbpqoqqd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3faetulmu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3arwezypz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3sxlaotbq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3nafxiipq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3fhnjgbui.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3avqcptol.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3wcpwjlmf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xkjomeca.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3fvbsuitc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ckrdbzqx.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3kfnsesdi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3secdbyac.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3enkvgvev.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3hqttjnoo.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3zzbdszoz.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3hlbiqitr.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3rfnxdxoi.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3yvllylru.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3htobiowp.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3vxrocgcc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3bcfvyrcp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3ddxvsnef.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3atajxyem.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3dkokbxkj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3gfwsiwyh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3vwcdcxpo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3opmqykit.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3eidclxhi.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3luqcigfj.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3jsnswqmr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3rzygpozj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3umjkonzd.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3bjnvojrc.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ddvuprzq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3izgwlkuo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3grrsrrhi.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3bwvoksvn.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3ascmftmq.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3pmsfymyy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3gtascuot.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3puijpeti.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ejbfbezo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3sjuojvpt.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3uagslihn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3rzrbjfqh.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3zhwumtfx.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3fguspffz.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3ttsqmmje.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3qbdmcsan.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3nbglmhxg.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ecwqdhag.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3kouigxde.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3pszawlfg.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3hsfuyeyd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3oetwdhos.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3alvscpau.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3qvktzntq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3rquvfbdp.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3cixwfgnl.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3vfgjpuzj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ukqsxjjh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3wgmmqjlw.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3qcsowwht.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3qxundaxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ntnhndjr.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3uubdgttk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3thgiubln.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3unjkulef.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3bbmflxwp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3nekpwthg.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3cggdwpgo.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3hkuoqsiw.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3xbyafmvf.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3qdulvtfs.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3cdbcuxik.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3xmtypoab.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3dlkfghsk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3asmfzels.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3ieqiysls.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3peooqgzn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3qpymgpkc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3zeydvemm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3hclcwtgl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3uxmlmhzi.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3hkoqnujp.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3ggwicstl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3ruabzaub.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3yvzarqgi.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3uinuakyy.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3xiqrvsog.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3noeifvkt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3hlsiimbs.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3dgrlekmr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3mipdosiv.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3pxigqcao.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3qxasppxt.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bmkjjzju.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3yngnqrea.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3wmdfltwn.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ztdwwwdi.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3bxjgcoux.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3jntvynke.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3gypdpekw.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3hizulhum.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3ebwlntix.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3uedrewvr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3rhhjtfrb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ogtsnmut.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3tdepcprr.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hrxlukrp.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3wolwasia.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3xaycnpqs.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3jmzwqrka.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3hufjrokl.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3swvxnovr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3fgbamclb.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3fxzvylcj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qbaaxtkc.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3fqjcrvyn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3ckmcvuln.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dvozmmfq.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3tvexzkqd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3dkachhzu.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3yydlkpbh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3uwyxglkp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3hozgelot.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3yhwtdqie.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3fsagpyts.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3jnwhqhcv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3jdjggtgl.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3fhprpgpr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3leiystii.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3ztfddkzm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3mwtvfzgo.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kqpsqyfn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3cdbjdwrf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3ajpjctpd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3psktdeji.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3zhmzzkhg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3evbnyzdf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3opguqahq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wnplnrle.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3tpmejiqy.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3qbrswfwg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ruajpuyd.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3fztawltu.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3gojrukvx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3epjjhyni.html

);
来源：http://www.52xcode.cn/Article/details/gt3dkvlzyat.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3ilwrumzg.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3zpdcdkke.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3zuqjqpgn.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3zhciwaes.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3qbmjqrbk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3lwgqihlq.html

);
来源：http://www.52xcode.cn/Article/details/gt3uxozdcdm.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3eybpjgvn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3utgwjzwh.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3rmssmmke.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3arwafwwf.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3flghoucc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3qzorawyr.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3bwltjtxr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3qojugjjj.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3bhxdtxuj.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rfanhozb.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3drxietqr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3mlqtpgho.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3dgachtgj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3hcfeyazg.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3sbllvdls.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3gwxuuczz.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3uswcsxjn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jgkokbxa.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3tgqdxocs.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3qanrenwb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3tckyemti.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3avppmtnw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3fysdfecz.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3qpzebdcn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3czkoqvyb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3dtqgezkc.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3obbelemm.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xtarpmpo.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3fgeacfah.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hsooumol.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3dhqoxobc.html


<!-- 参考信息 -->