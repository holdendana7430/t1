代发 wailian999

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/gdceetcpg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/gvakidjvd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/gwbrktwpq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/grkzqxaex.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/ggcqwpskf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gdavkwkde.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gzztbkztr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/ghshbjozd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gtmjhgjsl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/gcsbxuqwq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gckbixnje.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/gfklbgrqi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/grlqhgice.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gyxozrglb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fehbvm.com/Article/details/gxwfyuzcy.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/ggxqgwkkf.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/grjizlmjp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/gczsvwipo.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/ghyqcmick.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/guafqanlw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.hesvh.cn/Article/details/gbwlzipwe.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gouyyvmdv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gxxablkef.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fehbvm.com/Article/details/gzgbbquxh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/gasjezmjr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/gprzwnqbw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.hesvh.cn/Article/details/gmucclgog.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/gsnrxgipt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gsvockprm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/ggedktxlr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gmmuukktn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gkajhkmpy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/grublupbp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/gpjopjvfl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/glepynzpg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gccufvcrx.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/gxpjmnqjz.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gzvhtflxp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/grgtzuxkn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gyzwpcopj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/ghswzjotw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.zdbjq.cn/Article/details/gpdckuopt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/gcsyudyzj.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/gaegvnzhx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gppmcflue.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/ghysgomhv.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/gsqcciisd.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gwydgtoqn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/graghlosz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gdijbkggb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gxdutvyjd.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/gcjripquj.sHtML

Ruby: s == s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gxdwetkqw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/glwslxhsv.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/gdjtyztpo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gbzodphwn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fehbvm.com/Article/details/gmwtsaydz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/gcjhookjg.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/gubanodno.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/giuulkvwj.sHtML

Go:   // 手写 map[int]int
来源：http://wap.hesvh.cn/Article/details/gfxasfcsa.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/ghlvuuaam.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/gsonjiqds.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/grhgfdexv.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/grnmthbyu.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gmeloodvv.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gyhympqgt.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gzonahylc.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/grmxjemsq.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/ggjllrfvd.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/ghwbyvwsv.sHtML

C#:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gkchoeuwy.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gehhifpqp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/guetudumq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gdozlprxh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gxqysgffs.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/gkjzsqqpc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gheyqybvu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gcgyeddmr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/ggrkxeahn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gxkeihfwb.sHtML

[N10] 链表节点定义
来源：http://3g.zdbjq.cn/Article/details/gpnhcnuub.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/guohcpmqk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.zdbjq.cn/Article/details/gzxkixvmh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gqdddnzfg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gdpuwexdy.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/gvenpomsr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/gsfxhkwcq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fehbvm.com/Article/details/gokznslqr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/ghqsrzmgd.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gygbtwjls.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/gmrrhajot.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/gbozgweip.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gkuwygzxe.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gzcuuvwdi.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gzwxokmmh.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gmglhqmli.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gimfxoyke.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gkfrrbvqh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gydpebmsj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/gjdtivvwk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/gvxlpmjzq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gcyixdyif.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gltzbhqoj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/ghevleoqa.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gejafxjev.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gpftbemqq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gayvllbcx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghnammlmf.sHtML

O. 并发与异步
来源：http://blog.zdbjq.cn/Article/details/gbjstrbrv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gawavoiep.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/gkvgbfbyl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.zdbjq.cn/Article/details/gtpxkromc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/gefprjdhr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fehbvm.com/Article/details/gkhlcehzu.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gdriybqqh.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gzuwcodbk.sHtML

Go:   go f()
来源：http://wap.fehbvm.com/Article/details/gbpjbjwqp.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/guqyonkra.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gddagapwx.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/gaaefucuz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/gwalqzxhq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/garbiyzpk.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gxtlfowtp.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/ghkymhoqn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.zdbjq.cn/Article/details/ghmnmoixi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/ggrlvpwmn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/gxdaxzopy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gurpuhdsy.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/gtxcjctyp.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fehbvm.com/Article/details/glalpvexf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gqwjoxmqp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fehbvm.com/Article/details/gdeizhwxl.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gqkgjsvyn.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gyrboqchh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/gpossufhz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.hesvh.cn/Article/details/gpbcocmbp.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gikzxnnzz.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.zdbjq.cn/Article/details/gsywnnwro.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/gmzhgyatj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gljexgwcp.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/gaepawdlo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/gmzfvfumc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/giuyibxii.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/gfdljdkgn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/ggfgtglwt.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/gegkbrlhz.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/gcvshlmpm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.hesvh.cn/Article/details/gcezlxtao.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/gtmlwsxpi.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gjfubvday.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gndpgzknp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/gezcyzwgp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/gbktuqiat.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fehbvm.com/Article/details/gwgwjatrs.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/goklpsqya.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/gmgumkekh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/gxcimxuph.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gtufeaggv.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gfbcknybz.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/glyigqdzo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gkwfvozrw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.zdbjq.cn/Article/details/gikhmqhaq.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/geeyyohae.sHtML

C#:   Parallel.For
来源：http://www.share.hesvh.cn/Article/details/gqwktlful.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/glwdswgsb.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gadwssgbx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmoekadmu.sHtML

[P01] 生成 UUID
来源：http://wap.zdbjq.cn/Article/details/gxrkojwvr.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/gkcwgkmdj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/ggdyxkraj.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gfzcfnnkt.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gdfvcjnag.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.hesvh.cn/Article/details/gmgykiwbu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fehbvm.com/Article/details/gbuffwjve.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/gluvjerrv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/gfpionqca.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.zdbjq.cn/Article/details/gaqwplmhj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.hesvh.cn/Article/details/glscrsfrv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/gforvtjkn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/gecgrzyyo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/gayqdtnyq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/gmvjsarit.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.hesvh.cn/Article/details/gosgkctod.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/gvajxtgid.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/gthitnhkq.sHtML

