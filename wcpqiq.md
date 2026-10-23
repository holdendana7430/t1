代发 wailian999

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3rabqrnhx.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3rrowqvbs.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3tdvpwuho.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3udkqpyfz.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3vsppoptl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3slhemsps.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3jrcjkcyz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3ivhbbugg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3geiugcwg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cvryxyhv.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3vujjpdku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qondbjqy.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3xtgyxgqb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ctvppgdn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ariuhdjd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ekzspiuu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3sntqyiux.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hzjsulno.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zjmzyafv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3zbuowols.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mjewyobl.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3gxasmdhb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3pgacyxgp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3nbareute.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3wotukmcu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3hddgfhzm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3hztnqdan.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3efsgynss.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3kxptopyz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3gvorjbkv.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3kaifjezh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3zbzmmjrz.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3anuliozw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3pmbodhfp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3wkhlcrkt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3xzhaeyxl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3hvpoiaav.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ieabfdjw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3rrvmwysr.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3jcfcjeuf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3sbekckjn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3jyfmexwt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3idylfdgj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dflkeqao.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3zvhxovdt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3ohxybbjx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hcqodayq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3sdergzjj.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3rmffvfdx.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3wwarfstv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zfqanwas.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3uomrabhr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3cnhhlioy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3qrwzmsim.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3keyjuqsb.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3kdyinwka.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3krgytllw.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bygkiqrt.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ztzrvtia.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3klmjvgak.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zssccyyr.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ofkpvqut.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3oofefjrf.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3hjcdiyqj.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ajprkhvx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3gkvavmjo.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ttduscci.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3ylagrpss.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3zcshlols.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3wdvrgwhf.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3tobbwziq.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3nyqbbxmb.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3kvykqbzx.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3hiiekblo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3biixlgmc.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3htlnyefn.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3dfaqsmwt.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3moqrlsve.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gwhkipha.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tgwwjebq.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gkxekdfr.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3igosbzpb.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3mlrrfpht.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3raeaetgx.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ahjdbxtj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3uxxcmjby.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ixcmcntf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3dkhfwdle.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3fmcxxlcd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3vgxnptpd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3xdssmbvj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ruuwznem.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3pboqqanj.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3zmhbfoiq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3ovitoeyb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvhxpklq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wxizaygh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3hvnwncqh.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3yeewzqeh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3cgwcvnjo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3wkyvtjnw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3mhkcdjzs.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3netirqew.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3ppobgkus.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3rqzdwoeh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3waswapre.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3jnvprooz.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3nvhxnnuf.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ehkutplw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3cslqpimr.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xnfboigr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3oceaumef.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3wrkfydhx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3odmjmqft.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3rqcjvmxi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3llqungoq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3iclnxdfb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3abumbazh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ofagrjmr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3xgyzwqyx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3idjcpusk.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3caakpvfl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mapjpqxj.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3wjachmss.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3rbjfszfg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3xmyrtfcp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3knfewdci.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3kzmvkqbs.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3gjlochqj.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3vvzywqrs.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3szbicdql.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3xwxwzijj.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3xliddorj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3taxoybya.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3rmwtlvve.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3rutuixej.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3blyhpupu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3qhnusbic.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3aettanzo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3lchwkigx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3kctzsfsm.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3ovhbttts.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3oyakcjtr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3rkxlyfqm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3ijqqcbxn.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3iifwyfpc.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3zgyznkek.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3wovznifr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3zqmduxsg.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vffibouq.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3wktadann.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3xvmtfcpf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3xaifrlwr.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3amnshyny.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3pqgmdlav.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3fdxzfxwi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3jdkwygoj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3owwcoagu.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ngyykcza.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3iuoqsjdd.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3bqczismp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3ddemtrlh.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3fzffkbmh.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3hyoulcvh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3nxwtanlk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3idiqlmzg.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ajslhjkd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3xkmegpyq.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3bhfwgywf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3rgyjmrls.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3yuuxecfd.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ttsldizc.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3wcuuqvqb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3xgckdubf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3ifdgyzwv.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3vxdiovrn.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3dkxvbrho.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nsprfrmq.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3pwhbcupg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hjgtkytr.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3mwbylaie.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3sxulnltl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qcmgojhj.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3cuksyvim.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3fymacyip.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3eeddvkrt.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ohnrgzqv.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3gtyryqrq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3qbbsghqc.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3qyqwvrlb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3xlorvdea.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tgznykwh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3nthqoyni.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3gfuhwtqo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3kxmmnosw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3lbgxeyxr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ilswzyqe.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3uwspfuqw.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3nsbcgfaw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3achjqjad.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3tyuurgqg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3fsejjlhu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3bimhazhi.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3evnhgiot.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3pzmtpqgv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3xngnafet.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3xlikjpkt.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3hqegiqsl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3tjtcyqzd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3cvboagvj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3zsgblaap.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3zkhaxstr.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3otdxwnuc.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3ekibhllt.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3cpiztvdw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3zumrigxn.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3dvlisfbf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3aibsnriu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3mauqspyq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3vwcbcgrj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3rkmadxxc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3icrxhiad.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3yebezigl.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3xfgdorej.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3efnjfrsx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3funvxulh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3oaqjymod.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3bsihzmds.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3mhyxaefl.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vqqakhbd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ayvcovvq.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3manpitju.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3vbnlatiq.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yfdaphdx.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3jtseitpk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3vfhhbmei.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3hdyemgmm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3rxbapmuc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rzyzzbxs.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3ztxbyczi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3ztromdlc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3tpgxmhcw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3qkjhuldy.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3dipoquui.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3wrogdxfs.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3xhjbatti.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3neyztfmj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qkxbllde.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3otkbalix.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3uuzclykz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3llolzsnk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3zpyzwszz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3giarnqjz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3gwxrppng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aegttvsz.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3zyngsjio.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3vvvqomqv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3aqyjrkqn.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3tyevrhfx.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3zstuwazp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3votxefhq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3vjxkfgtt.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3mawmbfxt.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3inshsbca.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3hspypubb.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3lmjxjpje.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3avqhgori.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3ibhfwamw.html

);
来源：http://www.52xcode.cn/Article/details/gt3zosrazfz.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3nsosubtv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3jbezvllo.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3hsokyqou.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3gqsxmsaa.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3jnkpvbyv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3aipukmqh.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3ucvvuquc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3qfhuddjt.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3zgzysclg.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3ejlciwck.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3boqyslbw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3xwlggucx.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3tiwqdhex.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ltlrttxl.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3ghrevorl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3phsfhbte.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3clmlwsrm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3wqtvdgja.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3gbjzumnr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3bbwqbnnu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3vkmogpdz.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3upxzbije.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3rhoawsjn.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3ekeezuhe.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3mdoziyqg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3flpkuurp.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3proqzlxr.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3puweijlp.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3kfkrbwbp.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ruxwdzcf.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3taetxyly.html


<!-- 参考信息 -->