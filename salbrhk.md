代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gdzyuogsr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gzovdxxcs.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fehbvm.com/Article/details/glsppfnmf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/grjphopon.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gejqhsvlt.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gelebishp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gmgkmzlff.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/gawippdyf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gfpbmnznc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/glagopjjf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.hesvh.cn/Article/details/gaftonzec.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/glxxyrioa.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gyxyexqad.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/gxftrwivk.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/gwldpoypa.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/gvwevlgki.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gdnhpknej.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gmecvyibc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gwjhwupsx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fehbvm.com/Article/details/gungmjyvb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fehbvm.com/Article/details/gxnvflntd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/gzqriwcxf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fehbvm.com/Article/details/gglzvilwj.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/ggtyadqes.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gfgabgurp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gulhkdjvp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gumjijcyq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/ggfdogdbz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gzvnukyno.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gedefupor.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gidtxrqkd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gdyynlpuy.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/gjexydhzi.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.hesvh.cn/Article/details/gocsvakrj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/gtjokcqck.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gcnfneugp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/glsesnqhd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/gzqazcakv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/ghxvzjwoz.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gcupyehns.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/gxyvqdhyn.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gsbxaqpma.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gafuzmfrl.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.hesvh.cn/Article/details/guhxamabj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gkkitkgfw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gkbiqiyka.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/gwarinyry.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/glzjvxkhs.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/ggvekwglz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gzgvaaocx.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/ghepcbdrg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/ghfqavqrk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/gemzeglsr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/grzdjuwou.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gpmxwiyas.sHtML

Java: // 手写 HashMap
来源：http://mobile.fehbvm.com/Article/details/gqabpunro.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/gkoksmexb.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/gzotchdkt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/ghygjyoga.sHtML

[N08] 生成全排列
来源：http://baike.fehbvm.com/Article/details/gqkzgvsgy.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/gmgnhucaj.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/grtblxkmq.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gfqkbjhjw.sHtML

TS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gakrmdvdg.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gnonukjmo.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gehjenqzh.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/gbillriap.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gwjtxdohl.sHtML

[N09] 栈与队列
来源：http://wap.fehbvm.com/Article/details/gtcxljeon.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gpdfozybe.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/goaeoagxn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gjoqtwhlw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fehbvm.com/Article/details/gvrthesus.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fehbvm.com/Article/details/gxntkdini.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fehbvm.com/Article/details/gmwipcmnh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gixunbgqv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gjffmehwr.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gwhstltzx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/gxdeydvby.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/glvjwcyjy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/grsttwktu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/gbpxgmjik.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/giozuowxm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gkjgyyxfj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/gcrnnuuou.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fehbvm.com/Article/details/gvgdyzefc.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/gkzatkbrj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/gkfhwbokp.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/gwxvvqmxh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gklkohdys.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/guluqpgbe.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gktektvsr.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gvuyfofmy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gbpkdtxlz.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gyycklvwn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/gnchmlipm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gtswvyldd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/gmvdytpyo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/guwbxafwc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gywczzpqf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gxywxwujf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gvluwptrh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/gznplmpeh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gnkgsysej.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gyycitddz.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/gzudsqsrc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbqqrovtf.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/goalwljwb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/gtrdunylu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/gjobgnypi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gkoxbsdvl.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/ggkqcbllh.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gvwnhoynu.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/ggzufjoqr.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/gpwscppei.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gjrzhuqcg.sHtML

[O02] 使用线程池
来源：http://blog.zdbjq.cn/Article/details/guoicxxpv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/ghvepuhzq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/gejqehrvy.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gyeauvxep.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gpuulmooh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/gpycwooip.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gbapadblm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gjaivruwz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/gbqemixiw.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/gdtlgxeim.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gjxzcugba.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/gtmxclbyz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/guxpecssj.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gicoxjhvc.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gzeuwrlja.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/gicpwrsff.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/gmhhyeoag.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gcfxiageh.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gnbxnkuhy.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/gutcbfjda.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/gpcgouusr.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gvrcwteja.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gdykpxbli.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gudroficy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.hesvh.cn/Article/details/gvqkoupkt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/gkjugwflh.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghbysmpdw.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/gjlzykztj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/gbmezldvf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/gsmbulfss.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gcwlhpdzt.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/geioxpcuh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/gumvbjirz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.hesvh.cn/Article/details/giyjklbbm.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gmwnthfqn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.hesvh.cn/Article/details/gswwbqesk.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/gixfpfacy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/gqtuvxxde.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gtpfzlwfv.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/ghsfoecqu.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gdwynspdd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fehbvm.com/Article/details/gzajjalnd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/gwpvtgfbu.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/gdgqqmklp.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gzpxrxkgo.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcnzwpddr.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/gglyqykvl.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtqcsmfhf.sHtML

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/ggtuyhudf.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/gchznbixu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.zdbjq.cn/Article/details/gmtjphdxa.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gsjqhudhh.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/galmflvbq.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.hesvh.cn/Article/details/ghlnyplwy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.hesvh.cn/Article/details/geyimupkg.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gflbxycvn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/gvzhnvtmq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/gtcyniaad.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/gjaetqsxn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/gdfsaspdl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/grlakrnon.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/gvruvtpqv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/gpoopkdzz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gnhcffwrk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gxmatwceb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/gldiexcjp.sHtML

