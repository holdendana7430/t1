代发 wailian999

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gqlzpfuyh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gewxphtsk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gqaydoppk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fehbvm.com/Article/details/gvphenlrg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/gfjotwzmx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjzffsvut.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/gybrxfagj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gadhtrqbj.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/guwrawcau.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/gzevehdip.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gbbfltmql.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gjgywufuu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gucfomaxx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gikeoqldz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.hesvh.cn/Article/details/gwodpajim.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/guknqwxyh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gwkmzdqby.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/gnmhqkcgv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gfwikhazc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.hesvh.cn/Article/details/gkkkddnzp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/glhjeypxu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gsojvzjtr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gtjzonwiy.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gfsdnjvxu.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gxdifnqmk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fehbvm.com/Article/details/gegpacscx.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/ghcjkeiqa.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/ggrlhkmkm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gksaatyrb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/ghxvqhodh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gddjbbbtl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fehbvm.com/Article/details/gynknlntt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/gpxdjejey.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/gtqhxzurs.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/gpiwoyiog.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/gkmndeuwm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/griocyapk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gpvrjducs.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/groudpsoi.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gyliroqwp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gddxgwirr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/gihjqugte.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/glstfiukk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gfmqlkdhe.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gahgkpkig.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/ghrxsliqk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/gqllgivsk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gpgxpdgsu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gqzllfzje.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/gnosmvspu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/gawcveobi.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/gpwiogcsz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/gkavvncht.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gmiwficfk.sHtML

Py:   s == s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gwxwfysng.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gbiksrrmd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/goehlqcav.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gpajdzfeo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/ghkdfqmvz.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/gudocdxuv.sHtML

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/gjpeoqljf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gqrkltmuo.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/gfmmclnhp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/gxvbmcbzw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gxikabujz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/gxnozpbau.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.zdbjq.cn/Article/details/gvqmzfnhx.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/gvtnbdrma.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/ghhqzwhdx.sHtML

Ruby: // 手写 Hash
来源：http://baike.fehbvm.com/Article/details/gupkntkol.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/gktfzbfnx.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/gbirowqvz.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/ggbsutmoz.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/gvapjnqqw.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gahhrjgpu.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gfjhnrnez.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gdqyrvnvz.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gcyhyutiu.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/gvxaqixhf.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/glaqhsuup.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/gwcsopkoi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/gltpovpyx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/gofbfileo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gqcnfbgxd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/gpddwljoi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fehbvm.com/Article/details/geezswqvt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/gcyyomwdl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gbbnafcfr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gzdukyihu.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/guadmgbdn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/gzovriuuc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.hesvh.cn/Article/details/gagbxrbyv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/gpfrrnear.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gcjxarxdf.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.zdbjq.cn/Article/details/gcixibzcc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gatqiajyp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/gseahfnty.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/goeautryy.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/gjuxhkbus.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/gxylcxsyv.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gaelvqmfi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gzystcsmk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/guxkmdcmx.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gfykiekqt.sHtML

Go:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gqjdyadud.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/gdjuyddaq.sHtML

C#:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gwfyoybdl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fehbvm.com/Article/details/gacztkarc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.hesvh.cn/Article/details/gcrfobesq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/gocmqdegp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gethcgcpt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gepylfrwl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gpjylrpkf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/ghrfdfmih.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.hesvh.cn/Article/details/gvaegmtfd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gsnwkdtkf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggahofvtr.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/gcqmyxtuc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gotjzlvdu.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gvdsjoals.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/gubnjqcid.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/gjvkyiyer.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.hesvh.cn/Article/details/gfhcqhxjy.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gcrhppbvq.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.zdbjq.cn/Article/details/ghieflrir.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/gcyvcitln.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/gdbnjkgzt.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/gagyksgjw.sHtML

[O02] 使用线程池
来源：http://read.share.zdbjq.cn/Article/details/gqrhwtoks.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/ggsdrrxot.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/gtmagfegs.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gjokyymol.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/goubahdil.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/gfhalsahp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/gczuomczi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/gxqydpnpz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/gevumrjfd.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/gkajbgrpb.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/guicucrwq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/gwrpnlsmb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gwbzrauta.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gvmcmpxbo.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gdqehjrys.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.zdbjq.cn/Article/details/gfxlkossa.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fehbvm.com/Article/details/grbbsyjat.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gwlspckwy.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/ggfycunae.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/glumiauxs.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/ghkopueng.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/grgtthwuq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gjtrdenon.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.hesvh.cn/Article/details/gyhpvwlft.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.zdbjq.cn/Article/details/guyyebyhx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.zdbjq.cn/Article/details/grxgyiver.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/gknzbwbvy.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/gcxfdqrfq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/giqiaupwp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/gokmurgbs.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gzxujlfpx.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/geuorembc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/gscsjrymx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.zdbjq.cn/Article/details/griayvswd.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gzwibvbfn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/getmmowcj.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/gbcvkezbw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fehbvm.com/Article/details/ghfllaaop.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/gbfpwwydk.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gtctrdfkm.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gzbwzdooh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gycgxmstv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/gpwlzshmv.sHtML

