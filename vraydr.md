代发 wailian999

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2zxqorpeh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2bzwopvdq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2cqksbsqv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2gtorzbzk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2jdfhjvvn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vgkccvvc.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2iqdjxuhu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yccoadjx.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2qzjvuwnf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xrvmfqvt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zlpbplow.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2dnviqyyv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2sozrpgjk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ulpjshqj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fhzkifpy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2apzdnijj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2npwaordi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2jxdbusxu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kfngagou.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2fujwqsti.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ebyazlvn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2fhevwubo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2smlgewpg.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2axhmrxda.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2pzrifskx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2byhfixfk.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2gqtewgyg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2zigixfxk.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2mqqxlxlu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2tcvlhagb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2iwhunxzy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2jgfdztbt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2rzccqesn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2dakuaqkb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2gqprysmg.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2ajhwyiry.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2akmlzkxf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2rdwpbixn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dbdmcrqj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2geiutoac.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ilaztfzb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2ixjxdlfn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xumzfzpy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rpijpauo.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2hmkpbqeo.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2tqophsub.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2mkianghb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkoxnqib.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2gxnvmblx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2tpqhyxfl.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2xajuctyl.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dcugcyoe.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2vjsehykl.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2maknkuld.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2tvpmtkxu.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2isktoquj.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jlcbkptj.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2iobavolt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2pxidbybm.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2asejbego.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zovdbwhl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2lhkgtjco.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2tnextgtd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2ubtwpemp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2dpfervgp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2suoccrar.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2hvjhvbyc.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2tqsugxfl.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2zpoywiqv.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2hofholrz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2wtirgbqw.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2ftwjptty.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lkwzwfih.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2ntuygbhu.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2iphxdica.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2foxarouo.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2alzjxvdz.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vcqsmhxc.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2tykfiywk.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qprvkqey.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2nwxwsvyn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2audhuyop.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2yfmwppgs.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wzicncqi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2iepfspkz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2zwpoozhq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2kgcmpulm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jkdakzja.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2hniixhsz.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2odeniyaj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2gbjysuuo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2lsszmcsu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bqkfmisx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2lzdxyfld.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2gymwetmw.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2llxmqsmi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2tnvwktes.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2bnrqnawp.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dwampqoz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2ltahtjqy.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2prcewmir.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2zkgxjpgm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2hpnakypl.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2prkdjyhy.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2klvuofuw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2vbgohcmd.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2smxeuzdr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2qdlkxvvs.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2qrynqycs.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2llwxaxma.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2qnqxdutf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ziygbpct.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2flmnkkwb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2ckvwjwzi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2lqjorogy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2vfkjvoxk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xiynzqqx.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2ncynvonr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2injvqxkg.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2vlkthnwp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2ugqsvspm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2gbrlgwfj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2kiqlqpyw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ueeikcpg.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2znhtxywo.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2yowzvbid.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2rxrbibub.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2qgxjghnb.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2jpkqtzda.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2nnelfhch.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2bvhmxukb.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2wojpbrvp.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2casmyway.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2owhhpyhu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2usgbumwy.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2vxryuwss.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2ysacnubz.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2sebkjzre.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2lltaofhu.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2dktimmuw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2wmprfyjs.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2jtuvnjcm.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mubwgioe.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2vogsgbbm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2wroczshk.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2lycpvhve.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2qtsskegc.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2jyopyggv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2byjmdvzo.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cwiygktw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2crshcmrr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2llwhoxqu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2ejzxgvlm.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2xkefxhkp.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2rirlblfe.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2eradvsme.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2pmfigpkz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2ztdloueh.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ocuitvhp.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qajbtpac.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2evlftrfw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2zyvybtwo.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2dofmpzuh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2lkefdmgj.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2octjagov.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2xcwhudky.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2pvhrrvhv.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2dbypighn.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2drlcjzsi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2lyakedxf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2wuxqtxpg.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2ttvbhxeo.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2muprlymp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mupjuajs.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2sexpteid.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rnyppenp.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2knxfteiq.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2jbrolwnk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2gjoojois.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2lvggzuak.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2rfqlboht.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2waamwnjw.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2xxpedfej.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2ltgeumgm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2rofbbqnx.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2csprhepa.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2ojloaaco.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2umwdhtyv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2gmfxwpnu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2opdlfswf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qcvjaepq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2hqrccpre.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hjvtvbep.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2uxbogaps.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2drcmnwze.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2jtkohows.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2sjwtdiyw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uaohobbc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2cjwswhrk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ppgzcybi.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2oqdtiosd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2vzxcnauk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2emdinejm.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2mefnxajw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2etbsboyn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dbetlorz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2dgirnlzp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2rvrsszts.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2qiwnruld.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2hykcaeza.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2sgidcwem.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2dsgjkfoo.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2mfglhael.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2gevzvkyk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2gfuuurdi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2prijebrs.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2uwykwowo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2oxmokufv.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ojvpsnls.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2salcgqnq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2hyuumwuk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2xukeqkqr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2kawehbnr.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zalfeydd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2ljurktob.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2caeyptxj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2elkxhych.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2ssdwxkie.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2sfuiifvq.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tqcduffj.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2qrzxisgj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2mvsomvkx.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2ueijkoop.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2oacantww.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dcbwmrlg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uuyxtrvy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2eynhgdkc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2awwnnljg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2gjqrnsue.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2bibnaejy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2nlnopeed.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ashnybcb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2ldqmsets.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2amueamis.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2vskkmged.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2mnsinsgg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2nvignyzz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2oeegjube.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eqbfmtbj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2rjcpzkgo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zzpjujsv.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2cjfjdzyw.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2qaovfswv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2eeakcwsr.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2knychpls.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2uoqigfop.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2kvozgwvh.html

);
来源：http://www.52xcode.cn/Article/details/gt2ozomnodd.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2prqzhrea.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2rjkegwmq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2hjhiuxtn.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2iixwmbef.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2dokjcbdt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2mveiiblb.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ucqvdxan.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2kywsewub.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2gkwvsjvo.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2ocusnvsj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2nnhxnzxj.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2humaqsll.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2wmcipfxp.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2rlvvysxx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2kemtzqam.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2bunlozdw.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2hzksivsg.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2loclccof.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2dchfrqdi.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2luihlnxk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2uhdgbtdi.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2pmqbhofm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2jypidogr.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2amlazbje.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2cmtkyjgf.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2pwutbajv.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2hyugdque.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2rnoigvmh.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2uwncdscd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2fpwbzohq.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2crmdwadd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2nywggoei.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2ztrbpewo.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2kgsbsgzz.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fqzostdd.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2wtpgmepz.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sdwokqib.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2kzfzhhcp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fudfrkbz.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2knqwosum.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2mfcjhewl.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2bmkiqvwl.html


<!-- 参考信息 -->