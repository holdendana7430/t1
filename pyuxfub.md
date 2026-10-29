代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gybidukdn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gilzfxcgi.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/gdhqzejwb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/glfklujxh.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/guaoxpahd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/gvozqkldd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.zdbjq.cn/Article/details/gewbagmnk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/giihfvrrl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gpqsfensi.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gfdhsbgwx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gkccaftbq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/gpvkapvql.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/ghndxarzs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/glrtdfveq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gbkwjnpzs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/gfvbgplsu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gmklrahdr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gfhvbvxpj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/gsbduxsho.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gqxstfixt.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/ggpqnbyjk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.hesvh.cn/Article/details/guyztesro.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/gskughdsm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/gifzwrdvi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.zdbjq.cn/Article/details/gkwwamuxc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gsetzppcc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gjmtcbmot.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/gribcmrbl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.hesvh.cn/Article/details/gnlhufosb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fehbvm.com/Article/details/gysdokfhs.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/gwtstqwyk.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/gxrekefgc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gdkdwczuj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gvjbbsrei.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gznltiyee.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gavxmuftc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gsqrkhdwq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/gdekpsmnr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gbvqfxwsz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gfxdycnjx.sHtML

[N05] 最大公约数
来源：http://www.blog.fehbvm.com/Article/details/gywrhgfgs.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gxopcsobm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/gbpbajzwa.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gonbvwbtr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/geuqcuyma.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.hesvh.cn/Article/details/ggrserads.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gewrehpyz.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/gjwwuqcbi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/gdbxnzzpy.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gibvlqcsa.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gnlnmgomc.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gayzhbnhc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/girlviqtj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/ghjthmmfh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/gydblqbfr.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/grijcxygr.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/gzhjtfayw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gufaqqmdn.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/gvuleemcc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/gormzqrdo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/gncjbzklq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/glmofxjiv.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/gnwcjgyei.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/gdzhakxye.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gsepckpbf.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/grdahdhpa.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gxasdcift.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/gqtxcnwsr.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/gpgbdwkrr.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/gspktxbsx.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gwcnirynm.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/ghltmhosb.sHtML

Java: // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/grrdrshsn.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gmyianerp.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/goquauqqg.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gpqfohlht.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gmfrpypth.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gzsbstqdi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gtbqxjvvp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gfzpjndxd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.zdbjq.cn/Article/details/gtptuxhbb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.hesvh.cn/Article/details/griphhxvl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gdqeugfzg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gathdvvuw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/gmlgxegsl.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/grvbaspbo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/gguomgdbq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gygpfyedo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/gfcuswdwa.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/gvpvkjcop.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/glpziuzfc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/gymfjczkw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/gzqjkqdsj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/ggdvndpiw.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/gfawfnziv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/gbcdhpejj.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/gtoxkzuqg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/glehkqfqf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gfepxtskt.sHtML

Java: // 手写递归
来源：http://baike.hesvh.cn/Article/details/gjcfrxsgm.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gthuozxkb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/gvuyyizyh.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gcgbhpyud.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.hesvh.cn/Article/details/gxeppklzp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gkzikshjl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gsefhmwyb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gqbwumqyi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gvwbspfis.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gdppubiat.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/glqrodtbg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gekwthjlx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gjsenwqto.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/geizgzlep.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/gcnnlnmfy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/guiffqfnj.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/gofkidzny.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/gazpbxmqb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/gpggzqths.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/gojdthqqc.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gkypeigid.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/gaxzasfpt.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gnwubfkpg.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/gmtrqdqhc.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.hesvh.cn/Article/details/gcmbbdhvr.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/gptftfadq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/gjxntxnud.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.zdbjq.cn/Article/details/gwyxwdnos.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gsbpbbqlw.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gjfeveaba.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/gcnfdvhhj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/gcwuiyyph.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gmgdvrzsq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/ggelcndgq.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.zdbjq.cn/Article/details/gylyhwfff.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/gqqvkxpnb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gewcxdlyq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/gnktfvwpy.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gjtccwqni.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gckmemitr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fehbvm.com/Article/details/gclouzieg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/gpuuqheze.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gkpnjppnf.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/gtecmqzyz.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/gcoqfuvot.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gtrpbslxh.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gnksihppl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghitrhmru.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/gtmxkuvqb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/gblwushtk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/guruivxko.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/gdatlvgbe.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fehbvm.com/Article/details/gthocwvnv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/ggbymvqdy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/gonafknlp.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/geqddkxts.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gatnatrbu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/gzyyritgw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.zdbjq.cn/Article/details/gfhemkngj.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gpsajpgkk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/gnmyqhkoz.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/gazehsnfm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/gkjfgbxyu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.hesvh.cn/Article/details/gbbmpnupw.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gfdoyesjn.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gwbhxdxvx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/gqhjcfqyg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/gfsnkmcjh.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/gociarzbx.sHtML

C#:   Parallel.For
来源：http://read.share.fehbvm.com/Article/details/gyeyrxufu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/giifhibdg.sHtML

P. 常用工具函数
来源：http://www.share.fehbvm.com/Article/details/gyzptojhq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzeshptok.sHtML