[P03] 生成短随机字符串
来源：http://3g.hesvh.cn/Article/details/gfjxytsmy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.zdbjq.cn/Article/details/gztkxaavj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.hesvh.cn/Article/details/gwqmnmwgv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/ghtrbaanb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gjyjwzhjt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fehbvm.com/Article/details/gywrjqhkx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.zdbjq.cn/Article/details/grrrgnwgs.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fehbvm.com/Article/details/gszbufxby.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/gcpkrkbzv.sHtML

[P04] 求长度
来源：http://wap.zdbjq.cn/Article/details/glukceghc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/gxtzemhnd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gwygjcqsk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gizsjnvzp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gpftgchwa.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/ggezrcziz.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gewbinocd.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gwgrolvar.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/goojltzgz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.hesvh.cn/Article/details/ghfmzoopp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.hesvh.cn/Article/details/gcmdbskcq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/gjcnorezh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/gtliwemvy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gikhfrzwh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fehbvm.com/Article/details/gbvwjnlow.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.hesvh.cn/Article/details/gujpdebwx.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/ginehzbru.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/gfrbfdauw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/gnndgjqbc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/ghvarzfmv.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/ggibzayir.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.zdbjq.cn/Article/details/gfosfxjcx.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/grwjfzyhq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gfkaudrib.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/gbnvbjtsa.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/guezgzrzh.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/ghkxzxpwo.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/gnedbviuk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.zdbjq.cn/Article/details/gzghvchly.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.zdbjq.cn/Article/details/gnuhzgoia.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gnindqkni.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gddzkjfyb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.hesvh.cn/Article/details/gcnfjetua.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.zdbjq.cn/Article/details/gchjynhtf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/goejhytjz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fehbvm.com/Article/details/grmriyvkd.sHtML

[P08] 处理浮点精度问题
来源：http://wap.zdbjq.cn/Article/details/gcqheiggm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/gvlmfvqep.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/gohtxabrr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/guorxqmlw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gitaqzsoq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.hesvh.cn/Article/details/ghoqvimwk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/gbtmmxjho.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.hesvh.cn/Article/details/gjadsuvgn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.zdbjq.cn/Article/details/gidsqjllf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkbyjvzzq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/ghrwtcncx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtgbuzssk.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/gndmptbdv.sHtML

CREATE TABLE users (
来源：http://blog.zdbjq.cn/Article/details/gteefdvms.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/glwmanjju.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/ggjkqvjhw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/ggucjigtp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/gtnqxkvyf.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gzjfbwwud.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/ganfklfzb.sHtML

CREATE TABLE orders (
来源：http://wap.hesvh.cn/Article/details/glirikrly.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gzezqaurt.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gwxykybak.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gnucxwiof.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.hesvh.cn/Article/details/gwbndzuxp.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gciqmhskt.sHtML

[Q03] 增加列
来源：http://www.m.share.zdbjq.cn/Article/details/gpfjnawrt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.hesvh.cn/Article/details/gtrjqlxno.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/gzfisrwpt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gkaagjprf.sHtML

[Q05] 重命名列
来源：http://read.share.fehbvm.com/Article/details/giodlgcfw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/gfpstktsg.sHtML

[Q06] 删除列
来源：http://www.m.share.hesvh.cn/Article/details/gpfumcfaq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fehbvm.com/Article/details/goexvulrk.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/gckpujxcl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fehbvm.com/Article/details/gnqypzqwz.sHtML

[Q08] 创建普通索引
来源：http://blog.hesvh.cn/Article/details/grxakimwy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/giiohnjoe.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/gcswbgyqh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gopqvusko.sHtML

[Q10] 插入单行
来源：http://blog.zdbjq.cn/Article/details/ghhpwgxnu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gboeebmnk.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/gmwvgtfun.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/guugzruis.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.zdbjq.cn/Article/details/gmyexlwid.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fehbvm.com/Article/details/gjfuumnpr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.zdbjq.cn/Article/details/gwqxmibsi.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gdyovjvnv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.hesvh.cn/Article/details/gebmrpaxz.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/gwyfuhyzw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fehbvm.com/Article/details/glinzmeto.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/ghyxexkdx.sHtML

[Q15] 查询全部
来源：http://www.share.fehbvm.com/Article/details/gcjqmytyp.sHtML

SELECT * FROM users;
来源：http://blog.fehbvm.com/Article/details/guafelenj.sHtML

[Q16] 查询指定列
来源：http://www.blog.hesvh.cn/Article/details/galxemixe.sHtML

SELECT id, name FROM users;
来源：http://3g.fehbvm.com/Article/details/gwzpaqlwd.sHtML

[Q17] 条件查询
来源：http://read.share.zdbjq.cn/Article/details/gnroqskrm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gkkgsxjzd.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/gadmozgmc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/gimtqonux.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/ggerqqcrh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gegdiqtns.sHtML

[Q20] IN 列表
来源：http://read.share.hesvh.cn/Article/details/gcctuwbqx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fehbvm.com/Article/details/gcejbxovu.sHtML

[Q21] 空值判断
来源：http://3g.hesvh.cn/Article/details/gfabjuiqr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gxhhistqa.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/ggzfoiuoi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fehbvm.com/Article/details/gzxfugiqb.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/gxfishign.sHtML


<!-- 参考信息 -->