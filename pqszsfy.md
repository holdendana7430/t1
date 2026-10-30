代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmdrxqpa.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geomrzzil.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhwpqsci.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjoziqxcn.sHtML

Ruby: arr.sort
来源：http://wap.fanxiaobao.xyz/Article/details/gkelkkegq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fanxiaobao.xyz/Article/details/gysucjpie.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchaxljxe.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fanxiaobao.xyz/Article/details/gnhbbvvum.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fanxiaobao.xyz/Article/details/gawxcldqm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlzxeiym.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntubkrrb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxkuzbva.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fanxiaobao.xyz/Article/details/gpkpvanbn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fanxiaobao.xyz/Article/details/gplfkaofz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fanxiaobao.xyz/Article/details/grcaxjpqq.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelobupbv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gdrynhylw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqiomqmea.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/grxqxybqa.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fanxiaobao.xyz/Article/details/ghkokoizj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gilydmcfz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdutwrcr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gnbkhpfbi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtoyasgw.sHtML

[N05] 最大公约数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqqluhkz.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxdogdqh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwbxwzan.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfshpbxo.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamxejefw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gazmzpabh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gslspvewm.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvokjbvi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fanxiaobao.xyz/Article/details/gboiyiosb.sHtML

[N06] 判断回文字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gfoxkoagh.sHtML

Py:   s == s[::-1]
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnztwepj.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fanxiaobao.xyz/Article/details/gybfkwudc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fanxiaobao.xyz/Article/details/ghigzbwbt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbejroqir.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fanxiaobao.xyz/Article/details/gwfjetenq.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gjetdxwdf.sHtML

Ruby: s == s.reverse
来源：http://baike.fanxiaobao.xyz/Article/details/geoxfrywq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fanxiaobao.xyz/Article/details/gcvcuboii.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fanxiaobao.xyz/Article/details/gsrqbifqy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwdcluyn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fanxiaobao.xyz/Article/details/gduhmuvqu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwunyocsr.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fanxiaobao.xyz/Article/details/gonoyshmp.sHtML

Java: // 手写 HashMap
来源：http://blog.fanxiaobao.xyz/Article/details/geumphuaa.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqkkgunz.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqducogz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fanxiaobao.xyz/Article/details/gvbrbcfuz.sHtML

[N08] 生成全排列
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwzsrdqy.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckawshmt.sHtML

PHP:  // 手写递归交换
来源：http://wap.fanxiaobao.xyz/Article/details/govlytenp.sHtML

JS:   // 手写回溯递归
来源：http://blog.fanxiaobao.xyz/Article/details/ghatilnal.sHtML

TS:   // 手写回溯递归
来源：http://baike.fanxiaobao.xyz/Article/details/gqjfyzycr.sHtML

Java: // 手写回溯递归
来源：http://3g.fanxiaobao.xyz/Article/details/gptyltzom.sHtML

Go:   // 手写回溯递归
来源：http://3g.fanxiaobao.xyz/Article/details/giyvbobib.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtdaxnzz.sHtML

C#:   // 手写回溯递归
来源：http://3g.fanxiaobao.xyz/Article/details/geztyphnw.sHtML

[N09] 栈与队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvojzbutv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fanxiaobao.xyz/Article/details/gvswvfnxp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmmatcyo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fanxiaobao.xyz/Article/details/gjsabvmfg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fanxiaobao.xyz/Article/details/gkyqvmpal.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxuytraj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fanxiaobao.xyz/Article/details/gligsfbnp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fanxiaobao.xyz/Article/details/goenlmpkk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fanxiaobao.xyz/Article/details/gukdbnyic.sHtML

