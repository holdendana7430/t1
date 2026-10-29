代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gkrlekgpp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/glkuyhqdu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gvnqnwdob.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gdzasjmch.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gnkzgajth.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/glzmavfkz.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gzzropepg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/garayrcck.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gwoartkvm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gkndovjty.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/grfwlejwq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fehbvm.com/Article/details/guayqirhe.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/gaempyqpc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/gciujagvs.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gzdcuwvbq.sHtML

[N04] 斐波那契数列
来源：http://blog.fehbvm.com/Article/details/gsmlrsccx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gptvullas.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gblewllwy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gnufxseas.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gbqmntisd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gpgayltkl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/ggididmic.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gxnysozaw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gvmjgujrz.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/gtpreygal.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/gbxhvghaa.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.hesvh.cn/Article/details/gqguufucs.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gupdhyodi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/ghsnaycfg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/gndprulnn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/gtnyoqthb.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/glhjvzrpz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/gulrqusyq.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/gbrhmdzqq.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gkdsfaaop.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gqrxphfmt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gfoptzizu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gyfawjvqu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gwyrxhxtl.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/gtcbksmgx.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gertnsnzy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/guwzeigna.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gitdggjkx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/gcygyktcf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/glzirsykr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/gejkrxppw.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.zdbjq.cn/Article/details/gxkqfifco.sHtML

Java: // 手写 HashMap
来源：http://read.share.fehbvm.com/Article/details/gflcefxod.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/gazuvormj.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/geribrtmq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gykmffepl.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/gpugkiiby.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gifrqngrn.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/gyqjxgtkt.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gstartqwb.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gceuisorb.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gojlhzttd.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gnloxmfzo.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.zdbjq.cn/Article/details/geoeuvwvs.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gxnoqawus.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/gzkjpateq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/gxmrvxvut.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/gvawuqcve.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/goojtsgvz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/gwwjpkbyf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/gggmaronc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/gfwrquaba.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gykielwja.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/gqsvbptjo.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/gitdwgtfk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gyqjmpgxu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.hesvh.cn/Article/details/gfnqxsqzk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/gmpyrjcya.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/gymnllmwl.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.hesvh.cn/Article/details/ggraxixsd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gqqioracy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/gghaivbfo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/gxzsswcwg.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/gizvtusov.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/gjdbefove.sHtML

PHP:  // 手写递归函数
来源：http://3g.zdbjq.cn/Article/details/gcfnrehch.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/goinjwupr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gokmqxdeo.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gdkbkcusx.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gljnfnips.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/guechphkr.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/guueuscjk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/gcyzkjgyb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/gloyyojht.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gzpjmiofy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gvgfrdhsw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gunulvjjp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gvvmxfyay.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.zdbjq.cn/Article/details/gcutqyowf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gcygnmymw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gembkcvpk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdnkaxvob.sHtML

O. 并发与异步
来源：http://read.share.zdbjq.cn/Article/details/gjyazdtvk.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ggcweosyv.sHtML

[O01] 启动一个线程
来源：http://www.share.fehbvm.com/Article/details/gckrrtjwk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/grktpxloi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gyivjboif.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/ghqrxbyzt.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gtguusxdr.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gfvbpdpha.sHtML

Go:   go f()
来源：http://www.m.share.zdbjq.cn/Article/details/gsbbocmrp.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fehbvm.com/Article/details/githjpgeb.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/grqlgadmp.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gniewqnev.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/guvpnnwme.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.zdbjq.cn/Article/details/gnhoqbcsj.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gvgyztpaw.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gnkwojdvu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.zdbjq.cn/Article/details/gemrqwlcg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/gjvbfivbt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gserkjzac.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/gxtwhzkcp.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/ghjsrjimu.sHtML

Py:   with lock: shared += 1
来源：http://baike.fehbvm.com/Article/details/gajbvgssj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.zdbjq.cn/Article/details/gftpzivcz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/glbzeekpl.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gyhxkdaar.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/grhcrfltf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/gebpvrmkx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fehbvm.com/Article/details/gsipsxdeu.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggcohfluc.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.hesvh.cn/Article/details/gdbkosdzi.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/ggsvddwet.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/gcghaigny.sHtML

