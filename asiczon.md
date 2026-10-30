代发 wailian999

[M08] 获取系统与运行时信息
来源：http://m.share.zdbjq.cn/Article/details/gzbfnuowl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gennizatd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.zdbjq.cn/Article/details/gwulpzysy.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gbhiydxnn.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gyzglkdzw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/ghlykwzir.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/gajhxyptn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.zdbjq.cn/Article/details/ghznhmcjc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/gvzezavgp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfaweqprs.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/gkaqfdath.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvsoxinkh.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/gbqaokrgt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gcmwrgrxf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gnxsaifis.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gvqbgqvfp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gsyqwecid.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gwivgsoah.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gptbttnjm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/goxwxeipb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gdgeqpjbe.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/gxrrokbxx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gydwarslm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/gzssojtfg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gmnpxssfp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gnzjgqpcj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/gglemjbkl.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gzwtqcply.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gjnqmzbvz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/grxqtcxat.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/ggsjkilbd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/gzjnvrejp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/gbpiyvkxt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gtkkuwrat.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gnvbuoeuh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/gairmghni.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/gktgxtomk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/gruciciai.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/gpodfwqsg.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gyxhbrvgn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/goonadcto.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gacnprroo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/ggkgkcsoi.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gplvkuwrn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/gqpajevfj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/gnumesijf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gvidwgeoo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gprxqmael.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/grsxfpwhr.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gqabinzwu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/gibyhikyn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gttqmwgtg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gcheivnrp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/gojwxkmkp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/gmjbizxdy.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/ghhtkrlqj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/gtodcoaat.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/ggufigdfe.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/gjrgsjzbi.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gfnofwbao.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gvioluzxt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gtafpjeen.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gatlqwaov.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/gylkgeyxh.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gzqkogrhe.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/goyqkzbip.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/grabyuypb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gbksgtioo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/gjdtwqcly.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/gvbdkvqad.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gyufvmfez.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/grmcqwdeg.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gkzrbpypp.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gsnczgpxr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gkgxhhtkp.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gvzwcuaah.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/gokampvpa.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.hesvh.cn/Article/details/ggnisvehx.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/guimdojcg.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/giaaumacp.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gdtsagslf.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gwjwvqtll.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/gcnkoptct.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gsmvbkbyz.sHtML

[N09] 栈与队列
来源：http://wap.fehbvm.com/Article/details/gegzddpgr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.hesvh.cn/Article/details/gnpvclmjm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/ggyfrvtfn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/ggwwtpdch.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/gwfsutnzn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gxatbbhzl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/gawysanzg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/giwtfkrqo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.fehbvm.com/Article/details/gfdbxrkyj.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/gdwhsmjjq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fehbvm.com/Article/details/gswenjfek.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gilpgpdxp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/gtdfxfzdx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/gkduzreoz.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/gsqrcwktf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gwknrxjnj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/gvceeflbg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/gjmisvhaw.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/gkcvuprfg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/gjqeuwxzc.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/gewjkxdrz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gizvaagew.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gwsgkqqdo.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/gimtraoxc.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/grqgvhpol.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.hesvh.cn/Article/details/gjhimarps.sHtML

C#:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/glhiwljzm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fehbvm.com/Article/details/gfumssaub.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/gbrjrgppu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.zdbjq.cn/Article/details/gjeqxjcam.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gjspzsnuk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gsyvirrkn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/ggssjegzg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/gqnovqexb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/gqqvplchp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/ghtmnvfnx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkmyehncd.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/gqbmzhfzf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gduayrwss.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/grlrheify.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/gaehpevcg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/geisqlbur.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fehbvm.com/Article/details/gmkymgysf.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gzeugfkqe.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gggtjwwha.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gsshnalcu.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/gpmkpvpap.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/grjfyvvbe.sHtML

[O02] 使用线程池
来源：http://blog.hesvh.cn/Article/details/gjfbrnmik.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/gmjbhnuao.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/ggthvhhvj.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gcgtidpsc.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gdpxnyclc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.zdbjq.cn/Article/details/gkqzenlbf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/gghfnxiyy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fehbvm.com/Article/details/gnuvgupcj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/gccvrdidj.sHtML

[O03] 加锁保护共享数据
来源：http://blog.hesvh.cn/Article/details/gdqroynvb.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/golscnnmx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gdrxhsasc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/gyceftnps.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gtgpcqvzs.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gjqnpdhrc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.hesvh.cn/Article/details/gaarhufhw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.zdbjq.cn/Article/details/glouwbwgi.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gbtmaatdy.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/gconwhkdp.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/gqbjirksv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/guonjxeix.sHtML

