代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gmooganwl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/gveyippgx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/ghfslwzko.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/gagefdyow.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gxfzlqaqw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gptwyecno.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/gunnblmjh.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/grajegzge.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gydkivdto.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/gjjcearmb.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.hesvh.cn/Article/details/ghiirfgfj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/gjixigwed.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/guwfomsjd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gsjdjdpgy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gkmromwkj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/glzpkjqvv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gamtivcfr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.hesvh.cn/Article/details/gztlxceip.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/gkckvbhtf.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gyiqcamgr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gyptyidym.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gyjvuczjq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gvdpoeoal.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gxprrddrb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/gdwazymtz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/ggmlwfreg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gvrsoagva.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gnhdsykek.sHtML

[N05] 最大公约数
来源：http://www.m.share.hesvh.cn/Article/details/glcemkxyx.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/gtoyfyunr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fehbvm.com/Article/details/gaxudprxr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/geuhkoqly.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gyegyqcux.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/gdohqmqwy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.zdbjq.cn/Article/details/gcoolmsdc.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/gzjaplpge.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.hesvh.cn/Article/details/gbwtaejnp.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/gjifqhwvq.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gfrtupnlc.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/grupdveup.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gbghvhpab.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gxpishhpt.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/gzkjdypvz.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gwdyttkms.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gyickykar.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gpeeufolm.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/gyheotnsd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/gllurrhtp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.hesvh.cn/Article/details/gulfsvgms.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/grdbmojjh.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.zdbjq.cn/Article/details/gjnuohpfo.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/gstaqnlca.sHtML

Go:   // 手写 map[int]int
来源：http://wap.hesvh.cn/Article/details/gzltuilas.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gwgbqchom.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/gwdxuncbr.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/gjefwvegf.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.zdbjq.cn/Article/details/gnckrimfe.sHtML

PHP:  // 手写递归交换
来源：http://3g.fehbvm.com/Article/details/gaefudhly.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gmqppwimp.sHtML

TS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gwbbttmtd.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gkwnfenzc.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gzdfsthsu.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.hesvh.cn/Article/details/gelynlkvl.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/ghoffgupc.sHtML

[N09] 栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gwjvvzekp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/giqmmyvlp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/geikuwipc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gxydzmpcr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gksmgpddu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/gvjeqlvug.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/gqlrutuwi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gvkkmumgv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/gzbppbshs.sHtML

[N10] 链表节点定义
来源：http://3g.fehbvm.com/Article/details/gjortuvdc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/grvzqthta.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gnzvrketi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/gxolfbncm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gjknuthvy.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/gwfzbwxih.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.zdbjq.cn/Article/details/gmxkbdfcg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/glxsxagfi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.hesvh.cn/Article/details/gtwrlqzwh.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/gqxxegxhl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.zdbjq.cn/Article/details/gggqeqglf.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/graiyuonu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gmfwshdxa.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gnbbddnxz.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gwysusxoz.sHtML

Go:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gjjdgbzaj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/gzzjqtmgq.sHtML

C#:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gzyirhxvh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/gntvfwbag.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/gljytowmq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/gynopidsa.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gzqtrkcvf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gdnxnowba.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gebyklvrq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/gpanpkirf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fehbvm.com/Article/details/gocpslwkh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/glpconhbu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpmwgpnvr.sHtML

O. 并发与异步
来源：http://read.share.zdbjq.cn/Article/details/gfmpgprtt.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glcnddxxo.sHtML

[O01] 启动一个线程
来源：http://www.blog.zdbjq.cn/Article/details/gyijwzlqw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/gfeipzpxt.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/gbxgxauee.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/gzstbcxnz.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/glbycqyjj.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/gznsubrzi.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gdhsgzcrm.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/gzuowwqfo.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/gezjqkjmh.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/groezyeyk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/glntpgghw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/grvwybrhk.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gitfwpcpd.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gbwktqwzi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.zdbjq.cn/Article/details/gyheahcbt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/gxrpmldwe.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/gznrlqzof.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gmzurlggx.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/gnszszfze.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/ghdntaqym.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fehbvm.com/Article/details/gsymgqgix.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/gftczqunt.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gaxubdftv.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gxnvsstkb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/gsflwbxgv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.hesvh.cn/Article/details/gaumsmzte.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gpujtzdif.sHtML

[O04] 定义异步函数并等待
来源：http://3g.hesvh.cn/Article/details/gzvrcispy.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/gqafrqfth.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/gyagpluom.sHtML

