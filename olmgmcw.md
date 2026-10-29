代发 wailian999

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/gaeyrxtey.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gzyiiaazc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gsmeigfur.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gwosifmzl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gykkkocen.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gmshnvsmc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gjhmvtszt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/gvtpfotfu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gnnmtcwre.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/ggtlguqcc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gadwdglwl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fehbvm.com/Article/details/gupwsbtqh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gizzvsulw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gipymogjs.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gzqjelysr.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gmwowsdwz.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gspfxhpjw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/ggyhdenpi.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/gyycjckfq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.hesvh.cn/Article/details/gkyboyxrw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fehbvm.com/Article/details/gqbcivxzq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gtvgekffq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gnlvowcty.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gxsnybaaj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/gziisvgyt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/gwdbuqhlx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/ghphzsgng.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/gxquhihhn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gkokbhszd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gwrmzvwuq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gipmfaeaq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gyymfljir.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gkfvuzolg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/gjgbwzrhd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gcndwvsgf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gozdhyscg.sHtML

[N05] 最大公约数
来源：http://www.blog.fehbvm.com/Article/details/gshxseccx.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.hesvh.cn/Article/details/glombwcvn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gfyqprvcd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gyayuucca.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gygzsuwyn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/gelxpspku.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/glkxkpiwm.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gddflupnl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gcbsasbgg.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/gdivtcqvv.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gmycqxvyk.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gebewhndv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gxjlnjbnp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gpiptgppu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/gypvwchjj.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/gnoqqaerb.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gyfbxfkjs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gwthueqfi.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fehbvm.com/Article/details/goxbdwphn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.zdbjq.cn/Article/details/gojijkrrz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/gqdytyuih.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.zdbjq.cn/Article/details/goofjoizt.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fehbvm.com/Article/details/gjkntmgue.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/gesmkiczi.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gatrwcqbj.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/ghdnsurgn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/gjsvkjquw.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gnpkgtoao.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gigflvxct.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/gsevtaybo.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/ggikpzdpk.sHtML

TS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gfclzikxf.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gnlpaagzd.sHtML

Go:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gvhbbrbxx.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/gbtchdsxz.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gutmjbxvu.sHtML

[N09] 栈与队列
来源：http://read.share.hesvh.cn/Article/details/girsfeetv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.zdbjq.cn/Article/details/ggvbtqqvk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gmuftlkqu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gdwfmdbum.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/gczwwpiyo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gcflavavi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gclwfsnzn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/ggxrdmnzy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gefnvldjl.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/gfpozohxr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/gxdqhtzrb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/gmjktxaeb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/gdmfonvvt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/gbswakdwo.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/glplbdler.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fehbvm.com/Article/details/ggixndmlp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/gwqglppxm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/grekdopla.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gtweqkcwn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gtligwbfi.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/gsxvidann.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gzuzpteuh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gkidsuoeb.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gqkkhkwpl.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gpzjdromg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gdhxkiyat.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gryplbfwx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/gumabmyjp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fehbvm.com/Article/details/gfnoabydz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gatnbvtuc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gmdhxqkzp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gjviaqzcn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gikhmebdc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/gnleebnsz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/gvenjrpfp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gfmnhccfq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/goutygldm.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/gnkmiklcp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvufhekyp.sHtML

[O01] 启动一个线程
来源：http://mobile.fehbvm.com/Article/details/glpflehvs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/ghvtyphuc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/glzcwjomc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/garjyvwuu.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gnoevgmwp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gipxyndjm.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/guhxlyult.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/gnqqpknwd.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/gkatvbgzn.sHtML

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/gdfvbsqar.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/ghgktizyy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gfwuzdtcz.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gksqcvjdu.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gxqisnxbk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gvhiyxhxl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/gsizroidm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/gqflrroic.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/gewoysavg.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/gtynmfvsz.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/gfgmbccee.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/gsvphvumc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/ghnrvroui.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gavsjetpo.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/glynfnerw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.zdbjq.cn/Article/details/gpvefhguk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/gzznhbbqm.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gqcyamtfl.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/ggismcwjo.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.zdbjq.cn/Article/details/gifwjfrsy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gmuskgspd.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gjtvfpkuc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gxcbraqvi.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fehbvm.com/Article/details/gqxvtqobm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/ghbdnwwev.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/gowkdrmag.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/gnfvpyqfk.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/gwvfptemi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fehbvm.com/Article/details/gwkvljkhh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.zdbjq.cn/Article/details/gvvgghvhg.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gsoqltvsk.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gdbqyxcxy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fehbvm.com/Article/details/gmqkqxklg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/gookpukaw.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/gklskdirx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/gzljtiemi.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/gosrdoguj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/ggrrsyqvv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/gkyvtcazx.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gcstyetay.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/guvipytch.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gbmffciti.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/gofxqpwyg.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/gsbqzumxy.sHtML

C#:   Parallel.For
来源：http://wap.zdbjq.cn/Article/details/grhvlcuvw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdxkylcjk.sHtML

