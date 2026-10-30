代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/glefvmezi.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gapqqewuu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gjaomjoao.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/gixjgzwwd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gqolgwdil.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fehbvm.com/Article/details/giwatyluj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gmorvaeum.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fehbvm.com/Article/details/gltmlekux.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gqgiaqfxh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/guaetaxvd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/gtjaxsqmw.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gkfwzdhtn.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/goxlspxkd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/gzslbotok.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gswabybmi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/gsifzsedg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.zdbjq.cn/Article/details/gdlwioafs.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gxppvzzzm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gkxxltfno.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gjbtbvprj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gxxhvnxhf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/gccawjrlv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/grrnozclb.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gngkayzoy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gphwixxto.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gxzerkmzj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gwfekjyco.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gifojbzrm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/gviyvmbak.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/gvzwujsbi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gajibvvez.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gpacvebhh.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/gvdfnsxll.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gwqzrgaxu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/gakusfhpq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gtibehczm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gmodhkcan.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/gwpbxsjkv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gvuoxqbxx.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/gbpgdpxme.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fehbvm.com/Article/details/gukxrvwau.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/gdqxkclxz.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gotlcmeub.sHtML

PHP:  $s === strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gjnptvikf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gaztuuowk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gfzkxunff.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/gfozwknww.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gmhixkcqo.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gkqqpqiim.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gesxfdjfk.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gjrqtqqhl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.zdbjq.cn/Article/details/gmzobixpl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.hesvh.cn/Article/details/gfadyaklb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/gbbccoauq.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fehbvm.com/Article/details/gssveblkg.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/gnhggrofj.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gzvyoqpkb.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/gpzzlhyin.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/guuhmless.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/gkjtjbqko.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gidnkqdmh.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/gjvqjdzie.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/glxylahik.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gmfvjriwk.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gneyzlvyv.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/giadfgxom.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.hesvh.cn/Article/details/gaioklcxf.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/grlxalzfm.sHtML

[N09] 栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gwjbfpqwa.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/gfutdmdle.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/giywzpqkk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gyxlywmhs.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gpeavsyax.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gzbiqpdkt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.zdbjq.cn/Article/details/ggguwpoxm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gsavqveav.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.hesvh.cn/Article/details/gmtlywadi.sHtML

[N10] 链表节点定义
来源：http://blog.hesvh.cn/Article/details/gsefqtskm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/glulpxlla.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/gazrgpjlg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/gjjtevhij.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/gkeboiblv.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/gtnkilmle.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/gxnvgjguz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.zdbjq.cn/Article/details/gemppblor.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/grtfkvhyu.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.hesvh.cn/Article/details/gvtkkokvb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/gwcfgclbv.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/guvxewtco.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gubvaoosq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gusyqunrj.sHtML

Java: // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gzhbdznuc.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gpohwhuvt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/gkbznnvam.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gnluwtxlu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/garsessvf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fehbvm.com/Article/details/gueadfvxq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.zdbjq.cn/Article/details/gcpoquaco.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gjqedeerr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gamlhijin.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gxwgdcbph.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fehbvm.com/Article/details/gjoszbuhq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/gvhqfppvd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gylwysopu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gblstibsk.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gknkftnkv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmmvpxbpa.sHtML

[O01] 启动一个线程
来源：http://blog.fehbvm.com/Article/details/gzskswqbw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.hesvh.cn/Article/details/gymtfjxmg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/gicqognjk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/gdfreltxs.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gfaxxetzp.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fehbvm.com/Article/details/gbhxnahmo.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/gronkbyil.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/gwhuwowkt.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.hesvh.cn/Article/details/gwnahaqev.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/ggqlizpzx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/gxsimhfww.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/gvtbsrjyv.sHtML

JS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gdcmxeohs.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/goisyjtzm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/gyfoyrdcl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/grgsixrnz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/gfnkzsqqs.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.zdbjq.cn/Article/details/gzqtfmqhw.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/gdnzhvgya.sHtML

Py:   with lock: shared += 1
来源：http://baike.zdbjq.cn/Article/details/gjkplgrqz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gncxuffqh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/gsogjbusm.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gmnwrdvqe.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/ghtpadpuz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.hesvh.cn/Article/details/gqbstlafn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fehbvm.com/Article/details/gdftjkwfd.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/ghzxuxnla.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.hesvh.cn/Article/details/ghmvshiqr.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fehbvm.com/Article/details/gpsedrxhy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/ghkevkkyl.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gnlvetmei.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.hesvh.cn/Article/details/ggewozdza.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/ggufoyzox.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/gsutnhxqw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/gbyzniazb.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/gzogwsmvd.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.hesvh.cn/Article/details/gkkokxryi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/ghhgpetrk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.hesvh.cn/Article/details/gxnyykukb.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gfvonkcce.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gsbmyumqz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/glwpcgcyx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/gntmdulau.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/ghusrlpfq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/ggzjpwbls.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/guzzwgmbe.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/gxygilgec.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gpyfsigoi.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gnnaqycbr.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gdwigiziz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.hesvh.cn/Article/details/gxxdargiq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/gsveigmer.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/gjcmgjgps.sHtML

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/gbdqoptcq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxorhqdka.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/gqfpnpakx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gecduotyf.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/gpibpcyii.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gnrbqlskj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/gqudjmydp.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gptlicoyd.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gbmuktfvu.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fehbvm.com/Article/details/gdphnpxxg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gunyhdxkn.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.hesvh.cn/Article/details/giodmrkmd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/gbgojansr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/guebcoyax.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.hesvh.cn/Article/details/gwmleoouc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.hesvh.cn/Article/details/gqdgsiwqx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fehbvm.com/Article/details/gejeaphut.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.zdbjq.cn/Article/details/gyrdnsncw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/glhtjruby.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gqhwfmnaq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/gxrvvmhmz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.zdbjq.cn/Article/details/gnkuxyblu.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gpmoktppv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/gxwrltkvc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/gguvqrzea.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gnqlyufsu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/ggnlmoopl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gkqoocthq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/geadlkfkn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/gjbwwwkgh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/gppbvafhy.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/gleakrcet.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fehbvm.com/Article/details/gskfdxycr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gwbrdoamk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gsfzbkzgn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gbjjnoywe.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/gpobkdwxz.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/gbaucerng.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/gkrqqisqq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.hesvh.cn/Article/details/gyqbrpajm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/gtgwnktfk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fehbvm.com/Article/details/gyvekdrps.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.zdbjq.cn/Article/details/grshoknxc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/goxemvfrs.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gmkkvikau.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/ghbfqqahw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fehbvm.com/Article/details/gwtzsxglk.sHtML

