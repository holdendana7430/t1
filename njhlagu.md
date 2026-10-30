代发 wailian999

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gfezcdktz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/gkjtdeujx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/giwnrqgii.sHtML

JS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gngtkoymp.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gmxbylmfp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/gvhgbyndv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gyqqweszt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gkmabykab.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/gxifbemgk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gckjqnppc.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/gbtopmjyb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqedkpvph.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fehbvm.com/Article/details/gjmyjmwwk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/gjzfkpork.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gcfrokxax.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gqxcsrdps.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gmwtxtqki.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gzwffsixf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gsdrzyykz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.zdbjq.cn/Article/details/gnnpdawsp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gyjjrzcjr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/ghlgorvvq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gdysheayv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/giihhkklv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gkwmqyhee.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gsrymnwyt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/gkkxpoifi.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gjtazqdqy.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gclmwrcwy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gwjvpaqxw.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gtcvaqurs.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gwewqhsuj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/gxbnrdnzi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gecwgfuxx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gkifbyrnc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.zdbjq.cn/Article/details/grsnseftu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/gmbumgews.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/gtsvdlirv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gdfcyunnn.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gxukuslbi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/ggtmfkqzy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gbmtqtbsh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gmqbxpvsu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gurqgzgep.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gefyanuil.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/geguynpeh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gkxcvtysg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gjohbbovu.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/gxogjudir.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gkukxbbay.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.zdbjq.cn/Article/details/ggmlyoatt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/giptuiekg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gzumddxtt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/gkihitxjk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/gmbfurtwl.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/gixmnophi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/gvshakbqs.sHtML

[N06] 判断回文字符串
来源：http://www.share.fehbvm.com/Article/details/gzatkfqea.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gibnrbagt.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/grozhvsqj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gkqykjksh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gasthwpho.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/glykwibkf.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gsfdtnqje.sHtML

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gjqkhgujl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gsnymdbii.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/gfqcbupmi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gqfqzxdao.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gaiatjkre.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/gfmtwetit.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/gvgetuexe.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/gzbomollm.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/gybincqpv.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gnnevqpgg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fehbvm.com/Article/details/gqpeoyuue.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/grscwdcdx.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gldncvdbk.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/gjixtwlrv.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gwglcsbiu.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gqxtsuvxp.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gypitehfr.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/glsjbwevy.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gsoiaechf.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gnjoaatkm.sHtML

[N09] 栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gxscphjyw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.zdbjq.cn/Article/details/gndbpzxnk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gkzfyrxrw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/ggbjuvmbz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/gyxhltilp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/ggsxzgnfd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fehbvm.com/Article/details/gtnmjhtvp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gemtclnlx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.zdbjq.cn/Article/details/gzpxybmzl.sHtML

[N10] 链表节点定义
来源：http://3g.fehbvm.com/Article/details/gnvoggrrf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/gjzmdgmax.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.hesvh.cn/Article/details/glcqtygbq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/gcpzintsj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/gwjxyejwc.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fehbvm.com/Article/details/ggoeyojtw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/gxrrrrfft.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.hesvh.cn/Article/details/gzrzbqdzn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/gkzuwfomd.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/givjrwtpr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/ghgbtpzyu.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/gkxncqvyt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gyioxwxrq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gcyamfhgo.sHtML

Java: // 手写递归
来源：http://baike.fehbvm.com/Article/details/gtxoibter.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/guaedgujf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/gdjlextot.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gxxcqubwv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gqblfpojs.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gokkhlspm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/genqtbbua.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/grwkzukol.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gqdgikfon.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/ggabgxxzn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/gyknsyjpf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/grrfdeoqg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gyaktxgen.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gywfiugpr.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/ghswopnnt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grlzeehxt.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/gfpvqsnnh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.hesvh.cn/Article/details/gikivflym.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/glacffvtl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fehbvm.com/Article/details/giruuhnrl.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gnttuguhc.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/gebnbyzqi.sHtML

Go:   go f()
来源：http://www.blog.hesvh.cn/Article/details/glplmberg.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/gouojkmyo.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/grfyquvfj.sHtML

[O02] 使用线程池
来源：http://www.share.hesvh.cn/Article/details/glbinqddl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/gfeihaufj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/gmnrprkhg.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gcboaqsnm.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gcmnejhxo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/girbkxiot.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/glnqxwiwx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/gybmdubnp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.zdbjq.cn/Article/details/gwjtuvccq.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/gkidjbzrd.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gegnaqxfz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/gkdtzzjyr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fehbvm.com/Article/details/gihvekvnl.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/grudvjwhl.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gugjzuhqi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/ghzhdoaom.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.hesvh.cn/Article/details/girjegdso.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gburcutnj.sHtML

[O04] 定义异步函数并等待
来源：http://blog.hesvh.cn/Article/details/gidiysdtw.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.zdbjq.cn/Article/details/gsigrmzvm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.zdbjq.cn/Article/details/gshhyhtnn.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gokpbpdkk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gpaetxjuj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/girpmiqkr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/gznraurxw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/gtkfzbnfy.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gisvbfiok.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/glzrjzufg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/gkakmyrqa.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/gtrakzmkh.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gvdgbxqpe.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gggwuzcaf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/gcymiphki.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.zdbjq.cn/Article/details/gjatpptgu.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gklnzdazp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/gczeswudu.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/gdpnxsvoo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/gupwissgy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fehbvm.com/Article/details/gnnrmfshm.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gggcnivwj.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gruioossj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.hesvh.cn/Article/details/gyqzbaxfi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/gbgyolbfo.sHtML

