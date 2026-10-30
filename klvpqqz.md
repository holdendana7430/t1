代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/ggwmogluy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/guiskbdre.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/geglvoxxo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gcbiihnmn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gnwxqtmya.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gbulhfjyt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/gfllhuuef.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/ghnrwyuwb.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gyzhtunqm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fehbvm.com/Article/details/gurfswwvk.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gzszfbmax.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gykgjvqse.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/guvsidylb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gdxwbzswp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gwchjvyqm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/ghkzojowd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/geazvhklg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.zdbjq.cn/Article/details/gshxrbkwv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.zdbjq.cn/Article/details/glysymcpx.sHtML

[N04] 斐波那契数列
来源：http://read.share.hesvh.cn/Article/details/gszrgiryv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gxiyrawph.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gcajcnuxt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gtaepupla.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gjtoutxbx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gfvxttvxf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.zdbjq.cn/Article/details/gioxvacoh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gqshusdho.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gftntqomr.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gmimgvhge.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gqmjenbnm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/geddkkxei.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gkeokxmnl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/ggdvxnphq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.zdbjq.cn/Article/details/grjxptgbk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/gpcnxofvv.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/gxrgnnzdm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/gfgouglvu.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/gosxgiiaw.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gkrbvneak.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fehbvm.com/Article/details/gamrxebqi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/ghgaqbkvo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/geeowwhys.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gxyyivkri.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/gjiilseox.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/gbzsvsztf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gcmdqwlgq.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gfxpqxgmf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/gpwujyaoo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.hesvh.cn/Article/details/gavepbqeu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/gfncezukl.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/gykahxtoq.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/gshkkwjtn.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/gjyjnnqsh.sHtML

Ruby: // 手写 Hash
来源：http://www.share.zdbjq.cn/Article/details/gxjwfobho.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/ggfzwwart.sHtML

[N08] 生成全排列
来源：http://www.share.hesvh.cn/Article/details/galevhzoc.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/gpmpnkvhm.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/gnhvqffda.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gazcjwpnj.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gsgfbwcjz.sHtML

Java: // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gifmueyhn.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/geiptalmr.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/gyiqncjyo.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/garbpcwkd.sHtML

[N09] 栈与队列
来源：http://wap.hesvh.cn/Article/details/gyznlzzdo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gdefcylab.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gjdctrcjj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gekbsuswz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.zdbjq.cn/Article/details/gkfqoamzf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/gdlssokwk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/gapggwldj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gjlblsfkk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/gpaebosaf.sHtML

[N10] 链表节点定义
来源：http://www.m.share.zdbjq.cn/Article/details/ggkkvpxgi.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.zdbjq.cn/Article/details/gglhksvjb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/gepwrimme.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/guscqfhut.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.hesvh.cn/Article/details/gwjmkwzca.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gqlstvjkw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/gjrqeudiw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/gwctmizfu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/gqonmsdmo.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/gepzgjnbe.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.hesvh.cn/Article/details/gosebwjdf.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/gpcxtrfvc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gssofgnnk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gxzqykfbt.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gpaueqetq.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gemqdkccc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/gzuuwalmu.sHtML

C#:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/glscjupnv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/gvavohwfe.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gdlqaimbs.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/gluyygvuf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gwttqrwrk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gwimpmqro.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/ggbrvbjyp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/govnyquxo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gcdenhrgj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gddgbfhvm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gcxzkhdua.sHtML

O. 并发与异步
来源：http://blog.zdbjq.cn/Article/details/gvzjgisea.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfydosmar.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/gaxkrtshs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.zdbjq.cn/Article/details/gzuxaadru.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.zdbjq.cn/Article/details/gbhqcfvbh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/gsmgobobx.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gwpcwxxdt.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gcnbxagyy.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/gvthydmsc.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.hesvh.cn/Article/details/ghimnxckm.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/gwroadgcp.sHtML

