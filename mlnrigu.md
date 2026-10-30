代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrtmntzv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxwmsxvi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/glmpyuugh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhgclgma.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdoyyzrd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgxmqcda.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fanxiaobao.xyz/Article/details/gihjjpbcb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnkxbmwp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaailqpfh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnzesvwz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fanxiaobao.xyz/Article/details/garwllrrn.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjogpfcu.sHtML

Ruby: arr.sort
来源：http://blog.fanxiaobao.xyz/Article/details/gysgmfire.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptofszid.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbodhzcn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fanxiaobao.xyz/Article/details/gtyefbvvs.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtraggfo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsbnvpfk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fanxiaobao.xyz/Article/details/guqafarlr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fanxiaobao.xyz/Article/details/glejebphf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbwjxkkt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmibhrpxr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fanxiaobao.xyz/Article/details/ggepbscsx.sHtML

[N04] 斐波那契数列
来源：http://m.share.fanxiaobao.xyz/Article/details/gywhwdnaq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gtklovqqu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fanxiaobao.xyz/Article/details/gxvwryenq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gmopablsy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gbsgrltia.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkupoybvw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggohyyeym.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfuixxpc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpitwfer.sHtML

[N05] 最大公约数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsmwxcst.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fanxiaobao.xyz/Article/details/ggvggsntb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfqptxykc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlidoufp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkmxtnex.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fanxiaobao.xyz/Article/details/giylxoooy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fanxiaobao.xyz/Article/details/ggwmoxkiz.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giuzplfbw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfguonhjg.sHtML

[N06] 判断回文字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gtadhfpkh.sHtML

Py:   s == s[::-1]
来源：http://read.share.fanxiaobao.xyz/Article/details/garkwloqn.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvdlosqr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gqjvvpxcn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gzfgjtmga.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fanxiaobao.xyz/Article/details/gxuoyhnvz.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fanxiaobao.xyz/Article/details/gzueaglkm.sHtML

Ruby: s == s.reverse
来源：http://wap.fanxiaobao.xyz/Article/details/gjpgabfca.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fanxiaobao.xyz/Article/details/guekhvsml.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqipsfsc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufxnxwwg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpdzfqge.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwaismzzt.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjeydaoad.sHtML

Java: // 手写 HashMap
来源：http://wap.fanxiaobao.xyz/Article/details/gxpkphzge.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fanxiaobao.xyz/Article/details/gmbuksogr.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbzjoiim.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fanxiaobao.xyz/Article/details/gwihuksuw.sHtML

[N08] 生成全排列
来源：http://3g.fanxiaobao.xyz/Article/details/gyhumvmmq.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guywhohre.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fanxiaobao.xyz/Article/details/gqffcxxen.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofisnmob.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwaazzisf.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/guaicgymr.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzphcczic.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fanxiaobao.xyz/Article/details/gioslsecd.sHtML

C#:   // 手写回溯递归
来源：http://3g.fanxiaobao.xyz/Article/details/gfmescqja.sHtML

[N09] 栈与队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnokduhe.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.fanxiaobao.xyz/Article/details/gbuuqkcld.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fanxiaobao.xyz/Article/details/glfiwpewc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fanxiaobao.xyz/Article/details/gfsadegtn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fanxiaobao.xyz/Article/details/gkiyxdsao.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fanxiaobao.xyz/Article/details/gscgunidq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqltjquhp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuljtfzb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fanxiaobao.xyz/Article/details/grcdczqwi.sHtML

[N10] 链表节点定义
来源：http://read.share.fanxiaobao.xyz/Article/details/geyxushca.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnmgesxt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffplwjwe.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gjxfzzksx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fanxiaobao.xyz/Article/details/gbopixppr.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhvzdvzj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhvgptrc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrvznynj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkldalzns.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gtogkyfsl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgglolux.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcpzruhe.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fanxiaobao.xyz/Article/details/giuvifavg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fanxiaobao.xyz/Article/details/gralhnafy.sHtML

Java: // 手写递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/girokhwui.sHtML

Go:   // 手写递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkoeyraz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fanxiaobao.xyz/Article/details/glccmbrql.sHtML

C#:   // 手写递归
来源：http://baike.fanxiaobao.xyz/Article/details/gminchkzv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fanxiaobao.xyz/Article/details/grgwnpxuv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqncsjwr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fanxiaobao.xyz/Article/details/gtekkedsa.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fanxiaobao.xyz/Article/details/gjljbdlka.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fanxiaobao.xyz/Article/details/gycjlahup.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fanxiaobao.xyz/Article/details/gwxkhowzn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fanxiaobao.xyz/Article/details/gbohewajs.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gwgpbcrtn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmakwade.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gkholzxib.sHtML

O. 并发与异步
来源：http://baike.fanxiaobao.xyz/Article/details/gzvplxxzc.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzjjcouq.sHtML