Ruby: // fork 块
来源：http://m.share.fehbvm.com/Article/details/garcuufub.sHtML

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/ggeajatgo.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gsiphgzjq.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/geiwuuevg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gckdkmvnp.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gvapubsev.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/gdfnkzvam.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/gqnnewubm.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gpmsijrtb.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gwloogsdm.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.zdbjq.cn/Article/details/gavevcuqf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/gvgnulflq.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/giyosyznx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/gyfrebtwr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/gpktrrzfr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/gabfejzgy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.zdbjq.cn/Article/details/guoackxkc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gwaxvfjuh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gfeiwseme.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/grbgdjoys.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/gpginbyow.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.hesvh.cn/Article/details/gpqxaxrsw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/gaaavglyn.sHtML

[P03] 生成短随机字符串
来源：http://www.share.hesvh.cn/Article/details/gxftmuyug.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.hesvh.cn/Article/details/ggafhnycj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/gcouivmbw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gsxcawrjb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gjoqmzimc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/guphbclgw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.hesvh.cn/Article/details/gkyjemlms.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/gdtyulbte.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/gnrvnsofc.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/gcmskefqn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.zdbjq.cn/Article/details/govyugsoz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gaymbisqa.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gbezocjtj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gpqgndrds.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gpqcpvhzm.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/guppxqgam.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/gsjnyhwpp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/guwjvlezj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/ggehfvwgs.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.hesvh.cn/Article/details/gszoxkjik.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.hesvh.cn/Article/details/gbysutjtz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.zdbjq.cn/Article/details/grzcyoufn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/genrwmych.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.zdbjq.cn/Article/details/ginoepiyz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gdmtgtogg.sHtML

Ruby: a == b
来源：http://www.blog.hesvh.cn/Article/details/gmvogoglm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/gmeezqbwt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/gwzajgzuj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fehbvm.com/Article/details/gxsfgjkct.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/gbezecdla.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/gpalnbpbg.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/gfagqxarg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gunuzfryt.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/gaxpctlrk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.zdbjq.cn/Article/details/gesnuryzg.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fehbvm.com/Article/details/gyrtihhxu.sHtML

[P07] 防抖与节流
来源：http://wap.hesvh.cn/Article/details/gonqxxgvg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.hesvh.cn/Article/details/gezyjwwkb.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/gmyavpmrc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/givuigtii.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gcaexiwdb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gtkladnor.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/gzpipwawx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/gcmozbdrc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.hesvh.cn/Article/details/ggjefcwbd.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/gqjisfsye.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.hesvh.cn/Article/details/gohrbdxae.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/gkwhhtowl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/ggnbkmjay.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/giwmbxwcv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/gflseywcd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/grkxxzuaq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.hesvh.cn/Article/details/gkitveuog.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fehbvm.com/Article/details/gudsdxiha.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/getkdrmoh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fehbvm.com/Article/details/gocahmgeb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkkbwwiqe.sHtML

[Q01] 创建表
来源：http://m.share.fehbvm.com/Article/details/gelypbcgs.sHtML

CREATE TABLE users (
来源：http://wap.zdbjq.cn/Article/details/gxmhywmkv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gvgccbstn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/ghfugfqom.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/gkdvimzwp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.hesvh.cn/Article/details/gwwsfvhbq.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gunxlzyrk.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gjlgqcdzy.sHtML

CREATE TABLE orders (
来源：http://www.m.share.zdbjq.cn/Article/details/gzvxwxaob.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gbblffwit.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gmntxjaxr.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fehbvm.com/Article/details/gzsfqeqsd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/gptcbhhyz.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gybxyptmc.sHtML

[Q03] 增加列
来源：http://blog.hesvh.cn/Article/details/gqzirqadx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fehbvm.com/Article/details/gxoqxwrzb.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fehbvm.com/Article/details/gwiwicave.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fehbvm.com/Article/details/gjdtklpex.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/ggaddpeqh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.hesvh.cn/Article/details/gbuowwczi.sHtML

[Q06] 删除列
来源：http://blog.fehbvm.com/Article/details/gpkuqxqiu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fehbvm.com/Article/details/ggwqjgoji.sHtML

[Q07] 删除表
来源：http://m.share.hesvh.cn/Article/details/gwjtmnavr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fehbvm.com/Article/details/ggocgqefx.sHtML

[Q08] 创建普通索引
来源：http://baike.hesvh.cn/Article/details/gsxvwpdsn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/ggbboegra.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/gtpffiplb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gqscowckm.sHtML

[Q10] 插入单行
来源：http://baike.zdbjq.cn/Article/details/gawquvqfk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/gghnslzev.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fehbvm.com/Article/details/gkhaaijes.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gevpllvtk.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fehbvm.com/Article/details/gkphlyyba.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/gsiuhcuvj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fehbvm.com/Article/details/gxnoitnkr.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gbbzbaeov.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gaeqsmqzi.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/gowtwrndo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/ggzdfehvi.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/gvolaqqzv.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/ghdphvpdf.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/gjxeppmrh.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/gjbwsknzp.sHtML

SELECT id, name FROM users;
来源：http://wap.fehbvm.com/Article/details/gybkkxotj.sHtML

[Q17] 条件查询
来源：http://m.share.zdbjq.cn/Article/details/gughvweii.sHtML


<!-- 参考信息 -->