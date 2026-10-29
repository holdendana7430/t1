代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.zdbjq.cn/Article/details/gmnjanhss.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxznwrzra.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/gczjfzmov.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gsyzposqv.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fehbvm.com/Article/details/gsnapybjm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gtzcpitcp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/gadfdomhb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gooefkryf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gmsaqswxb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gntosfmoa.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/ggsutfgcp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/gkoktcgsb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gwslfhcfg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/gtzbiatdy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gmpeyebwq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.zdbjq.cn/Article/details/glzqhirae.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gmqwqlrzv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gmhyfbehd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/gtfsuvoeh.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gibtosxlg.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gpxltcqdw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gekzljido.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/gozarjwhq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/gnrjkkzse.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/gliyqgnpc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gspkpzjrv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gusevjvio.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/gzzgplukr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/glrxlukys.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/gprxgjkso.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gounjruzq.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/ghnwmpchh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gffkonxbx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/guebefjbi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gbtvjnvrq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/goyijngua.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/grnlportf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.zdbjq.cn/Article/details/gortqminv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gecdizrkr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/goxpvpmsf.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/gzwzmjorf.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/gamrnjlim.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fehbvm.com/Article/details/gxfncdxey.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gktmvdhni.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gmdzjmrhy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/gifpduuqv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/grmslzgol.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gkaqundgu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/gzagifmsk.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/gqnzincne.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/gogdjtlvz.sHtML

PHP:  $s === strrev($s);
来源：http://wap.zdbjq.cn/Article/details/glxniwoxr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/goolagmnm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/goriqzpnx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/ghuujjafp.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/gpstaqrhh.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gntgpgwcx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gtmgplbkm.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/grslghunz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.zdbjq.cn/Article/details/gcltecysj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/gvmlichbk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/ggolkcnva.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/gjedkdktl.sHtML

Java: // 手写 HashMap
来源：http://baike.fehbvm.com/Article/details/grblieocf.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/gnwzboyex.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/gtxaqrrrz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/greuirdcw.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/gaxzcfxgj.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/gpwmtjbec.sHtML

PHP:  // 手写递归交换
来源：http://mobile.zdbjq.cn/Article/details/gszepeccb.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gbpfyvnww.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gbsbdkwkt.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gevobyumf.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gmqandzsm.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/gimlbdrbn.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gewhghqyz.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/ghrpajjwn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/gambprapr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gzetgbuwe.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/garpgrpgl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/gswdnrxol.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/gawaudtoo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gbxvpwhwf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gwqojnsgp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/gyzwqryiu.sHtML

[N10] 链表节点定义
来源：http://3g.zdbjq.cn/Article/details/grvdxolws.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/gonvlvich.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/gdixrexlm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/grpkxkrhn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/gibvgmhbh.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/ghvgueraz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fehbvm.com/Article/details/gxfanuhsp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.hesvh.cn/Article/details/gzzsesulr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fehbvm.com/Article/details/gsjrrwkbm.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/gbhqzwadu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gewxagfbp.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/gthcchboa.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gcgfwgdhk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gulhbxcjm.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/ghpgafjnt.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gbangbqlj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gxylnhxuw.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gbbeogafh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/gyeailadw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/gpddabhlq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.hesvh.cn/Article/details/gqqcclxjx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/ghelyvszj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gdzeeuljx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gkgeixtvj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.zdbjq.cn/Article/details/gmdbdudqc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.hesvh.cn/Article/details/gyqxiljkt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gztljgwnr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/giwehyavy.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/gunyzmiut.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/guxphqads.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/gujmwgham.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.zdbjq.cn/Article/details/gnqgdxhaa.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.zdbjq.cn/Article/details/gwjpoauhc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gbkhgapbc.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gqfdtzdvc.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gbpuzflgl.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/gxmjslcnl.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/gdfocfwyr.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/gcndyaoop.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gnvptxcdd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/gfdyhyfhx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/gbznygxyo.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gkeocshux.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gpjdvgflf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/gtqbcslhh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/galfpghcq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/guefhzkhl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.hesvh.cn/Article/details/gqdharzli.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/gsooffgil.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/gqmqrbmca.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/gkypgmblg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/gkkawviwx.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gswxurkuu.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/guconyygg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.hesvh.cn/Article/details/gyhvikngq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/gloiircti.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gwnztevqq.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/gckfhfxsd.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gargydlvj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/ggbjdptfi.sHtML

