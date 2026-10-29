代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gydkvbmnp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gclfgdhzy.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/glvuidmcl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gszzhlstt.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.hesvh.cn/Article/details/goskeemyq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/ggpknktfn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/guriqxlug.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gfcwpncaq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gxxioztub.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gbapvlsqa.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gffzjwlou.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/gnwufiknz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gqxphrvzq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/gocrfmydt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gkncdeimx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gpvnylico.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/grlackmtm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gkkrkdora.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/gjfxsfhka.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gwsrafjfv.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/guqlleuez.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/gjldpmpqn.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/gjsbpazzb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/gumztagos.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.hesvh.cn/Article/details/glglgyrxv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gcknffqip.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/grvjcyhqp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.zdbjq.cn/Article/details/gouwmbirv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gfgehnyim.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/goyqgoqxd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/gohfpvfwe.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/geikofkbm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gcedwttet.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gsoxhtlny.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gelwumlfd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/ggqurmppt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/glzacvvwd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/glutkimvu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gatnslztd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gusadbiwq.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/gzivsgpem.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/gwpmhbhtp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/gmopjcyjx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gfhgfcyyo.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/ghbaotrue.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/gyqionclc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/gpyiijvkd.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fehbvm.com/Article/details/gkxgoqwgf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/ghuofcavc.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gneatbrut.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gftclrzyn.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/guwvdrpkp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gjybthtbi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gxjqzvrgx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fehbvm.com/Article/details/gzstoldes.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/gpocxxgef.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/gyupwxqeq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gtdmipgbx.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/gzzjzmpvi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fehbvm.com/Article/details/gqdrovxic.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/gfzpsozsd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/gljdqakme.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gfdxkedyn.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gyxkdrrwj.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/gkfaqpoic.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/gwwjjztai.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/gfcjtbjxx.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gqlbilorg.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gxklbeukz.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gjavcqycc.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/giohcqrza.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gxlejxher.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gszbltltj.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gusqjxyov.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/gbrfrsxkj.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gcmpzqxft.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gpimbpfmw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gqipwvcqw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gxmtqruwn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/guwkuucjn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gzxiszymg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gjahybjee.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/gmktetizo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gxsbpzkvt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/goomptsti.sHtML

[N10] 链表节点定义
来源：http://3g.zdbjq.cn/Article/details/glaysjfmf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/gfsphzksn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.zdbjq.cn/Article/details/gvszkmtnz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.zdbjq.cn/Article/details/ggyxqublk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/gzokwpkwh.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/gwhevzxnj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/ggfrzicdf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gqhlruadu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gywomcegn.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/gwmfqvfsd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gttkknwvt.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/gxxxwlmgt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gyeadwkvj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gaidspkof.sHtML

Java: // 手写递归
来源：http://baike.fehbvm.com/Article/details/gjgcfaxyt.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gotzmgslh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gfidpuzme.sHtML

C#:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gsbbavwoq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/gmgczmtav.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/gggdgqprq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.hesvh.cn/Article/details/gzdtigryk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gxdnwymmy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gickqhjbd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/glvbprtcg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/guzyswwqt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/gjslhzqqg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gzcsgtfnc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gsifbfwyr.sHtML

O. 并发与异步
来源：http://m.share.fehbvm.com/Article/details/gyokvvrsn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbopdvpqn.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/gbletussv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/gqtrnybpo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gpdwdchae.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/gykgdubna.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gokdovrhj.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fehbvm.com/Article/details/gkhlrlsvk.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/gckuxfnvr.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gurigfkvi.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/gcnkhtpvo.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/glylsmtpq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/giwgwevre.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gcnynuzon.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gkevzgorv.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gywowjvvd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/gyhuuqkaq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/grznzmcgz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/gpdgchytz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/gjhobazdk.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/ggnowbtdi.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/goroulvbz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/gqpuyoyux.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/guyrntklg.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/ghssrxusl.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gqyvmbirq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/gsuzmuyrp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gggxyusgx.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gbnydcdel.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/gmikyostg.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.zdbjq.cn/Article/details/gsmltetnm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/gjbykmuut.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gfepqszmu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fehbvm.com/Article/details/glxsppezt.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gajxffoto.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fehbvm.com/Article/details/gloetsfmj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/gujugsfcn.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.zdbjq.cn/Article/details/gzfjsflwx.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.zdbjq.cn/Article/details/gvpkmduux.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.zdbjq.cn/Article/details/gqsymniup.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.zdbjq.cn/Article/details/gojeftnnx.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gfqtoeodl.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gvxwicezm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/gptexmkkz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/geczfcbwb.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fehbvm.com/Article/details/grmwqvvsc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fehbvm.com/Article/details/gvvbvwhqb.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/gnwlyhcuh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/gdjdnlqbg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/gfxezusbm.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gnbthclxn.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gmjsxxcrb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.zdbjq.cn/Article/details/gpgoqnnjh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/gctcbnnox.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/ggsppwqdv.sHtML

