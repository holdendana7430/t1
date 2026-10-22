代发 wailian999

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2czphhypr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2cwpjgbod.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2bfxxmfbi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2todyrxtz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2esxghvpo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nafwjaxx.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2zuomymas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cogrdyub.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2pejgbzfj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nwgclcfe.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2rqpuwyoj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2rvxbccgu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2luamkfkn.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2keshsdzk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vhdkcmgp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2lexpcpku.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2eynahaed.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2onyvcysc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2virtcojy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bhaomxip.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2dzvkufwq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wlgbiuov.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2suvdader.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ndbvqvyc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2kycuwymn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2nrncdidb.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2witjxejd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2salthsnt.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2eojsnkgf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2zticktgb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ojmggdtm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2yntwabta.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2riseygev.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2ejoktjmd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2dmxgwesj.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2zgmyzuzn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2abmeobbq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2znfptgdt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2wmschmty.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2khxaeucx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2xixveagb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2nxxtvmyk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2innuadsg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xamxezgt.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2etaymgoh.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2qpzfldxx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2gpvfqbuy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2slcplcst.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2hcudvwup.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2agvrtafp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2szcriamf.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kfiinhgl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2wqugjjyf.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qmfdbkjk.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2cghbysnn.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2quuihjkt.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xvivxmsz.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dhusxfvl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2rcyshpnl.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2pgdfbdft.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zrmjggad.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2gsmvulpe.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2jrnxazwo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2dubmebrl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2gltsuknp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2jlccydoy.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2niqnousu.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2sprrktzt.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2spzlcuwd.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2aawcnwnq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2gvbuhade.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2vvvarjtm.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2sbzjeyee.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2kxvmmyuj.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2agudrtvw.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xsfudafc.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jswbfpwf.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kmygcjsl.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2sgdrpvom.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cuyjaptz.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2rrqrwuei.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ltsnpehs.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2gaeovlnl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rtbealmx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2jxogglam.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2vmrpjrbf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2btpunakw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nvetnhxo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2dghztioh.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2tylvavru.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2wlgdqgdv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2nemiyjbb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2uonabavy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2zlmgbvpz.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2jtquyqou.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2oryfsrae.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2qkyqfiue.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2nhwlvyxb.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vdsraobq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ewnycuga.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2bkmzutqz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2tjbuhunn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2scexnjhx.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2tjblvkgg.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xuyromje.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2fgpbhtua.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2chlkewms.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2ejdepiid.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2uexckvkh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2nejkcbpz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2qopaziwu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2rcknjflg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2rhsarogq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2ipwunxpn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2hlyrxqvh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ylfszmey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tizuehrc.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2xfdalhzk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zjdicrrf.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2gjwpqxiy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2wakkpqmn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2wzmqcpwt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2vjcnxkeq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2mbkvdgrc.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2pjzwngkl.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2uxqkstdn.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2opyofdut.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2wnpvdyuo.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2kkvadsph.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2velwpjhv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2kuelgqmz.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2epyghhvr.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2fbmnrogi.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2uksxmdoo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2sfdrxrpa.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2yehcyjrd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2qotjnayn.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2wujcorye.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2zbrjokkt.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2hvotwkty.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2imvfntfb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2kpfhselz.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2toezrxbv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2xbquweyx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2pdqljkfr.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2pwgxurhp.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2xzziogau.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2cuycdkmh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2tegdcito.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xmvhudjb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2wjlgzgrt.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2kyfghttp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2datzzhkj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2puukxgwv.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2unohrezc.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2rjxgmoeq.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ajnyegjw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2oqfqxohi.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2tobzrltt.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2cysfgjuo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2fjenxdbk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2wowfedui.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2cawkawko.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2ylndelgt.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2mnlssfim.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2ajevhmdi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2eyzfmetr.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2driktaaq.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2rnowlcsy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2cavynfkw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2prdqpofc.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2igxfifsg.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2mgqolhiy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jiamicwo.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2nhulsluq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sfykphbu.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2cbxewxdv.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2kbuqqaju.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2amsjxqgt.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2eoflktjf.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2npwanwgm.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nblpmezv.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2fkibdtfx.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2kkjlahmh.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2bfsttcir.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2bbblyfgq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2iseneoub.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fredamso.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2vbrxincr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2miwjmvzn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2uizxkqls.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2ohfnnaqj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2ktniwkgq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2vxtbzupu.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rqwgjeqt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2scafnwas.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2hpjgxain.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2tihnhjpv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2xtrmjhrf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2azukbzwd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2ukrlqawn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ojvtkauz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2yiwgiled.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2nkpzhffd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2yaaooqzj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2audvffcr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2wazaulwd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ztyvhung.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2vgmiqcnb.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2tswqyrkt.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2txsiwojf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2vsgwqnbg.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2lonxqouf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2sfhxvhpn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2inyatfbh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2jsswfqkk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2jkcyckzg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2ldpjults.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2dwbcrcpr.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2jvjltmbr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2lgfihvch.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2befjvflt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ilkzdswv.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zbrqbbci.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2dvuxxynd.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2roaxufbf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2utabcdqe.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2lrcrxdlw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2gmrwipuh.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2ckpdcvtq.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2rhgsfhod.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2jrbbyqft.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2ojuigbup.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2doojxuyp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2dktakocw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bxunrlvt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2jxlqwaso.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2zaeqapsc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2sojfixdw.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2ayzkhmvp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2jbjaazei.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2exkulqdv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2gggfxhpp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2rlddzcze.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2eftnyoik.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2tuxslnax.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2jroqbhxi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2uobchvrx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jrdxzlfn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2pigwidrj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dzcmzmyo.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2vowgmaim.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2zoenyrpt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2rtzgptdy.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2jvbusaho.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2suernops.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2wckrllev.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2xqketxlx.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2zeokrkor.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2pxkwdxah.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2dizurdiv.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2smqhqtrj.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2oswhtyos.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2xrnkdfai.html

);
来源：http://www.52xcode.cn/Article/details/gt2cccyiizy.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2yoofgppe.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2bdbmpqfa.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2mluqacog.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2hmnpufdf.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2hbupxfei.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2tniusnvk.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2zixfxbon.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2nbjelayz.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2nsgcjjbh.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nqbjlbas.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2nxddvesd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ybzlhkux.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2qtxujhtl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2wmjbsbgk.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2incmpyjl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xbmhphfh.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2wruqeqha.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2berupxip.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2hkvekdqg.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2yoeawncg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2lqhirnfo.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2kqbmfzbm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2twvpabna.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2wfpxnrzi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2vzbqmwva.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2pturqqkm.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2lpxjqkvj.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rwmkkuln.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2muekesjn.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yqghtabg.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2iyllusfb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vnnlggaz.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2iwbeknyy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2rnpdlpym.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2aoyuqbck.html


<!-- 参考信息 -->