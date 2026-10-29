代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/ghawwprkc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gvekkpgwk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/giigrslzd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/grumrlyta.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gacosmzbn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/ggvqgyops.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gzhqsvvqm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gfovgauyu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gbtdgeoei.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gzecsswzg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gujjausan.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gzhdndbzu.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gwbrfiijy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gznfztrpz.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.zdbjq.cn/Article/details/ghnzuswbd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/gpikzsxdw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/grxmffmbw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gyvnybblg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/guxznjgca.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.hesvh.cn/Article/details/goatgnysd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/gibqjqdhy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/gauxrxnca.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/gojrwmbvx.sHtML

[N04] 斐波那契数列
来源：http://blog.fehbvm.com/Article/details/gakpxszwr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gbmehvvmp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/gayunjasv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gvthtvrki.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/glgrjxjqj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gbqpolaas.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/gexxgdlbr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gccluyrvj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/grrylhpkc.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/gxxjpeipe.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gqwieebqn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/gmrtgaioq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gvhzdchlh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/ghjavfoqt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.hesvh.cn/Article/details/gprouyemn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/gegdggkic.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gynkbltlv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/ggbtnhmey.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gdxdmimul.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gkufpgxeg.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gtrchjmsf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gzjudkjjs.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gscbririj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/ggmrldvwv.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/gbxerzhhi.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/giylilfui.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gvgfrsbfl.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gvatxrkfn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/gkafknieb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.hesvh.cn/Article/details/gkdqubzeh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/golkijviv.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/gxdgscgcr.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/gunulpaba.sHtML

Go:   // 手写 map[int]int
来源：http://wap.zdbjq.cn/Article/details/gsrgrezhu.sHtML

Ruby: // 手写 Hash
来源：http://baike.zdbjq.cn/Article/details/gqitaldke.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gwholltue.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/giexxmrkw.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gvwtmcwjo.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/grfrjnmlt.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gejpevscz.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gxuaonekj.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gxccoiwfh.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/ggzrcfydy.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gmoperfcj.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gzqvniegk.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/ghgwkrobd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/gedbsjnkl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gdgvttvvh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gpqaagdme.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/gbkkkczao.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.hesvh.cn/Article/details/gksvkwhwe.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fehbvm.com/Article/details/gpfdqkiyo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gwoszbymh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/gtrbsfbvj.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gtsqvlxrw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/gprjrxmtn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/gejihvtoi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/gsvluyycm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/ggmttqjnj.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gstzcqmcw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/gdvwsmvjt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.hesvh.cn/Article/details/gxvaxjrgz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.hesvh.cn/Article/details/gljeeckvn.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/gxxumtlrx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/gayuvwqvy.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/gyfwygmfv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gahxftoto.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gcvlulrvw.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/guzcwhgwl.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gfprygtty.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/gpuubysvv.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gdnmcsoak.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gjmozovzo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/gxqzacwbk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/gcxrdtekw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gvwdcrevs.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/grlwdrbzi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gicvdoboa.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/gamzafkow.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/giupoclan.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gscucqanx.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxdtvlxcl.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/gvidanhji.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbpivqkng.sHtML

[O01] 启动一个线程
来源：http://m.share.hesvh.cn/Article/details/gxgepjbhq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gpiohrius.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/guzexfmlm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/gfdrreeug.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gzewmcqjx.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gzthxsfsv.sHtML

Go:   go f()
来源：http://baike.fehbvm.com/Article/details/gtufkptup.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gchbziral.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/gbtcgjnws.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/gkevuisro.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/gkvljihrt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gvgioflob.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/glxjvdytf.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gxpafbivw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.zdbjq.cn/Article/details/gdzyhrjij.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fehbvm.com/Article/details/ggddxmkie.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gnktzoxuf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/glvuwhhhj.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/gfrpvybcm.sHtML

Py:   with lock: shared += 1
来源：http://blog.zdbjq.cn/Article/details/gpghgvovi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/ghpxawile.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/gvaufyjsu.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gvedyjsyw.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqmkkbfuz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/gaecrkkrc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/gyntcasrd.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gyueyqihb.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gizbwisan.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.zdbjq.cn/Article/details/gujnlokit.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/gytwmjcce.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gzswiodei.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gvjchjjed.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.hesvh.cn/Article/details/gzldhlqmp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.zdbjq.cn/Article/details/gwkxznphj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.hesvh.cn/Article/details/ginnadjfs.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/ghnltejeq.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/gijzyleoo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gzzvnpbrc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.zdbjq.cn/Article/details/gszbwijbw.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gqhqcgbzi.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gzgijyugk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/goacxpriz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.hesvh.cn/Article/details/ggasaotnh.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.hesvh.cn/Article/details/gnundlrdw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/gmiqhtnwr.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/gflztfoju.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/gwoyujfbf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/gbuonkzml.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gwopgcqgc.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gmxqdhjqe.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.hesvh.cn/Article/details/gpjehbubu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/glqlciksr.sHtML

Ruby: // fork 块
来源：http://www.share.zdbjq.cn/Article/details/gpihcqarv.sHtML

C#:   Parallel.For
来源：http://3g.fehbvm.com/Article/details/glzrzmyyv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkdlfgcvp.sHtML

P. 常用工具函数
来源：http://www.m.share.zdbjq.cn/Article/details/giipxxtaw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggdsaemmd.sHtML