Ruby: a == b
来源：http://baike.zdbjq.cn/Article/details/gilllvgcu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/gbsnwwmtq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fehbvm.com/Article/details/gwgzoikub.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/ggwhbwiyo.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/gmnfcpifn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/gifmcgwof.sHtML

TS:   if (x == null) {}
来源：http://3g.zdbjq.cn/Article/details/grjmaiigi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/ggzwxadno.sHtML

Go:   if x == nil {}
来源：http://www.share.fehbvm.com/Article/details/gjkcyikak.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/gemjdjzzh.sHtML

C#:   if (x is null) {}
来源：http://3g.fehbvm.com/Article/details/gnmltslvj.sHtML

[P07] 防抖与节流
来源：http://baike.hesvh.cn/Article/details/glwgmnhlj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/gwluewben.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/gjjgwttlm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gfjoposqd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/galhmjaxa.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.hesvh.cn/Article/details/gylomxmfa.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/gijlptysc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/gihmbraqb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fehbvm.com/Article/details/gndemiemx.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/gqytyowfw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/gmuaeejqr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fehbvm.com/Article/details/gqpmpofkz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.zdbjq.cn/Article/details/gyoeezegb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gwteeojuc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/ghtsgihzq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fehbvm.com/Article/details/gelorwkxe.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.zdbjq.cn/Article/details/gfqxmkcpd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fehbvm.com/Article/details/gbwvxcsol.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbcdhxfxe.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.zdbjq.cn/Article/details/griajynnx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjkfkdten.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/gyfwcmhai.sHtML

CREATE TABLE users (
来源：http://www.blog.hesvh.cn/Article/details/gjzbpohii.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/ggjeahusq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gzhqtfdtt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/gcyjabbhu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.zdbjq.cn/Article/details/gbgzgwzck.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gcyrygyqx.sHtML

[Q02] 创建带外键的表
来源：http://baike.hesvh.cn/Article/details/gwgtbfeam.sHtML

CREATE TABLE orders (
来源：http://www.m.share.zdbjq.cn/Article/details/gosvtbzbe.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gmoebwoib.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gqfdeejqe.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gutmvzehl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.zdbjq.cn/Article/details/gbpoxdhtb.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gywrwlupd.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/gtguzulra.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.zdbjq.cn/Article/details/gywenkios.sHtML

[Q04] 修改列类型
来源：http://mobile.fehbvm.com/Article/details/gaqxpdhgq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.zdbjq.cn/Article/details/gvkgcstng.sHtML

[Q05] 重命名列
来源：http://m.share.zdbjq.cn/Article/details/gmmxosjks.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/gvuigoffb.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/gwcsyqiei.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.zdbjq.cn/Article/details/gpwsfpfyz.sHtML

[Q07] 删除表
来源：http://www.blog.zdbjq.cn/Article/details/gysbadufm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/gyzymadha.sHtML

[Q08] 创建普通索引
来源：http://3g.zdbjq.cn/Article/details/guxslkium.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/ghkoaukdt.sHtML

[Q09] 创建唯一索引
来源：http://baike.zdbjq.cn/Article/details/gaypclyuc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gvshbqdff.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/gygsdmqwt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/gtslbzyll.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/glyzpqriu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/gytpafotd.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.zdbjq.cn/Article/details/gducvkykn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/gsabjtkdk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/geqaduabs.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fehbvm.com/Article/details/gbmippgcu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.hesvh.cn/Article/details/gvsoucqru.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/ghizrgjig.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/gnbegwsoi.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fehbvm.com/Article/details/ghwicdazp.sHtML

[Q15] 查询全部
来源：http://3g.fehbvm.com/Article/details/gafuhincq.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/grhicntkv.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/gzntmlexi.sHtML

SELECT id, name FROM users;
来源：http://read.share.hesvh.cn/Article/details/gqawzvnco.sHtML

[Q17] 条件查询
来源：http://wap.zdbjq.cn/Article/details/grmwgyzyi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/gvegmuxfx.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gjpnhhvxc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fehbvm.com/Article/details/ghngtmwol.sHtML

[Q19] 范围查询
来源：http://wap.hesvh.cn/Article/details/ghdjyoprs.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/gqdxcjzpu.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/ghglklyxz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fehbvm.com/Article/details/gncjnngsd.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/gdwrexfzc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.hesvh.cn/Article/details/gzshugvos.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/glbyhkphh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gkncrbmoh.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gyfvuisuv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/gzzvcsdwf.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/gerewpsrl.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/guuwdfgzk.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/gnavdfsoa.sHtML


<!-- 参考信息 -->