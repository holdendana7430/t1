代发 wailian999

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2hmobcfea.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2rjvqrqbg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2rcaricot.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2axrdmzid.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2mpovdbmx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zwgqactg.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ggakhpzq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mgydazcy.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2dszqbulh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lnlaszfk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2lqpnpupu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2mevgdfbx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ciadydwi.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mduydefi.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zoouwahn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2zruwfnwp.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2biuwptpf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2dxkwrzfu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2sbiadbiq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2zkqybwup.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2bjxlenlv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2floaumey.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2dnzilcxq.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2yzslxdsu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2cxqkmxuq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2gcvclzzy.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2jwvrwnpq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2giueibrj.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2xhjfhgtn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2oscppzzk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ewmomghd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2pjktitzz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2jcveixce.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2pfrnyrpb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2uvawwwhv.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2rwomxntc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2qcdlclma.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2xommapnu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pgwszlgy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2usyqiiwe.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2tqpfilkm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2niylhtdc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2dmuymggf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2npwexhho.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2nskkxlfs.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2habyzqfe.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2drofnjvi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2njwbnwmf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hnntnryb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2lquqbuza.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2etydibqh.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xlpgxdem.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2xcgpshhz.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2chxxpnml.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2eovcgywc.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2nkjjiray.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hohakrxa.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2cgeawbni.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2fjhwdbrk.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2miahcjge.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2sytljfsq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2hxttkjhs.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2iwpcbfpt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2aaxqeynx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2lvaaotqk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2bxnutcad.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2pwrrelgq.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2sjuampwv.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2qmhtwluk.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2nwzpsrpz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2kcsqnfjd.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2asbywugp.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2fbxzeshn.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2tqbkvovp.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ldnoqqam.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2iytszbsi.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2eteadkwf.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2flajbvgb.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2aidaheze.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2davlcytv.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2muojvspr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2uupimjkl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rvvyiteb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2solbahdp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ralaalli.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2tljzncbm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2grqwlxfi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ebaalpzt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2btrekite.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2scoxfyya.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2vacnzljf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2mnvqvwfl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2hpzznqlz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2wkhpzgdu.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2hrwfiahd.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2yfymrtgo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2pjfihjcw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2eilswgqm.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2mfndeywx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2daecmvle.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2muxuyfpe.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2dhkqkfqa.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2bqbhjjov.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2fxmdxvjy.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2blwltrdv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2rydmnsck.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2atdmogpe.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2mzuonqon.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2glfsptho.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2mbjufyhc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2jegiwwyi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2hqbamdod.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2vwzutqat.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2cpjafjsr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2lznibrxb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2aiptbdzm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rsvcjsum.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2hnvzyggk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mlvsqqcq.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2xedgxesc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2cpuyhgir.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2ndqiicqx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2spiavwqy.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ctazyrba.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2pqvtvnep.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2zuxixrsj.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2stxheljr.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2rylsidva.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gpmhzvmc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2pjamtvbk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2srbemhyt.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gmcjyewq.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2igmnvsjr.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ltfyflqb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2zvekakbo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2nliisiqj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2cyxwoldw.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2tcokchgz.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2wvnddisi.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2ufevwkcv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2xbxoajqi.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2gkjnobxy.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dojxsjfk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2cvosnnyo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2nrokljmm.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqwewqfi.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2cprpsmtb.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2mepgihhm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2izqjvnra.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mpynwflh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2sxrrwcki.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2urqzxyff.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2vgkmztio.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2jsqthinl.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dklehrsv.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2vwkiyecj.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2hwkggifb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2hrtnllql.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2yoraifro.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2bmbsmlhg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2fgtxiqge.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2awnrzxro.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2exgyikgo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2zlpocica.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2ntbulrho.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2mlfxsqmx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2ikhbfoms.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2wdchsjpy.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2spvjlwwq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2clavhhgl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2gsliynpo.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2yofatzoi.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2anywjghw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wduhacos.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2onxhxkgz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ckbpmoza.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2mrzhadln.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2sdhsmqdq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2tibuoiue.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2hutvtxav.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2wlifjbbm.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2xbqexexm.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2rbwhpkxd.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2nppvsgug.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2dsjyiqcb.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2abhnemgz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2itpssigm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2wyryezuk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zwayuxnq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2oltgdott.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2zsphktli.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2qiblwdom.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2novtwwgt.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2ykrsrhcl.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pcexqbvy.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2mtjgbbuj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2xgjjnbbp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hwaxqapf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2lsyaccvc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2otukziny.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2qymemumd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2yemflueq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2eiuztsqd.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2sfawqpym.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2vphwygwn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2huagkflx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2gpfdqxyv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2gffjoyiz.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2zrxroklc.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2adedwany.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2ezvrudnj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2cnsrhaeh.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2ualxpfuc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2zozkilsv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2yblnzydy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2xjgmgigv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cccytcac.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2nbffqvnn.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2lsxghbyg.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2tizipzcl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2kyvxacbn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2mzquurkz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2qounibww.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2kxiddfsn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2bkfoclwa.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kucmkkdx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2nrfcxvht.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2atagpkjd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2mpvxxfdb.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fdfopobf.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2ignitiwp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2ykpkexrv.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2mtxuepbp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2slcpxtdq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ioykymam.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2cbftwxia.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2wxwfjbyq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2vjfowapg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2fwluwsxr.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2ruazfpmu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2ocfvhjhs.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rcsqvozv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2laqdyovf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pidrwzvg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2hmghgwhz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2emnniisb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2ygvzycks.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2mpqawfwq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vcwguxmi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2eqcljuai.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rmnhimpi.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2cwvglzep.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2qdatatrj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2tggkhwsj.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ylrmchdm.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2fhmoaduz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2bqyaqjnq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2jvtpjhca.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2etpuvwzg.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2ftbeyorb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2iqphxuky.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2dgnalrnt.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2hiuyrhmq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2lzneipvx.html

);
来源：http://www.52xcode.cn/Article/details/gt2pbwuhfce.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2fqplgbbv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2cmyzxtwd.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2lawgqcbu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2rwzdnlcj.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2oevrzdke.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2jjlfibum.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2gsfkmkfn.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2ipqonoiw.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2eunasder.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2alimnhwz.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2pcfiigyq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2bfywevoi.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2zampmvvl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2xrawdzst.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2uxjonoeh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2tiqoualt.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2cakorskv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2vobmeziy.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2szqrggoa.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2uqufanem.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2qmtpchfp.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2axuoijpp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2kwkwvmfe.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2amgstdak.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2pujdqokm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2xpoownqr.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2cnfmhqeg.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2andorwkg.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2uslcyjwt.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2djfykqlv.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2rmfkcmrq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2goyljnzi.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2dtrxhywr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2cfnpkhfe.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2ryrcejxe.html


<!-- 参考信息 -->