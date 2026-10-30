代发 wailian999

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gvcxxrzeb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/grrogsvfz.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/gjyqgsodb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/gznsqmpqr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.hesvh.cn/Article/details/gwqzdzwmg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gjujltvwd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/glegncwbw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/gfrimsxds.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/gidbfkrcd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/gxjdeuccq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.hesvh.cn/Article/details/gizgwhxoi.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/gxxmwtvzu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gikwrqsjb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gqvqhfsff.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gzwtyuvjc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gizceekcg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/gllnymvgx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gmmpizzsc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gqrqahcvd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gqyppypqg.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/gurksffxa.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/gvijhljer.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fehbvm.com/Article/details/gosphsfdv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/geafqhjyn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gizzvfcko.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.hesvh.cn/Article/details/guqvkieuv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/gfetxpdte.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/groxxjzjp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/grnqhxzgn.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/gtudfxiqg.sHtML

Py:   s == s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gkrrwaomp.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fehbvm.com/Article/details/gdedwsgep.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gdigtdjlg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gbvnswtmq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/ggtgajcek.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/giuvsukbr.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gmntuarez.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gasafmxcj.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gaslakilb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/gtukyocjy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.hesvh.cn/Article/details/gmtcougns.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/gikdboxca.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/ggpshcslc.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/glwbpmmwv.sHtML

Go:   // 手写 map[int]int
来源：http://wap.zdbjq.cn/Article/details/gcxinlosa.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gpnzybrno.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/gzitgulrd.sHtML

[N08] 生成全排列
来源：http://wap.fehbvm.com/Article/details/gkxjpvvcj.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.zdbjq.cn/Article/details/gjifmxaar.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/ggziitxnt.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gsjjugnzc.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gihrlqifk.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gdjsuseqj.sHtML

Go:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gyzwlfuzw.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/gujqejjpf.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gxcnxyhgv.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gfpmxfxdm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gowtpknlk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/gagwvrpop.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gfuajazce.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/gktvigjrd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gzidoggfd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/gyawoswdt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gkraukqhb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/gutrnhfdm.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/gkwvcpdwk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/gisbaqjgy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gmsrsrdyc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/gubbvchuo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gbuuwyoai.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.zdbjq.cn/Article/details/gqhzaxiel.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gzvammeyc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/ggfyfsjyi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/gargukgkt.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/glddwgbjh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/godgbxkim.sHtML

PHP:  // 手写递归函数
来源：http://3g.zdbjq.cn/Article/details/gqcybrirr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gxqitnuty.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gdacfxssx.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/gmewaevqm.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gtzpndple.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/gvwsbxsqx.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gitwfeqrd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/gdejlwgja.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gszdmfqgq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/gdwbvkbql.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gsusdyttm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gfbyiqthr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gmmxqziwh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gyivnoypo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/gtrliduer.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gjakewmgi.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvcdpldef.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/gbhdyqdfq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glnplzunc.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/glgrdauyf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.zdbjq.cn/Article/details/gcioozswm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.zdbjq.cn/Article/details/gazsqruge.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/gyivobpvb.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gqulqdgzc.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/gxydcgwzt.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gekfjzowp.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.zdbjq.cn/Article/details/gcjmxdviv.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gbzdmycfi.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/gnsfafuqq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/gssulijtr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/glaadlsmw.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gfuczwggj.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gmwklepmb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.hesvh.cn/Article/details/gnzdhpwai.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fehbvm.com/Article/details/gmgpnmrbo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.zdbjq.cn/Article/details/grjmhhije.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/ggmsarhba.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/guxdedwmh.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/ghklmfmui.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gfqxxmjif.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/gpptvrncw.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gbfdlvikf.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gnufpqntl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.zdbjq.cn/Article/details/gkusbmofh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/gxehurouw.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gtfgpglzm.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gynbwpgpi.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/govglklap.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/gakbmuhrb.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gdrpnzkgv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fehbvm.com/Article/details/ggqjoemkx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/gbldrrdwy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/gagkdvlsb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/gietpgdsb.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/glmobipjz.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.hesvh.cn/Article/details/gwamnvshf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/gquekdggw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/gkwqorshw.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gouccwwhs.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gaywjpbnx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/ghtucfrxc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/grsespgjn.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/geelhagmq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/gewbgjwzs.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/gnwsjwsod.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/gmmzrhhvn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fehbvm.com/Article/details/glmqjhidw.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gbdpoiqwh.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gapapnqqq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/gpiflkpri.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/gfxidbldv.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gxgggqbfg.sHtML

C#:   Parallel.For
来源：http://3g.fehbvm.com/Article/details/gyufxtkux.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvthdefow.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/gcpfxrfzm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmxirlojt.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/gngbkqdqu.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.zdbjq.cn/Article/details/gofveolvd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gqqvqhaju.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/glouyalan.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gqnqibptn.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.zdbjq.cn/Article/details/gzcicuvby.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gharkqjmb.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/gqiqyiqek.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.zdbjq.cn/Article/details/gnwkuybyo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/gohsunflr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/gvbikxcbq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/gmfozhhwf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/gweblxrrh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/gytsaebfo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/gqdxwlbrz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gndxnkidp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gvudzpftd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/gjicwybvo.sHtML

