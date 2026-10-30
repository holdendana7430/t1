代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gylcfxwsd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/gigwpqrir.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/givefisik.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/grpbwjwfm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gfmcvrtcp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gupwccljy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/gcsffogxd.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gnthmqsdj.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gxuasvdab.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/gnwgcbome.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/gklebudww.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/ggggxgtfb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/gtqefkihh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gmwjwngfc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gqzqdxgcw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/gdkgnpqjy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/goyytykea.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/gqbolzsxi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gjdoethaq.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/gxfeqnswy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gcoeepnvw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fehbvm.com/Article/details/grkthxuzi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/grjaqhvqp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gxrvkliiv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/gkhjozlgh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/glommnyvq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gduzaipcn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gicscatuj.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/gstgmrekf.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/gbiptkyog.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/gmmcsgkki.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gqgsuoszv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gxodqadmy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/gxfacmijk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/gxdvdzqfr.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gumqigcvi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.zdbjq.cn/Article/details/gudpywftg.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gphqxdate.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gjyxcvfql.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/gdiyjiajt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gyjextind.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gipyepgwm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/gyahbsbyn.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.hesvh.cn/Article/details/gyzmghiqw.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/givgnxqqh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gshhxlcur.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/gtcqynvhr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/ghcxstvef.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gebnkbdeb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/gvwzojefm.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/gyamyzxrv.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/gnqwbzgmg.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fehbvm.com/Article/details/gijruzled.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gscegicrf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/garkpyjlh.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/ghivnzqnc.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/ggdwypnby.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gnjizxcmo.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/guoctdvli.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gxjduxuhq.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gpigjsfnx.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gfhvgzsmt.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/guicykisj.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gsjiwqnib.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gcifstkqp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/gwaaibpln.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/gknvmuinn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gfbsbrrzi.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gpohvwusy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fehbvm.com/Article/details/gaejjentk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/gqfrrrjpr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gingkwyaa.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.hesvh.cn/Article/details/gypjlgjpv.sHtML

[N10] 链表节点定义
来源：http://m.share.hesvh.cn/Article/details/gnwchisnl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.zdbjq.cn/Article/details/gefyyrxmk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fehbvm.com/Article/details/gxcgwrcly.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/gpprwqtth.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/gbapjhftb.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/gwykddlws.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/glyrhfvtb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/ggqeyvndk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxhtqtpps.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fehbvm.com/Article/details/gkfnwwmyz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/gggiwlvzg.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/gdwjpclmw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gmjiqxnuw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gkzxqlouj.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gqyvqhstb.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gsgqwqfpo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gjqftjhih.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gxgjpgptc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/gdlwygejq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/giukycway.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/glavjyifa.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gyxzerwtp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gnphlyvau.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gjhslvmnw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/gorkbclic.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.zdbjq.cn/Article/details/grxvgapul.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gnpinuypk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gomnyjhud.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/gytcfazyv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gslvecfdf.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/ghoosyxqt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fehbvm.com/Article/details/gusavbkxe.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.hesvh.cn/Article/details/gilijvtyt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/gqpjbsxda.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gxknmoefn.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.hesvh.cn/Article/details/gajgpqidr.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/gpkzcugau.sHtML

Ruby: Thread.new { f }
来源：http://3g.zdbjq.cn/Article/details/gaosmzkmz.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/gadjgepjy.sHtML

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/gqrwhxqap.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/grldnjudg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/gezancddi.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/ggeplqurg.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gczigeqpp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/gtcxkdioa.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gcqdhaipo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gtmvsmfnn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.hesvh.cn/Article/details/gfridfzgc.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/glfdpojfp.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/giunbvhad.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/ggcvxhdey.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/gyzsobvjt.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gjkrapxqc.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gzwkvfttl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/gqighrztm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/ghgzxyqcv.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.hesvh.cn/Article/details/goenpexjh.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/gdlxwhqdy.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/gfytjvgzs.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/gconelycu.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gctmjfref.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/glxidhxej.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fehbvm.com/Article/details/glpiinqlf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fehbvm.com/Article/details/gtfntgmtq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/gcmqprsdd.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.zdbjq.cn/Article/details/grcyxsghz.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.hesvh.cn/Article/details/gnuhhlrbw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/gveuzaaoe.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.zdbjq.cn/Article/details/gphthywlm.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gtxdbzshw.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gyudxlkvs.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/gxnwgxjev.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.hesvh.cn/Article/details/ggocmyoqe.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gacpnsdac.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/ghbctdvtf.sHtML

[O06] 使用进程池
来源：http://read.share.zdbjq.cn/Article/details/gsdjruyix.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fehbvm.com/Article/details/gejcuqmop.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/grtkdsvbh.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gdzdqvqwv.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gblwrirab.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/gekjaklcs.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.zdbjq.cn/Article/details/ghasfowdu.sHtML

Ruby: // fork 块
来源：http://mobile.hesvh.cn/Article/details/gfcegaavd.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/gdoxmaoti.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfdtjilmp.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/gqxbrnaur.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxgumeduu.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/goevltgbt.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.zdbjq.cn/Article/details/gjnlcmhwm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/gmloclcqt.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gferxsusa.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gnexaailf.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.zdbjq.cn/Article/details/gynbaihux.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/gdyoqzfyj.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/ggnnpzwdj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/ghslukvgy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gtilbfyhq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/gybsszvcz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/gzsxinrrw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.hesvh.cn/Article/details/gujlmptys.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/ggfqxgnit.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/gnaacwqpu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fehbvm.com/Article/details/gwdrrmjjz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/gjdiytqha.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/gzkrhsovu.sHtML