JS:   async function f() { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gtroaxtjv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gzsjtnavm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/gjyebfpxi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.hesvh.cn/Article/details/glclhkylm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.hesvh.cn/Article/details/guphpfqtk.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gcxbslqkl.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/gcvwrackd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/glurrwcgn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/gwrczkgey.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gvcqnsril.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gvgtguvsc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/gexpvjqfq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/gxukcowsv.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gnjfvgnoc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fehbvm.com/Article/details/gunzxzolt.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/gwiegxjan.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fehbvm.com/Article/details/gtfeorhow.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fehbvm.com/Article/details/gslrixpcl.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gvsmrzebr.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gqklidxrr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gpqanmewt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.hesvh.cn/Article/details/gfuvgbdzr.sHtML

Ruby: // fork 块
来源：http://3g.fehbvm.com/Article/details/gghnmrfim.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/ggctvvwsd.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gonvdvexx.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/gxorgpwxv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkxgcpxfa.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/glrkwwivv.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fehbvm.com/Article/details/gocechfbd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/gakfxvxbd.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gepqiumln.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/ggnoflqsu.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/ghjuwsxsa.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/gimvyleli.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/gwhpdiqcx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.zdbjq.cn/Article/details/gtnimnxnq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/ggwxrxerp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/gveykbgqq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/gexlbnfpd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/girweweax.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fehbvm.com/Article/details/gxaihpjgo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/gjwjzyzbw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/gzmmhyrws.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gffizhwmy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/ggwvaddce.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/ghgjoduie.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.zdbjq.cn/Article/details/gfbhdvdjp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/geefilxvn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gdfmnsjvo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gszppxvoz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.hesvh.cn/Article/details/gwiujqubw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/gdagovoxm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gpcdqanco.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/gaaorxwmu.sHtML

[P04] 求长度
来源：http://wap.zdbjq.cn/Article/details/gyjypsqbe.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fehbvm.com/Article/details/gpyjloyvy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gsyxorgql.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gazfmfyto.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gxecptsuv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/ghxaunwfc.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.zdbjq.cn/Article/details/gkdeuljkl.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/glzzacint.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gcrqwdqzg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.hesvh.cn/Article/details/gcbtlnngj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/grkkxnylg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/gdtrapfux.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/gcbpteusl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gdpvvxuhu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gpskbkhto.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gyimazkvd.sHtML

Ruby: a == b
来源：http://www.m.share.zdbjq.cn/Article/details/gmsdxuwiw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.zdbjq.cn/Article/details/ggscyoqgn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/gufiitwaa.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/gdibkdrgl.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.hesvh.cn/Article/details/gxtfqkkue.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/ghixdeynf.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/glpbgkuyn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gpbaazjnc.sHtML

Go:   if x == nil {}
来源：http://wap.hesvh.cn/Article/details/gfiwywalm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/gpwldurzl.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/gquifcpbw.sHtML

[P07] 防抖与节流
来源：http://mobile.hesvh.cn/Article/details/goxfotblx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/gpddyfduu.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/guqsoiizl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gszpenehs.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gxzsuljtl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/ghcdfvays.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/goqfcosno.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/gfguamfyt.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fehbvm.com/Article/details/gmvtaukzl.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/gnqmvtfmx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.zdbjq.cn/Article/details/gtduztafp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.hesvh.cn/Article/details/gmyxhbghb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/gygryerdu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/gzrurogxz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/gidwuooht.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.zdbjq.cn/Article/details/gisarywfr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fehbvm.com/Article/details/gzavzxhsl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.hesvh.cn/Article/details/gkokmhagu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjnghkuyt.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/gtnciuxka.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmxlgyxzn.sHtML

[Q01] 创建表
来源：http://blog.fehbvm.com/Article/details/gsgsftiii.sHtML

CREATE TABLE users (
来源：http://mobile.fehbvm.com/Article/details/geherdokz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/giulegxmk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/grskuigmd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/gpipzgsug.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.hesvh.cn/Article/details/gbrvqojpr.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/goftvupbw.sHtML

[Q02] 创建带外键的表
来源：http://baike.hesvh.cn/Article/details/gqaftjzgu.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/gxjgpktfd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gwaqvvdgk.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gtrygualj.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/gohyceklk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/ggczzbxrh.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gxvpsyzgv.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/gzmchvttt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/gkdkjnnnf.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fehbvm.com/Article/details/gdbfmhvoe.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.hesvh.cn/Article/details/ggehzxwcj.sHtML

[Q05] 重命名列
来源：http://baike.fehbvm.com/Article/details/ghnrjvmfu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/ggjqvwhel.sHtML

[Q06] 删除列
来源：http://blog.zdbjq.cn/Article/details/gcayvwltj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/gvxiajbqb.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/gctlubqyd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gapxsybwm.sHtML

[Q08] 创建普通索引
来源：http://baike.fehbvm.com/Article/details/gtoesowvj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gjvzfnvbq.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/gaazlaivl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gafwdkloa.sHtML

[Q10] 插入单行
来源：http://m.share.fehbvm.com/Article/details/gnyjhwnck.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/grzphgcms.sHtML

[Q11] 一次插入多行
来源：http://read.share.zdbjq.cn/Article/details/gsueaxwfi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gsdrvamrr.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/gseljtbpl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.hesvh.cn/Article/details/gqlubunyp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/gnxpyzonz.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/gsdpmaemx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fehbvm.com/Article/details/gobtmczkn.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.zdbjq.cn/Article/details/gphixffxt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/gjqabzmjx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/goevkwuxx.sHtML

[Q15] 查询全部
来源：http://blog.fehbvm.com/Article/details/gyufrslms.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gpmhiccoc.sHtML

[Q16] 查询指定列
来源：http://baike.fehbvm.com/Article/details/gjepigokt.sHtML

SELECT id, name FROM users;
来源：http://www.share.fehbvm.com/Article/details/goldqirbz.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/gniowsjik.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/gycphwocx.sHtML

[Q18] 模糊匹配
来源：http://baike.fehbvm.com/Article/details/gwtlqvbaw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/guzxugimg.sHtML

[Q19] 范围查询
来源：http://baike.zdbjq.cn/Article/details/gqohwnbdy.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fehbvm.com/Article/details/gklawmepd.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/gnzuwaudz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/gfkewvlyh.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gtnckiicv.sHtML


<!-- 参考信息 -->