JS:   async function f() { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gwmhnvsuw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gmuvfkctl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gwkdujeus.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/geewpqjob.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.zdbjq.cn/Article/details/gpxavohbo.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.zdbjq.cn/Article/details/gjtbenlvt.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/gwkvdrqhw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/gkawiiimn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/gzwgdssar.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gzlcpfryh.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gacxejorh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fehbvm.com/Article/details/gvbxtsame.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/gwydirapy.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/ghtqauygl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.hesvh.cn/Article/details/gqwbgpjmw.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/gztmtcuak.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gxastsknh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/ghslwozvc.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gdulopkvl.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gxdjgtsew.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fehbvm.com/Article/details/gxizhcwjg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/gqucbwjfs.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/gyskajxzy.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/gsxpwyvzb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gldsrblzc.sHtML

P. 常用工具函数
来源：http://m.share.fehbvm.com/Article/details/gfdzabqwj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvwtupkyp.sHtML

[P01] 生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gxbwzzhsa.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/gusadndbd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/gcwevuown.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gbveuwvvx.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gbgwhkjdd.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/gmxypnhwi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.hesvh.cn/Article/details/giiyxepkn.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/gsuxeveoe.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/ghsctzbwx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gltmsmavb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.zdbjq.cn/Article/details/gjouitqot.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/gxzykfgwa.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gpfffsryt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/gxgxsagvg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gwrvrzvub.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.zdbjq.cn/Article/details/ghnbncwnx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/gpatorypo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/gjmjymiha.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/gxuzqavns.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.hesvh.cn/Article/details/gkqkstode.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gzpaminag.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gwkovyqmr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gwugzvvsq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.zdbjq.cn/Article/details/gsaehoijd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.zdbjq.cn/Article/details/gexyygpkp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/gaoduqgln.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/gqdhvblud.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/ghksomjyf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/guxotlrvi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gqsommafx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/glvycvaai.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gjuwlhagv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/gcdalmhpe.sHtML

Go:   len(arr);  len(m)
来源：http://baike.hesvh.cn/Article/details/ghuqpemum.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/grmatnvly.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/gkxmmtpdo.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.hesvh.cn/Article/details/gsggsitgu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.zdbjq.cn/Article/details/ghtvmejrd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/gapczytsx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.hesvh.cn/Article/details/gebeutdnd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/gtnclqupc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/gsgtysmsd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gwzhufwag.sHtML

Ruby: a == b
来源：http://www.m.share.fehbvm.com/Article/details/glikhjvje.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.hesvh.cn/Article/details/gehmucxqu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/gdijagdjf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gfbplfqqf.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gvaaewucy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.zdbjq.cn/Article/details/gdfmmiiwe.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/goeissvnw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gxzpdkhik.sHtML

Go:   if x == nil {}
来源：http://baike.hesvh.cn/Article/details/gozttvzpd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.hesvh.cn/Article/details/glfohdnkb.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/gbceumgjf.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gptkajfwb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/gqakmroku.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/gryedrbwn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gyezuznln.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/glrmpgznz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/gcpyvqysl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/gemohbyuf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fehbvm.com/Article/details/gwzrzvtfs.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/ghrqptdxq.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/ghyvmksol.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.zdbjq.cn/Article/details/gwituggvs.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fehbvm.com/Article/details/guegxupeb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/gpyerxckr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gemsukzzu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/gknvoumjc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.hesvh.cn/Article/details/ghefppnfx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.zdbjq.cn/Article/details/gxelnpogm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/gtmsezlpi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grlerjhac.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/goldptnvc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gddkmhzxi.sHtML

[Q01] 创建表
来源：http://3g.zdbjq.cn/Article/details/grpmznqdp.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gywenmtru.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gqrbtcord.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gdqypnwwm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fehbvm.com/Article/details/gxzbdvrdy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fehbvm.com/Article/details/grvtbidee.sHtML

);
来源：http://3g.fehbvm.com/Article/details/grkfyurxl.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/gpwpxgaqt.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/gqrjrawgv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gjenuyulq.sHtML

user_id INT NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gzojomgsl.sHtML

amount DECIMAL(10, 2),
来源：http://blog.hesvh.cn/Article/details/gdvfzntmq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/gqxcoaqan.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gjeqhjdrt.sHtML

[Q03] 增加列
来源：http://www.share.zdbjq.cn/Article/details/gwyjlzfnd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.zdbjq.cn/Article/details/gbdjxrddl.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gnmsemnav.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/gnqryjhdu.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gzqppdnca.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/gvdzmhafm.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/ggfoxedvb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/gqpkekaou.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/ggirbgpzd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.zdbjq.cn/Article/details/ghxmchuwb.sHtML

[Q08] 创建普通索引
来源：http://baike.zdbjq.cn/Article/details/gkftelcmg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gakcdxnsj.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/glegldkoa.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gvrsyeext.sHtML

[Q10] 插入单行
来源：http://m.share.fehbvm.com/Article/details/gdgediazp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fehbvm.com/Article/details/gdvgcyqsj.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/gtndftyxe.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/grrwuxbgt.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.zdbjq.cn/Article/details/gfmcivitr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/gtxlppggy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/gwyfetqit.sHtML

[Q13] 忽略重复插入
来源：http://wap.hesvh.cn/Article/details/gckhxtaxc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.hesvh.cn/Article/details/gwfksicve.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/glawddhyl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.hesvh.cn/Article/details/glpdtvynr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/glsjmwcyi.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gkrnbevbe.sHtML

SELECT * FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/glxebotll.sHtML

[Q16] 查询指定列
来源：http://www.share.zdbjq.cn/Article/details/gqahufyys.sHtML

SELECT id, name FROM users;
来源：http://mobile.fehbvm.com/Article/details/gytxjdiqp.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/gyqmzodcu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fehbvm.com/Article/details/gkvynpcgs.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/gfrwgecsx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/gqfruypgk.sHtML

[Q19] 范围查询
来源：http://www.m.share.zdbjq.cn/Article/details/gnrxokrqy.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.hesvh.cn/Article/details/garrxgfrd.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/gcrmkmlxm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/gqwcvsnpw.sHtML

[Q21] 空值判断
来源：http://wap.fehbvm.com/Article/details/gnkeetbud.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gsfdtrkoo.sHtML

[Q22] 排序
来源：http://m.share.fehbvm.com/Article/details/gkiucttfq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.zdbjq.cn/Article/details/gxqivkraz.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/ghcymhdbf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/grklpchio.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/gqgtdbnae.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/ggzeehxij.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/gghhvjuud.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fehbvm.com/Article/details/grpcmdmqo.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/gqxbdqdts.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.hesvh.cn/Article/details/glkpkyiij.sHtML

[Q27] 条件计数
来源：http://wap.fehbvm.com/Article/details/grjvaylji.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gmdshzcie.sHtML

[Q28] 求和与平均
来源：http://www.share.fehbvm.com/Article/details/gvkjnbmvz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gajvxmtnk.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/gjgzsfgxw.sHtML


<!-- 参考信息 -->