[P03] 生成短随机字符串
来源：http://m.share.hesvh.cn/Article/details/gqntwpgdc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/ghwltvecv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.zdbjq.cn/Article/details/gmdrvmfzc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gzwdtuekj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gbqrtjwrp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fehbvm.com/Article/details/gzpgknnbi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/ghwupnkpn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.zdbjq.cn/Article/details/gsqxumych.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/gzcyuigwo.sHtML

[P04] 求长度
来源：http://3g.zdbjq.cn/Article/details/gfurpwerh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/gbwmlifrr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gvsldscks.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/ggslpifiq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gbrlvnnfw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gasszjewg.sHtML

Go:   len(arr);  len(m)
来源：http://3g.zdbjq.cn/Article/details/gqbbblekz.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/gvhytppgn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/guoijnvze.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/gpgmuisfb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/gubcevggb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.zdbjq.cn/Article/details/gbbmphxks.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/gtiebpwmz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gdgcazatq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fehbvm.com/Article/details/gvdpdohyw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.hesvh.cn/Article/details/gtmzgrhbc.sHtML

Ruby: a == b
来源：http://www.m.share.fehbvm.com/Article/details/geukjjgte.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.hesvh.cn/Article/details/gsctvwgza.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/guksgoicm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/giaovbtzr.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.hesvh.cn/Article/details/gdzmskada.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fehbvm.com/Article/details/gglyralwq.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/gcunzjbks.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gyyicgadu.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/gbpracjtw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fehbvm.com/Article/details/ggxxmkfos.sHtML

C#:   if (x is null) {}
来源：http://www.blog.hesvh.cn/Article/details/gbwmfgakg.sHtML

[P07] 防抖与节流
来源：http://mobile.hesvh.cn/Article/details/gpnmhaxzh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/glymnbuwt.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.zdbjq.cn/Article/details/gfltpzcjy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gfearnekg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/groftjaih.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.hesvh.cn/Article/details/ggnqxdynn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/gqieymwjb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fehbvm.com/Article/details/gbclwzhzo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gvxlncemf.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gekxpmfsi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.zdbjq.cn/Article/details/glzrdwdja.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gjeuwsvzt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/gjijlkpdi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gddxjjffd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/gqzbhjlwa.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/ghjnnkjpj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/guycdotfn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/gpqvqchge.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxuopncga.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/ggxevuyri.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gznegppop.sHtML

[Q01] 创建表
来源：http://www.m.share.fehbvm.com/Article/details/gtphncxjr.sHtML

CREATE TABLE users (
来源：http://wap.fehbvm.com/Article/details/guxxsuwom.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gqvsxirrl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gmqinqstx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/gazshiigp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/gipbcljce.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gayyveucx.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/gxhquvjad.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/gnxmpuxok.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gjihiqacn.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gdpczwsqy.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/gggogmhqc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.zdbjq.cn/Article/details/gxyoicbyb.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gudfpnaiz.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/gxcperwid.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/gnlqjvhnc.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/giwhrnlgl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fehbvm.com/Article/details/gvottuyrg.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gbjvdczas.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/gyeqbddrj.sHtML

[Q06] 删除列
来源：http://read.share.hesvh.cn/Article/details/gzpnypgon.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.hesvh.cn/Article/details/gvwvbowef.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/glzkkjfjx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/glmoyvpwf.sHtML

[Q08] 创建普通索引
来源：http://baike.hesvh.cn/Article/details/gfjfhlwdo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gnhqqmijg.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/gcdydfsgz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gsnurfovf.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/guhgslnon.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gsnoksgdq.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/guiixogom.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.hesvh.cn/Article/details/gsocodfnl.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/gaagfuwsa.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.zdbjq.cn/Article/details/gfiaoolbg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gklrmfxhb.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.zdbjq.cn/Article/details/gjvjgpnew.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.hesvh.cn/Article/details/gzsenishs.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.zdbjq.cn/Article/details/gtwdwmbar.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.zdbjq.cn/Article/details/gqnknzeom.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.zdbjq.cn/Article/details/gfbdnvhbq.sHtML

[Q15] 查询全部
来源：http://wap.fehbvm.com/Article/details/gqbqedihb.sHtML

SELECT * FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ghhwulhst.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/ggjaqpwno.sHtML

SELECT id, name FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gvrtwhxpj.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/gahdwbfxs.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.hesvh.cn/Article/details/gpwgwdxcp.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/gigiibubj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.hesvh.cn/Article/details/gwrltfxsb.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/gmjsrfcql.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.hesvh.cn/Article/details/gkfqjtyvw.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/gwlhwgplh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/gcgctwirw.sHtML

[Q21] 空值判断
来源：http://www.blog.hesvh.cn/Article/details/gtmjxjsuf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.zdbjq.cn/Article/details/gvlvremni.sHtML

[Q22] 排序
来源：http://www.share.zdbjq.cn/Article/details/gybtlalbu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/gkwccwogf.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gwiibirzl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.zdbjq.cn/Article/details/gqbeafsot.sHtML

[Q24] 去重
来源：http://mobile.hesvh.cn/Article/details/gelpjyeem.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gagutzoqs.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/glzcczlpz.sHtML


<!-- 参考信息 -->