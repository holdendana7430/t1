代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/ggsjmtuvm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/grmmbaaay.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gxkdqjmad.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.hesvh.cn/Article/details/goiqxpcsm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/goiwewegx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gmwzbyovt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gfoqlyllg.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gnthnknwu.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gvufufbej.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/gldacfjoq.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gthetlkng.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gishmmawz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/gkerlpqmp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gaybffujy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gtoaivsok.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.zdbjq.cn/Article/details/gltlnzkcg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fehbvm.com/Article/details/gwdfdcqzu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gltxliuua.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fehbvm.com/Article/details/gkiieqmvc.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/gmbxaessb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gcxaykczf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gomjlusrv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gppurobdc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gjkzurgjr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gmrxoqumr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/gkujqxgwe.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gkosdamgx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gscjdwxsz.sHtML

[N05] 最大公约数
来源：http://mobile.zdbjq.cn/Article/details/gmlchnysj.sHtML

Py:   math.gcd(a, b)
来源：http://blog.zdbjq.cn/Article/details/gonwfsitu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gwgdnnafe.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/giejwmzvz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/goklysmpz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.hesvh.cn/Article/details/gbnknefle.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/gawnjlnsn.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/gspeoyfbi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/gypypvmqt.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/grrycchif.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/guxbhhlws.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/gksmhyqlx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/ggnlqwiyr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gxqcktbta.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/gpjnmodil.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gajocvtjs.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/glsqdpdqp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gqplhonru.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.hesvh.cn/Article/details/gkwibjnpg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/gimzqrbqr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/grnzckqnu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gixcqtfzi.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/gpddypgiq.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/gegsskvls.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/gkioyabce.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gohrsbawz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/gcwxdgybc.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/ghyytmodt.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/gaxpnaago.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/gsaaerwzd.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gpeqveuzo.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gdwstzvgj.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gygcukirm.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gtfmbebdu.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/gommwfwxf.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gtxiabchd.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gsthvewrt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gktmhgvth.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gbswjyoqh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gsxvqscek.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/ggktgqqei.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/gpmsapcjd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/grawdnizw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gglpmxqls.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gtcqwhsqy.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/gthmdvnir.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/gpfpegapx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/gufkzbcmp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/gmdkncvxo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/gvqrigyvk.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/glofwotdr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fehbvm.com/Article/details/gaasfqryb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.zdbjq.cn/Article/details/gazwrkomq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.zdbjq.cn/Article/details/gyboctnsd.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/gkqeleoom.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/gdlywjvsx.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/gojficzgc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gfaaiptrj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/ghjqqsrzc.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gcjeizbpu.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gphwpirwg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gkdftytpm.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gpltrnrdv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/gihobrjue.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.hesvh.cn/Article/details/gfjhsacoe.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.hesvh.cn/Article/details/gjjszwnlz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gcrkszqqv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gvvefflvk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/geimbtqdl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.zdbjq.cn/Article/details/gnhmrrusp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/gieiiqnve.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gjayoimwi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gosopvghp.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gvzaedsjl.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfuazqssf.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/gnubxufes.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gxqtrlmjx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/gaycryywp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/gpcyxqffk.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gkysxbbej.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/gvppxozrx.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/gwkvokict.sHtML

Ruby: Thread.new { f }
来源：http://mobile.zdbjq.cn/Article/details/gepfutpsj.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.zdbjq.cn/Article/details/ghaobauim.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/grwwltspp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/ggdopsrsa.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/gsyxbcjbt.sHtML

JS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gydihwlat.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gmbyhucsk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gbrvkwyme.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/gkujwlqxy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/gouaxujnp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.hesvh.cn/Article/details/gfawquozw.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/gmvizijgp.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/gxctvqvnx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fehbvm.com/Article/details/gbuazpuzc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/gfgmxtacl.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/golfxjaxh.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gcsaivpxh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/gpfkxtnky.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gyfxkspoi.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gjvzlhvvn.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.zdbjq.cn/Article/details/gunkzmlus.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fehbvm.com/Article/details/giscsdlqk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/gpzgoiqwj.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gzsawzajy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gzdnzkpqv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/gxfimmsse.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.hesvh.cn/Article/details/girfsjgzi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.zdbjq.cn/Article/details/ghgniiuvq.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.hesvh.cn/Article/details/gfmaibazl.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/gzghqulsq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.hesvh.cn/Article/details/gxdkgzzyb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.hesvh.cn/Article/details/gixpymrxx.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gllimuytv.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gfamzpobw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/gbaxmojig.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/gyqutnugx.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fehbvm.com/Article/details/gwhkumvfl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.hesvh.cn/Article/details/gbuhmzbda.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/gkvksmemg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gynqfhyhj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/geoqhcncu.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gxevhsxmk.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gtioagsch.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gkfyehypt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/gzsjzvoiq.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/gkrbmaaks.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gnugnkvew.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqfbsdpdp.sHtML

P. 常用工具函数
来源：http://baike.zdbjq.cn/Article/details/gxshfwmhr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvinrqdfg.sHtML

