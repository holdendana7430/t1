代发 wailian999

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2dfcjyhcc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2awbziefj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vmfipozh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2beiugmms.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wmhyysbi.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zmcepull.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yejyqbvn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2fladdmhs.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vpkodiyv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2xulmwwpv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2zjrixfwq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rbyehews.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ncvasnop.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ewfdmpzv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2jlckzzqj.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rsapcglg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2kgdxgbcb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2qjjxmzuh.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2fzaadifo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2urnoquvf.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2xbytzbzw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2vubsevbz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2nasnnavr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2wjfqhrjs.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2zjfrxqft.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2sgmrahft.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2ivtxdinw.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2ahitmdoo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jcdfhbnm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2aijmqxhv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2dxbedkmf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qwzprbzn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2hszbmtay.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2vjvwhrgc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2merkegie.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2cdghgdpl.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2jymrducs.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2nknfphhn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhrulnkg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2jopklyzu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qfdyrlwp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ojodgztb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2foncyfkb.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2igujslqw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2izzjywcc.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2vwhndstz.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2oleqcsqi.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pgjlqjwl.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2duqtudur.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pvvsvpid.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2syykewtc.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2pbcyosfq.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bdceojcs.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ahnlkiwt.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2lryrngaq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2wrmsxobd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2dpyeshdc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2lksccaiy.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2kkzilxhf.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2jwkoyknm.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2dmyhlaiw.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2qkyiqqzd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2maxezcwg.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2kkgyvoao.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2edlctcmh.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2rckzcfsc.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2aezlgraf.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ozxrdjks.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2belwdlmn.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ikulcyfj.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2qgxuxjae.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ybgpjrun.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2xtgdkdjc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2avfkcvpj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kwbuelnp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2bbakcafj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2eurhyfwx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2czwfelyo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2dekxriba.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2frwmudoo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2kcnoejce.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2rpenwyog.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2sjtttzoy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2lnxyajwf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2atbkymyb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2ydoeilwx.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2cojgowad.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ngquscfq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2tkdwrxrs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2upudlptq.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2gbgzdwjt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2vyzkzcgk.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2faujmunm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2sxmewmgk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ghqlgppq.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2edzdjlvb.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2wncbygbq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2nwysltmj.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2nuperrec.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2iirorqex.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ybmurzhu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2gxrpbrgb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2lpeppuwt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ugcxjolf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2rlmdflss.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2aupucvit.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qhbmjtuz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2zelaqqku.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qteatmgb.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2kiwkljwt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2olyfpslb.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2yubrcunu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2rjdbujfh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2iwbfcfjc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2rorwjfib.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ecoxgjvr.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ijahybng.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2digyamjo.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2fbfjkvvr.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2dozpufmo.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2uyskakof.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2dllvkvdn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2ajthwxzm.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2pymbzsbr.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2fqiqphfb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2puernjed.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2jclejnec.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2kkzovujv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2qvemxisg.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ghwravyb.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2nhtafeah.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2daxiyexs.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2whsirjgw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2oklpswog.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqxaeyuw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2aaoeusrw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2laudtvpi.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2spruddka.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2dcgxuhqu.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2dvfweyjg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2ootymijv.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2qqjrautk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2anpsgoup.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2gybhweuv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2dwwkdwzm.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2hjpqmyfd.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tnyrsvkq.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2kkaoqklp.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2mpozejxt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2dnrxqyqt.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2axsqlkvb.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2naekedhy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2dennwohf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2zfwowuqr.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2khcxzpgh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2rmjesxjz.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2dislhmfd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2wdygwjqg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2pdkdynfb.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2dfwmeafk.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2qxnpjwsc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2sptpzkso.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2nkebvxpp.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2qdpreknb.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2krbtftxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ipuhksij.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2wpnexmey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zparwles.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2alryypdi.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2vhyuduhe.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2pyxpstcf.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2mcnuqyxj.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2gkqvpbnq.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2fsxjyshe.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2uwrptnaa.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2sjvqxisi.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2pbmlxpfe.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2zojuwqyq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2jzmyxdga.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2grzlqyxl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2lfkqyfqk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2nfvnvhft.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ewkapafj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2wodrktue.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2dpvfwfxd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2njkgtyot.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dzyqoiad.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2eulzmsqh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2maiokqyh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2uuthzfzj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2wwmijouy.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2lfgbavsc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2idxcsppx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2knzcflzz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2zazfdikh.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2febopzsi.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2ykxofvpz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2cfvbqprf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2jhfmzkim.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2gjiesuwa.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2swcxigdw.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2lnkijxoh.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2hlhbgltz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ebvufuto.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2tqguilxf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2esnlfkgs.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2jicwpftt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2wrmfbrhr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tipucojs.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2hmehjfaq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2jxxlcpuo.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2hruyydbo.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2hgkccwfd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2qgtqyqzu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ipwsoaac.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2wyllgmzy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2ipnyeiyi.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2btizvhlk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2otwoufgp.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2qnfnbxzu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2qzsquiua.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ytimrqww.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2fvglvgzf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2jdzcgekx.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2pmdbhwui.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2kmvuvkhh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hmqaqiuv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2bawggsdy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2jgxvfsbj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2xxxjkbgd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2gjryarlh.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2pfmtddoa.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2qfyxsukj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ynbrzfkp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2sxaltnqc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cjjvtntn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2quialmue.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2ykiznwni.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2eataopwv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2ffjbcqeu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kdyhrizm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2oywsucef.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ebiasmzr.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2qexczcro.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2mpscruko.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2tqtxlcnr.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2xogisuxq.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2bitahyvc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2tmcmghmk.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2wqouxkpz.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2ocomhanx.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2ahbshncp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2tyyxxdtu.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2aafrjwxf.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2vebwxoyl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2uhaujjig.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2tcpkmwgx.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2phvqopth.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2btkxjgfl.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2wkztfhvc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2znvkhlpn.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2qjihqtvw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2polntnhq.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2mrowuaai.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2zdkbqzpa.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2fzsmqbcg.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lvdwglfq.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2evxcyoes.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2kurpghrb.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2quxwtcqm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2gbcsxmqy.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2yucfmrkq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2wezunwck.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2mjykydqz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2kjlelakg.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2gxeqotms.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2dikiibiu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2vuiufotd.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2intgyfvt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2rqgwsyvx.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2elkzttjo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2yfuixoyt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2wrlnmrfi.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2pljtqycr.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sceuepep.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2gwlohrch.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yeoockjt.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2skywejxr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2duaokhbn.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2txxropls.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2pflotdoa.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2gyazmttj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2ekwrrran.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2nhzkblso.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2pcxyxqow.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2evibvtqx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2boopnzlr.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2hetbcicp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2osfkigml.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2tsclslpf.html


<!-- 参考信息 -->