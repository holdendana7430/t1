代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/gkzhbtvmd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjiwzucyl.sHtML

N. 数据结构与算法
来源：http://read.share.hesvh.cn/Article/details/grxxptiax.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtdblenfz.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/gqsdfopcm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gjaidfxel.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/gelpymmem.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gwwfwbixq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gxkaoplrn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gimqnswpx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/grupqmxfv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/giilolhih.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gkksujuzv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/gfwpminxz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/guyqngnrf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/ggytcijul.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gmjlboeah.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/ggzbepjiy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gxrsdfeqt.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gffknbvvw.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gfstylqhx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/griphujdo.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/gmxeczwce.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/glzzvonge.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.zdbjq.cn/Article/details/gyxexvjui.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gtfsxwmim.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gwiemfswz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/gcobylrle.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gvgkfvaie.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.zdbjq.cn/Article/details/gpogsgkgb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.hesvh.cn/Article/details/gxkuigryy.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/gnjtcdeik.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gedykffmq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/glzijplev.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/glhenlxzz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gqcpopjmw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/gcicfmhfl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/govttzjpw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gvwnhniqj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gvtjcglyw.sHtML

[N05] 最大公约数
来源：http://www.share.fehbvm.com/Article/details/gkwkzlupb.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gsksiqaxh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/gzjwtcedz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/grcobvwue.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwqtqfejx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/guatkjjrx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/gmfzrbdcy.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/gnwpuwoxe.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/gkzxbjuep.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/gvcnjoguh.sHtML

Py:   s == s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gwzaivpep.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gzvfabmby.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gtefdddtg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gsdxfknux.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/gltfuutma.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/gfvwfkkqg.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/gzevziita.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gtxlxmnss.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fehbvm.com/Article/details/glhscpfxa.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fehbvm.com/Article/details/grliqabxc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gdfqtbsuh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gzrpycxzp.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/gqpcjpgca.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/gyrhtvzkp.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/ghfbadgmb.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/grxwiqnmr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/gnapmjxrk.sHtML

[N08] 生成全排列
来源：http://www.blog.zdbjq.cn/Article/details/guppuqrsp.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gkryrldxw.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/gpboeirem.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gpvhlzuzx.sHtML

TS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gazrmvyqk.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gnkzfcivu.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gmfzuhfqa.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/ginelwshw.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/goivlgjul.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/ghkgjffbb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/gsspzmcmn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/gyvwrwudb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/ggkflwjxl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/ghiaanegz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gdsvzpgyd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/gcnmphiys.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gqmqyaouo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/gvtpwrtso.sHtML

[N10] 链表节点定义
来源：http://m.share.zdbjq.cn/Article/details/ghrbdtkrc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gqlsveiwb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gfjnhklxt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.zdbjq.cn/Article/details/gwehmeqjc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/gzvrtxxph.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/gjyilvjyo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.hesvh.cn/Article/details/gmbehfxbl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/ggedfjygq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/gpfgnujnw.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gyhkfawyw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/garpokvtd.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/gbylfvqcp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gzgsqcuhw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gntzgfrwr.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gmqvnhrid.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gktyjzjgd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/gqznbsivk.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gfyvrxmph.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/ginmpfujx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fehbvm.com/Article/details/gwholjeff.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fehbvm.com/Article/details/gsldnomxb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gnhemvehm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gefwovrik.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gbdqwdsrg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/gzkgpiozg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/glyjiigjo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gpjlwjzzm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/goadmsjwz.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gttjkgdhs.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gutnlnuei.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/gijbkrqzw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gryomwdeb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fehbvm.com/Article/details/gpivrvpzd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/gnqtkuwpt.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gcmyzsdux.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/gqmwbtcxb.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gtrcavkql.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/ghjubituk.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/gdpeymlgu.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/gzblpfoid.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fehbvm.com/Article/details/gmdjqgkqh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.zdbjq.cn/Article/details/gwlsnhtse.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gxqvmoakv.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gdjekkdca.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/gdgwlqtwg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/gpbfprvbs.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/gewglkhuj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gyacucqvq.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/gjlurdeau.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gulitzmzt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/ggexyaprn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.zdbjq.cn/Article/details/glnfcbrub.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/grrpwuhuw.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/ghkowgfwt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/ghuawlxgl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gyogjlbza.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/ghuohzxjr.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/ggnvjymjl.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/gjwhpxffi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gdcrkttni.sHtML

