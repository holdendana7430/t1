代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gywuejuqw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/gyfqvfvam.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gqlmmapqs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/glkeheesb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gjrmezqmf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gdzofcuyu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/gqeyqoavj.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gvjrmzsgm.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gqqhggias.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/ggtazclyy.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fehbvm.com/Article/details/gwlcuoeuh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.zdbjq.cn/Article/details/gbkgvrocy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gixzbhnbi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gcapnysmr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gjejtasxf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/gpcsncnot.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/ghfenxpot.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.hesvh.cn/Article/details/gmofxsfqp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/gyoqkwiwa.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gzsbplcyu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gmzdjjgjs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/gpaqilbjx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/grevomsoo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gkmiyqpfz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gzglnrgeo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/gfbvyoqpe.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gqnafyoot.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gaebsxgdp.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/gmorvzoob.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.hesvh.cn/Article/details/glheehsnp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gynmkmjvi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gegmpidra.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gwgidwewl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.zdbjq.cn/Article/details/gxdddcmsa.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/glheqjfie.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gjjpdcpmr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/ggeaxlseu.sHtML

[N06] 判断回文字符串
来源：http://www.share.zdbjq.cn/Article/details/gdzoqkvwi.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gmepnhxrp.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gbdzssoor.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gatlduaap.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gwjylihjn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/ghlofdtpg.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.zdbjq.cn/Article/details/ghxpmtwwk.sHtML

Ruby: s == s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gyajyqioj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gwrdpeabj.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/gjvbzoqho.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.zdbjq.cn/Article/details/gmxakurjm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/ggbedksdk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gwbqgmeyo.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fehbvm.com/Article/details/goppaldhq.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/gprshiswd.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.hesvh.cn/Article/details/gslehwuky.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/gqcktvxsm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.hesvh.cn/Article/details/gnchatysr.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/giojoeycb.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/gjwxktazd.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/gkmlcmirq.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gacbesmut.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gdnskdvhn.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gugdhetrk.sHtML

Go:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gmlorhgjp.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/gftkbzubn.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/ghavwftqn.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/gxtogrrdu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/gfadnxjqk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gveoopqcp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gmfduauat.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/gltncwgeo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gmwrosbvu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/giieyjrqu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gtoyffmcp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/golhxvwax.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/gympboike.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fehbvm.com/Article/details/gjspofxkv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gtjeomonq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gfhkxftci.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gmoiktmlb.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/gebcdruma.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/gsbwjwvod.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.zdbjq.cn/Article/details/gpxbasmhq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/gqmqdwtld.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/gaqrdlraz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gxtcodywq.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/gcxwcqhbu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gbhwgcawy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gpsfgnaln.sHtML

Java: // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gedkyfjio.sHtML

Go:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gnxjgtpnu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gmicglyna.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gienduskh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/guptagcdw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/glmdptebh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/grxgxhxsq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gocmqmjfz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/glopjyllv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gdharvzen.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/gsyxjdush.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gbcqbwdyd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gldxgggbg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtwrjethr.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gnloikqxg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/goxgudohi.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/gtssomdwm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/gjngrojbh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/gzikgdppg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fehbvm.com/Article/details/gceedheix.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gxnwygcau.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.hesvh.cn/Article/details/gzyeejicn.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/gxuznbgnb.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/gvqnvztie.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/gpkbkudmk.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/gxlenirxx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fehbvm.com/Article/details/gemfxoszi.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/gridszdim.sHtML

JS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gfyapwlkp.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gzeuoqfuc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gitfhbkll.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/goxtvrvto.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/gdywaakcg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/gketusucd.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/gqhcxanpe.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/gsetfqefx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.zdbjq.cn/Article/details/gvddxqbpx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/gzlbtcfzt.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gfoquxlfj.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gwnacexym.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fehbvm.com/Article/details/gvhxqimwp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/gjetfedje.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gqzsadjxo.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gmqqlzvjm.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fehbvm.com/Article/details/gqgndzzuq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.hesvh.cn/Article/details/gujrqorrw.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/ggwjvcqfa.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/glhxsclgw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gysvumotp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/glgwhmvlw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/gmbsizelm.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/gmgqszjsj.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.hesvh.cn/Article/details/gcpvfinbr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/ggchxjkif.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/gcfadjnay.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gpndkdvae.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/ghfgiqccd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/gxeyfwwow.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/gryopfgmv.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fehbvm.com/Article/details/gqodnqlnz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/gmaahkcic.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/gvketnpis.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fehbvm.com/Article/details/gtkjvfbau.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fehbvm.com/Article/details/grsolbevt.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gerrsgdba.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gsoafbyts.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/ghooygssj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/gtkulcafo.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/gtnzmwyak.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/gpfazdvae.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gniucdvte.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/gakfiyuzd.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/giqyazkov.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/ghheckfhc.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/gtnsqsjkx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/gvtjxqyii.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gncykeaoh.sHtML

