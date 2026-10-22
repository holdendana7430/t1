代发 wailian999

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2cvsrfupt.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vwjvamwv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vggetyqn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vwrxrehy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qupjjesl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2amqkqfmz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nkojxmhk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2lehezagc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nbbtozfj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2bbbxibtn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2uypiruar.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2wnpdpxrt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ppsrvyoz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2dwnxhjse.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ahgihizy.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ggawnlka.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2chtxtahf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jcghntqq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2rakpghkw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2scbcpuii.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2lkmnwprc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2rbxnqcmd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2pnhsevfk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ktajpmcv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2arrxqlzy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2aisnujua.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2yffiqeex.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2jhppklkb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tpubmxib.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2vgjwzyij.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2szjcsjmj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2aepvmsdy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2jsqlnvoz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2suvanxbg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2nfsjnudg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2swsupivj.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2avlasnqv.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hrsvpvtp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qezwufrz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2xrkbhwbs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ncwhhrga.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2eydxvemm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2ebxfflbr.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2mpkfmgdd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2sergzbcm.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2knarkvvf.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ebpmrcpb.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ozwwpfhh.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zafkinlb.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2itvhkpta.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2daqeevhy.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2xrzpiazy.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ruihlsgx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2mcdanqcf.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2eampsitx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2avxvjsdb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2raliimtw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2nfkqzdui.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ocsbkyuc.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2mnfingcl.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2undlyrrx.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2nervbzcr.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2qyvoihat.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2majvctmh.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2ezqiddsb.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2thhzkyeb.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hrfcndii.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mradzgwb.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wzzgeifc.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dokmdxfy.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2bwftmnlo.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ftxrvtka.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2osylflvh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2ysxccpkn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2fhenbucq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2elicfqsv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2mxaevseo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2zzcnsdzv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2vzwdlivr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ipyhlyph.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2nxpyajuk.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2uhfynmlx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2nkmdowqr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdkahlli.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2feffhxhj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2mitmtcsn.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2xuqvofmw.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2vmrxilxy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2onnxzgfj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2xkfqnvqb.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2fjhdkxab.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2mdcducmh.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2rdfxenlm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2fvfaicrs.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2boscqsih.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2nvptnfln.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2pwiqcapg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2zpwdugch.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2mfxdnvem.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2hctywqnz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ittdhavu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2hxcbaxev.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2xctdjtso.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2qzbbnlql.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2xciwlqka.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2aiwuwizv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ykqozsqf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2uxrpfnwd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pyutrpsl.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2qpzajyax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oxamxujh.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2fdpivlmp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2sxssbbpf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2fsmeywvy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2mqrybaup.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2qdwsmxzy.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2pcqpowyr.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2bfdhiixp.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2luffiept.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2lusetszw.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2oqynizbh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2rqgmxfge.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2ydqtkpbj.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2vpwwmrbn.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2qjgtqams.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2wrrtwapt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2kagrjpsq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2mljcipgc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2neuqbbsy.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2jlsuzvps.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2clfvhzdj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2aqeowknb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2kgfcekgw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2rzfmamtd.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2mawpwbid.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2angbqqbk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2aylnvwjc.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2snkzfenr.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2peunjzgn.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2afzdwdik.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2egnrqgrh.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hbnrdxef.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tmbkudxk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2hleserwe.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2scktrcjp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2sevhpjmb.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2bsqoejkn.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2hppzwvwt.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2gkhrsarw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2cuvvqtpn.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2dkbgnxuk.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2pbiovqkt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2mtnwajcj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2sfzrrcwm.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2mvsbgplq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2jmsqtina.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2nstufypj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2pgoiljbb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2wvxizybq.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2rndlmtbu.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2rbeeuaym.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2setfuhxp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2jcnbnhds.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2qewavojc.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2cfqpluyu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ebdqjuku.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2iknghhjp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ftfrbwpv.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2myyajchb.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2vxxipvfm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2lczphvyb.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2febjpulp.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2etbsvzcv.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2diwchmou.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2neytjvhl.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2diwrtojt.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2udtsojbj.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2gujizpye.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2tzrwxzki.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2hcjseyst.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2jycfnekn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ualrlwoh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2uyflfgjx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2qrizudij.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2obcomnvr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2tslfrmau.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2xiolyeem.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2reunxenz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2eyhnkall.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hjkcpxlo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2yetrvlmb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2zwiydoru.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2ndshyfam.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2plzcckwq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2ktoahqef.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2peakcqcw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2rpsyefhn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qtgixtkg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2btisnofv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2muyixycl.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2zievtzfz.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2pxthqjth.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2lmkxrdxq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2yppyzapr.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2bldmgqva.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2ezxovomg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2whmfvcth.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2kpxsfotf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2vkmumiwq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2xdznmirc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2kckaeifa.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2zrlbgvhx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2egdubovb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2prgifytx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2jftygoqz.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2wdulfivp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2gbhaenxn.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ilimtxcg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2yimfbsxd.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2fnvjqtgr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2zizszvwz.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2vtgbqndf.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2pjabahky.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2yhrqsgwm.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2xoruynhn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xznicaql.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2tzbkvjcj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kdcbmbrn.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2fwzfmcno.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ijgvmlwp.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2dmhjrhiz.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2tayqxial.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2ftgqtrci.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jkdqimpj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2lxbfxytb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ltogjege.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2dmzjahsz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2yfymdtvy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2rcwukdnr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2xvrjcieu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dfmqcjha.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2yotestao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2exweyhhr.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2kewpsbvn.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2hckjyurz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2qesdmttb.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ayahfxhw.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2snfbjuum.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2agypeeup.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2hnyukmbc.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2okewrgne.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2truseqtd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2vwubbpav.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2oktcledt.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2zodubkly.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2sstznutf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2cpwadzvf.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2mdgrhini.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2oylunmpv.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2nsnzymms.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2dlcfdhad.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2oljyhlut.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2srbdkvyq.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2znvgwzpb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2zcxtokzz.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2kyfubsop.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2cwrxcvpr.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2yxnwphge.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2jxcdgwlu.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2bcezgrlr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2pbviyuns.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2kbbpeusk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2lrfcjbto.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2awiefsnq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2jruidxta.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2ymqqokrx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2cxgboqxn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2xdkskljf.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2bwjoxpvk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ewhcugyd.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2nmtbojgp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2nueskcgt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2cjceyhkl.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2ugytmuzg.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sbrlbmyr.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2fweelwon.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iqlnsiez.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2ccchfazf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2vfxqtrwa.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2fjtfkrlx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2xnoehpws.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2eukynavw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2mnfgnctz.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2lrmnmqnn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xxxeinma.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2mqsfrkrx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2nkaofqba.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2asrmybie.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2ggzyeygy.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2chlpfngb.html


<!-- 参考信息 -->