[O01] 启动一个线程
来源：http://m.share.fanxiaobao.xyz/Article/details/gincoopzm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fanxiaobao.xyz/Article/details/gutshbcmk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fanxiaobao.xyz/Article/details/gwfsffrkr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fanxiaobao.xyz/Article/details/godikydgz.sHtML

TS:   // 同 JS
来源：http://blog.fanxiaobao.xyz/Article/details/gfrwpdqrk.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fanxiaobao.xyz/Article/details/glebyawvw.sHtML

Go:   go f()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsiqycmr.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyeyprpsc.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fanxiaobao.xyz/Article/details/gucfmkysp.sHtML

[O02] 使用线程池
来源：http://blog.fanxiaobao.xyz/Article/details/gdmfqatvy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fanxiaobao.xyz/Article/details/gfnyjpttg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fanxiaobao.xyz/Article/details/grrkhcgzb.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fanxiaobao.xyz/Article/details/gvadajtss.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgzsugxd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gformyypk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fanxiaobao.xyz/Article/details/ggoqdlpkh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fanxiaobao.xyz/Article/details/gavvvdcyr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fanxiaobao.xyz/Article/details/gebjhqakf.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fanxiaobao.xyz/Article/details/grfbercze.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyussdbj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjtgwjsz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fanxiaobao.xyz/Article/details/gwizojtgk.sHtML

TS:   // 同 JS
来源：http://read.share.fanxiaobao.xyz/Article/details/gdomzvres.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuqxbyds.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fanxiaobao.xyz/Article/details/gkjkaobpw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gzcbngakt.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwvuoghx.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gkucwfwyp.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxfvueqm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewqsvwhy.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gvklpsjnd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmmpyvzf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fanxiaobao.xyz/Article/details/ghvgqiekv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fanxiaobao.xyz/Article/details/gkzuejmxu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fanxiaobao.xyz/Article/details/guoeppxer.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqjjgysg.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcgieuwj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzckrlse.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fanxiaobao.xyz/Article/details/gidoucvqa.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fanxiaobao.xyz/Article/details/gilobevaq.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fanxiaobao.xyz/Article/details/gquwkvtnx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbgoimli.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fanxiaobao.xyz/Article/details/gvhirniqc.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizeeeekk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fanxiaobao.xyz/Article/details/gjtddoycv.sHtML

[O06] 使用进程池
来源：http://baike.fanxiaobao.xyz/Article/details/gksfvmlzh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fanxiaobao.xyz/Article/details/gaipyxecz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbcapmkb.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fanxiaobao.xyz/Article/details/gxrsxjsws.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fanxiaobao.xyz/Article/details/gmespekwz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fanxiaobao.xyz/Article/details/gvagmwfgh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fanxiaobao.xyz/Article/details/gcdkdhqpn.sHtML

Ruby: // fork 块
来源：http://wap.fanxiaobao.xyz/Article/details/gumzqzspj.sHtML

C#:   Parallel.For
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsvrjvsi.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gpnmkclvp.sHtML

P. 常用工具函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnetkjruq.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gyvweztda.sHtML

[P01] 生成 UUID
来源：http://m.share.fanxiaobao.xyz/Article/details/gotjfymhc.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtfagqdx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fanxiaobao.xyz/Article/details/gpstwdvit.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftcntivv.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gtiymimtj.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gicomsdrq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fanxiaobao.xyz/Article/details/ggyivdqfz.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fanxiaobao.xyz/Article/details/grasckzua.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqzzpymv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhcdxeys.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fanxiaobao.xyz/Article/details/gejwnejsb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcyuxwoan.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fanxiaobao.xyz/Article/details/gnknbgffi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fanxiaobao.xyz/Article/details/gigdryxbe.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitfwhpot.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fanxiaobao.xyz/Article/details/gocyvrhcb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnikwndvw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fanxiaobao.xyz/Article/details/gahhxszji.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqbymtcj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpzunchm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxqolzap.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fanxiaobao.xyz/Article/details/gxgonfhvx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfcsbszh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fanxiaobao.xyz/Article/details/gjrhlkwrp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fanxiaobao.xyz/Article/details/glugpuivh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzgwzqet.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fanxiaobao.xyz/Article/details/gekbmbjdv.sHtML

[P04] 求长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgeuyyyv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggoccgdei.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fanxiaobao.xyz/Article/details/gytvvfatw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxpzcqdr.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fanxiaobao.xyz/Article/details/gomguxijc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fanxiaobao.xyz/Article/details/glzxhkcpz.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fanxiaobao.xyz/Article/details/gkcofbqmj.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyhmmuvc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwjszdzh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgplnayb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjyxnbiv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyavmump.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fanxiaobao.xyz/Article/details/gjcizryqc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixhvykmj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fanxiaobao.xyz/Article/details/gfjsurpkf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvzcpsry.sHtML

Ruby: a == b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwqnoiyc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmritkugv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhhmhbnk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fanxiaobao.xyz/Article/details/glrxjohve.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfoszbin.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdlywlvm.sHtML

