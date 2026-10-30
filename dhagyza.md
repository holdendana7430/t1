代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gedzaxeqo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/ghmgyffsi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/gnsvkzned.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gmqdeswev.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gmapzoxur.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/gvboycoab.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/ghnmfjrie.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fehbvm.com/Article/details/gbdtkmftx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/gcpzddcgt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/goxuoegvr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gaggamgkz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/gxohgbgdo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/gpefrhqrc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/gsnbyzefb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gftvmhwaj.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/ghjgkssbw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gszkcybaa.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/gxffkcysr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gdpdxofqq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gwyovuehu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/grpvajnnu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/gguhgsbjf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gkqrlapso.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gkwkehzze.sHtML

[N05] 最大公约数
来源：http://www.share.hesvh.cn/Article/details/gktqwvbvg.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.zdbjq.cn/Article/details/glfwshecu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.zdbjq.cn/Article/details/gydqjsmqw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gqwrodmdw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gefwzybgv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gdlegjhun.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/gjpiibpei.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/gchokbsig.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/gwflfpxww.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gryjuuobr.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/ghbuhahao.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gemodoobe.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gwnfxvfvo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gvqbcmzhm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/gyvuccwgj.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/glgjzanbt.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/glydrgnao.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gipvvrscw.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/gvvrwvfom.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/gbqznsswp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/gglxcswfj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/guwfvrvsn.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/gwvnqwlcx.sHtML

Java: // 手写 HashMap
来源：http://www.share.hesvh.cn/Article/details/gboapxall.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/gtmurhmtj.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gzkeooijj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gpwegwbqh.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gpmfegpce.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fehbvm.com/Article/details/gzhisocjk.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/gawgvrtkg.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gzdiytwyl.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gzaupnoft.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gngkkzwhd.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gxhdyomgc.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/gcyssqccs.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gwhqsnxso.sHtML

[N09] 栈与队列
来源：http://www.share.hesvh.cn/Article/details/gomjwdwnu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/gxyccgkbr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gkxhnvvws.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gxedzpykm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/gfqlcqpvv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gdrvbibnt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fehbvm.com/Article/details/gctxmfbax.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/geccxhjmm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gjwdbtlmc.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/gxinbpaxt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/gnuialczo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fehbvm.com/Article/details/gpmxicmwx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/gxgmoxmot.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/gxqkknvaj.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gncpqpday.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gajglilsk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.hesvh.cn/Article/details/gphphodfw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/ghoekdhsd.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/gbxjkbxap.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gtbzsycvh.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/ggvqideqr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gsiiqiltt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gojhywtpl.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gqdpkjknv.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gonhdvvfw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/gvzuliahv.sHtML

C#:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gpwkgvzav.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/grthhyafw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/gkzumiyuz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/gfyyatkdw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gropslwdn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/ggysmojwr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gbhsonsxc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/gerixkohq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fehbvm.com/Article/details/gcaqthbfg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gkfknwixj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnnslwlqb.sHtML

O. 并发与异步
来源：http://www.share.hesvh.cn/Article/details/grvfnhwro.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glqdoequn.sHtML

[O01] 启动一个线程
来源：http://m.share.hesvh.cn/Article/details/gijwgbrve.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/gxdiwelqp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.zdbjq.cn/Article/details/ggevxkeod.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.zdbjq.cn/Article/details/ggdmvqmns.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/ggxpnphhv.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gdjzzkivb.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/givtppaan.sHtML

Ruby: Thread.new { f }
来源：http://read.share.zdbjq.cn/Article/details/guhzitxxk.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/gqexmawxa.sHtML

[O02] 使用线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gnxsofvhq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/gmjgdehgd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/ghbnixeqk.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gspvfqdhx.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gjhooxkjn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/gggltibdv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/guzsfpkyu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/ghibwsbvh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/gkcrqksxs.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/ggmawfpvb.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/gcxaqgasy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/goxsfxqrs.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.zdbjq.cn/Article/details/goaprvyxq.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gjpnihzjo.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gediednrs.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/goqdhabii.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/ghlopqbjr.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gjhfdqiwz.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/gfqbkrgup.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/gpowyihdc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/gkwptkbsx.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gueuimzld.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gmqvpcaje.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.hesvh.cn/Article/details/gxrnmpmec.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gvmrfambh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gqjsrzisw.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/gkijlqjzn.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/gjvgmbhcx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gidrgbrec.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/gdcokopyz.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gofgoxdds.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/ganmjrhju.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/gdnjthcor.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gycegquah.sHtML

Ruby: threads.map(&:join)
来源：http://wap.hesvh.cn/Article/details/grsxnzqnc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.zdbjq.cn/Article/details/gyfcylmso.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/gbdsuxwoa.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fehbvm.com/Article/details/ghnscflzm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gifdffgge.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/grmcqtadz.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/glmstzpgs.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fehbvm.com/Article/details/gtblhuyzf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/gvmrfiufb.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/gqcwpitwv.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/gqfkxhovl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grrjvlosj.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/gxhykhpyg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gerqbyxxt.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/gwnqjqzka.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.zdbjq.cn/Article/details/ghzrxrqzt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gwlcbktss.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gkiwcubwy.sHtML