[N10] 链表节点定义
来源：http://baike.fanxiaobao.xyz/Article/details/gryuxhtsp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fanxiaobao.xyz/Article/details/gzziflzqa.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbcsxtyqb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fanxiaobao.xyz/Article/details/ggvwypxgv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfylhepi.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzpfaglaf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fanxiaobao.xyz/Article/details/gupibgzay.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fanxiaobao.xyz/Article/details/gclytmbes.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwoehivj.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fanxiaobao.xyz/Article/details/ggocdoacv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fanxiaobao.xyz/Article/details/gaetsmtim.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gmemcbsog.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fanxiaobao.xyz/Article/details/gijsihnou.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fanxiaobao.xyz/Article/details/gkbcbvhmf.sHtML

Java: // 手写递归
来源：http://blog.fanxiaobao.xyz/Article/details/gzvhwjciz.sHtML

Go:   // 手写递归
来源：http://wap.fanxiaobao.xyz/Article/details/glkukwvpa.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fanxiaobao.xyz/Article/details/gikyiotmg.sHtML

C#:   // 手写递归
来源：http://3g.fanxiaobao.xyz/Article/details/gtmlcohza.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fanxiaobao.xyz/Article/details/gdnkdlylu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fanxiaobao.xyz/Article/details/gbdqgfbjh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fanxiaobao.xyz/Article/details/gsxchoeot.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqffsayxk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fanxiaobao.xyz/Article/details/gatbxlmqa.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwanupha.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fanxiaobao.xyz/Article/details/govskklex.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gbomqhzbh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhggmgep.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gjeaqxyiu.sHtML

O. 并发与异步
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjocvpnc.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzryxaqy.sHtML

[O01] 启动一个线程
来源：http://3g.fanxiaobao.xyz/Article/details/gjnbzsopm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fanxiaobao.xyz/Article/details/gsyebajkm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gnosnjldf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbhbckhg.sHtML

TS:   // 同 JS
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmrlysqj.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fanxiaobao.xyz/Article/details/gacgxbvct.sHtML

Go:   go f()
来源：http://3g.fanxiaobao.xyz/Article/details/gmxequqfc.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fanxiaobao.xyz/Article/details/gabjlkrvz.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfysvfxw.sHtML

[O02] 使用线程池
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydzqqpst.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fanxiaobao.xyz/Article/details/gcyvjwyoc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fanxiaobao.xyz/Article/details/gbpkprryh.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fanxiaobao.xyz/Article/details/gausrnido.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnqvxfxx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtoizgstn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fanxiaobao.xyz/Article/details/gxpjnhfnl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fanxiaobao.xyz/Article/details/gpgmoatfl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fanxiaobao.xyz/Article/details/gfeyonsxa.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtapanpen.sHtML

Py:   with lock: shared += 1
来源：http://3g.fanxiaobao.xyz/Article/details/giclmoyfg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fanxiaobao.xyz/Article/details/goubiacfc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fanxiaobao.xyz/Article/details/gucjikbea.sHtML

TS:   // 同 JS
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocolexlk.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvgkklyp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fanxiaobao.xyz/Article/details/gmyblnfbo.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/geaefpqgu.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfddejhik.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gquetszlu.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gliyfsodj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fanxiaobao.xyz/Article/details/gvwxhwszu.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gperbttct.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsffwnon.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixjfkfml.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkgvumyp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fanxiaobao.xyz/Article/details/gchrpxptv.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gwpdizyfx.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjoxbrfz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwfwbymq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzbfxxpc.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlybvetj.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fanxiaobao.xyz/Article/details/gzupbtpcm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fanxiaobao.xyz/Article/details/gpftdfeat.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fanxiaobao.xyz/Article/details/gxjgiusie.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcepatygx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuluykdd.sHtML

[O06] 使用进程池
来源：http://blog.fanxiaobao.xyz/Article/details/gyrejkepd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzswvftrb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gspdmyaoj.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fanxiaobao.xyz/Article/details/gzyrducut.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzntshlw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fanxiaobao.xyz/Article/details/gnorzehcw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fanxiaobao.xyz/Article/details/guajlbunj.sHtML

Ruby: // fork 块
来源：http://read.share.fanxiaobao.xyz/Article/details/geluliofe.sHtML