TS:   if (x == null) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmmiaqqs.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gceyhzxiq.sHtML

Go:   if x == nil {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gybnpsjgk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmjfmvqe.sHtML

C#:   if (x is null) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlrvbcaf.sHtML

[P07] 防抖与节流
来源：http://m.share.fanxiaobao.xyz/Article/details/gespylpxp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fanxiaobao.xyz/Article/details/gngomjxgs.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpplfkoh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhufnmhe.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gzuxyupzg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gamvdzivm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fanxiaobao.xyz/Article/details/gyshhdfwv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fanxiaobao.xyz/Article/details/gtbpwlolp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fanxiaobao.xyz/Article/details/gqepjaofl.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fanxiaobao.xyz/Article/details/gfenqfikh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fanxiaobao.xyz/Article/details/gmikbxxau.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/grlxxsecj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgtxlnhp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fanxiaobao.xyz/Article/details/gfrskrvqs.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fanxiaobao.xyz/Article/details/gfyqqtrwj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fanxiaobao.xyz/Article/details/gaoqzhvja.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fanxiaobao.xyz/Article/details/gymdenohu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnzibjyv.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnipdxas.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwicwyxxc.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/grkjndgzf.sHtML

[Q01] 创建表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxgbenvk.sHtML

CREATE TABLE users (
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmiqcvxa.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fanxiaobao.xyz/Article/details/gkzdbbeln.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fanxiaobao.xyz/Article/details/glaqsxila.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfrndgyr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdigzvwg.sHtML

);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmaevdbr.sHtML

[Q02] 创建带外键的表
来源：http://baike.fanxiaobao.xyz/Article/details/gmvpjuxrk.sHtML

CREATE TABLE orders (
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxcsuqlo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbshgpzd.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftvpjnsc.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fanxiaobao.xyz/Article/details/ganfcuekr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxviavdcs.sHtML

);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnunqzvnx.sHtML

[Q03] 增加列
来源：http://www.share.fanxiaobao.xyz/Article/details/glfojadiq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyknwskp.sHtML

[Q04] 修改列类型
来源：http://3g.fanxiaobao.xyz/Article/details/gnnjxppbr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmfwwpow.sHtML

[Q05] 重命名列
来源：http://www.share.fanxiaobao.xyz/Article/details/giywowhbr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghluucbof.sHtML

[Q06] 删除列
来源：http://3g.fanxiaobao.xyz/Article/details/gvcejqbba.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fanxiaobao.xyz/Article/details/gutkllhhk.sHtML

[Q07] 删除表
来源：http://wap.fanxiaobao.xyz/Article/details/gsogixivx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhmxtxaw.sHtML

[Q08] 创建普通索引
来源：http://3g.fanxiaobao.xyz/Article/details/gprmaofix.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvumlroe.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fanxiaobao.xyz/Article/details/geeeryubm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fanxiaobao.xyz/Article/details/gahecgtil.sHtML

[Q10] 插入单行
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjrodsqx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fanxiaobao.xyz/Article/details/girpgydrb.sHtML

[Q11] 一次插入多行
来源：http://baike.fanxiaobao.xyz/Article/details/goewcpkbr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gwsntrasp.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fanxiaobao.xyz/Article/details/gznxnphgh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fanxiaobao.xyz/Article/details/gdoftysit.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fanxiaobao.xyz/Article/details/gyktykqki.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fanxiaobao.xyz/Article/details/gezwqujti.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/gnpowturl.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fanxiaobao.xyz/Article/details/gnioapgmt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fanxiaobao.xyz/Article/details/gxfhtcemn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgtgdepa.sHtML

[Q15] 查询全部
来源：http://mobile.fanxiaobao.xyz/Article/details/gmeudqpxn.sHtML

SELECT * FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqmutufp.sHtML

[Q16] 查询指定列
来源：http://baike.fanxiaobao.xyz/Article/details/grmxntqaj.sHtML

SELECT id, name FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gotbtkmft.sHtML

[Q17] 条件查询
来源：http://blog.fanxiaobao.xyz/Article/details/grlrglsfe.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmeyacxk.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzrtmkzu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fanxiaobao.xyz/Article/details/gygwlfywy.sHtML

[Q19] 范围查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyynrzqn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fanxiaobao.xyz/Article/details/gnpzwzgsh.sHtML

[Q20] IN 列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gderuxcyn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnoobyes.sHtML

[Q21] 空值判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnierchry.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbgxsfvk.sHtML

[Q22] 排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcegyqgo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fanxiaobao.xyz/Article/details/ghjgravhj.sHtML

[Q23] 分页
来源：http://blog.fanxiaobao.xyz/Article/details/gnmusgwno.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsikahhc.sHtML

[Q24] 去重
来源：http://www.share.fanxiaobao.xyz/Article/details/ggixketau.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gipcffnun.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gqggaetno.sHtML


<!-- 参考信息 -->