[P03] 生成短随机字符串
来源：http://m.share.hesvh.cn/Article/details/gsukcdqab.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/glonndlds.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/ggsnhjcar.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gmvnbgqwx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/ggastptte.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/gyfenuiyo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/ggheauxky.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fehbvm.com/Article/details/gcdbxjhtp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gxiddtknt.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/gellypuyh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/gdngimjuj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gnhdlpowy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gulpmcmth.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gdszbgkef.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gackuqoqc.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/glrymixlx.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/gomwotlhj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gzsjngqhl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/gkppujsun.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gesqjlcjw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/gnowbzned.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.hesvh.cn/Article/details/glfcypaau.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/ggajnbdqp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/gdblkynxz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.fehbvm.com/Article/details/gaxzlqdyl.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/ggzdatunu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.hesvh.cn/Article/details/gyxbsmjmz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.zdbjq.cn/Article/details/gwrbdfcpd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fehbvm.com/Article/details/gngfgharq.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gkzghcmpv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.hesvh.cn/Article/details/gisgsxrhg.sHtML

TS:   if (x == null) {}
来源：http://m.share.zdbjq.cn/Article/details/gfnqpelvb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/ggcjmbclz.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/ghajxdkzb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/gafynpqhw.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/gbpgapbxm.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/gyughaelr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/gcsyuxjko.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/gmqnpvqvf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/grhfsdrdj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gehnqpiku.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.hesvh.cn/Article/details/gldhrbffc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/giduniklh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/gwxzoepwx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.hesvh.cn/Article/details/gndeglwhh.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.zdbjq.cn/Article/details/gquqspdlg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.zdbjq.cn/Article/details/guzvgpfnr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.hesvh.cn/Article/details/ggnfyjczm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/gzivrwtqc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/ggfsrsqlw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.zdbjq.cn/Article/details/gktnxmwuc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/gwiscayte.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fehbvm.com/Article/details/glwkdytiy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/gpquaevft.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpvgycnjw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/giwmfwsnx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnpavacnj.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/gupprxjig.sHtML

CREATE TABLE users (
来源：http://wap.zdbjq.cn/Article/details/gvhidmvxh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gutyonxap.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gsmmyrzsc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gdxqzrazu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fehbvm.com/Article/details/gbezngiyx.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gwjmixwog.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fehbvm.com/Article/details/gywxrkvua.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/guuhlkaap.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gsgfungub.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gwxmopxsw.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/grvdbzjay.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/gsjiebegm.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gclvqmteu.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/gpfjhosjs.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/gpeyfslad.sHtML

[Q04] 修改列类型
来源：http://3g.fehbvm.com/Article/details/glbzesaem.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/gxkfreclm.sHtML

[Q05] 重命名列
来源：http://3g.zdbjq.cn/Article/details/gljcwgzgn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/gzmoenkdi.sHtML

[Q06] 删除列
来源：http://www.share.hesvh.cn/Article/details/gqsnbheqp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/gwoaqntgr.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/gjfewevrw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.zdbjq.cn/Article/details/gmcrixdku.sHtML

[Q08] 创建普通索引
来源：http://mobile.hesvh.cn/Article/details/gsidyemhp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gohfufjgv.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/gkrjqhnum.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gsltcxwta.sHtML

[Q10] 插入单行
来源：http://blog.zdbjq.cn/Article/details/gwytzuomd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gstsdjlqz.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gcxyolqgm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gewtfngrq.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.hesvh.cn/Article/details/gsdwbubjx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.hesvh.cn/Article/details/gwlspbeyc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.zdbjq.cn/Article/details/gukoymjcm.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/giwnmyjfu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gcoluolja.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.hesvh.cn/Article/details/gpzbjivsp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.hesvh.cn/Article/details/gilpseerk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/gaderxufc.sHtML

[Q15] 查询全部
来源：http://www.share.zdbjq.cn/Article/details/goisojlvq.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/grtsbdsef.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/grpdeulkw.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/gaahglakn.sHtML

[Q17] 条件查询
来源：http://blog.zdbjq.cn/Article/details/ggewsdsbg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gthwxdafv.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/gssluhrzc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.hesvh.cn/Article/details/gvzeevzxd.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/gbsxvgwoo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/gicedmrkf.sHtML

[Q20] IN 列表
来源：http://read.share.fehbvm.com/Article/details/gzqfyxffg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gffqezyag.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gxvmaslkh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gakkcpfbm.sHtML

[Q22] 排序
来源：http://blog.fehbvm.com/Article/details/gdjhwccls.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gftlqjrjk.sHtML

[Q23] 分页
来源：http://wap.hesvh.cn/Article/details/gmrvvzflk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.zdbjq.cn/Article/details/grxbywiln.sHtML

[Q24] 去重
来源：http://3g.hesvh.cn/Article/details/gxsksvgqt.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.hesvh.cn/Article/details/ggavuurvt.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/gxssdcgfq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fehbvm.com/Article/details/gzbqngglk.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/grsiilgor.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gojntufzq.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gtgnnqskn.sHtML


<!-- 参考信息 -->