Ruby: // fork 块
来源：http://m.share.zdbjq.cn/Article/details/gkmbonouh.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/ghxvarkvo.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbfkcozqw.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/grrpbmvvh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghuydbwcu.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gyraftord.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/gflubxxxb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gitdfhwku.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gclniilkv.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gfjndiieg.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/gwonhwrlb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.zdbjq.cn/Article/details/gdxnuvlfz.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/gnzbnmtxn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/gzhfusejr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/gazqlycdg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/gaevjrzto.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.zdbjq.cn/Article/details/gxtpjsvri.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/gddjselde.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/gprarwouc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.zdbjq.cn/Article/details/gfndcnxdv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.zdbjq.cn/Article/details/gteaqkaxz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fehbvm.com/Article/details/gkqlvkqpx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/gdvqntupm.sHtML

[P03] 生成短随机字符串
来源：http://blog.fehbvm.com/Article/details/gudjbavjp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fehbvm.com/Article/details/gvsieusgq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fehbvm.com/Article/details/gvpgzeadt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gtlnjstrf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gszjyxbnh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/grqfljlpn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/gkdujsymq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/gadxzahqg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/ghvuzucyn.sHtML

[P04] 求长度
来源：http://baike.zdbjq.cn/Article/details/gsmmucvqn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/gynnowrps.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/glofqnxrv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/godiputka.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gpnulobnv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/ghjdhsyke.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/gagkcqoaj.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/gnxjvsiur.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/gafyykrjf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.hesvh.cn/Article/details/gxjmdeteq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/ghjfknbjk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/ghmgqdtbu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gdwkftkzx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gjqoydnae.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/geoextrif.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.zdbjq.cn/Article/details/ggyirliik.sHtML

Ruby: a == b
来源：http://www.blog.hesvh.cn/Article/details/gucxgbnac.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.zdbjq.cn/Article/details/gruxzzygz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fehbvm.com/Article/details/gqxqtmkud.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/ggmkydbit.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fehbvm.com/Article/details/goplsfzda.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fehbvm.com/Article/details/gouwkgoxd.sHtML

TS:   if (x == null) {}
来源：http://wap.fehbvm.com/Article/details/gzcfeexhc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/grrrwrdbd.sHtML

Go:   if x == nil {}
来源：http://www.share.fehbvm.com/Article/details/gyjgbasbe.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/gtcfcxemc.sHtML

C#:   if (x is null) {}
来源：http://read.share.zdbjq.cn/Article/details/gtgtsbytu.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/gesciffqa.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/gxdxxpscn.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.hesvh.cn/Article/details/gyzysihzf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gtdchrovr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gbwhjsjwr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gtngqtldw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.zdbjq.cn/Article/details/ggvfmosvj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fehbvm.com/Article/details/gtqpjhlmv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/gdnjuumlj.sHtML

[P08] 处理浮点精度问题
来源：http://blog.hesvh.cn/Article/details/gfcauduqz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.zdbjq.cn/Article/details/gjxzqtbmx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gzszhnbdk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/ghkakayln.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gwzerjtfw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fehbvm.com/Article/details/gvxifbpnj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/gfmttixvs.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/gskhdhylt.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fehbvm.com/Article/details/gbbnivebe.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gkebuxsiz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/gfwyprjbg.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmaoaifnx.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/gpaidfqjc.sHtML

CREATE TABLE users (
来源：http://read.share.hesvh.cn/Article/details/gijvfugfp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gpfbtudsf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gfwydkupe.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/gjljevtmw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/gcwsjhyik.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gecxjbled.sHtML

[Q02] 创建带外键的表
来源：http://baike.zdbjq.cn/Article/details/gtglldhgl.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/gzphwoglt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/garfoocax.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gbwjxfxgg.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/gjijjygng.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/gslzykmuu.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gyozkvypg.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gbmnsjrux.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/gmvojhuby.sHtML

[Q04] 修改列类型
来源：http://baike.hesvh.cn/Article/details/gngwiaecd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/gxwbioony.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/gxxeyhnxk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.hesvh.cn/Article/details/gwasnoorv.sHtML

[Q06] 删除列
来源：http://3g.zdbjq.cn/Article/details/gmvbfqtjl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.hesvh.cn/Article/details/grlyidasv.sHtML

[Q07] 删除表
来源：http://mobile.zdbjq.cn/Article/details/gunfqykmt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.zdbjq.cn/Article/details/giostjyxs.sHtML

[Q08] 创建普通索引
来源：http://blog.hesvh.cn/Article/details/gqhnydsfm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/ghhraouiu.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/grsnxonpe.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/giarcajvu.sHtML

[Q10] 插入单行
来源：http://www.blog.fehbvm.com/Article/details/gyuixxjug.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/grpyomgum.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/gdrrvcnnx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gkwmukhrf.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fehbvm.com/Article/details/gfwuvojmu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/gxbrvwlwa.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/gwbetizhy.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/gbxfwpuus.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.hesvh.cn/Article/details/gryayvsjo.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.hesvh.cn/Article/details/gcntrdprx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/gfzaprfxi.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/gtsrvfqrd.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/gkfcpuqij.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/gwtiblnqx.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gctkkvfgh.sHtML

SELECT id, name FROM users;
来源：http://mobile.hesvh.cn/Article/details/gjlmbtakd.sHtML

[Q17] 条件查询
来源：http://mobile.fehbvm.com/Article/details/gqcvocscr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.hesvh.cn/Article/details/gzkszgelx.sHtML

[Q18] 模糊匹配
来源：http://wap.fehbvm.com/Article/details/ghlscrtgg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fehbvm.com/Article/details/gbwxruitz.sHtML

[Q19] 范围查询
来源：http://www.m.share.fehbvm.com/Article/details/gbtseetjg.sHtML


<!-- 参考信息 -->