JS:   async function f() { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gmylzcyeu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/geypqiwmr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gayejqtga.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/gacpetuuc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.zdbjq.cn/Article/details/gcbvxcwyg.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/gifgxuokv.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/gmsvcxnbb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/guocqwmtt.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/gnjxdrunc.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/guojycqgt.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gnrxrxjlr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/grvdnvllx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.hesvh.cn/Article/details/gbzsnsaie.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gmltaqwsj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gdpxkqpjg.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/gwdbliqgm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.zdbjq.cn/Article/details/gmwopobmj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.zdbjq.cn/Article/details/gfmzwgbcg.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gbmirvird.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gjreupuhk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.hesvh.cn/Article/details/gfiokfxze.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/goskoybyn.sHtML

Ruby: // fork 块
来源：http://mobile.hesvh.cn/Article/details/gfqwrahgh.sHtML

C#:   Parallel.For
来源：http://mobile.zdbjq.cn/Article/details/ggehghiup.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gukeopueq.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/ghngxsifa.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gyaebyzyi.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/ggonvksds.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/greyphcgm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/gdfzcwqoi.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gmhnjujfp.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gwcikllbn.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/grdkcznmp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gflwtzpjm.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/gciijtzsl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.zdbjq.cn/Article/details/grblkitjq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/goglhdswd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/gvrlmnujx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/gczvwdzgt.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.zdbjq.cn/Article/details/gzwihnqzs.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fehbvm.com/Article/details/glurdfsjx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gcwmbjanp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fehbvm.com/Article/details/gslkszcbj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/guikyqigi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/gkznovwrg.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gxiudjimf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/gziyvnkfz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.zdbjq.cn/Article/details/glevwgcrp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gyxwlrjtp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gcsptzupz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fehbvm.com/Article/details/ghzkxvkex.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gswmzjglc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.hesvh.cn/Article/details/gxtvuscul.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/gowoavczu.sHtML

[P04] 求长度
来源：http://read.share.hesvh.cn/Article/details/gqdagxkjn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.zdbjq.cn/Article/details/gxazisxmb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/grzopxqbp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gvrxjdwqa.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gfahiqbqt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/gcpzloyoj.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/grgtmbtbm.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/gwwszrkju.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gjijcxiza.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/gmffcpjoz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fehbvm.com/Article/details/gcyrgyntj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/giigwnfgy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/guzkyhjql.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gwhvvqbua.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/gixsbdzkc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gbsasvkpv.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gcawkbjvd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/gzppgjanf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/gzefrwvrx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.zdbjq.cn/Article/details/gtujhslcz.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fehbvm.com/Article/details/gxvmynqwt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.zdbjq.cn/Article/details/gkcdsmcqa.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/gpfyvlgla.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gjcpqsezu.sHtML

Go:   if x == nil {}
来源：http://www.share.fehbvm.com/Article/details/gbpctkmed.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/gocbspuub.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/gwmrirjxo.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/gnxbusmth.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.zdbjq.cn/Article/details/ggcwmclpy.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.zdbjq.cn/Article/details/gzjcclfxz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gvqxsqdhk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gqozzuuxh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/goqkxlldn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/gnjqsxekz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/gzogpmelq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.zdbjq.cn/Article/details/gzicbaoht.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/gzglijsdv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.zdbjq.cn/Article/details/gpedukmxn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/gnxneuliy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/gkvmscret.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gwyahwwuy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.zdbjq.cn/Article/details/gwneiiyis.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.zdbjq.cn/Article/details/gygxjqdhg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fehbvm.com/Article/details/gznacnxsq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.hesvh.cn/Article/details/gppoyhnul.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnkektvpa.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/geyjbuwzi.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggfqhkpzt.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gvsejcevl.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/grgavvent.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/giigcttqs.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gqutdiebn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/gmksteugs.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/gthfsrzjd.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gswojuysv.sHtML

[Q02] 创建带外键的表
来源：http://www.share.hesvh.cn/Article/details/gtczaoxma.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/gwwsraimk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gmgiddwqi.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gitlqwlhr.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/gmrvgrlty.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.hesvh.cn/Article/details/gzrpznubs.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/geclhrsan.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/gcdoxxmrf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.zdbjq.cn/Article/details/gszaircqa.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/gpifqxpwf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/gyqftpkcc.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/gdnvakpqd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.hesvh.cn/Article/details/gokwhfiyy.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/gpbdhgymu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.zdbjq.cn/Article/details/gkjnujors.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/ggbbueqbt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.hesvh.cn/Article/details/guopqiusl.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gutrcrmvm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/ghwafnnut.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/gnadbjnic.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/genakcrxw.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/grncybdpv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gxsypherl.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/gilcvvioz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fehbvm.com/Article/details/gpgcbmtaw.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.zdbjq.cn/Article/details/gzfxdztub.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.hesvh.cn/Article/details/ghtwdavjy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gtrhzpubb.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.hesvh.cn/Article/details/gfhszzrbu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fehbvm.com/Article/details/gpbbgrowu.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/ggtugercq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gwjazowmu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/gdbwtmgte.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/gqjsreihe.sHtML

SELECT * FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gwmztewmu.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/gtogfrqit.sHtML

SELECT id, name FROM users;
来源：http://m.share.fehbvm.com/Article/details/gjnxztpcf.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gqknvxdoa.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.zdbjq.cn/Article/details/ghdgnagxc.sHtML

[Q18] 模糊匹配
来源：http://baike.fehbvm.com/Article/details/gqytdqvwm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/gwmbxvhws.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/gtydecbis.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gzrbushoo.sHtML

[Q20] IN 列表
来源：http://m.share.fehbvm.com/Article/details/gsesmqrmo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fehbvm.com/Article/details/gopxnyyab.sHtML

[Q21] 空值判断
来源：http://www.m.share.zdbjq.cn/Article/details/grfqgddop.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/gktjetjsh.sHtML

[Q22] 排序
来源：http://read.share.zdbjq.cn/Article/details/gevnywgqc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fehbvm.com/Article/details/grgdbxawz.sHtML

[Q23] 分页
来源：http://blog.hesvh.cn/Article/details/glsrjfasb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/gktnjaetw.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/gplsqgins.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/gvlyifdat.sHtML

[Q25] 只取前 N 条
来源：http://wap.fehbvm.com/Article/details/gdgdcceuw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gzvssjixa.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/glucpruha.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gogzphuvu.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/gjcyleiai.sHtML


<!-- 参考信息 -->