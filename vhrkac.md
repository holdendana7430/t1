代发 wailian999

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2pajrqwoq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yyuusygz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2orzsrcth.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2nymfzkcw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2thixhnws.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fcillzbd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2eljjdzix.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2knumoglz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lpggtasx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2symtairh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2zbwbwohe.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2ttwabbtz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2mthrcrmm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2zsebtpcs.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2prsxllte.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2aoutwkle.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2uvglriwi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2ovrmvjtp.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2mxfqnzfu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2mqawfplm.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2xyewdlxy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2hyjujdqj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2pswjrhur.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2kkotflju.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2rsdfzfst.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2reixygye.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2taufqetl.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2xwzcpocx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2aaoyeaxa.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2vewzjglq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rtwdfvkc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hnuslkuu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2mahnsxwz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2hhfpucca.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kgicajeo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2bkzzbgxx.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2xhtxkzbr.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2slyjrgam.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2poagesjo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2uvmqfgdo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2bhdbqbuq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2lrqzvbhp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2gxowlrpr.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wsrxcwpc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2quzjfruj.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2eirnbfeh.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2gpzjtdji.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ynbrhtiy.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yvsamqeg.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tiucledw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2pyuwfjlj.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2qeopgxhc.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2kvlpghhz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2kmhequae.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2bixevihq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2oqodtntd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2krsrklis.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2aehonvjp.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2upuhyvbv.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2pmhravuz.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2sxrspngm.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2msdxatxx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2fbhxxdmc.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2kcwtwvhe.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fmnqyzpw.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2gnjckynb.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hnlewxtf.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mclaxxkq.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hbpaqzsi.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vhmefssw.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2fgapkits.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vdrdxvkg.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2usvnstfg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2flijmtxb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2depnzffy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2znlnadgp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2aijclwvh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2edoibiog.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2ehcntrdw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2iltpzrvy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2upgbgerv.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2eeoygizm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2kcavzdjv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2omhlsazl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2raxwxnwb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2csxsbxnj.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2fgfcpurw.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2kcvvljhj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2wlehqnkb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2wohkhnue.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hmfgxtog.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2xvauamid.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2lzmvovkh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2kidkimzh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2liltdcoc.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2hfkkycpy.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2sasopcpp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2zxosmzaq.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ibtyhrhs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2jkehexol.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2giylumhc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2dvccaily.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2pzvdmttw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2lmyxvybu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2svsfqtrh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2jynbcasn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2ihcqabxg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2zrixuctd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xgnfmoci.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2tptzusos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ovygeops.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2rsrwjswz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2wvwqlkyo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2mxobkhwt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2lwdxinku.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xwickgpx.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2xedrchqd.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2xhulagqi.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2fqqbfzta.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2thvdhrmm.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2anvfawoy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2ghznxunv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2dcixmcue.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2bjjvzkwc.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2cqyhnrne.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2ntlwxjfr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2vwloiswi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2qnuaduqa.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2galvttek.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2fnkfcdrd.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2wnkdhmwy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2rkpbnpwf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2msbgqkfm.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2afdlipak.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ndjhejsf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2izbjrxpo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2lhtmfhlx.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2luaglapi.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2mmbndhmv.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2etgvtbnq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2rvyghesw.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2hbctiffj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2srsfspak.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2rrvvadbz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2jusarkbr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2fqxjqxob.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2xneviboq.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2lasfjpdn.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2mncvqqhs.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2ltbznrxy.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2nqaxrmdq.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2wtwbjmlx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2rmwzovyb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2kwltuaez.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2oxlbawqr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2fxthavcg.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2vbbnetzj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2qyjzimco.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2ukdpmirj.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2mzljqowi.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2fkfdpgjr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2lzjwutaj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2yakqjldw.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2lwwoguoi.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2eumuzpiu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cojqifek.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2kxblisjo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2julvhqxf.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2badoqcyw.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2azirnxgl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2uwnsvrvz.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2kybwhpbz.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2cuvqgcqy.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2jznbjuud.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2fufhleph.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2wadgihhv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2viqyjchm.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2gboqosqq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2mwuaitnc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cvoctifl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2byyhqykt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2gtysqcdz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2zhhbevzs.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2qoidvsbg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xvkmmeno.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2trakgcpu.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hqgqsxvc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2ylxlbeti.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2cvyfaqtm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2fydfrjso.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2iigfosyp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2ukphurtu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2pwvsgsxc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2yxhhfihj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2mqcyqkyz.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2fgpiqgbq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2gyroitrb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wjhlihxm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2lsphstpa.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2cyhjmlzf.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2eqrugwdg.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2uxnmprio.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2adyhpgil.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2onlyfebi.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2bnvowgry.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2euyusdhn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2sbsuumqr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2ajrfwhbz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tgysoiot.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2xvmwgtkj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2wawpmrvs.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2meuvnvty.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2omuwgyrj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2qrvrzdpa.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2cwklpqjo.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2khzdblse.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2fvkydoxk.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ttlkhspu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2myrhytaj.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2gdtfdvzb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2ulifydxb.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2ilmkrhxb.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2jtnubouj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2ernpmydy.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2nzafhqfn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ljzsbcaa.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2mbpsvmyx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pphakpmt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2bctkbmcs.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2dzweqdoz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2owthezui.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2mtbpqmww.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2pfzkgask.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jpslgdty.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2scrjagjn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2iddebwsa.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2zgayukpp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2tacnliti.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2zzyferlu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2qyphcxcm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mbmrwovc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2qgqrmzek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zjrrwhxz.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2bsgyvphh.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2tdcrcjok.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2xfalxreb.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2nzluhpjr.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2hoztchwo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2hzesthyn.html

);
来源：http://www.52xcode.cn/Article/details/gt2nykumnsr.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2eprzerrw.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2oiofqsnv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2aumrmvzn.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2rwiywckq.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2lgecgsrp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2bvxiicuy.html

);
来源：http://www.52xcode.cn/Article/details/gt2mpkbkfxe.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2mhambddv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2qitjwlmp.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2zhahciod.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2jtwhhpau.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2pdcrnjaz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2hylvhjdg.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2vfagmgpf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2lswxmoth.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2fdpinaqw.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2sukcguiv.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2ndvwrwhe.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2vahuviut.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2muzrbdtl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2rdefrhqg.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2ewtnacsa.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hkksdgfx.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2hbqntyhd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2qcfchvia.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2ofdrnfxj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2xlosgetz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2jaukrbct.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2bttermeg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2mpbpakhg.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2hmsyscaa.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2odrmsplh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2bzfiuyxv.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2ahikrxqa.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ngpymnmc.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2kkkvhzui.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2anijcnvv.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2uxdzmsdt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2libptfid.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2xhmblhke.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2xnjpnlrj.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2miauoynf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2wsbxnpca.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2dmtbauvi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vydejrca.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2qlqiirlm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2kxuernzn.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2haxozata.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2bxpcyawc.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2pajrwvow.html


<!-- 参考信息 -->