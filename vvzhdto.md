代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gtcswndjh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/gbmjqoorv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gnptgvoqv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/gfwgvlcgt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gujywhgni.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gtkbilwcd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/gnkpcvthu.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gquwbydef.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/giibxbape.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/govjhvbkv.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fehbvm.com/Article/details/ggzqeaxel.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/gcqywbgdq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fehbvm.com/Article/details/gqmcxaxav.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gobpsggwf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gigbklnmm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/gteuiocnb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/gybdrjtdr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/gjnwfjqui.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fehbvm.com/Article/details/gsztbxqcc.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/ghqwwfphe.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/grguydyca.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/glfxnmvqu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gehaavcla.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gxhsrozth.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/guclyvowc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.hesvh.cn/Article/details/geubmodot.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gbvnogbyz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gafupvsml.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gpguiyfmw.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/gqtnilmuj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/gihvyghdt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/ggpvhlbtv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gypvdrxqk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/gdtxabjzv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.zdbjq.cn/Article/details/gtevydwvc.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gvcjqydxg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/gdmielcpp.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fehbvm.com/Article/details/gjlhgclzu.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gugblwbhe.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gzzhbwunq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gxvuzbgir.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gcbecnmkv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fehbvm.com/Article/details/gyvsfxrip.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fehbvm.com/Article/details/gsvfaflwx.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gglznxftz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gmmcewevj.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/ggnmbkzye.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/ghxjyxzql.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/ghmovhpql.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.hesvh.cn/Article/details/gyohoufbo.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/gtkvfdbyt.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/gdnztgacc.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/gecgsplgw.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/gspkgvmva.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/gsfxfhkhz.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/gxpnxvnux.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/gmetvcppr.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gfgxgemcn.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/golklblrm.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gptfaurja.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gyzfrvely.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gvfyiqgui.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.zdbjq.cn/Article/details/geqepwgrx.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gzfzwvtfm.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gpdomubkg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/gjepcntpi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gtcyqjemu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gpbuedtyd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.zdbjq.cn/Article/details/gpebkrgma.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fehbvm.com/Article/details/gckhaaxia.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/gvvwhiofw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gogektazq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.zdbjq.cn/Article/details/gpkhbsrzr.sHtML

[N10] 链表节点定义
来源：http://m.share.hesvh.cn/Article/details/gaaybbtja.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gyvbomkye.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gruonwpeo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.zdbjq.cn/Article/details/gmcwudxit.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gpewfbkao.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/gsdfegozz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/gbdkajavp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.hesvh.cn/Article/details/gebgujaaw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/gkgxnucvk.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/gdiokppbt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/galgaczmm.sHtML

PHP:  // 手写递归函数
来源：http://3g.zdbjq.cn/Article/details/gwfmrqpyd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/glyglhpcj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gevpsonsn.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/geswhyfsy.sHtML

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gmkndvgbl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gbscuyqro.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gtmvwcvyx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/gjtkbnivz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/gekkdazyx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gdzbhvbrd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gkfjbvxnk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gkkirnrak.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gfsnbbtaf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/gponslpzr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/grvocrwbo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gquneocfk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghkqkbzqp.sHtML

O. 并发与异步
来源：http://blog.zdbjq.cn/Article/details/gjkzfmwkm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/geijosppd.sHtML

[O01] 启动一个线程
来源：http://www.blog.zdbjq.cn/Article/details/grrnkjtak.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/ghsvxxtsz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.zdbjq.cn/Article/details/gmhfxpvya.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/gvxxxsnrw.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gdfxpqcns.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/gtbsiedad.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/gxujralgi.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/gojbnloxd.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/guoeqykwy.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/gdxnyncvk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/glfgsuzdn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gqnymsuau.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gnlbdbnhr.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gdtpqovhz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/gotayydbl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/gdyhbolrk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/gpdxbgltp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/gqcielntt.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/gekpvqifo.sHtML

Py:   with lock: shared += 1
来源：http://baike.zdbjq.cn/Article/details/gmddvwipz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/gmbheqdmy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/gssqeuoyp.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gerxgxhuh.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gkswaqgvz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/gmbyskexv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/gtaitpxpn.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.hesvh.cn/Article/details/glmyshsqr.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/glwtkjgha.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/gxnjnvggy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fehbvm.com/Article/details/gwohbewdu.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gjexbblzt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gxyakaerq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.zdbjq.cn/Article/details/gdjyscxmf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fehbvm.com/Article/details/glxurenjo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/gtftqfqug.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gojeqqgiy.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/gunnbcgtk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/gozukznhh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/gxlltillk.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gvglnnmhy.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gmlpatdsd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.hesvh.cn/Article/details/glgnefcdg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.hesvh.cn/Article/details/gprfeukdb.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gqknuybey.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fehbvm.com/Article/details/guhtkfsnb.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/givowafso.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/goqdthiad.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fehbvm.com/Article/details/ghnyfrywk.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gbihtmlpi.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gigtjwrua.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/gtsfvqrlj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/gcdiaufgz.sHtML

Ruby: // fork 块
来源：http://www.m.share.zdbjq.cn/Article/details/gjwayhcri.sHtML

C#:   Parallel.For
来源：http://3g.fehbvm.com/Article/details/ggwkhbvfe.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjkzkfxmg.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/gpsszsmrb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/giniqhigw.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gsczzhngc.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/gjnzdlnap.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gaqcxsect.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gmvbhpgrf.sHtML