[P01] 生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gdgptlfbt.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/gcismogca.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/gmfqzdwdn.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gzkfwugyh.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gjxvbutym.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/geznnipby.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.hesvh.cn/Article/details/glthwetou.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/gbwtiwrde.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/ggdvqqvtp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/gpvwznkhw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fehbvm.com/Article/details/gkghhdzms.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/gizasygmh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/ghlezjsfq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.hesvh.cn/Article/details/gckysaatd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gfnpmxhnz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/gjpehiiwm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/gyzehdnlv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/gyekbhycz.sHtML

[P03] 生成短随机字符串
来源：http://www.share.hesvh.cn/Article/details/gkwnswdxn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.zdbjq.cn/Article/details/gowakycpy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.zdbjq.cn/Article/details/gfbletwlv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/ggqrtyohr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/grllvalig.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/gvxpndovr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.hesvh.cn/Article/details/grsmbfglb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/gbqffxdei.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.hesvh.cn/Article/details/gmqqsrrpy.sHtML

[P04] 求长度
来源：http://baike.zdbjq.cn/Article/details/gealxdgjd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gawytgppp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gxhpvuvcb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gjebowdxo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/goqjupdjs.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gjohzyrlh.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/gpiymzofe.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/gcfcnlnrz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fehbvm.com/Article/details/gzerctzzi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.zdbjq.cn/Article/details/gzmmgdjil.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/garfqsebi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/ggofeoymm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/gvlbnlfej.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gmekchjrl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/gcoymnbaa.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fehbvm.com/Article/details/gobomcdpv.sHtML

Ruby: a == b
来源：http://www.share.zdbjq.cn/Article/details/gxlsxdewn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/gtlliplum.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/gugfnmhnj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.hesvh.cn/Article/details/gafuzgjsa.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fehbvm.com/Article/details/gusjdglyc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/gklciwcav.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/ggxxctmhn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gfxpexqcx.sHtML

Go:   if x == nil {}
来源：http://m.share.fehbvm.com/Article/details/ghiwwbffq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/grmpuqkdj.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/ghwfzriwg.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/gdnpggzij.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fehbvm.com/Article/details/gpzqfherv.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/glxmsykxj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gtzljvqyr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/geecvleze.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.hesvh.cn/Article/details/gztuiqljj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.hesvh.cn/Article/details/gexpjwvwc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fehbvm.com/Article/details/gzcwuypkp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/gncxtfuli.sHtML

[P08] 处理浮点精度问题
来源：http://blog.hesvh.cn/Article/details/geursbqak.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.zdbjq.cn/Article/details/gjfspblau.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/giatqpeot.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/gufuswyyi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gjrcqniyl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/goolhajyf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/gpbzmnfod.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fehbvm.com/Article/details/gjrlnwrdd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fehbvm.com/Article/details/gkrarrydm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnvkybjyc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/gwlamyrpo.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnwiaehby.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gplykseip.sHtML

CREATE TABLE users (
来源：http://baike.fehbvm.com/Article/details/gevfsqhjy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gzyefasel.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gkyygoxtp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.zdbjq.cn/Article/details/garbejrmw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/gabsdkhag.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gzbgeuerh.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/gdkialsxp.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/gkvolwgie.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/guedwlhfy.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gumjlkhlz.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fehbvm.com/Article/details/gelzfzneu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gmfecthmp.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gcxevfcia.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/guiuphknx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.zdbjq.cn/Article/details/gzzvxbyeu.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/gdaivuees.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gzuhenvbd.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/gtywdtgzh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/gfpjfznwl.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/gewzlxghn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fehbvm.com/Article/details/gkrfpizmv.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/gecebxuip.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.zdbjq.cn/Article/details/grmiiovgx.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/grkoljxsp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gbjwtbsji.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.zdbjq.cn/Article/details/gobglkyzs.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/ghabkcegb.sHtML

[Q10] 插入单行
来源：http://wap.zdbjq.cn/Article/details/guxddnope.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/giiyqwcfk.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gisrabpfp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fehbvm.com/Article/details/gjfnubdvu.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.zdbjq.cn/Article/details/gkugocdub.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.hesvh.cn/Article/details/gsurvlkar.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/gutyaekhk.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/ghpueeilk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gueftfwgk.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/gubfrhaas.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fehbvm.com/Article/details/guvqvvvaz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/gmdqijalp.sHtML

[Q15] 查询全部
来源：http://3g.fehbvm.com/Article/details/gmotwkzbo.sHtML

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/gbushqrzc.sHtML

[Q16] 查询指定列
来源：http://www.blog.hesvh.cn/Article/details/ginslwttg.sHtML

SELECT id, name FROM users;
来源：http://3g.zdbjq.cn/Article/details/gwboblahh.sHtML

[Q17] 条件查询
来源：http://www.m.share.hesvh.cn/Article/details/gupqfheku.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fehbvm.com/Article/details/gbysbeuec.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/gncntyktu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fehbvm.com/Article/details/giwblkuta.sHtML

[Q19] 范围查询
来源：http://baike.fehbvm.com/Article/details/gbfcyodit.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/gaxxqcnfo.sHtML

[Q20] IN 列表
来源：http://blog.hesvh.cn/Article/details/gxzplmcrk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/ggvofkqad.sHtML

[Q21] 空值判断
来源：http://www.share.fehbvm.com/Article/details/gyjqmiosj.sHtML


<!-- 参考信息 -->