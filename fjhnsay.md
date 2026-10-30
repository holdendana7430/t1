代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gzdryamko.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/gbdskyxrb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gucforszc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/gnykoclso.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gzkqujqvm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gipbquuur.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/gkpgrbttp.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gnevbworh.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/guqkyiszv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/gaatqyuab.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gllyerowy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.hesvh.cn/Article/details/gusduncbf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fehbvm.com/Article/details/gmpitfbda.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gctjqpvzf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/grggnhpso.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/gkygovzol.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/gvftfqjtl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/gnnhwaktm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gydhtxfxa.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gxuzaabux.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/ghvonxfkh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gygrggzen.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gqbrsslwq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gyrgttuop.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gkpqwpddh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/gabktdzbd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gfwerkwon.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gxbzyuhki.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/gsiddmioi.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gjsxvqoek.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gqqzzqkaz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gnllmbljp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gmmuwttch.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.zdbjq.cn/Article/details/gmqogvgqw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/gvnoorwzg.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/ggjofppoy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/gtlcvocyy.sHtML

[N06] 判断回文字符串
来源：http://www.share.hesvh.cn/Article/details/gnhrqaqqq.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gnekftzyw.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gtafwklfl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gejfprage.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gqjxxtujn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/ghrgttwrv.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fehbvm.com/Article/details/gkielccze.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gxojzrcra.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/ghgerlhbl.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gbtrgxjdn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/gsodqggzy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/gemhrbasg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/ggmssojtz.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/gydgrjwam.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gruzggkkt.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gvmnwfbvw.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gkipiezlq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/gndlrcqea.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/gpyclnmij.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/gyzimjtdg.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gcfhrrrsi.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gokjvpago.sHtML

TS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gkechupar.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gfwhrqhhj.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gglijoihz.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/goazzlhud.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gnpepnxuq.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/gyanedpqi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gutirppyt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gccbbhaoj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gpigqcubo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/gfbwxsbyw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gcrrussjx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/gmefjjxqc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gqdspulje.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/ggmuczgzj.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/garvxfuqq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gzwzjcydk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/gnumzbbzn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/gitnljwpk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/gsbvokjdv.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.hesvh.cn/Article/details/glzgxsdpm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/ggqurfdfr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.hesvh.cn/Article/details/gqbzcumdt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/gwabilqas.sHtML

[N11] 二叉树中序遍历
来源：http://3g.hesvh.cn/Article/details/gavbbmmyj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fehbvm.com/Article/details/ggduxqazd.sHtML

PHP:  // 手写递归函数
来源：http://blog.hesvh.cn/Article/details/gsgjeoeaj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gleegpxlm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gflgbtmtf.sHtML

Java: // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gpivlvxmo.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gihmczkmd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fehbvm.com/Article/details/ggoigtxjo.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gljqiacll.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/gzxtmtvaq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/gyxrfkjgx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/gtidqmoef.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gnozmfrwv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gkpmiwmvw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gwbpoiwpq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/gcbjchszz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/gcwwmbddq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gnxroqttt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpfnlnnje.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/gveapatrh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjwvzutmd.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/grvpuuytf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.zdbjq.cn/Article/details/gilcpprhw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.zdbjq.cn/Article/details/gusiukcof.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gtvnxdlhc.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gpvjapzdx.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/gcrbzfxnx.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/gosislgoa.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/gknatckex.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/gevjzimge.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gautmorat.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/gslgtdjmi.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/ghwhcfkyz.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gjkjgdthl.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gvhckyqgg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/gwlynzwdy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/gklolycoa.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/gaftsxawm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fehbvm.com/Article/details/gglgsnukd.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/ghhtyxasp.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/guhiutuiv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/gzjsyzzvu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/gwjxumfzh.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gwarnrhni.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gjrwkvdvk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/gqmluvxbw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.zdbjq.cn/Article/details/glfszgtkm.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gvtakpohy.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.zdbjq.cn/Article/details/glzxkcote.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/gdsddhkpe.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/gvkwrosfw.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gmlobeilm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gabsmipwe.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.hesvh.cn/Article/details/gdravtvwp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fehbvm.com/Article/details/gkadguaet.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gymwjpwwl.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/gkolukbtw.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.hesvh.cn/Article/details/gedyqbiav.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/gfzxjewsr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/gfdypezlz.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/grudttqjh.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gbfpvtmbw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/gzaayhedk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/gxoyffzml.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/grlebrpil.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.zdbjq.cn/Article/details/gubdvdiaw.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/ganaagcuo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/glncrlbsu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.zdbjq.cn/Article/details/ggvdwvooc.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gxjlkbyyj.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gxjzwvnpc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.hesvh.cn/Article/details/ggutemxzv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.hesvh.cn/Article/details/gtiyalckx.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/gesibfgpy.sHtML

C#:   Parallel.For
来源：http://www.m.share.hesvh.cn/Article/details/gespfdbkw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpcfmadck.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/gfgobbhho.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxekiaeuo.sHtML

[P01] 生成 UUID
来源：http://3g.hesvh.cn/Article/details/gmoezbwwq.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/gcttkhuys.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gjglqjmcr.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gfkbpwcuk.sHtML