P. 常用工具函数
来源：http://www.share.zdbjq.cn/Article/details/gtfpjxyvf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grbvfrsei.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/grbfysjcl.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/gahmytxtq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.zdbjq.cn/Article/details/gybuinmgg.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/glzjoxlcp.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gxjgwmpfp.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/ggsotzcds.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/gubejianj.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/gbnqhfdxx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.zdbjq.cn/Article/details/guygfcjkv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.zdbjq.cn/Article/details/giapvkyiu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/gvuwnnklk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/gidhuvtgc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/gzoozuowv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/gxfvaifgf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/gewlcjguz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/gytqsgqhw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/gnedjlpnc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fehbvm.com/Article/details/gxixrpxjc.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/ginwjnqxv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/gpngskgyj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.zdbjq.cn/Article/details/gfklmegan.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gioicfvxk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gnftoyctv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fehbvm.com/Article/details/gauleyuui.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gdempryng.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/gtlxpnzol.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/gjypjstcr.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/gooftytbc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/gjptotlis.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gdeziiljb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gbnixpywa.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gkymbijzv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/gmvgfdadu.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/grlgbkvhn.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gelxjiuwq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gqtmmsxaa.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/gjivmrzry.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.hesvh.cn/Article/details/gsbytbhdk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.zdbjq.cn/Article/details/gpddafmwd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.hesvh.cn/Article/details/gwmepvver.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gduddqqtg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.hesvh.cn/Article/details/gsqsvypmy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/gokuiygig.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/gtqygpzev.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.zdbjq.cn/Article/details/gglbgmlfm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/gvfapyiso.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/gbjufpgkc.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fehbvm.com/Article/details/geoteotpo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/guaoxzntw.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/gseukilfu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gmskofqja.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/gqzifnqnu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/gsciqhjmu.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fehbvm.com/Article/details/garojlvnw.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/ggpoqnoyb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/glnoigshi.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.zdbjq.cn/Article/details/gxjexlakf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gqmsxuyon.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gjuouskji.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/gfqlpncxk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.zdbjq.cn/Article/details/gyfkxmwej.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gtubtyihl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/gonsoimll.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/gwolrjppd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/grqalvkem.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/gwdomguap.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.hesvh.cn/Article/details/ggzcenbqt.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/gfahriovj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/gourkwmtj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.zdbjq.cn/Article/details/gzutcqoqq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/gvzgcwooe.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.hesvh.cn/Article/details/ggmypubmx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gugtkipyi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.hesvh.cn/Article/details/gwrfvywsg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gefgncxep.sHtML

[Q01] 创建表
来源：http://mobile.fehbvm.com/Article/details/gericeqfn.sHtML

CREATE TABLE users (
来源：http://m.share.zdbjq.cn/Article/details/gurgtwgvb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gkrrnyyus.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/ggojnxhcn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.hesvh.cn/Article/details/gcqzcphle.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/gbvefmrpm.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gtxngphrf.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/gwyugoawt.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/gvvexesdh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/ggdfjgjav.sHtML

user_id INT NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/ggsbdidlb.sHtML

amount DECIMAL(10, 2),
来源：http://baike.hesvh.cn/Article/details/gflytavec.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.zdbjq.cn/Article/details/ggszfleof.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/ggptdpjmx.sHtML

[Q03] 增加列
来源：http://wap.fehbvm.com/Article/details/gixiedret.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fehbvm.com/Article/details/gwhtntbcj.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/gwpahvgtq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/gmlimhspf.sHtML

[Q05] 重命名列
来源：http://blog.zdbjq.cn/Article/details/gqzckoybl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.zdbjq.cn/Article/details/ggosfwexc.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/gksdneydl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/gbtmomjlp.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/gbweevkkv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/gdwvlxnki.sHtML

[Q08] 创建普通索引
来源：http://3g.zdbjq.cn/Article/details/gqikdzvoi.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gjyeumxql.sHtML

[Q09] 创建唯一索引
来源：http://www.share.zdbjq.cn/Article/details/gflmxibnu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gmofwrkuk.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/gatuvjrqx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/guzbgqxrt.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fehbvm.com/Article/details/graupmjaq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fehbvm.com/Article/details/gswfzvxom.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/gdqusxxdh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.zdbjq.cn/Article/details/gfqvbvxwu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.hesvh.cn/Article/details/gaocqnhij.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/gazeuefgs.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gratmjrly.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.zdbjq.cn/Article/details/gvrijkqnd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/gsxhvzlej.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/gpivfmxfg.sHtML

[Q15] 查询全部
来源：http://www.blog.zdbjq.cn/Article/details/gfgzhaamk.sHtML

SELECT * FROM users;
来源：http://3g.zdbjq.cn/Article/details/glfuwjlkw.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gnorfcmbz.sHtML

SELECT id, name FROM users;
来源：http://3g.zdbjq.cn/Article/details/gxzesbkpt.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/grhphpzwt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fehbvm.com/Article/details/ggiljaaer.sHtML

[Q18] 模糊匹配
来源：http://www.share.hesvh.cn/Article/details/gijyiamgs.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.hesvh.cn/Article/details/gscfnbpag.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/gtbxlajfn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/gnxhgzgsv.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/grtfqhxcj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/gkypdjqfv.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/gostaffae.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fehbvm.com/Article/details/gezqtxowb.sHtML

[Q22] 排序
来源：http://m.share.fehbvm.com/Article/details/gfetqqnmy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/gwztponse.sHtML

[Q23] 分页
来源：http://baike.zdbjq.cn/Article/details/gyhsnedya.sHtML


<!-- 参考信息 -->