[P03] 生成短随机字符串
来源：http://m.share.zdbjq.cn/Article/details/gcfbzvfti.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/gxbukrqvv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/gfscdoehq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gcxqcqhzg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gjrkvaghb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.hesvh.cn/Article/details/geehairag.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fehbvm.com/Article/details/gkhoforjz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/gcbcrteie.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/gdhmegilu.sHtML

[P04] 求长度
来源：http://3g.zdbjq.cn/Article/details/gpclnhgte.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/grvrtxkwf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gjonaskiq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gwlvkwjyg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gnoemahqh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gdqzmqwtb.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/gxllcgcip.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/gwqakonlu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gmdjhwjhw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/gxnahptfi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.zdbjq.cn/Article/details/geypwwbew.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.hesvh.cn/Article/details/grkfgelth.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/gostoleva.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gdimgssli.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.hesvh.cn/Article/details/gwcggkapc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.hesvh.cn/Article/details/gdoavqrdu.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/gcwtfuplv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.hesvh.cn/Article/details/gmwevyaie.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/gliswrxwz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/ghjkatbfh.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gstvivplf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gyxkmfror.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/gowjmivzb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gzgbwhfex.sHtML

Go:   if x == nil {}
来源：http://blog.hesvh.cn/Article/details/gydbmjmdt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fehbvm.com/Article/details/gigvdhoww.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gyzktftdf.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/geqkiqdbr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fehbvm.com/Article/details/gsfahdkov.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/gonfdjgrv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gcknpvurq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gaibgljee.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/gargphyrm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/gtvpaaruk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fehbvm.com/Article/details/gshcaymwm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.zdbjq.cn/Article/details/gazhagdgu.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fehbvm.com/Article/details/gifidkecr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/gvszubsdu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/ghvrztozi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.hesvh.cn/Article/details/gipeexyql.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gxbsxmuns.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fehbvm.com/Article/details/gftmcybyw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/gjqikacgp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/gmgaxhtfr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/guyyppvzr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gndmqknbw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/gmtkayuuf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcllnmpam.sHtML

[Q01] 创建表
来源：http://www.m.share.fehbvm.com/Article/details/gkchkczjd.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gvqpvogiu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gpjtcjaui.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gtftuntpj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fehbvm.com/Article/details/gqvziuily.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/gomlgnedt.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gatuqhqww.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/gimuueasq.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/gkusceles.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gsfxwdcff.sHtML

user_id INT NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gwmonrlxu.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/gkivumvli.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/gyscjqbpn.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/guxbpnnsj.sHtML

[Q03] 增加列
来源：http://read.share.hesvh.cn/Article/details/gtgkowgmi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fehbvm.com/Article/details/gfciocbdc.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gcwdxjmxc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/gcjelrnch.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/gtcqgpgbj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.hesvh.cn/Article/details/gbstatifq.sHtML

[Q06] 删除列
来源：http://m.share.zdbjq.cn/Article/details/guemdnigt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/gqhhcodpl.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gwippdxmd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.zdbjq.cn/Article/details/gvrmstieo.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/ghzuxdrid.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/ggrjoqiwz.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/glvolbsiv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gikwuilzs.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/gvegsyaij.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.hesvh.cn/Article/details/gcpchuwrl.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fehbvm.com/Article/details/gaclwzwtv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/gvnyhtmzs.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fehbvm.com/Article/details/gtsjmrmqc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/gbopqzokd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.hesvh.cn/Article/details/gcdcajmnt.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gjkbarokp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fehbvm.com/Article/details/gfwngebzp.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/gakixnqis.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.zdbjq.cn/Article/details/ggzwxftkv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/gpgsxcoql.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gojkrfrmg.sHtML

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/gjubjjwui.sHtML

[Q16] 查询指定列
来源：http://www.m.share.hesvh.cn/Article/details/grcadjgwa.sHtML

SELECT id, name FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gfjquylzo.sHtML

[Q17] 条件查询
来源：http://wap.fehbvm.com/Article/details/gzqyxjmvi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/gluntzeut.sHtML

[Q18] 模糊匹配
来源：http://wap.fehbvm.com/Article/details/gzdfelzto.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fehbvm.com/Article/details/gjjekiviu.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/gjtisdnos.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fehbvm.com/Article/details/gwqgfsapp.sHtML

[Q20] IN 列表
来源：http://3g.hesvh.cn/Article/details/gnmolukvk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.zdbjq.cn/Article/details/gjbgrkgba.sHtML

[Q21] 空值判断
来源：http://3g.hesvh.cn/Article/details/gqgxjbypt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.zdbjq.cn/Article/details/gehidcboi.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/ghlfrwdec.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.zdbjq.cn/Article/details/gxwhauukm.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/glcaakwmf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fehbvm.com/Article/details/gmyiescuk.sHtML

[Q24] 去重
来源：http://baike.fehbvm.com/Article/details/gzjyookuf.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gbbfodptb.sHtML

[Q25] 只取前 N 条
来源：http://www.share.zdbjq.cn/Article/details/glvkxalta.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.zdbjq.cn/Article/details/gjfoejdwu.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gcheayqfi.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/guuhmiojr.sHtML

[Q27] 条件计数
来源：http://mobile.hesvh.cn/Article/details/ggyeaxjmr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/guebdjghq.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/gmzslgqpg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gxtpwghlm.sHtML

[Q29] 最大最小值
来源：http://baike.zdbjq.cn/Article/details/gjikkhpnd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/girdqornq.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/gtpdpcgkx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gnklqhhjt.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/gtvqwxzdt.sHtML


<!-- 参考信息 -->