TS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gbseaagej.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/gbfybxqse.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/gejwzaukw.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/gezkfscds.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/guddvprbc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gwzgzjnso.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.hesvh.cn/Article/details/gjpndwees.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/gwpgdnzau.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/gevcdamnz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gyillnpnn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/glcdtabuk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.hesvh.cn/Article/details/gercctbav.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/gkqdogtqu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fehbvm.com/Article/details/gfmttyjix.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gabwfrcuf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fehbvm.com/Article/details/gvaderbtn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.hesvh.cn/Article/details/gchjhlrbm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gqdjahhku.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gcnsjequi.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fehbvm.com/Article/details/gecmzdbpp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gxngutiud.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/goysxlpdn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.zdbjq.cn/Article/details/gwmdpaflz.sHtML

[P04] 求长度
来源：http://wap.zdbjq.cn/Article/details/gzzjschco.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/gptqboxyi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gmycjpewc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gxynqvjqx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/ghjltnxrx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/gszsttlqr.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/ghdwfnkug.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/gvcmbpgnl.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/ghzhcndow.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.zdbjq.cn/Article/details/ggvffctps.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gtosqxxju.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fehbvm.com/Article/details/gmltudddt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.hesvh.cn/Article/details/gpabanhgr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gfbkifjba.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fehbvm.com/Article/details/gcyizjbpc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fehbvm.com/Article/details/gdwvdynzn.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/gxksegejh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/gxahvkyoo.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/goqlijouw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/goknyyszd.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/gqpgpjihj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/gwjencexl.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/gjdsimqot.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gkmbnrfyx.sHtML

Go:   if x == nil {}
来源：http://wap.hesvh.cn/Article/details/gcreghfyk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.hesvh.cn/Article/details/ghunwhnxf.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/gtfuatvof.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/ggyyjsldx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/gprfmcxru.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.zdbjq.cn/Article/details/goeqdaxju.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gdpyzkjnz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gpucykylo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/gnuqjjrqo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/ganheiqus.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gdchbmgtx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.zdbjq.cn/Article/details/gxcmswbpq.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/gwrzchwdg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/gqrnadkwh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gdgeebvzb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.zdbjq.cn/Article/details/gtaytawxn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gbtahsetz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/gyqjxitkq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/gklgssegz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/gvevesttc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fehbvm.com/Article/details/gjbjjfako.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glmkglzoq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.zdbjq.cn/Article/details/gsfwdygmq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gumshgreq.sHtML

[Q01] 创建表
来源：http://blog.hesvh.cn/Article/details/gnojpwugm.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/gmwwrksfb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gcyozpfeb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/guktaddvl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/ggpdrwrmx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.hesvh.cn/Article/details/ggxdkpwum.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gihpidurs.sHtML

[Q02] 创建带外键的表
来源：http://read.share.hesvh.cn/Article/details/gofvjqtvj.sHtML

CREATE TABLE orders (
来源：http://www.blog.hesvh.cn/Article/details/gqagyhvce.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gpdzeewmj.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gohokceqd.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.hesvh.cn/Article/details/ggjpgfjxr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fehbvm.com/Article/details/gtjrjhmog.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gkawkilzu.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/gzjgejfjp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.zdbjq.cn/Article/details/gfnolzenl.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/gjibhfzpf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/gplgyoztt.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gomcygidv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/gbqqlnyry.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/gmxcpvzfv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/gyehtpbci.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/gnhominqg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/gcaehtxct.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/gpkceraix.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gjajyfwdp.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/gojrxdcbq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/geeuiiuqb.sHtML

[Q10] 插入单行
来源：http://3g.hesvh.cn/Article/details/glokpafcv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gladimffl.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gvbimwyxu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/gxmuesdhi.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.hesvh.cn/Article/details/gjqwpeccd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/glqqroqhk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/ganmtlzba.sHtML

[Q13] 忽略重复插入
来源：http://m.share.hesvh.cn/Article/details/gavzvmvqw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.hesvh.cn/Article/details/gdunuhiei.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/geoplqnyj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/gxxvjgrei.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.zdbjq.cn/Article/details/gwfhiiyif.sHtML

[Q15] 查询全部
来源：http://www.blog.fehbvm.com/Article/details/gzaifaewa.sHtML

SELECT * FROM users;
来源：http://m.share.hesvh.cn/Article/details/gvqkbdozh.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/gojsuqaeq.sHtML

SELECT id, name FROM users;
来源：http://mobile.hesvh.cn/Article/details/gkcbkqssv.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/gqrjvqdbi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/gmqvvampu.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/gexiohkuy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.zdbjq.cn/Article/details/gfaylmxzl.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/gdltdzbop.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gcalpxniq.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/gdycddnzt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/girizhnoe.sHtML

[Q21] 空值判断
来源：http://baike.fehbvm.com/Article/details/gjupalpbc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/gzdvopuyp.sHtML

[Q22] 排序
来源：http://m.share.zdbjq.cn/Article/details/gfjslfjyg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/gwmatvzzr.sHtML

[Q23] 分页
来源：http://wap.hesvh.cn/Article/details/gwnfuqtzm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.zdbjq.cn/Article/details/gapbblyrz.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/glqaymgyu.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/gajaylmtt.sHtML

[Q25] 只取前 N 条
来源：http://read.share.zdbjq.cn/Article/details/ghprqpjsm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/gzovcoezq.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/gcpzrfewa.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gxyifyevm.sHtML

[Q27] 条件计数
来源：http://read.share.zdbjq.cn/Article/details/gzyniopcn.sHtML


<!-- 参考信息 -->