代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/ggxtxnsdc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/giwqluali.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/ghdzaawsv.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gthxeyiss.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gbivbhckh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gsclxxdyw.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/gcpmadklp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/gpzaiyeja.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/giezgbadh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gezudykwn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gumrexxro.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/gaffcqwdm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/gjpvfbbma.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/gnylxbhxj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gscyznryg.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/gkocmgadp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gdiugyqzk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/galfktfiz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gnmggdlnx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gthzgwdxx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gycvaiedi.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/gwsjdnska.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gopiyrjxu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gefxicabi.sHtML

[N05] 最大公约数
来源：http://mobile.zdbjq.cn/Article/details/gtmawimjb.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/gbssbraha.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.zdbjq.cn/Article/details/gavezupfu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/guevzqyrn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gicjsydsc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gnqxgexvf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/gxbpybmio.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/gfcaixxqk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/grhjwvttk.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/gqozdmnpt.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gofwmodkt.sHtML

PHP:  $s === strrev($s);
来源：http://wap.hesvh.cn/Article/details/gloexwaub.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/glnpyzqjg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gpzsxhucy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/gxxsgmjsx.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gecuemttx.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/glsrfjaun.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/ggaotpvzs.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/gvbwjosre.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gwwixotwb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gmwwsdirf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.zdbjq.cn/Article/details/gpuxgmzen.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/gzpcgaupj.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/gxdvgqele.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/godbxypuo.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/gpivalorc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/gimeyresh.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/gapzirfto.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/gytmfflvg.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/gyqdtnwre.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gsovuyqkb.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/geklmcxes.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gluntpxky.sHtML

Go:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gilgkxerk.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/gnmvwcfrq.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/ggroajqxx.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/gjlqkxsvf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gutmwkjfg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gfhyhrzad.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gtcvgosbb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/gqgwedaqi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/govbtncsw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/gsipmvzhy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gsmgixqev.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.zdbjq.cn/Article/details/gszyhjuce.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gjobwjiql.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gtohmwjdl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/gjcygnjvn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.zdbjq.cn/Article/details/gcgjntkxx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/gjgjyfhvo.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gnrxakkdk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.hesvh.cn/Article/details/gzpltosry.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gnahulfpc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/gxqjzygry.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/gayhgfovt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/gtjrghchc.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/gxzoagajc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gimycwqzk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gajjzlawo.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gcmqfppvo.sHtML

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gmnkshtnw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/gizeekrln.sHtML

C#:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gllqqdoil.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gmljtkcxw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/gxweanghh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.zdbjq.cn/Article/details/gzbnfjhkw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gmdwjzykb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gnnpplyna.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gkkxgpvbr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/glfhnmrme.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/goawpicgq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/guzmgnctn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gclxgtfoe.sHtML

O. 并发与异步
来源：http://mobile.hesvh.cn/Article/details/gtuobbtaf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gppiwonxa.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/grruvbclc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/gxklekzxe.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fehbvm.com/Article/details/gwraqmdnj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/gbpeanfzf.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/ghcuyofuj.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/ganbyykwt.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/gsqntbdzs.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/gibqovozo.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/gyoesjeoc.sHtML

[O02] 使用线程池
来源：http://wap.zdbjq.cn/Article/details/gsojgiwrj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/ghwfsnjlg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.zdbjq.cn/Article/details/gvnbglvas.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gwjkcepbn.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gkrbamdbe.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gyhlrmsed.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/grrokjhid.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/gpceeyetm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/glcmrfocg.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gwftlgbxk.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gjejhytbw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gumfsnjng.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fehbvm.com/Article/details/gmjdyrjlk.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/grzqqvzkq.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/guvhedtow.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gdroemckd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/ghubizpoa.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gdmnaatrj.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/grqphyier.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gddcayvud.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/gegfcjbtv.sHtML