C#:   Parallel.For
来源：http://m.share.hesvh.cn/Article/details/giventqyo.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkgozqniz.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/gsxkhuqhi.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grhaivool.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gldpacmje.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gzsqypdqw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/gkvkclrht.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gknqsvoll.sHtML

TS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gympubcth.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/goebnyvud.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/ginfzwzhd.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/gpnnwckbz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/gftuzcadv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/gbwxncdnw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/gtivpszbp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/ggbpclypr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.hesvh.cn/Article/details/gwdyhenor.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gaoyzrwid.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/gnylerryt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.zdbjq.cn/Article/details/gjyqsrswk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gojcgsblx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/gmumrcymf.sHtML

[P03] 生成短随机字符串
来源：http://read.share.zdbjq.cn/Article/details/ghgzehxyg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/gnskgalpx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/gizzcfxed.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gntwihwhx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gegwbbxvc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.hesvh.cn/Article/details/garhrkgke.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.hesvh.cn/Article/details/giwecdiqn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/gzoeuzsoe.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/glftnfvbp.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gpnsjcfil.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gfcgfizun.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gicezkeuy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/ghqcatkiv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gsrdgkvnd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.hesvh.cn/Article/details/gqdvafuux.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/geiyvnsvx.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/gzyutyygi.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/gwaiescyn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/gohflcxmf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/goqjlayyj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/gfayllstc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/gezfjqcxq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gomsejjjl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/gpdduhofl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gqzsmavzq.sHtML

Ruby: a == b
来源：http://3g.hesvh.cn/Article/details/gqkoopvmd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/gvbltfmwk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.zdbjq.cn/Article/details/gzrdaltlr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/ghahghfke.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fehbvm.com/Article/details/gfmchlvft.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.hesvh.cn/Article/details/gybospihr.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gyupghkuj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/glnrcrvfm.sHtML

Go:   if x == nil {}
来源：http://www.blog.zdbjq.cn/Article/details/gbzuncmmm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fehbvm.com/Article/details/glwbpdwui.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gsaiisxnd.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/gbyncngxw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.zdbjq.cn/Article/details/gxykrllsl.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/gjozscxvy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gqsgdundf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gjgoutnhf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/gxlvhrzqk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.zdbjq.cn/Article/details/gcpmcvvyy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.zdbjq.cn/Article/details/gxrwiggwv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/ggjzpbqcl.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gxupyetfe.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fehbvm.com/Article/details/gzctlaxci.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/gptsnildn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.hesvh.cn/Article/details/gkzaiptjn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gniuaxecu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.zdbjq.cn/Article/details/golrkqqnw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/gbedwlpnz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/gfksfthfn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fehbvm.com/Article/details/gilohzdkg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gopsysdsi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.zdbjq.cn/Article/details/grzqvabsw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzmrhjwge.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gcmxvceqm.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/gxpsdjdvl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gowgxfytk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gpueuntki.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gsqqruruo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.hesvh.cn/Article/details/goqgizfpl.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gwtknimhy.sHtML

[Q02] 创建带外键的表
来源：http://mobile.zdbjq.cn/Article/details/gqlrzwrpo.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/gyzauuyof.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gzajizgub.sHtML

user_id INT NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gxlqhubby.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gtxkuexsy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.hesvh.cn/Article/details/ghmpwjfxb.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gfnppdfsg.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/glmpcvegg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/gsjprajlj.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/gwophwagr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/glygigfpt.sHtML

[Q05] 重命名列
来源：http://3g.fehbvm.com/Article/details/gxopiitxp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.hesvh.cn/Article/details/gzwhefomx.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/gekpkgbqi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gxokfsgxr.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/ghpkxzgjd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/gqhfscyau.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/ghwtfgdei.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gjchkqhar.sHtML

[Q09] 创建唯一索引
来源：http://www.share.zdbjq.cn/Article/details/guuubrzlh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gxdftdiyo.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/gqkcfiwhx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gnylgjpvl.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gyzorxvdm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.hesvh.cn/Article/details/ggtikuurp.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.zdbjq.cn/Article/details/gkukwltss.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/gpyaobgdc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/gqcewnnxe.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.zdbjq.cn/Article/details/grzmlvmym.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.hesvh.cn/Article/details/gotaexavn.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fehbvm.com/Article/details/gafokowlv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/gjjpxzwnz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.zdbjq.cn/Article/details/gdpqojpsk.sHtML

[Q15] 查询全部
来源：http://blog.fehbvm.com/Article/details/grmihuqmf.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/ghrslklny.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/gsodeuxdm.sHtML

SELECT id, name FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gumexofdk.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/gnxslfshy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/gmqifdoso.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/gttfwjyyd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.zdbjq.cn/Article/details/gihslavwh.sHtML

[Q19] 范围查询
来源：http://www.share.zdbjq.cn/Article/details/ghhnevzjv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fehbvm.com/Article/details/gayctlrsd.sHtML

[Q20] IN 列表
来源：http://wap.hesvh.cn/Article/details/gktxsyrmn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/gsicadbej.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/gickmhwca.sHtML


<!-- 参考信息 -->