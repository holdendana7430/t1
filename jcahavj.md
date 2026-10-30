代发 wailian999

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gorvvjarb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.zdbjq.cn/Article/details/gfovlmbca.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/gjsjlcpap.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/gyfdspnbc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/goalmncke.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gjngivvzt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gxbhddodp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/ggconnzau.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/ggdudjjsu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/gjtflptul.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/gqmmvtwud.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/ghxyngkuz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/glglwsccw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/gztxeruxp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gaupipnsu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gxvpzafua.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/gvrnbxqnf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/gfxoxaapf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gazisabar.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gzlseoqac.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gxiatmjvz.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gjhjajahl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/gxxshpewr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gflfzadma.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gzilccqei.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fehbvm.com/Article/details/gfmmbjiqo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gkvjmutbv.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/gyvvxqvfn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gaxtrzlng.sHtML

[N06] 判断回文字符串
来源：http://blog.fehbvm.com/Article/details/ggzotfrlm.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gzigigbde.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/gmysugtvu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gbevqjjad.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gjlwojjhp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/geykqdxgu.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/ghrhsrxgm.sHtML

Ruby: s == s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gvdphccbn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gkziayhsc.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.hesvh.cn/Article/details/glolkkezb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/ghqidxxtc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gvgfynvlu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/gqltlzbpk.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/gikymokmu.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/gnvhihunb.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/grppmklcd.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/gdxatuxvo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gsigyqsam.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/ggyykpqib.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/grugltxey.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/gvkpyasmi.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/ggewokikt.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/grymnxehw.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gowjzixcl.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gmxdngcul.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/gqdbcqiuj.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/glwnzdstg.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gynjhkltr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/gdijfrzry.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/gjokhtyle.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gwwuadeep.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/gesqyjech.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gvoixodnr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/gcnqvkntg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gffxqiprm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.zdbjq.cn/Article/details/gwwxurzsh.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gtfxyvrxm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/gemuvwlwx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/grlwtgjjq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/gafqouywx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/ggmxhxjji.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.hesvh.cn/Article/details/glliopylm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/gcbdnitzx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/gjsyhqaid.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.hesvh.cn/Article/details/gozilazde.sHtML

[N11] 二叉树中序遍历
来源：http://wap.hesvh.cn/Article/details/guucuocey.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/ghzyjelrg.sHtML

PHP:  // 手写递归函数
来源：http://3g.hesvh.cn/Article/details/grpnyjdio.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gmdelluku.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gabcpkuyx.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/ghryzyyeq.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/guxkersxy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/glgnmqjrm.sHtML

C#:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gjexgyvmj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gjptghbrp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/guzzccqru.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gevtuorot.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gtnpvmrrf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gdvdcjaxc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/guhglrtki.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/ghtaqcwjv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gdoxbznuj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gmkowifyw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzxvvthmi.sHtML

O. 并发与异步
来源：http://www.share.hesvh.cn/Article/details/gjmxuhpwp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gasawpbwo.sHtML

[O01] 启动一个线程
来源：http://www.blog.zdbjq.cn/Article/details/gcwllwfwe.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/glutmyzyj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gpltjvkws.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/gaixlmikx.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gbfdvqrrj.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gnrubifve.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/guyfyxhsn.sHtML

Ruby: Thread.new { f }
来源：http://blog.fehbvm.com/Article/details/gdrsckywe.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/geosbltff.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gwrqrikfj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/gyvobgfsb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gzlesvbbs.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gmrylnohg.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gcotfjrsg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/gzclaufzp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fehbvm.com/Article/details/gbvjdcaii.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/gtcepkmyc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/gvyjsjsyy.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/ggybfwutr.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gvukilwok.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/grafhvdpq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/glqtdeysd.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gcawaksgs.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gatibueyh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.zdbjq.cn/Article/details/gnxbnwvnr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/gomeeeqai.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gdncnrzcr.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/gvmsqqffd.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gbxcgppgd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.zdbjq.cn/Article/details/gohlccwkn.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/ggefybicj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/grqofeydi.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/gwsppxslq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/gmxjbbyql.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/gxndxeniv.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/gepyfacvl.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/gftyenwfr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gozgeecif.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/gboisglcj.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gfujitalr.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gsgwzgepq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.hesvh.cn/Article/details/gzggvzinf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/glgmslrca.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fehbvm.com/Article/details/gmnirbpdz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gyqevmcqa.sHtML