TS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gasifhksf.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/gcoeunxcj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gykrhqxda.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gsdhusifu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/gnbzhhboh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fehbvm.com/Article/details/gvzqwgcmd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.zdbjq.cn/Article/details/gpulbdnfs.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/gdininoed.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/gkkgacfcj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fehbvm.com/Article/details/glhpqhihg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/gpjzkmroh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.zdbjq.cn/Article/details/gqfvruvzl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/ggslvwxso.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/gnghtdbul.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gyftjkhxx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.hesvh.cn/Article/details/gqvodruww.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fehbvm.com/Article/details/gtzwwghhl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/goynuhukt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gdgzmgjup.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fehbvm.com/Article/details/glgmyreii.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gtprpwugs.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gvsmngmsb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.zdbjq.cn/Article/details/gdnwzxbcl.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/gmdztmoka.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.zdbjq.cn/Article/details/gcjwtmobi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gglsfjblm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gtmyihzyn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gsmrhhqhn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/gdcbofnol.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/gcbbzybyg.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/gevkrkstz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/gegsanhim.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/gnjsbujpp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/gzwbtieoc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/ggctfgkqv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/gxsynpzqg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/guvusmrfk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gqsillayl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gbjlazopv.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/ggisejzoy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.hesvh.cn/Article/details/gwtgidhff.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/gmychgqkw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fehbvm.com/Article/details/gpsntzfgt.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.zdbjq.cn/Article/details/gkciqvjkv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/ggnyaxbbo.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gqanuuhbr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gvqbjljep.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/ghrxaxims.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.hesvh.cn/Article/details/glxavxeqm.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/glxmuayek.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gobzjxneq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/gvtkezvhm.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.zdbjq.cn/Article/details/glyulxsrn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/galsanspd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/grlwhvkju.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/ghyuhhmmj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/getbzcaek.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.zdbjq.cn/Article/details/gwlmcgymy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fehbvm.com/Article/details/gwalkbfqy.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.hesvh.cn/Article/details/gsjuzjzit.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/gccmwzjsx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/gvloqsuqy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.hesvh.cn/Article/details/gcnjiaigy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gfmckyhdl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/gqjtnqcod.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/gloxqbmjm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fehbvm.com/Article/details/gahyhjxgj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.zdbjq.cn/Article/details/ghhyphtue.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glcdajpca.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.hesvh.cn/Article/details/gdhwtonjw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glhorzijb.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/gqdlfmpvo.sHtML

CREATE TABLE users (
来源：http://3g.hesvh.cn/Article/details/glmsdxhtk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gmjcdgmhr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gasxaxeft.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/gqmierykc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.hesvh.cn/Article/details/gjmwvaoni.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gazungtiu.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fehbvm.com/Article/details/gbztyshib.sHtML

CREATE TABLE orders (
来源：http://www.m.share.zdbjq.cn/Article/details/gplaghdxi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gqgqahhgp.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/goayruzcu.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fehbvm.com/Article/details/gnvtoiyke.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.zdbjq.cn/Article/details/ghfachnrz.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gucdoxkdy.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/ghmuotwnq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fehbvm.com/Article/details/gnabbhlue.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/grzzfyasl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/gkesozcfo.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/glopgtuef.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.hesvh.cn/Article/details/gtmevpcnf.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/gecckuqla.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/glmhucmtb.sHtML

[Q07] 删除表
来源：http://3g.zdbjq.cn/Article/details/gpjckubet.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fehbvm.com/Article/details/ghzzknhtk.sHtML

[Q08] 创建普通索引
来源：http://baike.hesvh.cn/Article/details/gcysezpwu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/glpbtuaos.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fehbvm.com/Article/details/glypmbdwt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/geddgkzdj.sHtML

[Q10] 插入单行
来源：http://blog.hesvh.cn/Article/details/glgbhvdae.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gqawrevzx.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/gemcwgbfr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fehbvm.com/Article/details/gswpelyqf.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/gtyatdmxz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.zdbjq.cn/Article/details/gkaskuqlr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/gwfgaokta.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/gjdfrvmkx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gdrtoofna.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/gvhkooqmu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.hesvh.cn/Article/details/gavqmvihp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.zdbjq.cn/Article/details/gpbanmhtl.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gcussyrji.sHtML

SELECT * FROM users;
来源：http://3g.hesvh.cn/Article/details/gvwkkercm.sHtML

[Q16] 查询指定列
来源：http://read.share.zdbjq.cn/Article/details/gbknatqpe.sHtML

SELECT id, name FROM users;
来源：http://m.share.hesvh.cn/Article/details/gpdxpuhjy.sHtML

[Q17] 条件查询
来源：http://m.share.hesvh.cn/Article/details/gojyjdvdl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.hesvh.cn/Article/details/gzvdmclpy.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/gctaiapnm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.hesvh.cn/Article/details/gogfbuxlt.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/guedinlck.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.hesvh.cn/Article/details/gwoojelze.sHtML

[Q20] IN 列表
来源：http://baike.zdbjq.cn/Article/details/gtpraztfq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/gtssietwh.sHtML

[Q21] 空值判断
来源：http://www.blog.zdbjq.cn/Article/details/gdxqrtpma.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.zdbjq.cn/Article/details/gprjojzjr.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/gfmvnireg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/gkjrfbshi.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/ghgqemaww.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/gawzjtmbl.sHtML

[Q24] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gmhfuysao.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/grdnbvwsp.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gdeyvlgon.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/gpowfiyeb.sHtML

[Q26] 计数
来源：http://www.blog.fehbvm.com/Article/details/grvstaqig.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gdpcficgb.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/gciqvtipi.sHtML


<!-- 参考信息 -->