C#:   Parallel.For
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebadhtzp.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/guoccqozw.sHtML

P. 常用工具函数
来源：http://3g.fanxiaobao.xyz/Article/details/gvqumiuwl.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqsibpet.sHtML

[P01] 生成 UUID
来源：http://3g.fanxiaobao.xyz/Article/details/ghvtpbqik.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fanxiaobao.xyz/Article/details/gcntelihi.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthurdczj.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/gwtphmjmu.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqrfdhkt.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvfyouir.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fanxiaobao.xyz/Article/details/gerfcyprx.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fanxiaobao.xyz/Article/details/gguhfaumb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fanxiaobao.xyz/Article/details/geqkpnceg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fanxiaobao.xyz/Article/details/giehfaxht.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fanxiaobao.xyz/Article/details/gcfossxlx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fanxiaobao.xyz/Article/details/glgbwqhue.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfbrhmqj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fanxiaobao.xyz/Article/details/gltalqetu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fanxiaobao.xyz/Article/details/gocfwqsyg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fanxiaobao.xyz/Article/details/gemhdxzwb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfhyzcsp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fanxiaobao.xyz/Article/details/gzprbcjdd.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhbwmyih.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrxitffc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fanxiaobao.xyz/Article/details/gclcoqjvr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwexsemvg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fanxiaobao.xyz/Article/details/gdnajhrzh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fanxiaobao.xyz/Article/details/grfbqrjmg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fanxiaobao.xyz/Article/details/gimctjcaz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqewhipv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyigadawt.sHtML

[P04] 求长度
来源：http://read.share.fanxiaobao.xyz/Article/details/givqiqwwp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnqszqud.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fanxiaobao.xyz/Article/details/gompvtndr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fanxiaobao.xyz/Article/details/gnesmcfey.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fanxiaobao.xyz/Article/details/guzhbhnkq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fanxiaobao.xyz/Article/details/giswduhjb.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fanxiaobao.xyz/Article/details/gsjqufoao.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdxxzrqg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fanxiaobao.xyz/Article/details/ggzkdvrqy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fanxiaobao.xyz/Article/details/ggmxrbhvj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gsylkelwl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqcmnfnj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fanxiaobao.xyz/Article/details/grexzxszq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhahmjsw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlnjsstv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gukmvlhxb.sHtML

Ruby: a == b
来源：http://www.share.fanxiaobao.xyz/Article/details/gxawpdtef.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fanxiaobao.xyz/Article/details/gkaqayvka.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fanxiaobao.xyz/Article/details/gcfromgdh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fanxiaobao.xyz/Article/details/gutmjnvwv.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fanxiaobao.xyz/Article/details/glbztjoop.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fanxiaobao.xyz/Article/details/gznkjyjxr.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopcvgyqu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfpkntzh.sHtML

Go:   if x == nil {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gtppaylpn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyhkqjfq.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrpgcfxl.sHtML

[P07] 防抖与节流
来源：http://www.share.fanxiaobao.xyz/Article/details/gcejwjuvh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fanxiaobao.xyz/Article/details/gzyuzxozj.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppqyeonc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlbjltau.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmgggokk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkwfguzs.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fanxiaobao.xyz/Article/details/gyookcevh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgcetuuo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fanxiaobao.xyz/Article/details/gewnsenlo.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fanxiaobao.xyz/Article/details/gvutspskl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fanxiaobao.xyz/Article/details/gflyqiehd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gxxjuhkij.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fanxiaobao.xyz/Article/details/grxzofbsy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fanxiaobao.xyz/Article/details/galgvlrms.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghhulmfa.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fanxiaobao.xyz/Article/details/gnraiadgp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fanxiaobao.xyz/Article/details/giofdegar.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fanxiaobao.xyz/Article/details/gmvbkghbd.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gqyrvjngf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhxbypzf.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gkuzhrwxf.sHtML

[Q01] 创建表
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwhektqh.sHtML

CREATE TABLE users (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgeanpvd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwidrswe.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fanxiaobao.xyz/Article/details/gjrncgzhr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpfljayn.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fanxiaobao.xyz/Article/details/getwsmqpl.sHtML

);
来源：http://blog.fanxiaobao.xyz/Article/details/gluznaqfj.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgzhlyag.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowxedzxt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fanxiaobao.xyz/Article/details/gflmidnrl.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlxvgyky.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fanxiaobao.xyz/Article/details/gmauueczu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnpgjgvo.sHtML

);
来源：http://wap.fanxiaobao.xyz/Article/details/gixtasykm.sHtML

