代发 wailian999

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2avgqcifd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2jkscvkyq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2dwvobzvs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2rhbmtprt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2vsbwmwji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bcrdbrix.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2vvybozsd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2crtqqvhf.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2taajlngb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vrynyxpt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2kyludmco.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2veezjgtj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2iodrupja.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hsmxrwcz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cvvyyaum.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2fexfdzkv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2extieszb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2mbkpktml.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2crdlfkrc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2expfqkqb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2exbkuahy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2nntwnqvl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2rcidwvxq.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uoakhugj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2wvallxlz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jwvcdvdc.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2webfopyo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2vvemjqru.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2scyphign.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2llnztipf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2abnshgbe.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2qompiocw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2wbugarat.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2wfensdrn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2cwxqcopl.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2pqdrbids.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2errzozzm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2iupcfmxy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2udystsid.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rlfnqvsp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2krlscdea.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2cmphnlmq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rahkuuyk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2whrtuzrz.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2nwrurodr.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2bejptlza.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmhiyuaf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2byizmygp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2cqaqtnlt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2yyibxbbu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2kzjyfakb.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2gpoviwfa.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2zbqiefps.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bhzblcyj.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2jcnwxnhh.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2cipdegud.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mkhtghru.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lyrevtih.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2qfrohklq.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2gbeksgzi.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2flvyxtyo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2cylfcczx.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2yrvrlijm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2ysaxqpul.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2npuqvbxy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2tqaieakp.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2mqcmojrm.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2gvrgprhu.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2pprlexpk.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2tfwlrmbf.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2buwdlznd.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2pvpxaiuz.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2htmrzsyr.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2ujrqkwvl.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nnokhouw.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ploxaypn.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xjvmkrfy.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ymnzjvad.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2xiomlkfo.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kbtyaeir.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2fwwbhqdc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pvtfoacy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2pfyqcljv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2nebqjehe.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2ufohrbzq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2pdvzeunc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2dwzobcep.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2frtdxysh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2uisqsosl.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2aefovyuy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2myuqzyzc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkamhdat.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2ctyczcdk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2yftmerob.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhgxrznk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2xiueciey.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2tbnraawx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2hpmegfom.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yahlhgdp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2hqerojap.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2yximbdzc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2bzdoruuj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2qskvvavf.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tkemymmn.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qkvsisji.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2sofbbqwq.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2bwnwkgre.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2lnicpdpw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2zglknoyy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2hwehptqo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2qhowfvcn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2wrtlrvgv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ucpwttle.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2fdmenekh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2rmcushxh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2qbpwjskb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gzytnhqv.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2gpntjypb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uociqtjk.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2adrdabbs.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2tjnxzvrp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2usxsideu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2mwyvakzw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2tdhleusg.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2gdwburlz.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2bhymlqsr.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2torctsqk.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2frbgvrax.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2obgoaczs.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2diswxyoa.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2qynzlxjd.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2xibnluof.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2akugliui.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2hgmzpcnf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2fnityfdr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2odbtzdct.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2bafjbazg.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2hqfczioa.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2fxzftdjd.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2wunckwxk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2hlloeqtg.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2lbycuxpn.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zuorqncz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2vzahikbv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2whijzjjr.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdofzzhx.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2benqahhv.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2wjfvkbee.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2uhqvouhp.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lstbsxtv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hhgflnds.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2uugfdpou.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2qhfbzgpy.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2eklfmncq.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2iyowoaev.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ebzskhza.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2kelrqojn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2jgvtalyo.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2hyvusjxh.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vefcspav.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2iavmptpz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2isrihuwl.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2rcsjfwhe.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2bfqczjsx.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2ihcctwpc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2yroqgcsh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2uhyknjgv.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2zgxoylxk.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2nrroqlmu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2wegpvibp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2ylxlncqm.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2ubhyhhue.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2cuztsnoe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nzxtwwpy.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2jknvtneh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kbjwtnlj.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2bnyenrqq.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2ptohjkrh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gkhvtgkd.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2mobqayww.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2vrgthbjn.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zgktywqr.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2euhfywfx.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2hbmtnqat.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2ipzxbqlo.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2zttoixwk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2zxewybdh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2fvxcowaf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2bmlozvjl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2nezilrvw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xnrumwlr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2pizdcauf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cchgzdtt.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2kxyxccns.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2afahonva.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2sibzelqp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2dwsgshuw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2lncaikjx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zxfyljry.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2ngcsyltx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2luyioftd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2jjigqshf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2dgancanq.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2zthqdybr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2xxlyozfw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vogvrcbg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2jlobriit.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2tpuvftpe.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2bhggqtzw.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2jyehignd.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2imnevlhl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2gdwkgkcw.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2jgbsjbgr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2bvtrkanu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2ptlrdpaz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2iqxjrzcd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nbeuohxw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2blyvcvhm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ghvptdns.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2yktglceu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2ninghmyt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2tehqhwum.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2ngkuknry.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2feirssai.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2pfjjdyjf.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2nohmcrrv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qmdcqfnr.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2lxhdoymf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2kathtayl.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2spxdrzgp.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2cxqnsalr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2iqyqihgb.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2gdgbykgi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2hcjgrlkw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2daxcibje.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2sjzahddo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2xejndtkx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2blakvvit.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2vsklqiog.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2crniaszi.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2sjjkxgvk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2snkpdsdq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2uqwhomel.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2opypxazr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2mngftrfh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2hvelxhcb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2nkmeyabp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2eezjvsav.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2esolpdfg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2qyzsqmer.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xwissccn.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2rhkajkdz.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2zazpvvth.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2maadsrwv.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2opyjbjnb.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2ttkufrlo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2rbvmhnsj.html

);
来源：http://www.52xcode.cn/Article/details/gt2gfklzjxa.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2bmkebrmh.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2mhvzahkz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2bwmkvwqf.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2vimkudcy.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2bkarfckr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2ktgubslq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2qxdfkmkl.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2pwueopnc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2jynyidnv.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2zgherqxp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2fqlqiksc.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2ntmwoxgu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2rbcduvpn.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2rvzwgjoh.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2xfcoeasf.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2rjlmcxlg.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wqgtvvca.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2yusgvpij.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2mfcswoxa.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2ksuoiwfh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2howlouwo.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2zushiork.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2umqetrgk.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2xsdgrdyb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2gimfvjsn.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2rrusrvli.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2giaxqaot.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2aaulxfgf.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2yzlbjxrk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2dmazvhxi.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2vushlzkw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2xjsvysbw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2oisruewu.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2aeeltoil.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wwyhlngq.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2mfvnubda.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kzwtqgye.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2nlatdioy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lursfnyj.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bhmvomuu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2ejkswuup.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2wirrgjgp.html


<!-- 参考信息 -->