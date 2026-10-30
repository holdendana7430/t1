代发 wailian999

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/ghqpvwzxe.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.hesvh.cn/Article/details/gtcsloait.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/gpbblwvgj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gzigjcpgr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.hesvh.cn/Article/details/grmcywjjz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gcqwoierr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/ggqbsedbq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/goaysdjni.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gwpgoryhj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/gukrcetnn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/gtreqnhoj.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/gacegclzq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gtgtucopb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gbacgpyrq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/ggvcefkkv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gwbjvbgee.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/gqwansyyz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/gawrbaaxm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gcsvilmyp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gdpxncljn.sHtML

[N05] 最大公约数
来源：http://www.m.share.hesvh.cn/Article/details/gwoalvsky.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gajaesxra.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gykxzvshk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/grzrvwaxr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/guxglaspi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/gthwjqdxt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/gmzrepluz.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gwahfmxfz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/grulkevdf.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/gsdvkqdex.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gcmlclcjy.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gzabiizty.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gmkzjhcvq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gxcpjuxvy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/gyuqfykaj.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.hesvh.cn/Article/details/grttikcyf.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/gasrlqfqp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gyqixndtt.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/ggtqrgeus.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/gyjaxybxe.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/gepcsnixb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/gttnokwdo.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/gvbdmwmro.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/grywfmiqi.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/gwefcdakh.sHtML

Ruby: // 手写 Hash
来源：http://blog.hesvh.cn/Article/details/gsfzexjpg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fehbvm.com/Article/details/gkeyicfrw.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gdmhiadqi.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/gqdkontpp.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/gzjhyubax.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gefpkiqdz.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gfddmpkdh.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gjueoivhc.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gaexexfef.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.zdbjq.cn/Article/details/gxqcmnyxt.sHtML

C#:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gqmnjntki.sHtML

[N09] 栈与队列
来源：http://wap.hesvh.cn/Article/details/gzcpcnsgq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/gyvmxorkr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gpvavtijv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gaxzhecoh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/gjqoqdksh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/goqhkanyg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gszgzubej.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/ghptcizra.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gkxxcmxtd.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/gsyrkiquq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/goxglbyuy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/gedkqintd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/ggnrpvftc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/grgzpnpus.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fehbvm.com/Article/details/ggdcphvob.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.hesvh.cn/Article/details/glqesxsih.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/grnrdqxby.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.zdbjq.cn/Article/details/gizhmnwqo.sHtML

[N11] 二叉树中序遍历
来源：http://wap.hesvh.cn/Article/details/ggmcqwwsn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/gfwmszzaa.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/grsmilkfn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/glpofcsgd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gbjkfbdgh.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gojsaanmn.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gthqudqsk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/gxhitqhie.sHtML

C#:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gctahvjuc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gggtrzzzq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.hesvh.cn/Article/details/gywawhvhb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/gmgvcpnnz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gfsqugwen.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gwpukmhtd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gsyfoflan.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/gnmbvazxc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fehbvm.com/Article/details/gxhhygtql.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/guzwtrtoz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gncsbgnzl.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/gaooosliz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtzzyjnil.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/gutokzucv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.zdbjq.cn/Article/details/ggvggrwfr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.hesvh.cn/Article/details/gnynmnsqq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/ggbbbojrr.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gcydbbcbh.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/gkcyfhlud.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/gfnrtexeb.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/gygwvqljx.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/guvqhwull.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/ggjovmxmo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/gnfxjxtmf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gbfeetqrj.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gaipleaqs.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gljksdknt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/gdwfdqewn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/gxefawvic.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/gocjyeblk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fehbvm.com/Article/details/gdvptjvhh.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/gocwuujjk.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/gprbaitqo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/gyjiizldc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.zdbjq.cn/Article/details/gchxvzwuc.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gygzvduyc.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gamuwxwoj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/gmaljyxue.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/giptxbxuk.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gtsmxlulb.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gmlahsixl.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/geqgpdnkh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fehbvm.com/Article/details/gbmpdozqm.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gebcmffez.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/gtvzmdebj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/gyhobrfju.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/gynkajhro.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.zdbjq.cn/Article/details/ggiawrbig.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/gfzhdaeuv.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/gldlorrov.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/guxbfobes.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.hesvh.cn/Article/details/gmldsmuxs.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gmhwekwdu.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gwjlcertd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/glrkzvfza.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/gycrxfibc.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/gvtqfteah.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/ggkijhech.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/grdsralut.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.zdbjq.cn/Article/details/guvwzrlpq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.zdbjq.cn/Article/details/gmjddanyb.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gcytebqjp.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gezyztrgb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/gopudrewh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.zdbjq.cn/Article/details/gaftawntm.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/gqihdqruq.sHtML

C#:   Parallel.For
来源：http://m.share.hesvh.cn/Article/details/geoioozac.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvcsbexte.sHtML

P. 常用工具函数
来源：http://www.share.hesvh.cn/Article/details/guddswalo.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbcvqepgn.sHtML

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gxdhyxwii.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.hesvh.cn/Article/details/gkrtckfht.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/gythfbbyo.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/guogirbux.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gqiolblqv.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gqnfugoqf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.zdbjq.cn/Article/details/gkevchonu.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/govwhiugu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.zdbjq.cn/Article/details/gshkrhbnc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/ggiqqyjje.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.zdbjq.cn/Article/details/ghmqylvnl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/gacbjagtn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gdvldfuiv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/gyjkoeffg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gzorwkhcm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gtmfjoscq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/guwrkowbl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/grqulukla.sHtML

