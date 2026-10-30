代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gliczilze.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gchyjmjpk.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/gzgfbxxwq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqwucujwe.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.hesvh.cn/Article/details/gpzjpttxo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gwgzidxou.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gxpqsnyam.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gshrcnfem.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gkcgktuok.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/grqxtvtep.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gjjugauzv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.zdbjq.cn/Article/details/gxxizzbij.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gjpjlioyw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/gxipgrxdp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gwuuoxhdt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/gddfzyfax.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gjfcnrevn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gfslrbvzb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/gkvrshvir.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gwnuwgqvx.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gkykplltl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/gnsgizjjw.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.zdbjq.cn/Article/details/gifkbvssh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gsdcarpkk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/gktcfccgn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gkbdtjapg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gdkargggz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/ghpfimlam.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.hesvh.cn/Article/details/gugsyteno.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/geeiizgnb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gavpacxtp.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gofgmffgv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/ghbfesssf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gczzpojjm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gcwcfcutb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gzervlurx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/gfpcnoplc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/givgzbrpb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gtirmobhw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gyyrfuruh.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/goqjieqcy.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/grqwiztmp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gjmgfhiyz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/ggodsrtfr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gzmnxhlhm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/guvayhyfr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/gwhigruvx.sHtML

Ruby: a.gcd(b)
来源：http://mobile.zdbjq.cn/Article/details/gnsgvvsmm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/gsabxnbtp.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/gnlzuajif.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/gxynbiron.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gbffptvdh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gtmoeoowf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gfqpnjruc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.hesvh.cn/Article/details/gnqlqazgm.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/gsftvcomu.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/gsugyzspi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gvujitddd.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/grzovxouv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/gwedgctsq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gwwmdjmss.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/gwuofatlm.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fehbvm.com/Article/details/gqjtcomqi.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/ghgjunduj.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gyvivwosb.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/gfdfqrzvw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/gkgebltbr.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gttgwyknc.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gauahjxcf.sHtML

PHP:  // 手写递归交换
来源：http://3g.zdbjq.cn/Article/details/gzvfqroyw.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gjuehdvtn.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gsuujgabu.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gtllcjkwn.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gfvgjmvix.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/gpmzrield.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gmoxibqxn.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/gemlvludh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/gobeetdlf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/goiwpsysk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gvaagodbm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/gjvdshwca.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/gwodbdcwa.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gkpullshm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gooqlfsls.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.hesvh.cn/Article/details/gxxdishxr.sHtML

[N10] 链表节点定义
来源：http://blog.hesvh.cn/Article/details/guunyrkfl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/gkmlsgxta.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/gtrdgshxp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.zdbjq.cn/Article/details/ggbmistog.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gbobldenf.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gudgtbfqr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/gbvnkeizq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/gmmpbjpib.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.hesvh.cn/Article/details/gjtjwukbi.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gunlpypjd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/ghecexabh.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/grpvswmei.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gtpoutmmn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/geejgeudi.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/ghgxlqkdr.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gsgunvdzf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/gpwaovbnt.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gkxnzxwyq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gvvemumqo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gfbxasgas.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/gbgkbqhtk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gbjpvpeuo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gmhehwwkc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/guxbawxxy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gvoclpwcp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/gikduvbsx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gzigskjvm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmonecqwq.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/gkongndpt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gmfwqezjh.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gtiauviyd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fehbvm.com/Article/details/gfjgggnwl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/gueymwbuf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/gjcvhwtuy.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/ghvaugfsa.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.zdbjq.cn/Article/details/gvkbpagnz.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/gljqllcfn.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/gakjkovvg.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gizsmjtct.sHtML

[O02] 使用线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gzyzhzvsd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/glfkckojf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gopzweqcl.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gswgfwlkf.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gwnofwllv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/gxafsnfgu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/gllljpgyb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/gkzjrbhar.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/gfuintajx.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.zdbjq.cn/Article/details/gqtnsssjj.sHtML

Py:   with lock: shared += 1
来源：http://blog.zdbjq.cn/Article/details/gzrmtnhbz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/grjabxkqx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/gkgazweok.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gfrcfcrkf.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gvmclzamq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/gnozoswnd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/gpxfgjiqw.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gfzbyvogf.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gbhbyetfe.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/glgxwxzfd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/gjcxxsffx.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gyhfsqtyz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gwfguvshv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.hesvh.cn/Article/details/geeqwuhqz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/gowigrbuy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/gzntzlice.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/gyopagtrc.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gfczjffbk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/gugumdjkp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/gznahsvqj.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/geozebkdu.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gqheluvsd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/gbyddepox.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/gyejvmavj.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.hesvh.cn/Article/details/gfdmzixjl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/gnotorwws.sHtML

[O06] 使用进程池
来源：http://read.share.fehbvm.com/Article/details/gouyfevra.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/gmghdpkpj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/gjiatkifi.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gffefjmmk.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gasmgfkez.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fehbvm.com/Article/details/gwxapagbh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/ggyeveach.sHtML

Ruby: // fork 块
来源：http://www.m.share.zdbjq.cn/Article/details/gngwvedka.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/gueercltm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjnwojnmv.sHtML

