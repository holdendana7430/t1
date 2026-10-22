代发 wailian999

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2amnhlkrv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2oxkzskad.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2vhxbfrjr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2nlejrsaw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2aedpalfh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2snarwbrn.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zgezgwpd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2zbmrdruk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2scmspsou.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2ivyvlquq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2spolfwuj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2wrbipcxj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2sykdsdzq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2opazzxkz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2sesuvfxx.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2miyflgpo.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2rvaxjryu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2ktjmgjnq.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2lfwgclzw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2jdoilouc.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2olnjheuw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2jzlfbcre.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2hutezpzo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2acfrlmuz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2dliblvtv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2olubutjf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2ztlxfrof.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2srihntwd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2prvssrjz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2uxxczduq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2mnbadjed.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mevolccd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2vppxalqp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2cixufmfn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bkkzpvvp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2yniuwusv.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2ikhdnpuh.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2xtosxxje.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2gvhvognr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2pekyiuic.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2kqyduhdq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2siubkxwe.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2ivcopqbr.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dbfmjzwc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2wxxbepqm.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2osxrdezs.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2onqawkdl.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fmxpuuhh.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wwvxnfek.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2nhzsyjsv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2fcsghcld.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2hvequsdb.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2eyszptri.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ohhyklnp.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2brxdvwxr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2iabpscfz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2qgxzttir.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2ylohoqwd.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2axgbuvyo.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2miozlcay.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2hguhoben.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2qcfwirqt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2yzytwqcz.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2xeudrazi.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2rwpjhywi.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2ukydavds.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ewahgeml.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qxqmjdzr.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tdfxeaks.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vougwrie.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2zozydfed.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2sfuikyrh.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2bsveocqx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2xwycexcm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2hctxayce.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2dkciissq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2wyvhgjoa.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2wouvjatr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2gcektnbv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2moxxardx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2reuvbipj.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2uneoupnd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2nywgoepa.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2kugalekc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2daxrgaaj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2icntbqlj.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvvtdmnm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2lgqctyrz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2fglkiyzl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2yhaqdnxh.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lgyvvrdx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2mxkxcnxy.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2xqsnwfsf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2wviluout.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2alpiabhd.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2yxbqffaa.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2mosqdsak.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2phobeguq.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2mnuvmdgq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2yxvirngx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2zmxrxzoq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2zvgbshjh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2cgkzaelj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2safezouz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2nqfqemcs.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2akhvuuib.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2nqfnjlaa.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2guljcuav.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yijiqqoc.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2gnyqcpuk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tcttzpng.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2fiqyzqhv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2kobmauat.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2lyyhuryi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2lejdkraw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xejuclnz.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2xymvgmkc.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2gigsfyri.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2vcpotfmo.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2ndlfsjyp.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2ulhduzka.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2llvytwhz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2nkkcjxnx.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ebybrugv.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rbrvxsvr.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2aybekquu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2mnmepmto.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2kynkfqwp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2skpppxqg.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2nzuvwsrp.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2yzsjnlll.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2ezmsfnyk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2tavhztdl.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2tlfslwez.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2idylkcqo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2ywwddaey.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2vxcveivv.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2epolhfhl.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2optpkobt.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2kiildhav.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2wskjpajc.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2djljdeay.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tvzbwjcg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2scxrbjzh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2ctzjhdbt.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2nwnagfiy.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2gdpnbead.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2buvwhhdh.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2uwgrxnsl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2ubkpxvue.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2nrodrkor.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2mmbohksi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2ffxemmeo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2dmbynmcw.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2hlzfjfik.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2glkhqghm.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2updlxvnm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2ajpyjwwn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2sgzekocy.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2wsierpqd.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2nhuhdcfu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2zpisdxzl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2dysfxtmu.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2ovewtbir.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2cmwjhtat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hjcnwgcg.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2wmjjlmrc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2osjotaps.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2gfcffmia.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2lugyzqxo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2snkkmwpu.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ylctdyty.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2karilohi.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fjjntqtr.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2jtooctoc.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2nubcdqhw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2owicwwrb.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2fkusepzb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2qarqlscp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fjgifjxv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2kgahgxsy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2mqclstxv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2gofysllp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2qlnbljui.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ujvssmxf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2sgviijpk.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tbingbcd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2hmpzzotf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2adoxsmpg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2flpyyfbx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2akpkipsg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2jgtxjhar.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2gljlwwzt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2mtoxzgcm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2jbgpozmj.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2bvugyoek.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2suyytlhm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ubkuzaxg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2sdtjbeqk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2voccjure.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2jbuczhfx.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2zmakordj.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2ssugdggv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2vzvtcxhe.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2kmlkenjx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2jftfcaod.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2lvxgdrer.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2iqwhmayy.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2eiafwrhf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2mppigyip.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2znllseav.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2vkeahrny.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2lwaegmwo.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2diqyeuuh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2dbmrlkvl.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2igmjfywt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2tyxezpnj.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2sfdocowt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ugulfctb.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2qjtphwgl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2mwnweyfi.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mmltrswv.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2fnoamqjm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2iparkzqd.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2ttatvtvk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2wdczkwit.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2nuiypkym.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2kahhujlj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2fbhifygf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2lflmfpql.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2rvpdpmxd.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2efurvlwe.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2pjzxunme.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2qorhsydk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2qnufnzoa.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2cbvjhhbr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2txethvlj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2cepyphyj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2menaksef.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2nhjojfwq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ifotzjdu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2vemjfdhm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xvjhjfxo.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2lhrjffhy.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2tivivvld.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2abpaonko.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2cekbrjri.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2oqcqcfud.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2qkfofgmg.html

);
来源：http://www.52xcode.cn/Article/details/gt2kfcsbnor.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2qehnpgaj.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2ndfbpzil.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2qgdypogt.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2hgqpprbj.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2dwqvbtig.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2glzyyrkd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2eqyzeyux.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2inmtusxy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2slnwmsvl.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2qzqwbldx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2naxefumr.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2ioriqesj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2thjaoqks.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2hvzgsafx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2zqlkaixl.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2tvbylmcd.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2azdcpori.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2vuwqhuiq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2kfegkqnx.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2ulqxcdvt.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2gdjaczbn.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2kujmorji.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2fwxwgtlc.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2ygeqfnwe.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2cwqhwtkd.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2agrwwyfp.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2zjgrqxrv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ktzvjlln.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2jpmalqzw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2amabavbn.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2iehwixuf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2tprcoeyf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2asbdajys.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2konmyswg.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ykswsmdm.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2vqikvuit.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xiggohhh.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2desdpodl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jmgzjlcj.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tpfirgue.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2wvmjfuks.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2togfsrel.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2luizaghj.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2gbpfiicc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2quqvjyrc.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2ialfgipg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2alqomdml.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2oadcuvbp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2eccxtepa.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2mjjurjhk.html


<!-- 参考信息 -->