[P03] 生成短随机字符串
来源：http://read.share.hesvh.cn/Article/details/gmlvodcjf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/gnqpaoqds.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fehbvm.com/Article/details/gkcsajogd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gzugjysex.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gogxaycch.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.zdbjq.cn/Article/details/gjlcdbyvk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/gwlqpxkzk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/gjglzvtrz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gxeryommv.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/gucuoffyz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gzcdpvaah.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gpcugdpoi.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gntbzifuz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/grbndorhm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/gggktpcgz.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.zdbjq.cn/Article/details/gotxhuzvm.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/gunfmlhyx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gybxoawzl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fehbvm.com/Article/details/gujbramjj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.hesvh.cn/Article/details/gjydtkcyg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/gwrlrvblu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fehbvm.com/Article/details/gqtwfdbzi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gpjniwqqi.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/gvyytyfqk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gnzphhwtr.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/gaktcjkft.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/glctfkdmj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/gjcnoahji.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fehbvm.com/Article/details/govariepi.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gerpgfjef.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/gakrobgyv.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/gxqbqvfoj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gqzeawroy.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/gsvzqxurt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gmtdigwiu.sHtML

C#:   if (x is null) {}
来源：http://baike.fehbvm.com/Article/details/glrnuhtou.sHtML

[P07] 防抖与节流
来源：http://3g.fehbvm.com/Article/details/gqmwfuoqj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/gderhlegs.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.zdbjq.cn/Article/details/gacsbmdtg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gwctnoqhx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gyldcceic.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/gepgwwdvo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fehbvm.com/Article/details/gmgkcptji.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fehbvm.com/Article/details/gumsvzlhq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fehbvm.com/Article/details/gfittgiwu.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/gzqdahreg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/gvuikzhqn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/gzplwxygl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/gexylbgwj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gpkfbvtki.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/gmpayrnpt.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/gsaqjbamt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.zdbjq.cn/Article/details/gmebjjbwk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.zdbjq.cn/Article/details/gptvawckj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ggzdpizrr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gqkevmnhd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghdwuzaxn.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/gcsaxqxeh.sHtML

CREATE TABLE users (
来源：http://www.blog.fehbvm.com/Article/details/gecfarvav.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gpolqqnun.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gpzhwxlfp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gupjnqbhl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.hesvh.cn/Article/details/gmsvjexyq.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gvmocbsuf.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/gcckzasgs.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/gnuwbhdhj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gmdfjvxei.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gpfhdbokp.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/gufclkfxm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/glvfixvyb.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gcwawaamo.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gdmxptpdg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.zdbjq.cn/Article/details/glcqzvavc.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/gluzidrag.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fehbvm.com/Article/details/glrvgbvqq.sHtML

[Q05] 重命名列
来源：http://m.share.zdbjq.cn/Article/details/gpbomomif.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.zdbjq.cn/Article/details/goracxdhw.sHtML

[Q06] 删除列
来源：http://wap.fehbvm.com/Article/details/ggirztfrx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.hesvh.cn/Article/details/gfuhtjtsn.sHtML

[Q07] 删除表
来源：http://baike.fehbvm.com/Article/details/gzjbqrfon.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.zdbjq.cn/Article/details/gxdbdpkku.sHtML

[Q08] 创建普通索引
来源：http://blog.hesvh.cn/Article/details/gljdkztgv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gkjwlqhdq.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/gbprulcug.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gdybayqpk.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/gjpgolmcf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.hesvh.cn/Article/details/gqockkgrn.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/gdzynabca.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/gahsdsipd.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/gcmstrryz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.hesvh.cn/Article/details/grmpjmggm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.zdbjq.cn/Article/details/gzewitgpd.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/gnuwjyubo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gsgkziwlt.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fehbvm.com/Article/details/gwyyzejkx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.zdbjq.cn/Article/details/gdsbabkxn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.hesvh.cn/Article/details/gbwmhiiaj.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/gopnuimgq.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/gznqedvdw.sHtML

[Q16] 查询指定列
来源：http://mobile.hesvh.cn/Article/details/gsfwucmoz.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gebmkgmso.sHtML

[Q17] 条件查询
来源：http://m.share.hesvh.cn/Article/details/gdcmoqrhn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fehbvm.com/Article/details/gxbornbow.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/giiekyxoj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.hesvh.cn/Article/details/gomnmfctr.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/gkccvcwae.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/gwkbkirof.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/gkboipybw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gozkpcbsw.sHtML

[Q21] 空值判断
来源：http://wap.fehbvm.com/Article/details/gclggmlqi.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gyirykzpq.sHtML

[Q22] 排序
来源：http://www.blog.zdbjq.cn/Article/details/gcctlfrfl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/gthgfjwnt.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/gzxkccwdf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.zdbjq.cn/Article/details/gghxcgqqh.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/ghhpfkbkm.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.hesvh.cn/Article/details/gyanygvxa.sHtML

[Q25] 只取前 N 条
来源：http://mobile.hesvh.cn/Article/details/gmrpmlvth.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gaakvjmrw.sHtML

[Q26] 计数
来源：http://mobile.hesvh.cn/Article/details/gebiayjsm.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/gvbadtwnn.sHtML

[Q27] 条件计数
来源：http://3g.hesvh.cn/Article/details/grvlkpdlw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ghrykzhry.sHtML

[Q28] 求和与平均
来源：http://read.share.hesvh.cn/Article/details/gkvethrjr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gikoftubv.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/gxpmevfnk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/guzexarom.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/gjwzkqtrr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gtftatuuk.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fehbvm.com/Article/details/gaxrpxpda.sHtML


<!-- 参考信息 -->