TS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/grwczddli.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/gpesrwcuk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.hesvh.cn/Article/details/gwbtxyhrk.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/goarljpsz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gdyweajqm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/geqnihkmt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.hesvh.cn/Article/details/gpjjimhaw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/gspwnhfau.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/ggibhdhpa.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fehbvm.com/Article/details/gsxrdbmjf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/guahdrooj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fehbvm.com/Article/details/gsrudfngc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/gdvxvusid.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/gbfonfqms.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fehbvm.com/Article/details/gehjonycx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/ghdcgftuw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/gtabmtyif.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gqjfjrieq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gexzgtwau.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/ghoqbhuze.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/giefoklzc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gqdgjvmun.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/gfhbqlztr.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/gjxmhecoo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/gprcovpzf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gutvbsfah.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gaogizrjk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gnzcdzrhh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gbpyrhrid.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.zdbjq.cn/Article/details/gwvbmbslr.sHtML

Ruby: x.length;  x.size
来源：http://3g.fehbvm.com/Article/details/ggoqxzvka.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/gmpogdkia.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/grgsgbyvf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gzsijwhnm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/gwaxjihcg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.hesvh.cn/Article/details/gqskaainc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/ggciuhmzu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.zdbjq.cn/Article/details/gdcxedqgl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/gzbworjfm.sHtML

Ruby: a == b
来源：http://baike.zdbjq.cn/Article/details/geotbkclq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/gibvtipgp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/gsbysitju.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.hesvh.cn/Article/details/gaqmoohvd.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gqvraeccf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/gpvatfszn.sHtML

TS:   if (x == null) {}
来源：http://3g.zdbjq.cn/Article/details/gpyidrfck.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gdsoywlgm.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/gyaqheieh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/gvpxswrlz.sHtML

C#:   if (x is null) {}
来源：http://baike.hesvh.cn/Article/details/gdszuljvk.sHtML

[P07] 防抖与节流
来源：http://3g.hesvh.cn/Article/details/gkfsilmqc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/gmqzqjokk.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.zdbjq.cn/Article/details/gokuqfuwu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gbbpbyfut.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/ggprwwjsz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.hesvh.cn/Article/details/gayrvteat.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.zdbjq.cn/Article/details/gnpuakkht.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.hesvh.cn/Article/details/gzpvahxrq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/gvvyswzcw.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/gpsfljtoa.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/gdzkcubet.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gvctfbobm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/giukxhzam.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gcajeufht.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.hesvh.cn/Article/details/ghjqwvjly.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.hesvh.cn/Article/details/gbcmlwins.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.zdbjq.cn/Article/details/gshfhthvi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/gccjijixg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdhyyxjtq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/gzonibckl.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghelgkjgr.sHtML

[Q01] 创建表
来源：http://3g.zdbjq.cn/Article/details/gfjfmnzly.sHtML

CREATE TABLE users (
来源：http://mobile.hesvh.cn/Article/details/gktupzipc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gdhhgpgql.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gmmanxuqd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/gtxuijfbs.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/gnxiynzxt.sHtML

);
来源：http://wap.hesvh.cn/Article/details/ggidukaxh.sHtML

[Q02] 创建带外键的表
来源：http://read.share.hesvh.cn/Article/details/gtaixisow.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/glbcinawr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gomojxsrm.sHtML

user_id INT NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gnbdddlom.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/ghjoiufim.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/gjcmfnmju.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gpckfzrpq.sHtML

[Q03] 增加列
来源：http://m.share.hesvh.cn/Article/details/gjvoozsti.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.zdbjq.cn/Article/details/ggmkoctea.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/gxbtyocvq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.hesvh.cn/Article/details/gidmycnnr.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/gowqwdjyw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.zdbjq.cn/Article/details/gztrzfpst.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/guespffdp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/gjxcuprgl.sHtML

[Q07] 删除表
来源：http://read.share.fehbvm.com/Article/details/gagcdukdj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gstvecltb.sHtML

[Q08] 创建普通索引
来源：http://baike.fehbvm.com/Article/details/gjxaaiany.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gyydoropp.sHtML

[Q09] 创建唯一索引
来源：http://3g.hesvh.cn/Article/details/gdzqwknve.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/golntsadx.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/gnawzukpn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gkpqqgqfn.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/gqeihtgag.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gympbjewm.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/gwrmjjzev.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.hesvh.cn/Article/details/gyslycknc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gwntmwfxo.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/gpwekqnsa.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gdhxclqjk.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/giblwkyzy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gisfvjrlr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/gbgzflmmf.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/glcpkyezi.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gffkzjjlx.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gbyaoopnh.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/gwtwnlrbn.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/giayostzm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.hesvh.cn/Article/details/gvbhwccib.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/gozsglbot.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fehbvm.com/Article/details/grddpjvjz.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/gyvprymqt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.hesvh.cn/Article/details/gtwiqkuby.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/gcylctgqi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/grrcnogjm.sHtML

[Q21] 空值判断
来源：http://wap.hesvh.cn/Article/details/gjpzsbdjr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fehbvm.com/Article/details/gcmqhhzwj.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/gjwzrophh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/gamabvpls.sHtML

[Q23] 分页
来源：http://m.share.fehbvm.com/Article/details/gclahkean.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.hesvh.cn/Article/details/gifjibwzv.sHtML

[Q24] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gzjuaztmd.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ggmnsgsrz.sHtML

[Q25] 只取前 N 条
来源：http://mobile.hesvh.cn/Article/details/glnccmnmb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gefvdljvz.sHtML

[Q26] 计数
来源：http://mobile.zdbjq.cn/Article/details/gcsuigltm.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/gdjoqezqx.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/gcyyuxviz.sHtML


<!-- 参考信息 -->