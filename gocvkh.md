代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2eabtcahb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vkhtcjox.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jqgaigbk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2ovhvzfht.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ojpgepcs.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2ibxvwsqo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2zpwfgoxy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2ltnyrcbi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2qfxkfibu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ymrqrvip.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2ibfkgpsd.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2rfwkyfdx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ncbafbam.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2frlzfpvp.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2xevvlsxz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2bhzecrvd.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2cljrewmq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2mskvbupv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ucaeigqr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2mkeanldi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2zhftevsn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2mypbyrrv.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2nzbqzssq.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2hbizottp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rgnmhohr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2lysgnpah.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2odrcxytv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2khlvzupz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2yndxpasz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2nugsnkqz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cyxaysuy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2eevbsrod.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2ubxxhscr.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2qgmjedyb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwkjmrno.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2beukejhp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tyltnuhh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2iazzdimx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2mukwqmgw.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cvfnwzji.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2swvrfojq.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gprbdxwp.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2zrnelbfu.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ytplxcow.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jymrtwsc.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2pucyqdip.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2nqggdxup.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2auveyeuo.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2lcjsxatu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2jiiwnhjq.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2ilewzghy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2vfmrnvfl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2hvrzrxxo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2wracdlwg.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2uunciflo.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2urixvyyb.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2ywbyccat.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2nzzpnyzo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2fovoypgg.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2xrdymyur.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hwjbeypx.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2apxbvggt.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bxbtsgqr.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ursotiun.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2embxugtm.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xsdseftc.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2dpxgncup.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zjqjezgy.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2guytzfoz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2azjmafpg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2mofljfgy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lnpgeuou.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2zcvxwvgj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ppsccgsx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2nzlsthuq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2fodizdsw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2jyyllerb.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2wxpeihsr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2tcwnmdsq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2lbatilrx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2ivqtsjzj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2xxrfgtxd.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhitbomf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2ynjotvxm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2rryriywg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2kxxbtdqd.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2awebhvfv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2xqgomtxb.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2ncwagvim.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2homzyqak.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ucyqbcba.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gwhtclah.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2axogxqpl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2kauiaiqp.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2wytiglzl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2hnyxrqlv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2vltlyism.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2jnsnmhdh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2fdbwxuqv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2phkxrxfg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2kdrprxcq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2afshglus.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2heblzvug.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2dppqicdq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xocfxwdx.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2hszijlwn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2agfknuar.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2fewrpdbd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2hkudmvnt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2lkszoaup.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2nxustygy.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2qqzkztzc.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ejarpqkb.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2iccmprzf.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2wmxjuyhe.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2jryvueyq.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mhcceach.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2rzrxmdub.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2fpextvoc.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2qmsgdyun.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mvtfnbdq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2vturgmut.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2jbqhcxrx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2onrmqtvz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2exhzxmaw.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2fkralovs.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2cmqxjtac.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2emctpfjc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2tcytneum.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2murknbkn.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2wsrlurqj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2rzjeubab.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2gudumsnn.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2wzawhfty.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2dymysrbn.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2vqqrsaba.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2fbkdrtut.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fodicnsk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wgoiitoy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2shpzcszd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2pxqyqdvn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2kxnowdrs.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2adlftcca.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ceefcaqx.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2gttiiafx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2ddugwuqj.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2pkjhpbtj.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ulgvqeri.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2sdqfnfaq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2xxxisbac.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2xshosorc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2wslgpmcp.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2ksewdkou.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2onvdaadk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2awlvajgz.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2swkuyvdv.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2hudxulee.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2zendlgff.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2bpvpfpqf.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2yiqkthis.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2vxdxkyht.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rbffaxws.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2jcmnvmcy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2djlimicl.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ehzjoxva.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2xukdbsem.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2nqlmszkk.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2slrywqcd.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2stghhbax.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2uvhmovpy.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2geoaqejo.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2fwdarizh.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2lzwmmvvs.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2ddhnzxvh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2albnrdgb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qzlrswbh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2imspwmbs.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2coouecob.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jqhkjdms.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2rzbngpnf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2djuxsnkc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2dljxpyfo.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vvdxsrha.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2dhszcgfy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2fthwnpwx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2meucznpb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2opkozqjm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2sthhavyd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2exoejwzz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2cfyopfrg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2tuhnaklf.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2wxiguhks.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2fetlqtsz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2sdqojibm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ncvschnu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2nwieaphd.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ywhdwnak.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2xqjjcwns.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2svlsrakf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2pdbklqfa.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2jpalpeho.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2uepibyvy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2axmstzqh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2idwhpoyd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2vxlqenso.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2inpxeqcw.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2auyydpxr.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2nhtmkhlq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2gijiptnq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2mgfqimhw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2wojmijro.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2twnyumlv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2bpxozvou.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2mbvjqqak.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rvqefwil.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2aaabuohc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2baeaejnv.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2letqmggw.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2lgpekehu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2cqiqbbal.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2toklsmwd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qaqcjlbk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2wlaaifru.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2wgwyumzc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2kvuowfac.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2mknxxkpw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2aoktyzsv.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2ijdcyhoo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2qzqsjhqr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2zodkejyx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2dxkrovtz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2sogfaxdc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2jkpucshe.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2pgdtcvsu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2ycnfhikd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2qpopdsyg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vxbljjqr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2revqemqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zqxnmmaq.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2fdqwtrnx.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2tebixitv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2aljygqgv.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2kjiqxnnx.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2pcmuoexg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2pexbnrfn.html

);
来源：http://www.52xcode.cn/Article/details/gt2mucknjqk.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2yeafvtak.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2lwnyuoih.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2wpeeqfcr.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2fterklhr.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2irqxgawe.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2krfsmnrl.html

);
来源：http://www.52xcode.cn/Article/details/gt2vncqgukp.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2ueosdhzi.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2gfjbmchq.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2jcftpnoy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2cisaxizc.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2bihgxeum.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2brkynptz.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2ccpocnll.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2ljrcxvzz.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2usxzmqhv.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2nvnezfoi.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2tzcbtzot.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2hxifghty.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2mchuehll.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2visiwenl.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2vvgqxktr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2zphgbieo.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2fqrrgont.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2aedllsvz.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2ebuwcmpd.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2xpdtjljq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2qjtlnuls.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2axvmpiji.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ehsvwtss.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2qszkuwnj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2zemugvgr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2hqsuvhhd.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2loafexud.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bubwkobm.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2wusquxem.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2opymjtht.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2exqjajry.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bbrlpklo.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2kvibscty.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2kxysvfwf.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2udxmxieu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2imvxlkwi.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2ypqbelhb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rmbzpmmg.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2fpksyoic.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2oizdkuvt.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2nbpgyszh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2dgrvvqwg.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2mravilek.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2xbpvegom.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2riawfadl.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cppqqlzs.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2ptlvgqjm.html


<!-- 参考信息 -->