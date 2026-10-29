代发 wailian999

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gctcufhpd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gcdmphpdd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/gbcmjwflu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/gifuhqwfc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/gfzglqhyo.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcqamgarb.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/gcgaiwrsk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gyogzqjjp.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/gusquwpxx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gklmyyhtw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/ghflmhiag.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gqrjjhdnb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/glspxgcqv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gdocgldxb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.hesvh.cn/Article/details/gvkeilwnn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/gupaktnok.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gekwlmufk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/gfurwamfo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gzjzukrad.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/ghuyhluis.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gotghsoof.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/ggguujgmr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.zdbjq.cn/Article/details/gqvqutrzd.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/ghoujmjow.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gnlymzlio.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/gwbszwxjo.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/geewtoogx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/ggwfurjnl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/gwfdtttxj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gkzvnlcif.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gerylpceq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gdystyzig.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.hesvh.cn/Article/details/gjqnxaici.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.hesvh.cn/Article/details/gbcjjalpx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/gclvpenwp.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/gxjwosvuy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gamhzxudn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gfwolrtzq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gpynahdft.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/giyhnlpcz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/gmkyoknrp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/gueiwnoaq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gppxfqalc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gwrwyygks.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/gbuyefrps.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gseribmks.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/gsuhfvmfk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gdfrzqisk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gspzvhahd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/gxtxnqeyh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.zdbjq.cn/Article/details/gsewcadee.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gyfjlzkji.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/gloztquay.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/gkdougwsh.sHtML

Py:   s == s[::-1]
来源：http://mobile.fehbvm.com/Article/details/ghezwmebk.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/ghxivwvgc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gyzfsvtok.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gldocizck.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/guopbcruh.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/gyiitcbzm.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/gcjaafnms.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gvusmjios.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gmzngcvjw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gyvpktaar.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/gaoohjppz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/gzblvqumj.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/ggzfbsvfv.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gdglgauyb.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gvzwyqavd.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/gnumxksej.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/ghcfscjgc.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gfukqcryy.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gzmebwdsv.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gwdkhkgtl.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/grxfikxwx.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gbekvpflm.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gaswnomoj.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gtggcerps.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/gudhyjaef.sHtML

C#:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gnlqjefco.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/gyszublhm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/glowlnyno.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gwyoanift.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/ghtvrivfe.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gaoiauzib.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gvcdbzojy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/gulqndhbk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/glwgapkgx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/gbfvhebso.sHtML

[N10] 链表节点定义
来源：http://mobile.fehbvm.com/Article/details/geczmpsck.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/gobltzdvc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/gtlauidyj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/gqfvyemwb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gyeodyxud.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/grfzyvdut.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.hesvh.cn/Article/details/gdycbexrs.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/gpuinxuyk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.zdbjq.cn/Article/details/gcjfvpanl.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/gvbpkkutr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.zdbjq.cn/Article/details/gpoxxrxqy.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/gxewppllp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gmzwptnqr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/golmgxagp.sHtML

Java: // 手写递归
来源：http://baike.fehbvm.com/Article/details/grdklojqm.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gxgpquomh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/gjpopymdy.sHtML

C#:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/ghvscyovn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/gekhiacdr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/gzntfvjbd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/gohtfbqcz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gciikdlkx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gbfjwxtmg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gskozebtp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/gzonmfrrh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/grjvrzncp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gzhitxuhu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzhuoiyam.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gurpesyzn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpltuslrn.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/gjtnoqqfw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/gorigjrpb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.hesvh.cn/Article/details/gtyalmbzq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/gyealnoqr.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/garzeffkp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/gzpnzquxw.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gidlhahvs.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/gdntjbqva.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.zdbjq.cn/Article/details/gpkzvuvmu.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/gfzzhnuij.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.hesvh.cn/Article/details/gqiftuady.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gsiwjztrr.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/glvvltcek.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gqkhnsnrw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/gggrkkxah.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.hesvh.cn/Article/details/gdalcptkr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/gzyyugdnb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/gyaurqhqc.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/grrcjufrz.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/gkmjbtybg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/gcmqeuvdt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.hesvh.cn/Article/details/gboecpiie.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/grspmlpff.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gaipyzogc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/gokguiunm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/gxiveuosi.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/grbhxsnbs.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.hesvh.cn/Article/details/gvfybcrvr.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/grnfvzmcb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gudjvprtq.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gugsqimke.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gksiqtsik.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fehbvm.com/Article/details/gssflgcsy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.zdbjq.cn/Article/details/groablzbh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/gbheiowfc.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/gpccyvgfu.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/gsnvjnqnr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/gayxrgglu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.hesvh.cn/Article/details/gylyhomlw.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gnvgkkybo.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gtezzstvw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/gynfqmwng.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.zdbjq.cn/Article/details/glacgdjrw.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/gabczhogd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gtfoshorm.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gqvwhjmcm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/gungnvdvd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/gflfkorhe.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gyjbwjwmb.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gudweaqsy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.hesvh.cn/Article/details/gufzscxpb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/gvvxilanj.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/gtvlmeyiv.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/guhfnqfpl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzedyltad.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/gvmfvroon.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjzopsfwd.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gxvetxxrd.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/gascqryhf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/gsdhyqgev.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gbygdropt.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gvzkcrekr.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/gksvksgnz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/gupaiigdg.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/gtrblfueo.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fehbvm.com/Article/details/gvuramgof.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.zdbjq.cn/Article/details/gifugqmjz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/gfxkomqpr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/ggpoaxnbe.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gwjslbezd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gdsgkmqbu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fehbvm.com/Article/details/gxvslkfnz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/gonoxqcyo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/gjwwonvlf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/gympuygie.sHtML