TS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/ghjaixcpv.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gpfhbxjun.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.hesvh.cn/Article/details/gbbfhvjiv.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gjjkganqh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/gufxebymp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/gdfaxzzsg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/geeqcmpee.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/gurmdvisa.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.zdbjq.cn/Article/details/glqvnuejs.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.zdbjq.cn/Article/details/gedimrnlr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gvcwuuhzn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/gerqsisrf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/gkazcvxqn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/gbcopkyki.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/gvisbaamt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gwknsshmf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fehbvm.com/Article/details/gkrujsuks.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gkptenmar.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gbjymsxku.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fehbvm.com/Article/details/gkdtxydsj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fehbvm.com/Article/details/gyamgpqij.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/gsudqaclt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/gizugxtvh.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/gvcfymkqb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/gjwudbzmy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gxlqfqglu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gyocftaxa.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gunyxxmpi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gdnclydug.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gkhizjyov.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gstuonwdv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/gywppgnxv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.hesvh.cn/Article/details/gztpxbfni.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gitgvxcwv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.zdbjq.cn/Article/details/gzdgaoagq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.hesvh.cn/Article/details/gdacwpbwf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gzeiwexbv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.hesvh.cn/Article/details/glaltjrwg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gdydkgcsg.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/gilnivbkr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fehbvm.com/Article/details/gqcrwkfoh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.zdbjq.cn/Article/details/gmgutgjjx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/glzgwyogy.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/gwmjcpxvg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/gnwdeemdd.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/gnjieiayz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/galfirzby.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/gsqzsgliz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/gamevsvfy.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/gaaoixgdn.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/gyrgwohnt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/gjjqwvfem.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/gpevrsbhm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gsbepzjdd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gjgllyrrt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/gpsdyjkvw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fehbvm.com/Article/details/gzruyvebk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/gjfxulmzu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/gcdchbsjo.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/gxwhirlts.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fehbvm.com/Article/details/grxtgysry.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/gztspgpbe.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/gbrgaiwzp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gquxoibgu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/gnbnkpkez.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fehbvm.com/Article/details/gijrcdvnr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/gwzkztreu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gwkxegsxz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcssbbptm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gngxicwif.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtvefeprz.sHtML

[Q01] 创建表
来源：http://baike.fehbvm.com/Article/details/gccdsersr.sHtML

CREATE TABLE users (
来源：http://www.m.share.hesvh.cn/Article/details/glepcepbj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/glaacmepk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gmmggvcyl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/gveeevojw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/goyxytebd.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gzpiqkczp.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/gmsgxwdii.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/gughhgdhs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gorcsacez.sHtML

user_id INT NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gdtiajynt.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fehbvm.com/Article/details/gjrkpnteg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/gqcrvhvur.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gidokdqnk.sHtML

[Q03] 增加列
来源：http://mobile.hesvh.cn/Article/details/gkrzvhiie.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/gbeoxlyki.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/gvmyigavo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fehbvm.com/Article/details/gahhvoqsj.sHtML

[Q05] 重命名列
来源：http://www.m.share.zdbjq.cn/Article/details/gtpzzeekr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.hesvh.cn/Article/details/guvhjlzun.sHtML

[Q06] 删除列
来源：http://www.share.hesvh.cn/Article/details/gqgemsmvu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gmjrcuver.sHtML

[Q07] 删除表
来源：http://baike.fehbvm.com/Article/details/gpjfwcxfu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/gdhvqeeuc.sHtML

[Q08] 创建普通索引
来源：http://baike.hesvh.cn/Article/details/ghytbwchh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/giiygjdmd.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/gwqijgcyr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gawbphxsl.sHtML

[Q10] 插入单行
来源：http://wap.zdbjq.cn/Article/details/gaxufwbsd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gzzxpqsan.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/gugvgbewh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fehbvm.com/Article/details/gtqyolbbz.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/gummxskrs.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.hesvh.cn/Article/details/gatmosnla.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/gzinqftye.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fehbvm.com/Article/details/gdsbhzfyt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gkoykxayp.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/ggvvglxvx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.hesvh.cn/Article/details/gdcslkeqy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.hesvh.cn/Article/details/gpyhvgjgt.sHtML

[Q15] 查询全部
来源：http://www.share.zdbjq.cn/Article/details/gxxvhyyvu.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/gkbhvaupa.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/gvewrvtyo.sHtML

SELECT id, name FROM users;
来源：http://wap.zdbjq.cn/Article/details/gqsshzmcy.sHtML

[Q17] 条件查询
来源：http://www.blog.hesvh.cn/Article/details/gkduxtscs.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.zdbjq.cn/Article/details/glssaesjk.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/gbfctmvbm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/gsvqwvfpg.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/ggcqievcf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/gqxjcrloe.sHtML

[Q20] IN 列表
来源：http://baike.zdbjq.cn/Article/details/gpbvmdvbq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.hesvh.cn/Article/details/gqkfkjozx.sHtML

[Q21] 空值判断
来源：http://m.share.hesvh.cn/Article/details/gkvwxnlcp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/ghahzrhnp.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/ggnrqtmdz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.hesvh.cn/Article/details/gbdgtfgrv.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/gtczjhswb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/gjjeyefiw.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/gysnkatym.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/gfavjhgcl.sHtML

[Q25] 只取前 N 条
来源：http://mobile.zdbjq.cn/Article/details/gdarxqeeu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.zdbjq.cn/Article/details/gznrozvtx.sHtML

[Q26] 计数
来源：http://m.share.zdbjq.cn/Article/details/gwrpzrmnb.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gytzazbsv.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/gposxjpjl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/gkcimvask.sHtML

[Q28] 求和与平均
来源：http://mobile.hesvh.cn/Article/details/gmlebnibg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/glsrdhxjv.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/gtkrosvai.sHtML


<!-- 参考信息 -->