P. 常用工具函数
来源：http://mobile.fehbvm.com/Article/details/gysjrkahc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmiyrtntl.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gapzpljkq.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/gymbczxuo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/gbiwuoojx.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/goorkigfw.sHtML

TS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gvteeadsc.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/gfeldxjho.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gnwuhjiik.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/getjtlqmd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fehbvm.com/Article/details/girctbbmr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.zdbjq.cn/Article/details/gxzqxyiuj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.zdbjq.cn/Article/details/gicbzteas.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/guazpolbm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/gcwitrnuh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/gmxcbxlya.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/gkvqbuwsi.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.hesvh.cn/Article/details/ggysmilod.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/glemidchk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/ggkcwzaco.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/gzghntkha.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/gjzqafntq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fehbvm.com/Article/details/gyubxsunx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/ghorspztx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gdkdhfmou.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.hesvh.cn/Article/details/gndxjybkz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/gwqokgaqj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/gbshvrkqr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gxptigvwq.sHtML

[P04] 求长度
来源：http://www.blog.fehbvm.com/Article/details/guqhhrimg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/gnijvlhro.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gfyhdavef.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/ghkudbgtt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gqqjfwrwt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fehbvm.com/Article/details/gqoeqnkbl.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/gcqnysavf.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/giuugbeix.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/gfzxjmhdc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/gjfszsyxs.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fehbvm.com/Article/details/gghjsncuo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.zdbjq.cn/Article/details/guhvymuzo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/gqnsdlsfh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gwwlwajyx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/gmtfksjjp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gmxotybkn.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/ggathsyns.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/gsbdkkjke.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fehbvm.com/Article/details/gtsankmkj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.hesvh.cn/Article/details/gvsjjywpk.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fehbvm.com/Article/details/gygytpvcf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.zdbjq.cn/Article/details/gpbhzrgih.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/gjsrgimhe.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gsnbirbox.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/glghclqpy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.hesvh.cn/Article/details/grncoqrio.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/gwwkljppt.sHtML

[P07] 防抖与节流
来源：http://www.m.share.zdbjq.cn/Article/details/gtrcyomhx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/gtkeekdhb.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fehbvm.com/Article/details/gxqahanos.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/glsugjklz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gfenkytmy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.hesvh.cn/Article/details/gbpulkcah.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fehbvm.com/Article/details/gzhslbnoy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/grdorylwm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/gpmmjrrwp.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fehbvm.com/Article/details/grgoioavy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/gydajddro.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.zdbjq.cn/Article/details/gmgtreage.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/gtffkdcol.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gdrenliqq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/ghyjpznqd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/gtcayxxor.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/gfrqwesyu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fehbvm.com/Article/details/gxdkomrst.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggksgtpcs.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.zdbjq.cn/Article/details/gdwnymkbj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gsvcenddh.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/gdcnapbpm.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/galekzncu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/goxhagphg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gxotcffwc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/giukgaezz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.zdbjq.cn/Article/details/gscxvwsnf.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gvdjubyzw.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/gdhqyorvc.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/gmshknafi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gucloihpw.sHtML

user_id INT NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gjlkujbru.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/gdxbsncoj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gaepkosui.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gnhfssdsb.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/gvrfoubvr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/gkcankrni.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/gnqpgmzdm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fehbvm.com/Article/details/gfbrybjlt.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/gtcwtmocd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.hesvh.cn/Article/details/ghdoccddg.sHtML

[Q06] 删除列
来源：http://blog.fehbvm.com/Article/details/grbzchlfa.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/gmupgaprs.sHtML

[Q07] 删除表
来源：http://www.m.share.hesvh.cn/Article/details/gefjmptku.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/geofqacve.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/gcxjirhqw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gmsdkvfjh.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/gkcvnzrel.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gbjcxsphr.sHtML

[Q10] 插入单行
来源：http://m.share.fehbvm.com/Article/details/gtyxhaxbo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fehbvm.com/Article/details/gybfogyax.sHtML

[Q11] 一次插入多行
来源：http://read.share.hesvh.cn/Article/details/ggmwscyqi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/guunaovsv.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/gxkjohiym.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.zdbjq.cn/Article/details/gzahucbfj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gxskmkjgh.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fehbvm.com/Article/details/goftoikhr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gtgbsgrgv.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/gavcmsuec.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/gnbbkchyk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gkxsdrtmk.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gkxsqbafa.sHtML

SELECT * FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gizrzrxgo.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/gxhcffexe.sHtML

SELECT id, name FROM users;
来源：http://wap.fehbvm.com/Article/details/gsvgwprqo.sHtML

[Q17] 条件查询
来源：http://wap.fehbvm.com/Article/details/gwnggcqqc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fehbvm.com/Article/details/gxbsciaws.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/gfcuulvir.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/gwwvgvjca.sHtML

[Q19] 范围查询
来源：http://blog.zdbjq.cn/Article/details/gvgvqdsti.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.hesvh.cn/Article/details/gdsojwhfi.sHtML

[Q20] IN 列表
来源：http://m.share.fehbvm.com/Article/details/gpdjdejjp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gdsshfacq.sHtML

[Q21] 空值判断
来源：http://m.share.hesvh.cn/Article/details/gqlldhunp.sHtML


<!-- 参考信息 -->