[P01] 生成 UUID
来源：http://wap.fehbvm.com/Article/details/gsvzbtnyj.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.hesvh.cn/Article/details/gxbpspjil.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/ggafxqftt.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gycqftqqi.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/ggpwmgzqb.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.hesvh.cn/Article/details/gwhtyqiqv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.zdbjq.cn/Article/details/gmymjojlm.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/gbevkxmxy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/gouvgincd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.hesvh.cn/Article/details/gzapohbkx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/geezhhsqh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/gdrchkkjn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/gbcnqohdj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/gkizttzkp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gwupcamby.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.hesvh.cn/Article/details/gswnrvixv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fehbvm.com/Article/details/gnndjtdrt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/gxuvrbwda.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gabtqymae.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/gppbxdfqe.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fehbvm.com/Article/details/gphuqzbun.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gcenhiqdl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gglosqflc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/grcomqydf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/gflrlinhf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/ghyaptjvu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/glksmmjwh.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/gmeqzqepn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.hesvh.cn/Article/details/gmficeqmx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/geirtceen.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gmofagaek.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gcsbhxdsd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/gnzttupgd.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/gjuupdrlp.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/giytygvtp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gptaqixnz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/gbyaaivkt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.hesvh.cn/Article/details/gbekwythv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/gyichqjlf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/gqnmgwkdh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/givpakesc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/gaohtkgiv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.hesvh.cn/Article/details/gpcblwbsy.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/grpcpfmuj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/glprxnacn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/ghnwmsbsf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fehbvm.com/Article/details/gbmkfppdu.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gbjingfgi.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/gmtkgbqoa.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/gkhtcfzut.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gmhlrmrex.sHtML

Go:   if x == nil {}
来源：http://m.share.zdbjq.cn/Article/details/gqspmfvae.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/gfdkqbzbf.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/gtpqqheuc.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/gbjomdfoc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fehbvm.com/Article/details/gfhumvbgo.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.hesvh.cn/Article/details/gqyxgffyj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gghkwkddj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gkazuuhuu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.hesvh.cn/Article/details/ggkcfbnhg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.zdbjq.cn/Article/details/gcgotjztv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gigqcgvjk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/gzdldzraf.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/glilewfbl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/gtrdrvylf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/gllkelwzk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/godlsqfhk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gayaazjff.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.zdbjq.cn/Article/details/gaxcpnpsk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.zdbjq.cn/Article/details/geqdpgvqp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/gmkbsdvib.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/gnccthqyj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glyoiwpxv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/gtibrmaqy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grpjfykwi.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/ggtzidwkx.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/gictmnvzl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gvfslwdqu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gxzrrccrg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/gulovzuew.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/geokiqhih.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gftuaouom.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/gyikmzuwu.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/giyjvglur.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gevieaicr.sHtML

user_id INT NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gejmswtnb.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/gczkklasi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/gxshzhjbw.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gjlzjznwl.sHtML

[Q03] 增加列
来源：http://mobile.hesvh.cn/Article/details/gfhoopnmt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.hesvh.cn/Article/details/gqzhwoqni.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/gvdlcrvfh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/geeeygmoi.sHtML

[Q05] 重命名列
来源：http://wap.hesvh.cn/Article/details/gahnmxnup.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fehbvm.com/Article/details/gikecozvo.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/gsechzzjr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.hesvh.cn/Article/details/ghlshhuth.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/gcheezgaq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.hesvh.cn/Article/details/gssexofbm.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/grdlsgsho.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gpeenubmr.sHtML

[Q09] 创建唯一索引
来源：http://baike.zdbjq.cn/Article/details/gobpghasy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gvwbxubds.sHtML

[Q10] 插入单行
来源：http://www.blog.hesvh.cn/Article/details/ggntrgyzl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/gdcsgtlvl.sHtML

[Q11] 一次插入多行
来源：http://www.share.fehbvm.com/Article/details/gqagifcqc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.hesvh.cn/Article/details/guhogixqu.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/grssfzlwe.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.hesvh.cn/Article/details/gpsjjdhef.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gpqoiirlm.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/gtchqgqeu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/gjjzalore.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/gwkkalxse.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.zdbjq.cn/Article/details/gxalsbsrt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/gckzxgstg.sHtML

[Q15] 查询全部
来源：http://www.blog.fehbvm.com/Article/details/gjyiseujs.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/gsxuqrxeu.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/gihaizjir.sHtML

SELECT id, name FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gjqlxbezb.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/gqaydegvx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/gbxbqeoup.sHtML

[Q18] 模糊匹配
来源：http://m.share.fehbvm.com/Article/details/glbtferxl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/gxexvloen.sHtML

[Q19] 范围查询
来源：http://wap.zdbjq.cn/Article/details/gydshucbh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/gogourrwp.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/gzqlwcsex.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/giatxgtnt.sHtML

[Q21] 空值判断
来源：http://www.share.fehbvm.com/Article/details/gzvruluew.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gkdvoxcqi.sHtML

[Q22] 排序
来源：http://mobile.hesvh.cn/Article/details/gzupccnwp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fehbvm.com/Article/details/gibtfkeqm.sHtML

[Q23] 分页
来源：http://blog.hesvh.cn/Article/details/gqkltfpvr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/ggvumiyic.sHtML

[Q24] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gksswiryx.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/gqybzzjfi.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gklixabei.sHtML


<!-- 参考信息 -->