JS:   async function f() { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gozwkrpfd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/ghvbrsyow.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/grgjanmys.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/grljuqxoq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/gfuqanqnw.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gjspbqpag.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/grfqwqrmk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gjhphimco.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/gsxexxxhl.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gdumkfkum.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gvtspsqoe.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.hesvh.cn/Article/details/gilvjkweh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/gkgyqfknu.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/glytygyzn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fehbvm.com/Article/details/gfzhgwxaw.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/gzyswrore.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/gqsvtglhf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/guwkqosfi.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gmiybazrz.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gouzvhkbs.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/gfrsceaor.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/guqygabki.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/golbqcvnc.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/ginehtzum.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggvopfybp.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/gyptfubkc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grzonpltr.sHtML

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/guhnapckq.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/grqojajxj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/gnvxavlac.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gjxadnzty.sHtML

TS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gmkuswkrv.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gkiegbhzo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gloitohlu.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/gqeceltca.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/gfyhrhnpe.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/gwidgwtmy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/grddinpxm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/gbqojjeyz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.hesvh.cn/Article/details/gqncihefs.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/gctgrpyby.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.hesvh.cn/Article/details/gyjtmgauc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/gaxhnkyke.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.zdbjq.cn/Article/details/ghekgihko.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/ghxhdcvkn.sHtML

[P03] 生成短随机字符串
来源：http://read.share.hesvh.cn/Article/details/gggmqshaq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/gcuwuwxmt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gojqebelc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/ggnlrzbwa.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/grdxxyobf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gxjollzao.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.hesvh.cn/Article/details/gbzloorki.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/gavcarlxq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/gvptsyxhu.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gpuidlbmb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/grwavypdc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/goberfvyf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gciwscxmo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/glhgqxseh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/gceiahhdb.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.hesvh.cn/Article/details/gkswxqnga.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/gypfsvbyb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/ggiofurvg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/gnbftpxll.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.zdbjq.cn/Article/details/ghpakgydq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.zdbjq.cn/Article/details/gryzrlgfu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.zdbjq.cn/Article/details/guaybmddd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gahneoumk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fehbvm.com/Article/details/gylorbgtf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/gaqgvhbqh.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/gxqzlnvcr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/gbvknmndm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/getineypz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fehbvm.com/Article/details/gbktejzuc.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gommrccnn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/gjxmudwas.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/gmpmficma.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gqerppchn.sHtML

Go:   if x == nil {}
来源：http://www.share.fehbvm.com/Article/details/gjdhcliif.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fehbvm.com/Article/details/grmkeekbv.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/ghfkszqic.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/gdxpgusvw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/gguzjyllo.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/gdryvqivm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gltkzgfot.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gxizavkfh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/gmdxjbkpa.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.hesvh.cn/Article/details/ghaewhond.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/gcvkterha.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.zdbjq.cn/Article/details/gneeranag.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/gzncxjssd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/gvhcquudq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/gbdufgxeh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fehbvm.com/Article/details/ghzrkyngx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/ghqkydgts.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/gjajokygd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.zdbjq.cn/Article/details/grnlygzyg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/gesxfjoqf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fehbvm.com/Article/details/grcibswsu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghyzgyovs.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fehbvm.com/Article/details/gggldexdh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjvcehlrq.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/gwlrktfva.sHtML

CREATE TABLE users (
来源：http://read.share.hesvh.cn/Article/details/gfxoyiugk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gueckowno.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gkasuxylb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/gawelnrel.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/giokukopr.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gizreretg.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gjlkfemnd.sHtML

CREATE TABLE orders (
来源：http://baike.hesvh.cn/Article/details/gdumsrjct.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gkrqcfkkv.sHtML

user_id INT NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gpstkbpum.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gqnzlgpdi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.hesvh.cn/Article/details/gtkaajuym.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gcjjozfjx.sHtML

[Q03] 增加列
来源：http://wap.hesvh.cn/Article/details/gkljanwby.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/ggnqdpxdu.sHtML

[Q04] 修改列类型
来源：http://www.m.share.zdbjq.cn/Article/details/gainzrxpg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fehbvm.com/Article/details/gwzkqsiug.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/gmbmuoejg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.hesvh.cn/Article/details/gvkktcrnn.sHtML

[Q06] 删除列
来源：http://mobile.hesvh.cn/Article/details/gepodutrp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.hesvh.cn/Article/details/gjpdpnzda.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gxpbpbbgu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fehbvm.com/Article/details/gxooezzza.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/gybtspcoq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gyzggnbvl.sHtML

[Q09] 创建唯一索引
来源：http://mobile.zdbjq.cn/Article/details/gskntjcjq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gzfpqogux.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/gkjggucur.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/gdpmccuej.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/gkwbvefbq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.zdbjq.cn/Article/details/gzvbxxlps.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fehbvm.com/Article/details/gklaspxyw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fehbvm.com/Article/details/gmagbrqql.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.hesvh.cn/Article/details/gqvknlxny.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gwetlpjjk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/gmtbcisma.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/ggrgwjszy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/gvilztxhj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.hesvh.cn/Article/details/gcnzugtta.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/gbosyxtcg.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/gsjxqxlxw.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/gupzcpsfv.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gebzorxhf.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gobyoneum.sHtML


<!-- 参考信息 -->