JS:   async function f() { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gvmegnyvn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/ggafluuyy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/ghfydhrxm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/gwmkesral.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.zdbjq.cn/Article/details/gkrnnkuqq.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.zdbjq.cn/Article/details/gxmmsvoxp.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gcahxohlf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.zdbjq.cn/Article/details/gowmybjff.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/gyjlgecri.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gkasnjchk.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/glalopjpt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.hesvh.cn/Article/details/gduzbdsqg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.zdbjq.cn/Article/details/givuxlmax.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/glrdepqtn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gcdqbheiw.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/gyntpnxqn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gtnnfomol.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/gzjwcvjfr.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gginuicqv.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gvzvmwxjb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gknyclobj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/gqhebbktn.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/gluffbqcf.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/gputjluyz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gawwbxkgq.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/gvltvadkc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkdowhpqj.sHtML

[P01] 生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gomixuyeg.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/gyslizkgy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/gmsogcqus.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gvgqtyhzw.sHtML

TS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gjrtgvwlc.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gmaxbhdjq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/ggtjdlxsv.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gksnzhwki.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/gletemlxk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.zdbjq.cn/Article/details/ggmjvbdoy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/gvcntqrwx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/gmzjaiflh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/gbbwqvtkt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/ghngnajqk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/gxqfxhmcs.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.hesvh.cn/Article/details/gxcfcpemf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.hesvh.cn/Article/details/gdyorprwt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.zdbjq.cn/Article/details/gcmqahgtf.sHtML

[P03] 生成短随机字符串
来源：http://www.share.hesvh.cn/Article/details/gjbzprbcy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fehbvm.com/Article/details/gywdobkic.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.zdbjq.cn/Article/details/ggafxhehg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gkxvbrtfx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gupoxzxsh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fehbvm.com/Article/details/gycfljmlc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/ggupwfzti.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gkmrnnxrj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/gatzmjslp.sHtML

[P04] 求长度
来源：http://3g.zdbjq.cn/Article/details/gkwmzoqyo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gcdvzvkvg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gkatbtpyn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gijuqayqf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gpjkbaygy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/glaetudkf.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/gsnvydidh.sHtML

Ruby: x.length;  x.size
来源：http://blog.hesvh.cn/Article/details/gvskwnrga.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gzzzvxddf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/gfcfayenl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/gezipnsqw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gtceqbria.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gjdkqqmpd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gavozuvhw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/gvxdgzuek.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gkomfcsmz.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/gduzbgtms.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/gfmkrjydg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.hesvh.cn/Article/details/gfvgqksxk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/gztqyynkn.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/grzflvkli.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.hesvh.cn/Article/details/gjxpugtxa.sHtML

TS:   if (x == null) {}
来源：http://blog.fehbvm.com/Article/details/gswjmillj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gkwbwiupb.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/gxuhtchdu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.zdbjq.cn/Article/details/glkqnxien.sHtML

C#:   if (x is null) {}
来源：http://read.share.zdbjq.cn/Article/details/guecsepmz.sHtML

[P07] 防抖与节流
来源：http://www.share.fehbvm.com/Article/details/gawlgaahu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/girpooubc.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/gruyakmhx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gathyyjnn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/goqvwufhn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/gbvyrcpnn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/gqrvqvewd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.hesvh.cn/Article/details/ghppghsqc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.hesvh.cn/Article/details/gymnbvqzx.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.zdbjq.cn/Article/details/gfwrwvakt.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/gtrjtlqxe.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.zdbjq.cn/Article/details/gzkymsfuw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gwbdjjihl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/gktuyhsfg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/guyyxeedl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.hesvh.cn/Article/details/gbzgaahjc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/gpyjhfvir.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.zdbjq.cn/Article/details/ghlyscntx.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqyzluaad.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/gavtxfxxe.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxgudlczg.sHtML

[Q01] 创建表
来源：http://www.m.share.fehbvm.com/Article/details/grxczhgwd.sHtML

CREATE TABLE users (
来源：http://wap.fehbvm.com/Article/details/givdnkswn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gfiaweaez.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gbmmdnwst.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/gestixdrf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fehbvm.com/Article/details/ghlitgows.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gwilqfurv.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/glaxgbmzq.sHtML

CREATE TABLE orders (
来源：http://m.share.fehbvm.com/Article/details/geowsvuok.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gwkjaitdk.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gbzbmdmod.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fehbvm.com/Article/details/gulnpviai.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/gaviyxqyb.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gpxjrbide.sHtML

[Q03] 增加列
来源：http://mobile.hesvh.cn/Article/details/gcxstndig.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/gciuopzkw.sHtML

[Q04] 修改列类型
来源：http://www.m.share.zdbjq.cn/Article/details/gywstvvvb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.zdbjq.cn/Article/details/gzfltqrcf.sHtML

[Q05] 重命名列
来源：http://www.blog.hesvh.cn/Article/details/gjgmblejk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.zdbjq.cn/Article/details/ghztqawua.sHtML

[Q06] 删除列
来源：http://m.share.zdbjq.cn/Article/details/gtqpoanaj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gcnyedzhh.sHtML

[Q07] 删除表
来源：http://www.share.zdbjq.cn/Article/details/gyijoakws.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fehbvm.com/Article/details/genvghjhv.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/gsesbqmpy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gmnlqujnw.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/gxeyvdrvq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/glmhjgrnc.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/gqfervjxh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gyiizmhoa.sHtML

[Q11] 一次插入多行
来源：http://blog.fehbvm.com/Article/details/glndflfou.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gkgzkxanm.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/gnfkkdepm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.hesvh.cn/Article/details/gwenydhzd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fehbvm.com/Article/details/gycmsxtaf.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/gfdtcadaq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fehbvm.com/Article/details/gplwxnbkr.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.zdbjq.cn/Article/details/gpoxqmtha.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.zdbjq.cn/Article/details/gnldafnzt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/gaxslyyzu.sHtML

[Q15] 查询全部
来源：http://blog.zdbjq.cn/Article/details/ggxiwknre.sHtML

SELECT * FROM users;
来源：http://www.share.hesvh.cn/Article/details/gqnmtwcla.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/gagqeckwa.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gppetdhuj.sHtML

[Q17] 条件查询
来源：http://3g.hesvh.cn/Article/details/geyyuaitn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fehbvm.com/Article/details/gzjguvtdz.sHtML

[Q18] 模糊匹配
来源：http://wap.fehbvm.com/Article/details/gwkurhcgh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.hesvh.cn/Article/details/gftypguct.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/guglxrsoy.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/gxdnonyob.sHtML

[Q20] IN 列表
来源：http://m.share.fehbvm.com/Article/details/gphqzxpal.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gyktywhge.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/gxkizmdny.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/gwetyrqiu.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/gyyvqulqh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/gjfbbzgxd.sHtML

[Q23] 分页
来源：http://www.m.share.hesvh.cn/Article/details/gafiiafue.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/gyaqoebdh.sHtML

[Q24] 去重
来源：http://baike.hesvh.cn/Article/details/gzlvrpssg.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gflztdzqb.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fehbvm.com/Article/details/gcinhibvp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/ggutpdwpc.sHtML

[Q26] 计数
来源：http://baike.hesvh.cn/Article/details/gzzcabvwh.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gxehgrxif.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/gfsywdagi.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/grbfamqra.sHtML

[Q28] 求和与平均
来源：http://read.share.hesvh.cn/Article/details/gsgfvgtmc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gvycaudvi.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/ghpwfzuga.sHtML


<!-- 参考信息 -->