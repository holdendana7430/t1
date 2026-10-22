代发 wailian999

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2tkbmfenw.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2freoxira.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2creniusv.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2xjakvirj.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2jgyekxgp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2zlczeqmm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2okdvwaed.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2peamxppi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2zoimlaru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vvubovcy.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ryoxojxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rmelfxns.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2zurnaffd.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2erdfulpv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2cdqsaprw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2incibkyj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2bfpcfmty.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qmkgbgnw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uvooiovv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2dxfdnkep.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ucsplcye.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2cmuwkphd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2truavifj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bfevpdca.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gulrwpdz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2dotsopuu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2ltowyvjf.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2xxyacvlk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2xgawflko.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2ewzslcat.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2iygetjas.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ubkjlvpv.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2ktpcssoz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2puylgtju.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2fphwopid.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2qfcmnwsf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2mnmnknvf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2cockunnt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2biqlzlxz.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2frkjoavx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2widylqid.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2cgwywnhh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2eweastgy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2uqgbiiof.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2lkxllept.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2hfmxvxzl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2teofohlm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2midtspha.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2terztszw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2crkrdngy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2eexfhkfu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nscgecpv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnazsiwm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2bpzxjwkm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2pskkrzwu.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2iynhrwzn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2edlexkbr.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mqyfkqnh.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2foqznmct.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2blsvqpbi.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2atlryfkn.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2eqwvejsy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2ytlvmnox.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2oostqzhz.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2sbxsyusc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2eyomewnx.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2vkiboutd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2xydmkpsp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2lykutdza.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2ycfycddh.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2qhwlyamb.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2oyzbodiv.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2enytmawc.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2maexyxfe.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2nuuhtbvp.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2aashqekq.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pmbushdi.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2ndeczxqe.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2octfcrfk.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jeavmiaq.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2owdbjrii.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uwswfodg.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2zwcbptdk.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dcowugpd.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2gallxujc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2qhwvlcwt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2iwarcjjs.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wbyhhjbd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2dmcyidyi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2wumdedaw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2fgseqizt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zahlgdvv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2cpuqukwn.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2vwneodsd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2yddqgjyd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2fwwmavwd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2nbosqptd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2iarnbbjt.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2emmktjnu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2qmkqqemu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2xdistvte.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2wsuqrvns.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gaqximnu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2kflqwmml.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2wmxuesmf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2jazrygjx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2kpibjpsp.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zwjnpgta.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2xgqvyvfm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2zmawpdux.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2tivneglh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2oedxiumt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ggkzobpo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2ybblbkqa.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ktwweobm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2bluqorbo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2hujxshmn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2xzqtsjvv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2tjaoduhz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ihlczdsn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xmoiwxfu.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2gouzpncx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mwhjekjy.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2ysrqednr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ifvrkrvy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2tyeabtey.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2aijavulj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2jnldfpsx.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2iffoevvj.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2rgvxnhcf.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2indseqnr.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2hexcateo.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2tcbonewr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2gytaukds.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2kaiskqfe.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2uhkljpyq.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2jhzirqzd.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2kfdytwkq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2miqekyyg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2otxalalx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2ybhpinwr.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2ikauqvsk.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2zgtbdjsr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2eiofdjfo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2risuvioo.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2mpvbxsln.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2gjrzjzvu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2mxgyesyi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2jeronpvp.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2hdjsyfch.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2nwbdwdie.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2rkjpgdtb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2rznnfxww.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qrrwxwaf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ljbrdnvm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2qybqbbec.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2xgexrogc.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2dwzxvqgl.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2mqzwvqtt.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2sslqplhq.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2sznosnpy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2vejhvpzy.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2bwrckiol.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2xqhbfgbj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2fjgiscdb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2brjewsgh.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ymohymot.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2nawdvljh.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2qwzogheg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ggufioov.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2orkembbh.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2wkddopot.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2qknezrek.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2eqmwvqkh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2wbrhvheh.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2kosqcbar.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2kshhgllh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ianhawft.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2ygzegxwm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wtzlkuyw.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ufyuxdfq.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2armoprve.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2uuwytsal.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2vkqpzuze.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2uhqdwyhn.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2dwkiqdgx.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2fvrfirxu.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2cztufqji.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2mbkgbmxg.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2kjpqsgvg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2lpsxqlcb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dseczfqd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2onkhahgq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2jpyzwmox.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2juwspmhk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2fmofrquv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iwyuqzsv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2edvrjnwm.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vjrklcuw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2iiwazrpt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2xyorwyls.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2vajomcup.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2xojwkrev.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2keconjqx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2stigpdsu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2lghhjjqu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2jvjnyiku.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2rcstdfii.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2swyrtscb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wcubkwoz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2rjylcgnz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2amiunbpp.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2hdvwarjq.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2ewyhggon.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2vzguldld.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2tjummwge.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2mvnotmyk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2jswcwtgh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2aydirxxn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2pefmzwhz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xqkszsgi.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2xwrrofeu.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2jqdrysfb.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2kzsaidlp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2bxodlfry.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2kxqueyyn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2pqonerwp.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ehcusohd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2tqnctlgi.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2iqmvyekq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2nyobtgaf.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2ecqjroio.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2klcytczq.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2zdwqpgst.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2ejuaycng.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2abojtwbt.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2kcqqfimz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2uwpwhmil.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2khndswfh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2twikarbh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2zhlzjpkg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2rynwsblj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2syuppjkf.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2rnaaekdd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2jhvmlcum.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ssxvvodk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2mnxjnioi.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tfamvezi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2dhlvftma.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2lytzdgfj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2rlyesofm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2nqtkhram.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ezyjtnqs.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2xrubqvgl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hnxfheki.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2dekzhzti.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2tvrmlwzt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2qumhzknk.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2uuiycroq.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2lutqxhgt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2ruibocps.html

);
来源：http://www.52xcode.cn/Article/details/gt2xxhnfnrc.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2tdglqndq.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2czpoulsg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ycdcbryw.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2sfxyecxl.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2jycydeya.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2cqnvyzts.html

);
来源：http://www.52xcode.cn/Article/details/gt2dzlylqxj.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2skdxpubo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ivetsvdr.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2xjcwtluf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2fkpurpsw.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2hrbbgdem.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2fksceqor.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2lhishbsq.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2smeonjbt.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2qgpqvuuk.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2zpyhpseg.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2whihemsn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2vdzsnokx.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2glubbzrs.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2znzcqedc.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2ofwhqjqc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2psjnrsmy.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2rvjcalpc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2wrmveemo.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2qwsbrxex.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2zpllgncy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2tuzznrik.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2jddxdxae.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2thxsscpc.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2ybckwdbo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2wozldhej.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2dbotujlq.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2vqiwkpth.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sylrbifz.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2xoahipad.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mkbmtxlg.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2whhcipqg.html


<!-- 参考信息 -->