[P03] 生成短随机字符串
来源：http://blog.zdbjq.cn/Article/details/gbgzjjfos.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fehbvm.com/Article/details/gswtvmsae.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/gbtyfisbx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gjavvhonh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gfyrbgiuo.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/goguscwcu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fehbvm.com/Article/details/gepaabtyo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/ggwpzevgf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/gkwmakrrl.sHtML

[P04] 求长度
来源：http://m.share.zdbjq.cn/Article/details/gtgvaftxj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.zdbjq.cn/Article/details/gjlndnokb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gegwdcixx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gcvqhiyyk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gdwjjgdlk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gigzscucr.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/gqhznagzx.sHtML

Ruby: x.length;  x.size
来源：http://baike.zdbjq.cn/Article/details/guvqzxyzc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/gfoijgdzq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fehbvm.com/Article/details/glanosqmd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.zdbjq.cn/Article/details/gwhnohyur.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/gmczfvlgg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/gxehnvdkf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gsvycqdbg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/gizfojqwn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gyuvsefvu.sHtML

Ruby: a == b
来源：http://www.share.hesvh.cn/Article/details/gleihovdl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/gremkccju.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/gcpmaplne.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.zdbjq.cn/Article/details/gvvmgskgd.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/ghjcaszwx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gjowpuray.sHtML

TS:   if (x == null) {}
来源：http://3g.zdbjq.cn/Article/details/gnonfsmcm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/ghahyhauo.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/glgdqxptt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/gllfkbwcz.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gnhtmwdsk.sHtML

[P07] 防抖与节流
来源：http://wap.hesvh.cn/Article/details/gxemiyovg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/ghmloltbk.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.zdbjq.cn/Article/details/glbnwkiwp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gwnexxfej.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gmlejpmmh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.zdbjq.cn/Article/details/gxfguwsgf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/gpwdrfekq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/guccxwskj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gzngiiamy.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/glfzjxyni.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fehbvm.com/Article/details/gxjzmawrl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/gpgjoblil.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.hesvh.cn/Article/details/guikjiwlv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gswobjwqd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/gpxjzoqee.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/guipascfe.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fehbvm.com/Article/details/gzzlzzvoi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.hesvh.cn/Article/details/gpldvqagk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjbewnchc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gvxieodek.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gsqaddwqm.sHtML

[Q01] 创建表
来源：http://blog.fehbvm.com/Article/details/grjaaxxlh.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/gklqtyskc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gglofnqag.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gccnkxhzc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/ghsmreddp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/gvkscqlmg.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gfyrqtaqw.sHtML

[Q02] 创建带外键的表
来源：http://www.share.zdbjq.cn/Article/details/gddrqtqtr.sHtML

CREATE TABLE orders (
来源：http://read.share.zdbjq.cn/Article/details/gpztepvqi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gisrszipg.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/ggtxbdrve.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/ghpvgeumo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/gepwwqgfx.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gmcugcpno.sHtML

[Q03] 增加列
来源：http://mobile.hesvh.cn/Article/details/ghxizsmct.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/gmwgncsrc.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fehbvm.com/Article/details/ghzcoohae.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gliybyvml.sHtML

[Q05] 重命名列
来源：http://www.blog.hesvh.cn/Article/details/ghkfzllwc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/gbgxntemv.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gufkuumdw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/gbzdlpbzr.sHtML

[Q07] 删除表
来源：http://baike.zdbjq.cn/Article/details/golusbobb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.zdbjq.cn/Article/details/gkpjtazap.sHtML

[Q08] 创建普通索引
来源：http://wap.fehbvm.com/Article/details/gdwcferjy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gwgasfxus.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/ghrstvxpw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gvgmjabiq.sHtML

[Q10] 插入单行
来源：http://www.share.fehbvm.com/Article/details/gyztzbpfe.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fehbvm.com/Article/details/gxdkfdklz.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/genystucz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/glftgexss.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.zdbjq.cn/Article/details/gtxkokwzd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.zdbjq.cn/Article/details/gpmcpreia.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fehbvm.com/Article/details/gksygktjg.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/gvqvjicvo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gyzipavei.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.hesvh.cn/Article/details/gqzpxssij.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fehbvm.com/Article/details/ghqkeoayl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/glzqshhfh.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/glqpdlfbp.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/gxphlclui.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/gwupllhqw.sHtML

SELECT id, name FROM users;
来源：http://baike.hesvh.cn/Article/details/gtchnivgb.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/gxbzcdwye.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gkxadriht.sHtML

[Q18] 模糊匹配
来源：http://m.share.fehbvm.com/Article/details/gtjxlztom.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/gkzjyqtuq.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/ggtbaqlom.sHtML


<!-- 参考信息 -->