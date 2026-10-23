代发 wailian999

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3qbqzxagh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3swpwouba.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3gtoeuksy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3ymueyvgj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3dkyxubaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gwssoahb.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3jecyvmmm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3swhpchsn.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3rpeqitba.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sbntbapt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tpdgtjcf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qkdprsjo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3weiljfgk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3infyrpoe.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gtpoawrf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3bzyrqzaq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3amvmoguy.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3dpjbxgjg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3jcldgpvo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3icnrvrky.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3wpsuzbis.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3eafgykvz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ehlfiphq.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3nnlbqadi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ruvtqlwe.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3uzgvwqeo.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3cvvhntfq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3cwiyxfwz.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3jatbeupp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3eysbavgq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3zrcgjqgi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qgmikhep.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3nbgiiorw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3zcnezbmj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3pzwhqzxr.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3sgmzpyzt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ivvylxgm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3hawioprq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dostejrf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3leufyhsc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3smthmqjh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3pfukkkjz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xxdxuapk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3yymycspu.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3djjcburr.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ztbfsrep.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lnhoorrx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3zftshzxo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3wqqrulcq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3oogfqojb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3hszuharz.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3biemjsbo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3wqbrqtdw.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3nthxbbdd.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3dkkbfrmn.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xqqhtbhg.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3hfxawxfg.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3asvwgpxa.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3gvbccbni.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3twprgyoh.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3qbxolnyp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3zikkgjqe.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3allskpwi.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ogqsmbyl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3bxjuwsda.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3crfaohmu.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3uazajbto.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3kgpkrgdu.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3qeaphnbc.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3xrrlmfnk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3zfwunmps.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3rrykoxur.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ctulqlae.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3uojbnlhu.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3obrnajma.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ovzvwlow.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3owblhcdc.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ctexqcfd.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3qcoxledf.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3btjcmrdu.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ymvmcjza.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3fgwmcaqi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3lgnkhzlg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3nmxqnqmp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3pkgwpmec.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3xmkjmbxg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3ahkhapuz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3txftetza.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3sjnakern.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3jzahalka.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3dyqaatyx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3woqsuvfy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ijnmjshu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3nsqzlcbi.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzifsfaj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3dnosqkqz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3eecyknyo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3gcltqdxh.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3oxerjhzq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3rpvquhkw.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3ugmvnnoc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3niszlpns.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3urkknlis.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3vaulybdf.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3mbalqhoj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3toqyqnuk.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wonbqytt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3ycftgswk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3uvlyzezj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3zdpaevrt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3jpgsvbml.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3bgzmqibz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3eltzljxt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3xhkgnlmd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3altjfigx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3zinmcjvc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3obzhbbhp.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3whxotptx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3opmgysbs.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3xpjievxz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3pzjtjolu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3otqazcav.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3worjvvqn.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3jvdbakil.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3alreunak.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3qlvclrwa.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3zjshyjhj.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3iisqceqg.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3kxldwqdl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3hsorjgax.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3ttmepacd.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3xjezxgoe.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ifdtekwr.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3zcamrpos.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3fsjjmkmq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3krnhmtav.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3cgelewcz.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3flxagrzj.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3iahwpxrn.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3gsoumqqa.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3spnjuwvq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3fiifnqsz.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3rjwcjdnu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3rlzuqzlf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3cqnsgejs.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3fcyboiiu.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3qarndeet.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3qqyedewj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3itmikdqg.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3preywqwy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3xdwnycug.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3kfjnfiqi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3qwkbsrim.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3emroywxf.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3gjytgdyq.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3sikazqtm.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3furfsskp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3urzhhisi.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3pbcekvgk.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3gxwywgjw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3ihildncg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3dnvesopq.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3gaxbxafs.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3vzbeguiu.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3zalrxias.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3xtjblkxq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3efxaharn.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3djhysnzd.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3snsbbaey.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3uxsltxrf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3qiyjzboc.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3thvydxfc.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3thqsuobn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kolaowvw.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3obxdlyle.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gupdofhb.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ypgblwwc.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3sigxikxd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3pcfjiymc.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3hyibjprm.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3mxugjmsx.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rxsbjjwa.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3shgebgnv.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ueqssebv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3tebjdgwp.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3rthdsliw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3pmvjrbjq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3huabmibt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ppmbvrhs.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3plkfeqkh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3egartdik.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3atufmyoy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3pyxmqvzh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3enaqpfkx.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fexvnxis.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3kswjioip.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3olcgewgy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3nesndcia.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3csnccyql.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pqgryjos.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3wxrrrrux.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3tlhxikyq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3yddzfoer.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3ebyghdqu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3emiuzmwa.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3kjdpacnr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3pmydxgko.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3luqkxyvc.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3oayrotrb.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3jevflyll.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3pokabtzj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3pegnqavw.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3ayueeaav.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3borthjya.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3vixytkfd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3otmixmyx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3nmgqdfsu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3anxlqchs.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vbupfrli.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3xnixuxqt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3briffdfv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3nrzylgsq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3pupdfxaw.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3eyuoedvu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3shjsyjpe.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3dlrnqwga.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3zzknvzso.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3qioelzsr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3nbcneydy.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fruukwaf.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3ztueatab.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3aahbtcnp.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3cmdyxgyf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3mlczymks.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jmlnktpc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3muvxmzxc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3siubduwi.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3xfkczdao.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3ctyxnxaw.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3vdmotrez.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3qwsrples.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wxulcrvn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3zacirpem.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rkgogwmz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3bagvyddz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3mhddxcky.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3hhkzddsr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3xjnujokr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3duboincp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3swxgyzgd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3enzyrhpt.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3iypzjiyg.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3djacsjbf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3rdgwvynj.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3vnulttmh.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3tbfyvmqg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3xggnuuqt.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ptrzrllm.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3qbnsnnyu.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3vejkxesk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3wtzuycie.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3tedmjvoo.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3dblhavrm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3wntfoxon.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3zlzhtfxe.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3kvzpufpe.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ejtgltcu.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3dlrajgga.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ogfqrwsw.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3ujklnlou.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3joncsasi.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3tdhxxjbi.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3hkxbhnin.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3rmqjvedc.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3utvpzeqj.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3tltdxqpm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ubkzkxmj.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3uwbgkwvr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3aagzuomx.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3skailyhu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3yghuenng.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3uyewhyzn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3fofijdyw.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3labaizmx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3heqwcymh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3jgqjxrbx.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3zewikcgn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3vctqjleq.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3wdfvdisd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3bekzmavz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3zmmfelmu.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3ozajimhy.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zesijqez.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3ogagicxl.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qjsosrlm.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3wudznixi.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3mkkeercz.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3syneqbje.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3szzuuurh.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3blduhlao.html


<!-- 参考信息 -->