[O06] 使用进程池
来源：http://wap.hesvh.cn/Article/details/gxdjykwad.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/gnzumibjh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/guzieukkn.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gozpdlqbb.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gpwfaewrn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/gtvmzvnua.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fehbvm.com/Article/details/gsszekexf.sHtML

Ruby: // fork 块
来源：http://m.share.fehbvm.com/Article/details/glmcexdqn.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/gjtruxhse.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpgmrjbyn.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/ggbytttla.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzoelkwlm.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/gkrhzbzvj.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/glxfgntdz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gkmbmkzva.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/ggdqytxkj.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/guptzsdbb.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/glsbjjwyu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.zdbjq.cn/Article/details/gljekuniv.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.zdbjq.cn/Article/details/gthtbmjoo.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gsswmuwsl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/gwlyjdwob.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/gvgcmeoxy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/gskbcjuyb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/gawbqninw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/gnzhgitmm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/ghatyltay.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.hesvh.cn/Article/details/gkivtmxhj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.zdbjq.cn/Article/details/gznstrryz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fehbvm.com/Article/details/gvlfchxan.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fehbvm.com/Article/details/glerenpnm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gvwcuxfsg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/gyrlazqoe.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gtzpdlgnk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gximoucos.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.hesvh.cn/Article/details/gjftbkpym.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gfovlqpyy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.hesvh.cn/Article/details/gpqeiqxnc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fehbvm.com/Article/details/gumvamkxz.sHtML

[P04] 求长度
来源：http://read.share.hesvh.cn/Article/details/gldksowxu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/guodmbylk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/ggqmhjork.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/ghtlufqxn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gcvzwbtvs.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/gtzcqhvyt.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.hesvh.cn/Article/details/gqwmjjvuw.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/glxbqxfyc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/gswluoweh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/gwhgltaud.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.hesvh.cn/Article/details/gtktejctx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.hesvh.cn/Article/details/gikeerulo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/gfoesrmap.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gvmmlwavv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/gjkcxbpfb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gijirhnbz.sHtML

Ruby: a == b
来源：http://www.share.fehbvm.com/Article/details/ggrxzwspu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fehbvm.com/Article/details/gagnvvxmg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fehbvm.com/Article/details/gopnzenba.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.hesvh.cn/Article/details/glnjjtnwg.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/ggqmrddak.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/gdvcrqgki.sHtML

TS:   if (x == null) {}
来源：http://blog.hesvh.cn/Article/details/gnywtvfor.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gznejpnna.sHtML

Go:   if x == nil {}
来源：http://read.share.fehbvm.com/Article/details/gitcjovoc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fehbvm.com/Article/details/gtfpcxabp.sHtML

C#:   if (x is null) {}
来源：http://read.share.hesvh.cn/Article/details/gdvfmbkmi.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/gueafmyvq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/gaqdsraat.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fehbvm.com/Article/details/gwfcienxj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/glltzprrz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gsgyjopud.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gtbsmdfhb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fehbvm.com/Article/details/gnlchnvgq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fehbvm.com/Article/details/gwwganfgv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fehbvm.com/Article/details/gdfsdjxtg.sHtML

