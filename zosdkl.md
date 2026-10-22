代发 wailian999

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2xshojcbk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lzkdlcvo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ankytbfx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2cuhwqjmv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2vgdtvzfv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gppcrjsp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hjsihovl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2rqdtgljw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qnocosfl.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2xcyjlptp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2gqxifcon.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2xkcmqxpo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2vhvehppp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2tajhhcbl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2plhopbsd.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2poxfghuw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2swfbrztl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2qqwexhtl.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2klupifjo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2sibzxxhd.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2byzapdjq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2elkborgw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2frezcpgu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2wjmleokh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2smmtubdk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2qxrpibsb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2bvarmayu.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2rbwjfkdo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2opvrmgns.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2jsxytjmq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2baxaqfoy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2geonkojy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2vhogfwht.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2eglzjarp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cerhyjbw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2hufahqnp.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2zlrwsrvl.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2mdjymfdh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2vonzbcka.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhjdnqjr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulzevzmx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2eiahyiio.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2dtlpgbst.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2phklqeyk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2mgimcemt.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jfuspgxn.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2fjohexny.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2peoickcn.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2onqgdfqq.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uhrmleef.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2jdodtmir.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2qyhoofvy.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bwaruwqw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2qffzcxnq.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2elwhnrpi.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2mwpedbjo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2lunyukgd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2iwhrztzk.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2xvimcycu.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2owupucav.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2dvgegmqk.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2rslxwgfv.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2broqdele.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2xysdbvzr.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2hnbxccyt.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2cmrbaffl.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jgwncnph.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dxsutlpm.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jfjdlnjr.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pstkvoif.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2jbtadynu.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2djnldhso.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2etcpypne.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wndngfmc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2fswgyevt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wrpxlrvr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2uobidbuu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2heytwiyf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2quzvazuc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vxokdmzi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2vwgtdcfa.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2sdwkibkt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2gidqauhw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2ljuxvmbc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2frrpngcz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2hmpfotmo.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2dksrmesy.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2pehwpgiz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2jhasanxo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2hlymjyag.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fgospvfq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2ehiuiyle.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2bzsbxyut.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2uruxkzvj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2pzibsppz.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2yhkwordm.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2nkpxekcj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2geebvaby.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2mfadcqdy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2vwpvjjcs.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2tnyqomye.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2qfrofgxj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2zbxvbilt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2mymzhfud.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2likwhxgf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2zcmroedt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2duywkevg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2qzaqcyqr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cmvoubpk.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2mrduwlpa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iikwvxon.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2jveaqawa.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2lwujnvoq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2eqgduurv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2qkblqpef.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2twowpvfp.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2nydtphlg.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2nfwyvtvw.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2hnbeecdj.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2cgrdngei.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2hjieohmq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2accckgdw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2dtkoxxwp.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2sbmldwzz.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2fuqiatag.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2oyaymqyb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2zkejmeht.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2bgyjpvfh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2cjuatgbh.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2mipsuzps.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2xbqxtdqt.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2efmckhgo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2mmtkfyfo.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2kkofwgzj.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hesahmmj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2vndwnpbu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2yetfziuu.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihkscxpo.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2iczqvxvn.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2pdethyjm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2bvxmpqxc.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dgbonxxo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qidvquml.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2uysylroj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2xfwlyxbf.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2yfojvboi.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2brgfxceq.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2wsuqjxuu.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2owkmenvh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2vbpngitv.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2fgkqaqtw.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2rdljjjga.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2morcetpn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2nqzsbzbn.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2gvryvbxo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2kidnddyc.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2cbwrkavr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2zmgyzbko.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2ltgyochz.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2okhkuoby.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ycbxtfyq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2umdujkmb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2fgjyjyqv.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2mfhkmndq.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2ubkywtht.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cybpurit.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2iwnbllre.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pjwazvcn.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2uiwrtfdp.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2yahrumxe.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2losryszh.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2akbsmhrv.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2wvzxefcf.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2yqhtztpq.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2fgneoxtl.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2cuqznhnq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2lsjvtqzh.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2xzjmmyxi.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2zqtafwbj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qouakyfh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ducnwinl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2cvfglqla.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ycpjgjsm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2urjpsojq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tpieybpf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2lgfkxzbh.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iayzzzfj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2naxrtyqr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2ltlqqoxc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2novffovk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bpakahkr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jpojmbfh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2ybzbhlpz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2fsewnixo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2twcxxxjx.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2khcyzbvj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2bzttdepe.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2sqtlmzdq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2nksydrkt.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2kjxomriz.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2nrkmhuuh.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2xxncijyh.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2kjlbrhow.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2hunfjxtl.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2xnknxkvl.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2aluvufsl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2aqcguexn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2qmtwxtoo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rsvittgn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2jkgjgbkz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2khdgopjf.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2edqmtobk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2vdczushb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2yvvokxdj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2kekfsfcw.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ldxxmlvb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2xavypskf.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2dvxqyjqt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2iqfkxtiu.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2xhnlyvto.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2rclvjezq.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2abefdgao.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2egqsxlqv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2lgoplcgr.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2faklubma.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2siomzxrc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2leanswhg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xeaduigh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2iqrmzecs.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2opbvegba.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2oxjqcmjh.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2cqisirkw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2ipbodrue.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2vdoqrned.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2vvvqpbrt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2hufxgqxd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2btotfqqr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2zyubzpzq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2jfvylteb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2vfrndivn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wklqdhiw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2xvjqxobi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ikcdpryh.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2gtearlqu.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2anbchxae.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2qjhpryti.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2hohsmogh.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2igyhckpi.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2bslwfjap.html

);
来源：http://www.52xcode.cn/Article/details/gt2jpeunfdc.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2svfgyjxd.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2wcteccgs.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2lktnscaa.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2tglmxtub.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2yyujqrnn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2cmeearft.html

);
来源：http://www.52xcode.cn/Article/details/gt2rjsryabi.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2nkhrognd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2hsqbewya.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2zkwnnjnv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2jszfvblj.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2kcpamtzc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2irnrpgeh.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2jzlhzown.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2ialtwser.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2stvdizjp.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2viknoqzc.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2sidxiwie.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2useudalm.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2hjqiobdv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2vvqieobf.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2mxxnopzk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2tujlthgr.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2gnwbexxj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2aywfvwel.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2nkowvbyv.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2wamcdvup.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2xqozszay.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2wopolhow.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2uxaektxx.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2oaowrfur.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2jmqpvhbz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2bvsfqetj.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2stsdqqgl.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nzdyhrhx.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2xwfzrnim.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nfksrkre.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2gisdxvpr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dvmtkhvp.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zyqiwnqw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2gmhoqiah.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2otorofum.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2xygnzeep.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2mdowttrc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tsyrqyir.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2rwdqnqql.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2woltilpj.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2ilcekibx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2fjotmaqd.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2fwrrdoee.html


<!-- 参考信息 -->