[Q03] 增加列
来源：http://blog.fanxiaobao.xyz/Article/details/gnafdnszl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gnrxbyoem.sHtML

[Q04] 修改列类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gakghhjky.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fanxiaobao.xyz/Article/details/gimjlezbe.sHtML

[Q05] 重命名列
来源：http://read.share.fanxiaobao.xyz/Article/details/gemgfvxua.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fanxiaobao.xyz/Article/details/gwembhtpj.sHtML

[Q06] 删除列
来源：http://baike.fanxiaobao.xyz/Article/details/gydxmgbsj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzibaftp.sHtML

[Q07] 删除表
来源：http://3g.fanxiaobao.xyz/Article/details/guuivkhkd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvowmbtz.sHtML

[Q08] 创建普通索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gpeckdyps.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fanxiaobao.xyz/Article/details/gefxhavze.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgqstjrj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fanxiaobao.xyz/Article/details/gbitviqxy.sHtML

[Q10] 插入单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvakqqbzx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/ghmymwiok.sHtML

[Q11] 一次插入多行
来源：http://baike.fanxiaobao.xyz/Article/details/gbnsrqqrp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/gfzdojqsy.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fanxiaobao.xyz/Article/details/giaoekvog.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukicagdc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fanxiaobao.xyz/Article/details/grciffsrk.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fanxiaobao.xyz/Article/details/geisehywt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwholhmr.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fanxiaobao.xyz/Article/details/gbwqkqcwg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fanxiaobao.xyz/Article/details/ghruaxclq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmwkpizg.sHtML

[Q15] 查询全部
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjmmoeut.sHtML

SELECT * FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsrwhoeo.sHtML

[Q16] 查询指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlxdezeb.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcaqjkqdu.sHtML

[Q17] 条件查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytdtpnhs.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggliuzfyk.sHtML

[Q18] 模糊匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwmgdswl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fanxiaobao.xyz/Article/details/geimzostp.sHtML

[Q19] 范围查询
来源：http://3g.fanxiaobao.xyz/Article/details/grrucpnnt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuaupeko.sHtML

[Q20] IN 列表
来源：http://wap.fanxiaobao.xyz/Article/details/gqjwbhfhh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuutwdox.sHtML

[Q21] 空值判断
来源：http://3g.fanxiaobao.xyz/Article/details/glbixybzd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrronzhx.sHtML

[Q22] 排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnyboqrt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fanxiaobao.xyz/Article/details/grywjvtgf.sHtML

[Q23] 分页
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchsycxok.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fanxiaobao.xyz/Article/details/gbvrewtpz.sHtML

[Q24] 去重
来源：http://3g.fanxiaobao.xyz/Article/details/glfhybjfj.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ghqvjphie.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwoexqte.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fanxiaobao.xyz/Article/details/gkwcnitsq.sHtML

[Q26] 计数
来源：http://m.share.fanxiaobao.xyz/Article/details/gefsfxeun.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gbxolnzqa.sHtML

[Q27] 条件计数
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuhczmui.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gorphyqsf.sHtML

[Q28] 求和与平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gdibokoon.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gfzipgosm.sHtML

[Q29] 最大最小值
来源：http://read.share.fanxiaobao.xyz/Article/details/gcukusupb.sHtML


<!-- 参考信息 -->