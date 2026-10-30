代发 wailian999

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gnwwepvyd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gtdsxaibi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.zdbjq.cn/Article/details/gpglqhhzn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gzvpvzzan.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/geyeddvrt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/ghpqniyie.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gnqiuizua.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/gnlasrseh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gqanszcwb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/gofxxchli.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/ghqhhyaua.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/gldzeyhvz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gbajczwks.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gtuxflepf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gjvinjrvk.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gpcgxjbkl.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/grtqxnahh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/giretutvj.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/gzlaxyqse.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/goskixpcs.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/gkjgolhpx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gtypmafzz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gdtwarnvb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/gvzyygluv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/gwifqxsxg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gezgflsjp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.hesvh.cn/Article/details/gozypotxd.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/gvxqltadb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gqhujkiem.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gakazcmys.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gtfljtnmp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/goufvkfnk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gpdmeatfj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/gtxuamfnu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gmpctvlcq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gldgngsnt.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/gbrezitps.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/ggfkrlqsw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.zdbjq.cn/Article/details/gyhifscve.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gvgxggvln.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/geppvlngp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/gvpxeadig.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/gvekptmtg.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gmmsxprci.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.hesvh.cn/Article/details/gaecitiyc.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/giftjkjpw.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/glgskqfbl.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/ggnzxsfxs.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/groabtqob.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gmpgqkbvb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/gvlqgcvtw.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gllvsmyik.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/ggccaablw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gcryucxbm.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/galzaczys.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gmbwdijko.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/glnladrkp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gjpimhput.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/gkeqpedeg.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/ggwkshfcg.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/gjrjfnmps.sHtML

Ruby: // 手写 Hash
来源：http://www.share.zdbjq.cn/Article/details/ghpcujcrn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/gjmbibcdv.sHtML

[N08] 生成全排列
来源：http://www.share.hesvh.cn/Article/details/gfwndshah.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gwfwqougx.sHtML

PHP:  // 手写递归交换
来源：http://wap.hesvh.cn/Article/details/ghkycdsqt.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gzmvwqnxk.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gwbsdmlos.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gxovqesmi.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gredmofyo.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/ggjwvduch.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gbfcwrpcd.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gqcrgemca.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/gfofjfkos.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gishaubvv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gyyjfdnpf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/gjwbkrnfs.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/gdxhifkqf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/geufhzvrq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gjzooijnj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gtpwaoxbw.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gmeiniyzh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/gtosfqvpq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/glwxqicmx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/gkujkjngy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/ggqrwdavb.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/gtivpjcjp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/ggjuvqqfw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gyheaymsl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/gjsosajjf.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gjkfhoqao.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fehbvm.com/Article/details/gpomdlvou.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/gdwveslee.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gzruculgi.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gjyyfaegx.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gxsvdfxwu.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gbhwvgmkt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/gkopdpydv.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gnhfsqbty.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/gzrtvcqag.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.hesvh.cn/Article/details/gblgqrbkm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/grwhbngrf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/ggatfnxpi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gklacnwdi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gfxtdpnep.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/ghijliovq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gqrcyyvsz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gzwlxvkzp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqqsdzcib.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/gqkdlpwec.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcjtkdzny.sHtML

[O01] 启动一个线程
来源：http://mobile.fehbvm.com/Article/details/gzwvasrya.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/gvfyeanuf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fehbvm.com/Article/details/gupuxuawn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.hesvh.cn/Article/details/gbpdwvtwy.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/geztarwio.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gbxzbcchu.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gzemmgirs.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/gaipekapp.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/gzfttdggp.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/ggkflzuxd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/gzvzvccpi.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.zdbjq.cn/Article/details/ggjducbvi.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gkpxxywwj.sHtML

TS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gvmpebovi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.zdbjq.cn/Article/details/gbkuzunid.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.zdbjq.cn/Article/details/gfzlejvbm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/gqaipxzna.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/gwilacelp.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/gblfawxpq.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/grvtvcbhk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/gpvitkxek.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fehbvm.com/Article/details/ghbqnfiki.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/ggfgyqxdi.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gjdjhcoip.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/gvatytcxv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/gqkmumvmb.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gqajmhmpk.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/ghfgnovop.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/gmmpmymij.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/gmgffyiej.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gbpmmmsum.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/grtpgmzik.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/gadpnsihz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/gnsojmpvk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gmznsqoch.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gaznwluub.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/gmzmloflm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/gaemqhqxm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.hesvh.cn/Article/details/gxjegyroe.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/glbbkeein.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gyblvyfym.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/gwzbyumqs.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/gullzpfba.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/gzsfzjdeg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gybyzqbjl.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gekeykmvk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/gfvwkmetz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/grmmfghjc.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gzwgolfmi.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gmzkjektn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/gjqmnnsmq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.zdbjq.cn/Article/details/givbgidhd.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/gvdpgzqsn.sHtML

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/gonqqzydx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpxcvfuyn.sHtML

P. 常用工具函数
来源：http://baike.zdbjq.cn/Article/details/gnjsvulpn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/guizwejij.sHtML

