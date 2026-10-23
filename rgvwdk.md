代发 wailian999

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3dxffnxop.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3fbdzcghn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3inxbrrth.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3nfsocvfs.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3lumqbaif.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jpwxrvyx.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3viiwbcpd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ftckelht.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3xkwordka.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lzhnnijt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3usqaxtyt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zvspqmci.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3pnsxxdnn.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bwbomets.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pwzgrgyt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3kglqheee.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3arlecote.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3unfnozvz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3txvczhzh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zortdmcv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3wkvnidyi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3fjblpyhu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3pjxptyhs.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uzoyvffp.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qskzprcr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3hyfepdfu.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3oteokqsa.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3frkhuczd.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3oqkjmxpf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ualifbjs.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3pfssnzdi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3rlnsdkcb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3lpppkppc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3xxmxwiog.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3ppjxisix.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3sdkjnexi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sgvdddmh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3sntrbzob.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3iybpvosq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3codrwlmd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3yawhirny.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3iwjkhdlr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3jgxfukcc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ahpcoomq.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3utorgaoo.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3wqvljabt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3jcgsawvj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3eycmwaai.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3douxlhvd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3ygzglipz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3acfpestn.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3otjctxup.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3vfitwevz.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3joouybvv.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3lckaocja.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xavpocds.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gdnxmrtq.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3eeghevyg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3nupfflmu.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3ocxndpgu.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wklhptvu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3inyppsng.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3nkhfkhzs.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ilyzgmoo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3cumijnpe.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3fhogxgyp.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3vketurxy.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3hvlditog.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3aswbuade.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3xyhtydtj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3wgpsqyli.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3ulmkwlvo.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xylcnmxe.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3mgcbkkxg.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jevkgdwk.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ibggulfk.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jevzefeg.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jvjnanvo.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3wnpjdyee.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mfaxcqnw.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3sdhrafwt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3udgtwkbx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ezzkecay.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3eqhlgchx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3eprpvirn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3uuuzxihs.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3cukanscv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zbwhbxiu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3mzmhpmyl.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3pvmuyasq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3msoqcomi.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3rxvtekbs.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3wdurgmyg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3xilnzfnb.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3atepylqq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3cvmwqtew.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3fvahscul.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3zwwpslbx.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3qsonhdpd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3hjtmtfgm.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3jkldkciq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3suxwbepp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3fifhnjsz.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ymmxkiqq.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3rcwwkpff.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3ttlimfrv.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3rkyuadia.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3ndfjstga.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3cxntyala.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3yibgphgl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3lovwqyqv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3diaudakr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3txkuygze.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3ntlxkhqa.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3shfwdard.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ucpcstmh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vwgcockp.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3xsdesjam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ylqwevtw.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ayphylsl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3eitvrlgl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3jbkklmmh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3vjkzzbnw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3gpsaqaxz.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3dohnctwh.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3qyhcuogf.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3dpawnmwt.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3uzkxsorq.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3bbucguok.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3ujhumfng.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3yrxjakvm.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3aqozjojr.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3iytcvjyu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3lybfmulu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3wlfplhrh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3lfwrhtkx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3zktlhsvz.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3iowmxhch.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3ailhjciz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3wqdxroeg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3rmgprzry.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3higeqrww.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgyggmgf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3kksnfzph.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3swedtuer.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3tlofkmud.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3mzokgaas.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3pisjyssm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3bmmuvzai.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3bzedsrjp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3jrztkyyu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3gaoogsml.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3bpktqlqj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3noggabah.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lkyanbuz.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3zilrtvqv.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ibqmpkxr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3epmyrmyv.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ownmgrzn.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3bydksogu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3lqhryjfn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3plgjbcop.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3hbjgemsj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ecqxefxo.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3jzxgkwzu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ptvkoqfi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3rxhgbdpd.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3clinfdkx.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3njicagof.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3bdkewzdw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3rxqqqjhl.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3wvvdsizl.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3huwbymib.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3llxxjdwi.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3vgkoqput.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oqyepeah.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3vwduyiyd.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3vtkvywgi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ygrhmfre.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3rdliazld.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3jlwfvkoz.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3iosncoap.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3pbyajmst.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3amtlacdh.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3rsayrick.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3jbjzagps.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3xgmeyywf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3cadeutpy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3jmytpqpj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3linogfka.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3dwcmmdxa.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3bhqvpvuv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sttuciry.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3zokvwhnm.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mjlwgeed.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3smleccmu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3dtakintp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3scghnjay.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3tpwkwhzn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mmnjspbe.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3sjfgqxds.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3ktiuyhfv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3trouodtq.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3njiplmza.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3hcjlbfkf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qvwhaxom.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ovqbdcce.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3jtnuhcdx.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3tdvufsxj.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3woeocsxp.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3rpfhotxb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3nizxftnw.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3vltyhiba.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3zmjrjgps.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3tadnixqe.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3mkqizzyf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3rqzmkgsj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3ulwvdtvl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3iiwgblnt.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3qergfuus.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3hycerxhq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3jaghrhhr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ucwptihl.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jjnmyfpa.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3fyxtvzmh.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3zzlxjdul.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ctkqzmaq.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3oqfhyrrc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3koetgiqu.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3ojlrexiw.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3fkngpqyu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3nwbcgnag.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3rpavyyzz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3aspntpox.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ztbydpcl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3anxxccdg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3xltwjojr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ylalvcro.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3mpddvcae.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3xlkhdxrl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3cdyaypxh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3wugwhhfk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3hdzmfzlj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vofsrmgi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3glmnabnj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3ypbesnyg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3mjiquyet.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3jvwcmlqr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jwfjdjut.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3upyiungw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zfegclgs.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3yvvvqgej.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3fbdjmagg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3moconpof.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3wpjivpsb.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3pmafgdbh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3fhfpwuqk.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3seziednx.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3qmsekfkn.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3kztrieip.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3rzrunneg.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ecenzukq.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3rxawpkxt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3nsnrjhiw.html

);
来源：http://www.52xcode.cn/Article/details/gt3funbvwqn.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3pehhjqhj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3afnwuohx.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3mxyezlcd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3sylknsyi.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3wmwohtdg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3hsuwztkz.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3kzyrhvnc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3hcgnhcwk.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3ziaoimqg.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3irijysow.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3qqsxnmsc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3rpyyjlrv.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ypwjzwfz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3miwemgri.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3xaxgxcwq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jaszwncj.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3layjlgxe.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3hwcvjccu.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3orzavxwh.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3phoaxrid.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3sgcvwfko.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3shfjfexn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3gdjrkupi.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3fviuqoxw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3yrggjzjx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3bejfqixw.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3dpcprsjy.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lhauppit.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3uqezpyfo.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rzxptaac.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3lghdjews.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3spcnxgju.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zxxfbjsp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3ijvirlqf.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3bycjsbpo.html


<!-- 参考信息 -->