代发 wailian999

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2rmnhvwqo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2vwgnvxmg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2xrvdnugy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2leubwqkx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2pmvkplsr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2idwrkwft.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2nplndlgj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oibqueye.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2mphyfdmx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hvqztbjv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2lxvfkhut.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ffrnwwfe.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ncfyatia.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gnpktfyo.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pugixboc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2ijgzybsw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xlsvvpnq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2hwvsehcc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lupwamsm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2hivtfpyc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2piuglctw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2azyhniyi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2kuxesljp.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2owuktbii.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2umqvsigf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vahtzyhp.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2ygaxuvkm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2hckzenxr.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2fidoewlk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2toyobsao.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2bayoozvs.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2jedkjdiz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2efciavyl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2frvoxzop.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2oxerdeap.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2obbcgvci.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bddhakbs.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2dymufxtz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2guppfvkj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2mykrvqzh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2xrdqxnqv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2vafwoqdz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tmvqerso.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2emyrprrs.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2mrjohrzf.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2btdobycy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2trbnfdgo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjpcoxzg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2janvdtdb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2bitihxpg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2nlilbsbr.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nukhwtdp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2htgffpuz.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zqywxhds.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2hxrqilix.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2hzprzqgp.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2quespday.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2aulubnpk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2ducxojry.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2enbcjrah.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2qswclzes.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2srgdrnra.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2lksxpkpz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2yabfvnkp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2yinfexpn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2klobrkdh.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2enueqirh.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ynoksmlb.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2cfhigxkg.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2xhvuufww.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2uvituxsm.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2kivbbmgg.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sdwaymjg.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2yzjahyqe.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nwucuuqx.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2suvwulqi.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vrzntuyl.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2srjkemua.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ixfpvkgg.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qbmoytbm.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2skrlfuct.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2agplwvfx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ablupsbu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2zluoqqtm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2kunqyick.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ctxfzkih.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2szbygusz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ogqqjwdn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2fkcapefe.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2zhtzxnyx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2rquporfr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxxtcdtx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2dgdipucy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2vfnzclfo.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2jyuchhmz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2cpzhlhtc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2pqohpxml.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2ojphxphb.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dxqnsaim.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2vpuqzmof.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2bcbhuipg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ksrkrusl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2uaqukrhb.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qbnlbpgp.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2uszboltl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2xzlvdber.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ndlqzuya.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2dchwohtb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2csblbivh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2aqycgysg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2egjdtwwz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2xxkgsbly.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2gpbcmkin.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2mudvxbnl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2gsbamphh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2raxgldps.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rcgjhiul.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2vzjjighp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2haqwihft.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2rctvrujp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2jatzbyqn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2focsoxhr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2atnqbdkq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2yebnjagn.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2qzgwnqyj.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2djspuzqy.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2oqppmgll.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2cvbtvsql.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2qzpvhvan.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2uqovphgw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2juwhxksp.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2gwtzehgz.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ygkhrktp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2anuencnc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2ivoobhyq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2hdvjahte.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2xczoeskl.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2gwzdcqtv.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2vjaadeif.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2szjlfjka.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2eqzhdkrs.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ezvkhrbq.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2hoscamyb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2fegnscto.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2bjofdpss.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2oituyssw.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2cillytzs.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2foqjfbjn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2scdkiosj.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2jkybomue.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2kowzbdoy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2tevmrntn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2iuiawerh.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2vdzgcvht.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2wwdmsdkz.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2lhxamxao.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2brlqkvaz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2xwfhrbqe.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2heaxbxtx.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2esnsginb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2ktmmbyuk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2zdqtkuap.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2qyboklgc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2drrzsorf.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2yyrbymgh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2cesogsoy.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2ipvbxhsa.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ykgrplwu.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2bphynvpo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2lsksltgi.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2tjxmcfld.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2jrxbdrwb.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2jejromal.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mymrzjdb.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2fprwpfth.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2srntougn.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2spxkirps.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2yzgbmznu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2azxvnvcx.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2yyxxprny.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2hjsluzot.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cujifryl.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2wbmfessh.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2poynmvwz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2dkidczwy.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2nzswqppw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2laqsxlqt.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2ccwnvmdy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2khosyltj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ufqqoapg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2bxyrplch.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2nkdoltqc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2olpsobgo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2jjyjkclh.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fehnmvne.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2fhetalok.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2fycmfonu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gszncwro.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2byowaivk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2ugpazsax.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2xlngbauo.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2npzcebvh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2lnthaigz.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2rxvoemnp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2hvqneibu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2gnhzfwsd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2awtqtonp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2rmrmpheh.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2fhervpos.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2nkwvijkz.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2euydejal.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ryfnuoya.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2eqahubfr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2vsdatgpe.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2obgoydjb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2omdlnsdq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rhbvlarv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2qkfiymfi.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2moauuclz.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2wuwyffnq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2dpglrnne.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2pwqbnksi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2cmaxrysk.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2afkkofqz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2zludkbog.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2pctnmdeo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zzzhajht.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2wzheieni.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2lmywobvo.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gpmiqhrf.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2rpesawzb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2loyujtjz.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2gtdxtjqs.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ntipovju.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2jkeyedpm.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2ejwgwdcs.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2ohtcqcec.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2hlejjaaw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2qxwzxmfj.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2nekwvysx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2ufmfnawg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sleshsvf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2bucsnjes.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pmadmymr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2wuicsvux.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2lmpjibdr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2cnnvvyzk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2pqgeorgf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zecnvyoo.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2prkpgpwj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fnpzsyaz.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2oebwhuxl.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2vjyseftw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2rthqrsgk.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2adaucfrm.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2dkauxtns.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2bwsdlisi.html

);
来源：http://www.52xcode.cn/Article/details/gt2zilrfiyu.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2vlxvcmme.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2mlxbtvew.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2tzusmvig.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2jkdkabas.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2ofrowfka.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2yqpbzstx.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2zelctinm.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2rygehwoi.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ibsvsrfc.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2yypfejkq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2mrmrytsy.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2ptyntxvy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2eqrdthub.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2idfxrcuq.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2xinaqzyk.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2pfsnnfur.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2stxjbqif.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2ylvfqrux.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2gisstkcp.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2owvkdfou.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2lbjekkbz.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2ookufelw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2kehcvavi.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2wrwvpqla.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2zmpabsry.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2zwrzasqf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2lxesrfot.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2shxtmfnj.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2upbyemfi.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2tzxxgzyh.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2sdfnbkit.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2gislhivp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2ukojwptb.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2zleiqbsj.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yjsmhirf.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2xbfkojcn.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aacdhfov.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2upknvxhw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2qiiopmsc.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2qpdmsgno.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2nbtrnvgg.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2pcbbuqow.html


<!-- 参考信息 -->