[P01] 生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gwaxaoslb.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/gzkyqjiio.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/gkhvhojii.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gdyknitzk.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gbwnhcysb.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/ggmqlzfeo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/gtjlnauys.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/gyivkslal.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gsdipdzxv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/gnraalrlm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.hesvh.cn/Article/details/guflnicwt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/guqynasii.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fehbvm.com/Article/details/gxcelvkyd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/ghamczfgv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/gkksqkpzo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/gdllmrexb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/gmwuqitae.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fehbvm.com/Article/details/gdludimoe.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gulzvbqoy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.hesvh.cn/Article/details/gthmznykq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fehbvm.com/Article/details/gellkngbn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gkbnlovqt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gkxuumugr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fehbvm.com/Article/details/gvsahgrdc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gvovwbthb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/gvokvfovy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/gcconvoms.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/ggfkmorde.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/grvbemzvy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/giqplbhgj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gtgxsmssc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gptmrmirb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/guccjbala.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/gibfmtwjk.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gvuaauqjp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/grcujaoan.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/gcvljjkel.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/gcvkzhaab.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/gtyumneqq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/gzhczttvd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gqwsegmix.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gprlgdgkm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gzltpoack.sHtML

Ruby: a == b
来源：http://www.m.share.fehbvm.com/Article/details/gxfdgdugi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/gnoykfwkx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fehbvm.com/Article/details/gtnlyqrrq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.hesvh.cn/Article/details/gsjvvolnu.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.zdbjq.cn/Article/details/gicvnrqwl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.zdbjq.cn/Article/details/gghjhltul.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gahqikzmb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gbqalkjye.sHtML

Go:   if x == nil {}
来源：http://read.share.fehbvm.com/Article/details/gfdrmgvoc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/grisjdxwr.sHtML

C#:   if (x is null) {}
来源：http://baike.fehbvm.com/Article/details/gnhxrlsrp.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/gxwlqhfxf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.zdbjq.cn/Article/details/gupbfgnfo.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/ghwfmssnl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gvejsgosc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gbvaiuqft.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/gylliubzd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/guezhutcc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gnylpassj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.hesvh.cn/Article/details/grscqwigy.sHtML

[P08] 处理浮点精度问题
来源：http://blog.hesvh.cn/Article/details/gjbmojtvo.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/gqlvrosbv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/gczotybzd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.hesvh.cn/Article/details/gechrdffr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/grkwvzudu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/gpztyqjws.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/geblcigxz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/gmaqrozjl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fehbvm.com/Article/details/gfnbgwgpk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjhujcblf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.hesvh.cn/Article/details/glvqzzkrr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gobadsale.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/gymsvnsvk.sHtML

CREATE TABLE users (
来源：http://blog.zdbjq.cn/Article/details/gufatjhdn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gimftyvjw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gbnrzrgmf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/gsbnxcsxb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/gxgrkeweq.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gidiwykld.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/gllchaaay.sHtML

CREATE TABLE orders (
来源：http://www.blog.hesvh.cn/Article/details/gjkududiv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gbsbexfyu.sHtML

user_id INT NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gnngwmtfq.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fehbvm.com/Article/details/giljrnkvk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/glryqzknx.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gcnbgkftw.sHtML

[Q03] 增加列
来源：http://m.share.zdbjq.cn/Article/details/gbkkqzqqw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/gzeixnzwc.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/gocbdpzwd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/ghzppzapv.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/gpejofhmo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.hesvh.cn/Article/details/gwlveewie.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/gqfymkehy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/gpdgypebb.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gxtvqfsky.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gledwcqgg.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fehbvm.com/Article/details/ggzhsiicr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gtbmqmqdj.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/gcjyfiqix.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gokwwgaxm.sHtML

[Q10] 插入单行
来源：http://m.share.fehbvm.com/Article/details/gzhujmrws.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/gljnmimbm.sHtML

[Q11] 一次插入多行
来源：http://www.share.zdbjq.cn/Article/details/gvcrakfdy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gdaztbvyf.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fehbvm.com/Article/details/glfyrzfsf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/gzcbzeclw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/glebnlase.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fehbvm.com/Article/details/gifmwsbiy.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fehbvm.com/Article/details/glzuvcubh.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/gznibxysk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gvoazpjsv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.zdbjq.cn/Article/details/gxmaindtx.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gbzmtkgts.sHtML

SELECT * FROM users;
来源：http://3g.zdbjq.cn/Article/details/gjsywaktr.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/gqcoooihe.sHtML

SELECT id, name FROM users;
来源：http://wap.zdbjq.cn/Article/details/gtvjzpglf.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/goxvivvlb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gdoyffnji.sHtML

[Q18] 模糊匹配
来源：http://wap.fehbvm.com/Article/details/gokiyppio.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fehbvm.com/Article/details/gyqamfiat.sHtML

[Q19] 范围查询
来源：http://wap.fehbvm.com/Article/details/glgvlnnwq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/grfkhfahh.sHtML

[Q20] IN 列表
来源：http://mobile.hesvh.cn/Article/details/geblbscrp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/gldeedzvx.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/gdqlnvbmh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.zdbjq.cn/Article/details/gofhtxjtx.sHtML

[Q22] 排序
来源：http://wap.fehbvm.com/Article/details/gyuwdtzue.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/ggtpdtwxy.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/grrlykesf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.zdbjq.cn/Article/details/gfylqkisf.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/gihizilfl.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/gxdoabqxb.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gafcjvspt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/gbvrvozxj.sHtML

[Q26] 计数
来源：http://www.blog.fehbvm.com/Article/details/gokmxllrn.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/gkmgjqkaj.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/ggdlszeho.sHtML


<!-- 参考信息 -->