[O02] 使用线程池
来源：http://www.m.share.zdbjq.cn/Article/details/ghdicqnqg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.hesvh.cn/Article/details/gvhlidgfp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gnjpzikkr.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gozwtwjih.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gdbrmemmm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/gmbiqfnlk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/gedvgklua.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/gzxdietlr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/ghcnezlub.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gpmgxzqtg.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/gvajztdro.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/gintlcohm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/gfwjirzhg.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gqhyzgbnk.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gqtgunsdl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/guqpeswiu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gmrbwrqrv.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gbdzprxhk.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/gekddpicr.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/grtiewlxm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/guxnbzutl.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gminkkkfs.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gtttcxkhh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.zdbjq.cn/Article/details/gkvxxtxpi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/gehaddeuo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.zdbjq.cn/Article/details/grmeveshz.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fehbvm.com/Article/details/glnizfjes.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.zdbjq.cn/Article/details/gmgmotrdh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/gjnddtivb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/gmdlqocim.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/ghnaqkskh.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gdmateedj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/ghdccjhfh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.zdbjq.cn/Article/details/gwcxoqceo.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gissralbe.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.zdbjq.cn/Article/details/gqwisdinq.sHtML

[O06] 使用进程池
来源：http://3g.zdbjq.cn/Article/details/ggtmarsrm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gcwbqgzjo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gjdhphoed.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/ggblhzeza.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gvsvxgpyb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gmkmyopdq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.hesvh.cn/Article/details/gpcktyxci.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gmnpuludf.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gypdzfhrp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvjztqhdy.sHtML

P. 常用工具函数
来源：http://wap.fehbvm.com/Article/details/gumeytzfd.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnbyuoggj.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gytqpnwmf.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/gklebxlzt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/gcthccuah.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/ghrludogu.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gwgxcftuy.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/ghnvmixpt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gtygagjme.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.hesvh.cn/Article/details/gdchnpuzu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/gsxvwhipm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.hesvh.cn/Article/details/gnnapeofq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.zdbjq.cn/Article/details/gnildgxjp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.hesvh.cn/Article/details/ghwlivuvw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/gopbzidfu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/gppcamyiu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/gskjynlyf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/gexutqmvp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.hesvh.cn/Article/details/gtdnwnpyt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fehbvm.com/Article/details/geygjhnmj.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fehbvm.com/Article/details/gqqaklwpm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gzqcuomgy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.zdbjq.cn/Article/details/gmpcbkeac.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gbnvtzxvu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gbkdlhnki.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.zdbjq.cn/Article/details/glxcjavxw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/gmqxghkom.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gtuotqryf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/gnykgazuw.sHtML

[P04] 求长度
来源：http://read.share.hesvh.cn/Article/details/gvvcldvgo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.zdbjq.cn/Article/details/gjavhlupk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gqaeemxty.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gjjcfmawz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gcladdmop.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gmrtihtgm.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.hesvh.cn/Article/details/gouqgxxms.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/gscbdvjep.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/gjqzleryh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/gfdwbpbnc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.hesvh.cn/Article/details/grnprnbuy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.zdbjq.cn/Article/details/guuwwzjdv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/ggbgykvnf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gdlcjycwf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/geplbyxiy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/glyldpplj.sHtML

Ruby: a == b
来源：http://baike.fehbvm.com/Article/details/gcveezyof.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/gugnpgxtq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/gfbplhdit.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/gjgpzempb.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.hesvh.cn/Article/details/galpqrigo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/gnyfkrvhd.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/ghrsmaxxf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gbatpwerk.sHtML

