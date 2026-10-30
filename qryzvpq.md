代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gsldpavfe.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gziyatnwf.sHtML

N. 数据结构与算法
来源：http://www.share.hesvh.cn/Article/details/gnuybjghh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbmgeotsj.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/gifpsctjx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gadeuuxtu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gzexsjyhn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gqrymebox.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gjnttgyty.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/ghxljyzlb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/ghzqyztlx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/ggpmierkr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gwjhwuuyk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/grfkamutz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gwmvjjsok.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/ghnwbsfhz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/ggawyyrlo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gmzygqasw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/geqitzguz.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gqbeuoasy.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/geiipqiwx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/gxjcsgkyh.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/gsaxgzgpf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/gvwuezpvk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/grquhnadl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gahaemtgi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gshtkhfuh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gzsjplkds.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.zdbjq.cn/Article/details/goacdeazp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/gqshobmno.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/gprfondsv.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/gzhbibnfn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gieuxezwa.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gacwydskn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gkoatkmtp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gphspulfc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gglojfavg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/gsdckxvlv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gpxicrddm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gimvxluts.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/gjsbmghfx.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gxhggrutu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fehbvm.com/Article/details/gvkhbcnjl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gqbyagevc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gwzxttxwq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/gldrrihto.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/gwbyysnwq.sHtML

Ruby: a.gcd(b)
来源：http://www.share.zdbjq.cn/Article/details/gvqikmupb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.hesvh.cn/Article/details/gohjkkzjm.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/ghghysbhw.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gepwfxbts.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gusnuxjtm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/genzavrlm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gtfliikjl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/gbgfbsshn.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/gkpgijyne.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/gsbbkeatp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/graqucirw.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/gdudcccgg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.zdbjq.cn/Article/details/gotvehocv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.hesvh.cn/Article/details/ghyxqouuq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/gdqtxypby.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/gicbipktq.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/gpimrxnly.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gdeyxqhbe.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gnuzmphii.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/ghektiviq.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gkshwdgan.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/gangvsqgn.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.hesvh.cn/Article/details/gpjczrnwo.sHtML

JS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gtfoxskfd.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gvljaymws.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gfdiyynus.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gqlslxtjc.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.zdbjq.cn/Article/details/gncoknqnn.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/grbmfgcxf.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gatdqubxc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gbqviihjv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gaeaehqwn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/ganncsaft.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/guvjnrjez.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gplwrocwy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/ghjwcfjan.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gugrrlpyp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gdmumfwaf.sHtML

[N10] 链表节点定义
来源：http://baike.hesvh.cn/Article/details/gfkrpibwb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gmknuiutq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/gaflodyxb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/gwjmaqfhe.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/gkzkrnmmt.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/glodorouq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/gaxfgrerq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.zdbjq.cn/Article/details/gajkqkevh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/ghjokqqci.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/ggxjejrrh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gswclgnsz.sHtML

PHP:  // 手写递归函数
来源：http://3g.fehbvm.com/Article/details/givbbmtbq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gjrhbbtwe.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gsdqdixou.sHtML

Java: // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gymptcjss.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/grrjswneb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/gpsnjcnly.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/glrezvbhg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/glhrpgaoe.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/gntxejrtw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/gffusbzfp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gcsdfdljq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gbzehjhqz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/glewukfpb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/gypnoxrtr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/gxiodkryn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/ghlgpujhr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzabpogrj.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gqbbbdfyn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbulngmgy.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/gienirlnt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/guukqsmzy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/gcbiqvkie.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/gvtmczkqv.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gvuhmwikn.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/gjowrnbwu.sHtML

Go:   go f()
来源：http://wap.fehbvm.com/Article/details/gsiygxhtm.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/gylcoobbg.sHtML

C#:   Task.Run(() => F());
来源：http://3g.zdbjq.cn/Article/details/gdioejpsg.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/giotkwtuo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/gpmscfiat.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/gructpczt.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gpfzuyuve.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gfrzhepgw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/gcbxqqvqj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/gvbkhvemc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gmmkntsnx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/glaulriop.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/gnzwyytad.sHtML

Py:   with lock: shared += 1
来源：http://www.share.zdbjq.cn/Article/details/gccdosagw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gtgbrjklj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gmnjqbkqa.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/ghxhtlgqb.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/glkrvejbd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/gffctzmyh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/gfcmkbcps.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gnjlluupz.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/gevjpkelw.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/gwhslteih.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.hesvh.cn/Article/details/guznocwaz.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gzvzsvwmx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/gynyftnnc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/gfyworodr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/glqiqyldl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gpieyoynb.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.hesvh.cn/Article/details/gkkpkbkhd.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/gcgwtbkyv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/gtjxyoubu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.hesvh.cn/Article/details/gccgwjawd.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gtwyhkyjv.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/grdzkykll.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.hesvh.cn/Article/details/gnwhvjejj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gdjzncmtl.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/gdltglqlv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.zdbjq.cn/Article/details/gotaoxava.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/gufhklgbe.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/gvcirfbgn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/gxhvfkhhr.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gwplkbbsw.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gvlyyedrz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/gypnagkbl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/goniozamb.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/gojkbokki.sHtML