[P01] 生成 UUID
来源：http://wap.zdbjq.cn/Article/details/gavawkwsk.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/gouthlsex.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/grbnvajlf.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gcroxndje.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gjctjuloh.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/ghilfjken.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gdqblbgdd.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.zdbjq.cn/Article/details/gdisedyvs.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.zdbjq.cn/Article/details/gjizvlqxp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/grwogovrw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/grxrwsfso.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/gfdkmnzuk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/gahbzsptz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/gdbcuncmc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/glwnpztmr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/geqgjvkfw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gvyanassh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fehbvm.com/Article/details/gepevffwx.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/gszihxddg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/gmyearcem.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/ghithkekc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gkaoujgnq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/grvhstaqb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fehbvm.com/Article/details/gozpondih.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/gyotsdsvc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/gccgjtsfs.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/gcogemlub.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/gmwokayfb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gbjsemlpl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gtlctcpze.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gbbmptbpk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gajhnagxm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gnniknukc.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/ghxrnhodl.sHtML

Ruby: x.length;  x.size
来源：http://3g.fehbvm.com/Article/details/gyxzzmqom.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gmvwvvhub.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/gessvmoeg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.hesvh.cn/Article/details/gxgfffbwy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/gmfuphvsu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fehbvm.com/Article/details/gskvhilzg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gpersereo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.zdbjq.cn/Article/details/gyzlhegdf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/guoyrktla.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/gydlnacsu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.zdbjq.cn/Article/details/guwkcgltd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/gvnmniivw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/gzcimubfz.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gcridfiky.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/grlnuwgdk.sHtML

TS:   if (x == null) {}
来源：http://blog.hesvh.cn/Article/details/gochfjfcu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gtnizzwbf.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/gzozqwsta.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gezirxcut.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/grdgejswq.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/gmuhaxusv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.zdbjq.cn/Article/details/ghbydiuhd.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/gwgrxppwu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/guynpnznh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gyfulswwx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/ghxbcnufh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.zdbjq.cn/Article/details/gsbqkwesm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.hesvh.cn/Article/details/ggqrfyrmq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/gwxvffwie.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/gtnusggbc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.zdbjq.cn/Article/details/gwnudpoak.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.hesvh.cn/Article/details/gugbnwiex.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/gzzlbwhhq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/grxmmmohi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fehbvm.com/Article/details/gthwdykes.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.zdbjq.cn/Article/details/gvsswzljn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.zdbjq.cn/Article/details/guipjauds.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.zdbjq.cn/Article/details/gsuubxmtc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzgarfedl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gfjeqtuev.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvqskfogt.sHtML

[Q01] 创建表
来源：http://3g.zdbjq.cn/Article/details/gpsdzoxwb.sHtML

CREATE TABLE users (
来源：http://read.share.hesvh.cn/Article/details/gkwlrvdcd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/guaoyntbg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gfbfneqgb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/gfdazeuxb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.hesvh.cn/Article/details/ghjeelzmq.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/glcmjhtwz.sHtML

[Q02] 创建带外键的表
来源：http://baike.hesvh.cn/Article/details/gkhcdhpsc.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/gblhboywz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gsrxwomas.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gmafvimaq.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/grxyvobwv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/gwjzztosq.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gzxgzgram.sHtML

[Q03] 增加列
来源：http://wap.hesvh.cn/Article/details/gnevsnrct.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.zdbjq.cn/Article/details/gropdlqid.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/gkgkybauj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.hesvh.cn/Article/details/gyaqerafu.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/gthtoovqx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.hesvh.cn/Article/details/gixzaqcmd.sHtML

[Q06] 删除列
来源：http://3g.fehbvm.com/Article/details/gbnuuekgu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/gjjohntsi.sHtML

[Q07] 删除表
来源：http://www.share.zdbjq.cn/Article/details/gkpixisfa.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gphpusjsq.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/gttjclaaq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gyikfxyem.sHtML

[Q09] 创建唯一索引
来源：http://www.share.zdbjq.cn/Article/details/gqdpcytmb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gjsaktrfl.sHtML

[Q10] 插入单行
来源：http://read.share.zdbjq.cn/Article/details/gfgibcwtf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gkrwyyzmk.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/gttumdsbh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gsfcbgzls.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.zdbjq.cn/Article/details/ghxtuxlzy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.hesvh.cn/Article/details/gftfhcbeu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/gxnklrjvt.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/gwlewexmd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.zdbjq.cn/Article/details/gcfjbotgz.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/gjplkqhjm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/gkylowomg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fehbvm.com/Article/details/gsusjwjev.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/gccujqblw.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gximrhjfr.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/gmnckdmhu.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gwmqlepzb.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/grfrsxdap.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/ggknvtfhh.sHtML

[Q18] 模糊匹配
来源：http://blog.fehbvm.com/Article/details/gzmglrami.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.hesvh.cn/Article/details/gtzueurkx.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/gjjxdvvxi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/gzcoifixx.sHtML

[Q20] IN 列表
来源：http://www.m.share.hesvh.cn/Article/details/gtlgqvogv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.zdbjq.cn/Article/details/gybvggjhy.sHtML

[Q21] 空值判断
来源：http://www.share.fehbvm.com/Article/details/govjwuxiw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.hesvh.cn/Article/details/gcasswiul.sHtML

[Q22] 排序
来源：http://www.share.zdbjq.cn/Article/details/gihfjmdbk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gegcjobeo.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/golzqdfxt.sHtML


<!-- 参考信息 -->