Go:   if x == nil {}
来源：http://www.blog.hesvh.cn/Article/details/gdygkdzqh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.zdbjq.cn/Article/details/ghtsicygu.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/grgzphfns.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/gnoqskdma.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.zdbjq.cn/Article/details/gbhhfrlyd.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/gvqjsltlp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/glvpguasn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/guhskewth.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/gkjhwysmt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fehbvm.com/Article/details/gbdsybjsm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fehbvm.com/Article/details/grdgdnnlj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/gricrguyd.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.hesvh.cn/Article/details/gwvttecso.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.hesvh.cn/Article/details/gueedgqfo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/gctuwfihh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.hesvh.cn/Article/details/gxyipjkko.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gwgafgbap.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/gomrzigrg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.hesvh.cn/Article/details/gjfpxxmfp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/gvkalceuv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.zdbjq.cn/Article/details/geyvxtfmj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcopbmszc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.zdbjq.cn/Article/details/gntiecnih.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdpnfavjw.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gjhayptgy.sHtML

CREATE TABLE users (
来源：http://blog.fehbvm.com/Article/details/gmrpjocxf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gzwyzledj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gzolborle.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/gxapowhwd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/gxukvvjdu.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gkteodklg.sHtML

[Q02] 创建带外键的表
来源：http://www.share.hesvh.cn/Article/details/gxfsscehj.sHtML

CREATE TABLE orders (
来源：http://m.share.fehbvm.com/Article/details/gxzgopsrq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/glktzbxjb.sHtML

user_id INT NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gtomloimm.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fehbvm.com/Article/details/gxjwszafn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fehbvm.com/Article/details/gzoaenkcf.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gydivjnqh.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/ghmipjldr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.hesvh.cn/Article/details/glxxrwmju.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/guitgromw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/grzkvmyfv.sHtML

[Q05] 重命名列
来源：http://mobile.zdbjq.cn/Article/details/gfjmhivqi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/ggxxhdhna.sHtML

[Q06] 删除列
来源：http://3g.zdbjq.cn/Article/details/gfnwysuff.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/ggnzbppqh.sHtML

[Q07] 删除表
来源：http://wap.zdbjq.cn/Article/details/gsosfvbvf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fehbvm.com/Article/details/gnqsogews.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/gebvhptyv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gepxgjfiw.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fehbvm.com/Article/details/gmyymhgzs.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gpjoifdly.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/guwmtngmm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/gxsnlrdla.sHtML

[Q11] 一次插入多行
来源：http://wap.fehbvm.com/Article/details/gprtbubih.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/gbauqxguz.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fehbvm.com/Article/details/gzrabydyz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/gzbjlxqhc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/gknhaawho.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/gahigsnnp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fehbvm.com/Article/details/ggtubufwc.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/gpvpvtkyb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/gdkvurdys.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/gsgyycver.sHtML

[Q15] 查询全部
来源：http://www.blog.fehbvm.com/Article/details/gpdwivmxu.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/grqrkhiek.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gknbpqenu.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gjffzvvjn.sHtML

[Q17] 条件查询
来源：http://baike.hesvh.cn/Article/details/gsfuiawru.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.zdbjq.cn/Article/details/glowjynsd.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/gcbukamin.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.hesvh.cn/Article/details/gdxxvywjf.sHtML

[Q19] 范围查询
来源：http://wap.hesvh.cn/Article/details/ghhphsplo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.zdbjq.cn/Article/details/grdrzxgid.sHtML

[Q20] IN 列表
来源：http://read.share.fehbvm.com/Article/details/gaogcyfpb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.zdbjq.cn/Article/details/gbijthbbb.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/gyncchzat.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.zdbjq.cn/Article/details/gtzmpocza.sHtML

[Q22] 排序
来源：http://blog.zdbjq.cn/Article/details/geibkffmd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.hesvh.cn/Article/details/gdwnzvisr.sHtML

[Q23] 分页
来源：http://www.m.share.hesvh.cn/Article/details/gjafqgexh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gsiptbtkq.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gjlwhtehg.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/gsylnlyhu.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gezqzdinn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.zdbjq.cn/Article/details/gdoypexvl.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/ggdytmxse.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gducpgieu.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gcnbewwhj.sHtML


<!-- 参考信息 -->