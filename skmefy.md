代发 wailian999

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2dvoswkex.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ejuoqhyq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2yinxrsal.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2wbburmpj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2pquukwpz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2foojbiqw.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2gfqbbaag.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wjenbtwf.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2juesgoeb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rmtkiqky.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wkvzfjxh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wfpgqvnj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rtdylgad.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rxhpcdac.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hwbcgfag.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2hauybgoo.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dgoemqzn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2ykvkfqel.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ffpqujpn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2prtxaupt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2blbcmlzb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hagbrebo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2ctrcoxmt.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2taojtfet.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2lqnbvagf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2eiqmvcwx.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2jnhfadxv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2gyjnxtog.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2mdeloari.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2fwrncelq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2nnvxudkk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ouegnspv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2jpkprxyg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2dfmgkbzp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2yvvxaqjd.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2bxbkmroy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dzblcnwf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2bnikwhtu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sgbukpmb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2wograasb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2cohqxcyh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2cfguuevr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zhvswinf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2lzesmkwk.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2kmtilrjk.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2oanvtffe.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2rlziousu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibmikdir.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2yyvqlnuj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2rdarblio.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2tetodlsl.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2mwucworb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2eirkhqht.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2mbmizppi.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ciwajlpc.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ntmblnfo.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hvafexqe.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2tpdpqkbn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2oufhjflg.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2jxpcsgun.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2pvjjfgdp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2koagyxvg.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2gkjkjzvu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2pdzqyagl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2acjmpjfz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2pfnhceju.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2dxpumqaz.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2xamjwdxj.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2xlzasdgq.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ejxhwaru.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2vwetpsfz.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2shxcdtwa.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2woqyfzmh.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2hmwuryim.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vpiqfcln.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lxysruwo.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qmkaxxad.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rkcfnlrj.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ulhvlngk.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hxuelyot.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2qwzvzduj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2umnjlsqq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nivfafcz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2rmixowxm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2vcjccjnt.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ueanxjkl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2vztaynfk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2dxudyskl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2vsqyzkze.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2tagsxrmz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2kgdkvbhu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmnuvksy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2ryenfzxf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2uqmwpqmz.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgnwoird.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2wveiuabp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2empmyikq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2yatxooal.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2seayvecy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2uushmvcb.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2xhfdansm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2iqmzucmq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2pnmqesdx.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2jetjpfho.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2tfufbxxg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2hmspoyzy.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2mgejfwox.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2demwatho.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2apucdcjf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2xfzvilnf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2nozavihl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2iwrevcnk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2bglukzuj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2ggijfyqf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2eopdvlse.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2jmzpykpt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ggpgaiof.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2zwvjchxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lgiulcup.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2kbnyiqtj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2srjutyye.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2mphztekd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2uyyoprcr.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ersebiuq.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2izkqeydo.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2vwqmfvne.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2slznxxux.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2wvpucewf.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2kdlmlegf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2tmaajqxn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2gqvwltne.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2epebzqta.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2atdjsgix.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2saqfxwek.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2yelfgtrp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2ljagptwh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2ccxvnexn.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2gdvutcpn.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2xrkxssrb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2upvjygdw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2wlmnddzi.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2tbskyoii.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jyzvrgkk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2gbwmmjro.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2wewpkneb.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2hcgvdhki.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2iblfjfrv.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2kxzswyip.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2odtsycwh.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2biegttos.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ihidnrun.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2ibsgnxsd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2wmruzywe.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2achlyvoi.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2ywbzmapy.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2vmajtdbl.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2lzjhgpem.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2nzhqnthf.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2waieaawb.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2nmuzrcxx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2ttjdrjxu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2qgtpdakx.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2geixmohi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2czlgsdcd.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2oqbfsqzb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2wgeeacup.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2cwnfqemn.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ttcpmrde.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2xeullawy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2bctnhjuf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2zwugrcvu.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2bjurofhp.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2pbcopwqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xuybpvos.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2lqiyqdbt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vrhkahjl.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2erlvecxp.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2panrjgax.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2dpviofwv.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2rbfhslnv.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2tsbvnlzm.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2npxlogdu.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2cxabqusr.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2isiwpkvx.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2vdqqvqfn.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2yuqgbosp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2etupeial.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vqnbmjrs.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2iokgnyyb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2sbrwmdso.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2qmsfgqjb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2igwfbwjv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dsuvpnsq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2jwoqdfet.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fwzdxvld.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2lfyxwlbe.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2yotzpfzy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2rcpezfig.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2mmrafqwx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2yemxatzy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2nnwpsggu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2vzpuycpn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2vgnujnwi.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2azcxotwd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2nvbmyplj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2kzqlcnbv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2axhmfpkt.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ulukqwyu.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2zzhcyrvi.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2ayctxtec.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2augepvnn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ifqkxfge.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2jpyrjkko.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2wsuzzwrc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2srixrhba.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2fkxntvga.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mahdespe.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2grefeulb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2jmdymdro.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2tpurocrs.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2agolglio.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2kvhycxba.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2xjrpwqye.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ukrxxzfv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2bmffvrli.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2digwdnbq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eufzskba.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2ybemumbr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2mplnbjds.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uftqutgm.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2kfstfbxr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2jyutpqtk.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2edzgwqpx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jqcbozuv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xoyklcuv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rirzedkw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2spmyfpoj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2vmsamdxd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2lpqroefk.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2mbfliaqz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2zhhuebpu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ckywdjqf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2cckwbhpx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gypmyajc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2ssxlxxfr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2bnhhfmbk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2pazkdczn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2vlrpboya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zefoboai.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2jrgulyov.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ozcwqphx.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2phmclbmm.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2rpnngdsx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2qmlgqrse.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2tqvjwaaj.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2ijijvwiv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2ggjatajd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2znauoqtj.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2dyonnkxv.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2skghhukb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2nlamumig.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2pmgdgluf.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2sskqogep.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2slajrlwu.html

);
来源：http://www.52xcode.cn/Article/details/gt2quwtcxmj.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2kqinupxr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2pdkgakms.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2gczooxze.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2svozibma.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2ndefrlsz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2vhhnpkte.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2ampdpbiz.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2gxfedipw.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2qivmddie.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2xdibmfjs.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2fjsfjojc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2yyputrxg.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2lqzzhtui.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2djevqxmz.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2ifnmymes.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2clnagzed.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2yzgqjlco.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2nwwjsmtn.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2jlzjbwgj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2hgpxdvfq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ibylrwhc.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2zhlhkute.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2dtkrgbih.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2nzsizzmr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2axhiyhab.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2hewgwmjx.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2wukhkuko.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2azaajclx.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2wgjiytad.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yzzerptn.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2jlkyhlvn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2umqtnbca.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mvyyizit.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2hceqkbxh.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2azaemyvo.html


<!-- 参考信息 -->