[P08] 处理浮点精度问题
来源：http://blog.hesvh.cn/Article/details/ggyndposz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gyhjbmkyj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fehbvm.com/Article/details/geverkify.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/gpfznickm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gkropbrpx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.zdbjq.cn/Article/details/gawaglwes.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/gxseytkjv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.zdbjq.cn/Article/details/gqiyzvbgt.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.hesvh.cn/Article/details/gkyheoyhz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnuftggno.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/guacddpdg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggfvylwod.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/gzfmsaudl.sHtML

CREATE TABLE users (
来源：http://blog.zdbjq.cn/Article/details/gfqgtposh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gwjuvtaep.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gjjqnciyj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.hesvh.cn/Article/details/glsvwtocd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/gqcsrvcyg.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gqoloarsp.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/gnuscxetn.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/gpmphpeqb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gpmpwizcg.sHtML

user_id INT NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/ghkbyakli.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fehbvm.com/Article/details/gbhzubfln.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fehbvm.com/Article/details/goyomffap.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gqkjcstjy.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gjkqrztdu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/glhijbohw.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/gmacasonw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.zdbjq.cn/Article/details/gbrfnboig.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/gmmcgfjio.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/glpfzeqqo.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/gxrcehfzk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/gylrdfxeb.sHtML

[Q07] 删除表
来源：http://www.blog.hesvh.cn/Article/details/geenfjagz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/gwqxrolto.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/gcubhzobp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gofwrneoe.sHtML

[Q09] 创建唯一索引
来源：http://mobile.zdbjq.cn/Article/details/gapencshg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gwszhifez.sHtML

[Q10] 插入单行
来源：http://m.share.fehbvm.com/Article/details/gytofwqsf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gdlbljeop.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/ghuqplmun.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fehbvm.com/Article/details/gyukrxsta.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.hesvh.cn/Article/details/gvhkduoua.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fehbvm.com/Article/details/gswfassnu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/gmidxbnzv.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fehbvm.com/Article/details/gxemyfokt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/gjvfcwcbh.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/gshgskicl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/glgkyxkws.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/gwiqkxitj.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gblklmepa.sHtML

SELECT * FROM users;
来源：http://baike.fehbvm.com/Article/details/gsytysaze.sHtML

[Q16] 查询指定列
来源：http://baike.fehbvm.com/Article/details/gpjcgrlta.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gvbnpzyou.sHtML

[Q17] 条件查询
来源：http://3g.fehbvm.com/Article/details/gycbflmkb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gwnrkievm.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/gnuqtlhuq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fehbvm.com/Article/details/gkjneqjvp.sHtML

[Q19] 范围查询
来源：http://baike.zdbjq.cn/Article/details/gfxweiwfj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.zdbjq.cn/Article/details/gpgatvpfi.sHtML

[Q20] IN 列表
来源：http://3g.hesvh.cn/Article/details/gobmuhbco.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.zdbjq.cn/Article/details/gwnxvbvbw.sHtML

[Q21] 空值判断
来源：http://www.blog.zdbjq.cn/Article/details/gumafmmag.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/gfzjlkmhc.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/gprrjwrst.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.hesvh.cn/Article/details/gxheswgfh.sHtML

[Q23] 分页
来源：http://www.m.share.hesvh.cn/Article/details/gwwrjvmhu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fehbvm.com/Article/details/gzbajzxca.sHtML

[Q24] 去重
来源：http://baike.fehbvm.com/Article/details/ghtpinjox.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/gplgglqhr.sHtML

[Q25] 只取前 N 条
来源：http://read.share.hesvh.cn/Article/details/gitfqesev.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gqozxrsck.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gkndovudp.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gtejsbbdl.sHtML

[Q27] 条件计数
来源：http://www.m.share.hesvh.cn/Article/details/gjcrttdym.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/glgwqwzka.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/gizujjzck.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gvocanevf.sHtML

[Q29] 最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gdrqoxgrj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/grieaopxp.sHtML

[Q30] 分组统计
来源：http://3g.zdbjq.cn/Article/details/gouhybhuq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gpvtztkpf.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/gvwxriefo.sHtML


<!-- 参考信息 -->