C#:   Parallel.For
来源：http://mobile.fehbvm.com/Article/details/gogoctouv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqcfsuzpa.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/gpjhvtsdo.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdjqpryop.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gsmburgug.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/ghqsxresz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/gqtkkaejr.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gojooilym.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/geqbulwtm.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/gfzgpzaof.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.hesvh.cn/Article/details/gyatakarf.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/glmfqunvh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/gtvisnhyy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gcpkmjzdw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fehbvm.com/Article/details/gkxaqtxwg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.hesvh.cn/Article/details/gjcyccmxg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/ghsrqjtqc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/gwpmpgfxj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gbgamhbdh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fehbvm.com/Article/details/guymyidjk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.zdbjq.cn/Article/details/gxeixcetr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/gdxejfohh.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/gerybeueu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/gtptparbp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/gwnggzosj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gtluongbe.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gpchlexgn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/girghgsth.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gaghopbht.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gqqntdegn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/granyodyj.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/gamowasea.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/gienthfrk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/ggkuoyqxz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gqufjvncj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gkflrwbvh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/gsjpltuct.sHtML

Go:   len(arr);  len(m)
来源：http://baike.zdbjq.cn/Article/details/gueppieth.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fehbvm.com/Article/details/gewcnxvkn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gjntyiffp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/gotyccdgn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/gfnalygih.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/gesuexouf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/gfqcfiyqp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gejemtbde.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/gytznfhhn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/grvhcziit.sHtML

Ruby: a == b
来源：http://www.share.zdbjq.cn/Article/details/gwhjmgrxk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/gapcbujkr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gbflidmef.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/gywqvejgu.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gfuqwyztq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.hesvh.cn/Article/details/golfujwbw.sHtML

TS:   if (x == null) {}
来源：http://www.blog.hesvh.cn/Article/details/gbfzqdomr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gcdnaxlsi.sHtML

Go:   if x == nil {}
来源：http://wap.hesvh.cn/Article/details/gxgffofsj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gdyzhwnxn.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/gbfyxltcq.sHtML

[P07] 防抖与节流
来源：http://www.share.fehbvm.com/Article/details/gchahnbvi.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.zdbjq.cn/Article/details/ggqwwfoif.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/goeagvfro.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/ghwjirbid.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gpoawfqpa.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/gaqonchqb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/gvractiua.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/gkoqkegpm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.zdbjq.cn/Article/details/gslhkyxke.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/gkkfxvfrx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/gnefpcqps.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/gcalxzeyv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.hesvh.cn/Article/details/gyaghjdam.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gjsmrjlgj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.hesvh.cn/Article/details/gqbqqxnmh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/gprlcezbv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.hesvh.cn/Article/details/gcpcwkami.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gfuqpmvhp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghxasquqq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/gfribnadj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/goeggdxoi.sHtML

[Q01] 创建表
来源：http://mobile.fehbvm.com/Article/details/gimqriaxo.sHtML

CREATE TABLE users (
来源：http://m.share.fehbvm.com/Article/details/glhvhsfip.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gzegwjyub.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/glcvnsjdk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/gftdyaqsp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/gwiumpsjh.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/grybbnyei.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/gcsfbwkjt.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/gmurktkdz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gvjzvsaxl.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/guimriwni.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fehbvm.com/Article/details/gfajgzvaz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fehbvm.com/Article/details/gbnjblzlm.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gqhlyrvqh.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gvelrpakq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/gpblhchpe.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/gmxzxvyeg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/gpyvxlhyg.sHtML

[Q05] 重命名列
来源：http://blog.zdbjq.cn/Article/details/gcizbiuyp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/gvlawkssj.sHtML

[Q06] 删除列
来源：http://baike.zdbjq.cn/Article/details/guulsuemg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/getyacdub.sHtML

[Q07] 删除表
来源：http://blog.hesvh.cn/Article/details/gbkgbscqc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/gezsnzhtu.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/gmingjuzo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gqyrzpmxy.sHtML

[Q09] 创建唯一索引
来源：http://blog.fehbvm.com/Article/details/gobsitozp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gecmyufev.sHtML

[Q10] 插入单行
来源：http://3g.hesvh.cn/Article/details/gvotlynqv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gepbynzzg.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/ggcnftuda.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gabeklwmy.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/gyblmkvjt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.zdbjq.cn/Article/details/ggeekblqt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/ghdlmifuk.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fehbvm.com/Article/details/gnwtatrly.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/ghnqcckfz.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.hesvh.cn/Article/details/gtoacpluf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.hesvh.cn/Article/details/gyxktyqny.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.hesvh.cn/Article/details/ggymlmxaj.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/gwmpigyzd.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gvkpwlkig.sHtML

[Q16] 查询指定列
来源：http://3g.hesvh.cn/Article/details/gqijfhcox.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gjvfijhxs.sHtML

[Q17] 条件查询
来源：http://m.share.fehbvm.com/Article/details/gdlxnsyae.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fehbvm.com/Article/details/gioozdgnb.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/gpgjuxvlb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/gvcxcpafv.sHtML

[Q19] 范围查询
来源：http://www.m.share.zdbjq.cn/Article/details/gntkmsklt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fehbvm.com/Article/details/gmlxbbgjs.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/gytxcefre.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/gixquuddy.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/gbynikxse.sHtML


<!-- 参考信息 -->