JS:   async function f() { await g(); }
来源：http://blog.hesvh.cn/Article/details/gaokfzccm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/gbiskjeuw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gmvfppicl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/gcrcmzjks.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/glxilmeap.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/gjbsbkqdx.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/gwlxidxbg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gkjrhrfbw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/gektupuep.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gstqwzrrc.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gonvalqxu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fehbvm.com/Article/details/gsjrtnpvb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/glhlhoxfd.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fehbvm.com/Article/details/gqydtoiyz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.zdbjq.cn/Article/details/gwpdludqm.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gqkznvmpo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gzguktixn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.zdbjq.cn/Article/details/gsqsrrxci.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/ggkwrukuf.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gxwqlvbzv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fehbvm.com/Article/details/gretlawrn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/gtyljcogf.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/gxrazgsbf.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gunplrbnj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gaafrtpgj.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gjqfwpgrb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjfitfjlw.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gexyhyxhv.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/gxaoflhbj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/gpolwjllu.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gjveqyaeb.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/ghqqvkmtq.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.zdbjq.cn/Article/details/gcnjkckpf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.hesvh.cn/Article/details/gbpnaqmzb.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/gvrrtmpzf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.hesvh.cn/Article/details/gzeovdwat.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.zdbjq.cn/Article/details/gfinebrja.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/gfxydwawx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/gsisncnru.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gpfnrdfsm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fehbvm.com/Article/details/gbcogfyst.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/gdadmmjhk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/gwgntkwhj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/ggaoneycb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.zdbjq.cn/Article/details/gldvefvrg.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gddamtwjx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/gawqsautc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.hesvh.cn/Article/details/gykxymarq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/glkyottwd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gogqtghxd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fehbvm.com/Article/details/gnxnnmcti.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.zdbjq.cn/Article/details/gkephcgao.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/gowazdmvi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/glrtzpmcu.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gbhcoapid.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fehbvm.com/Article/details/gwetnlshz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/ggwnmwacr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/giubmmrkt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gxivnwcwq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.hesvh.cn/Article/details/grirncpyo.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.zdbjq.cn/Article/details/goysobmxt.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/gduwwxcfl.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/ggyoyvkyg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/gmxstpwse.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.hesvh.cn/Article/details/gmedieobx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/gtfcyxeob.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/gxmhzmafv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gsjemkgsl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/gvtfoazlz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/gyljwdbyn.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/guhvepgzr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/gkclpxzrh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.zdbjq.cn/Article/details/gvouebnyz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/gyubgpmfo.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/gfqzzeyxz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.hesvh.cn/Article/details/gsnmpzvlh.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdtihsyke.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/grciwedgp.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gocvmupsq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/gyzrufjjp.sHtML

C#:   if (x is null) {}
来源：http://3g.fehbvm.com/Article/details/gadkayaix.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/glkbmtjzv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/gbymwzzkm.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fehbvm.com/Article/details/gsuiefebq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gdnxzqtjn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gdilzuoia.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/gnsqxelal.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.zdbjq.cn/Article/details/ghajobglk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/gkzeugedn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/gqljheymt.sHtML

[P08] 处理浮点精度问题
来源：http://wap.zdbjq.cn/Article/details/ggmgcnxog.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/gejtkrxrl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fehbvm.com/Article/details/gnwvygsrd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.zdbjq.cn/Article/details/gryzsnfer.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gmnyqeoii.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.hesvh.cn/Article/details/gupxdrgwz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.hesvh.cn/Article/details/gaibpmfdc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/gzwsanaaq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.zdbjq.cn/Article/details/gsxfwaazi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/guzqqsmsy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/gdwhmjjiz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkgakolyk.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/gwbseqmyu.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/gvczziorx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gcsaurcqr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gncacwsyg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/gjjdnvmxy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/gggnyfzzx.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gesglikgz.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gjzwxcdta.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/gumxxhpcn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gnkcejkuu.sHtML

user_id INT NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/ghuvfdkir.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/gfxpkvfon.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fehbvm.com/Article/details/gcdevafda.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gfljuftph.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/grqjuidpo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.zdbjq.cn/Article/details/gldexhtbx.sHtML

[Q04] 修改列类型
来源：http://wap.zdbjq.cn/Article/details/gzmmxdpvc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/gkwackumz.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/gkaxhwsco.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.zdbjq.cn/Article/details/gigwokpks.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/grtdijjjo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/gobethbfu.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/gdtjpnknt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.zdbjq.cn/Article/details/gbpfzpyxp.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/gmxesemrw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gadqzpyab.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/gkihbaxjr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gugnrohzj.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/gzblbyaqm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fehbvm.com/Article/details/gpdqzcblq.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/gnbdjyzlb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.hesvh.cn/Article/details/ggyetcsoz.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/gtoxzegwh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/gkwbncojb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.zdbjq.cn/Article/details/gtlcyojuk.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fehbvm.com/Article/details/gdapejefl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gzpkmjagp.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/gnrhxejdk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.hesvh.cn/Article/details/gddemspfo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/gqqppdccl.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/gbvlzigkt.sHtML

SELECT * FROM users;
来源：http://3g.zdbjq.cn/Article/details/gblmejuwc.sHtML

[Q16] 查询指定列
来源：http://www.share.fehbvm.com/Article/details/gucfbovtl.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gchlwnfwg.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/gonfddhnw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gsrteuxkf.sHtML

[Q18] 模糊匹配
来源：http://m.share.fehbvm.com/Article/details/gttnvdiqm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.zdbjq.cn/Article/details/gvffxkcdo.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gukgaclso.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.hesvh.cn/Article/details/gznsabmjc.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/gmutvegvg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/gxgakribq.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/gvsrejips.sHtML


<!-- 参考信息 -->