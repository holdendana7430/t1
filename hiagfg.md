代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2tfoytxys.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2udunflcq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hvrxipqi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2zwnpxclf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kpxghmzm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2rewwtkve.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2tmgapyak.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2wxjojrmc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2tjgdnyfl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2zbrrhhrj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2nnhawmpr.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2obgzrvub.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2iucvycnx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2jhcztsmm.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2dexagojx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2yxucjmgd.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2hmyvrmhu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2uoirrkug.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2tiqygbfi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2odcstugv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2cnbehagc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2jjwmblmb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2tnxctffq.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2svhqqcqw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2kjuqpzql.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ffvmqjgg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2hapbwbbv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qicotlem.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2mthsmerm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2vuolmsug.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ywdslwwv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bplizemg.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2mbauqdcw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2jwszgdwy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcsbcuie.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2dnkezdzr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfhjxngz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2fmjbvsio.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2egaepsjb.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2vmxvfvlu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2lnkzyqkm.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2lzdlwrju.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2jctuycci.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jxlzxztw.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2trvhwext.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qsosrtfz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2avjurosa.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2wtlxugqe.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2gextwuer.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2vhybfiid.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2zcrnnenn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2wxboiqnu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2ftgueyuu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2iurplujy.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2dcgmgcbd.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ruymehsj.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2wsoyvwpf.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2kquzrync.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2kepkyftt.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2ughtutcc.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gswoqukn.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2pkhynxia.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qqxdyozk.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mbuymkhl.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2slkjebnd.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cjbuseii.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2pzfghicu.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wdernywe.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2tfqjljzi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xmcpamsu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2cihsrmys.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nuxtkuno.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2gvbxvbcn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2albvming.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2ehybxris.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2goxzxqts.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2abbitnff.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2utivuqeq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2qwdgqbda.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2fsknrnjw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hwpccvot.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2xeovouio.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkilnvxu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2tgwghphb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2qymbwqed.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2xuzfmqpn.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2soizooih.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2rexoinbx.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2ritijfki.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2uzzjrenp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2iomlzelh.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2dtujcpkh.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2auiupvhd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2ehjejnxa.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ggsdyjdo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2rwulmaav.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2cvkggaso.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2fptcuyla.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2saqhfzqn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2smwtpjjk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2pmakeghb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2onpriiut.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2pxgvjxgj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2lqblcsbm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2irnvjxub.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2rvkqodtz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2avgkspoh.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2birhuqsn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2pgelojsj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2qicwwrqk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2mlruijbs.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2tljdiseu.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2vxvappzr.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2kqxvmaod.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2zgepycsp.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2wkrcbepq.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ttclaplz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2pcazdlaa.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2pgspsfed.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2vsozlqna.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2frzetlty.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2osfqevle.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2xqxznzct.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2ieqpwyfp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2gpvybhen.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2qedijvoz.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2haxlrhrg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2xqagcgvg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2bfwompib.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ikoddjgs.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2snbhpscf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2tscyzswt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2zwwplgyq.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2jrormgsu.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2dutfyrmg.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2nquyihqp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2jcmrxmcj.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kfaydpro.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2gejfhacu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2zwgisxxh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2piwyoycu.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2yqjjihuf.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2tbmktiqm.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2bbepiyyn.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2pogjxyuw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2auhugszs.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2gbktyenc.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2mersmskt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2faqugfuu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2bprdeiqa.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2iiilbqbe.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2bptccaqu.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2amzcbwdh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2fyaicnac.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2rkekphgr.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2dfiolnms.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ofnxlafa.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2rfsnkpbf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2nxvgjjgj.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2didpyuka.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2uqwxnysy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fjjylzjl.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2axbqqdrg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vqxrrwuy.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2hyzlqcez.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2gzqltcok.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2wowklwak.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2vpteaijy.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2fcyzgare.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2scggbfqy.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2kigrkihn.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2fhdumwij.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2hdfjvmei.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2jpwlxoit.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2rfpemcpl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kabcjwwl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2dnkfouby.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2jyngchxf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2bfqqujnv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2vhjpejxg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2dnyermud.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2xfppteab.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2eojueekf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2mwjncxdk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2fbagmmxo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ckvlwwwj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2fvreujgk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zrbvekve.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2gsqtrsvb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2govckxht.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2buethfnz.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2frhjbinr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2ooumuofv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jhjwayuo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2moivjhml.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2imabdddg.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2kezohnnx.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2nobuievw.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2plwryzmf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2wrfeithg.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2ggfixymy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2lalbwloi.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2dbcqhmiq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2ktjwptso.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cfhumubw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2balsmlbz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2wiwrddrp.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2cqyscdzv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2wdhtqvwi.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2msdkpulz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2jvicfgiz.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tryavhbx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2jthdtkgk.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2hkgowknr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2vxmvgcoh.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2ksnvithf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2wgtnzxre.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wcvfwsvu.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2rwzfmmjv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2zzkvwqml.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2midbhkrf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2tqlnalzm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2htihsavu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2avevhomc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2lmrlfvze.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2plmjgpcg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2ovszxrmi.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2geyskjpn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2ievoshxi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2xdtcjjsk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2misvrdnd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2tuajcdpg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2mwxompdl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2rcaknswy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2qmtjzkie.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2cqxilype.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ylollbvl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2ndmnfzla.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vexzegrt.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2erbzpylf.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ovoozhow.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2hbziympj.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2euwfijcv.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2gwwkwbqs.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2eikefrvh.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2tkrqteny.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2dncapqkc.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2llyctpux.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ebwcinft.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2rwtedsea.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2qnaaqywx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2dmdpvctg.html

);
来源：http://www.52xcode.cn/Article/details/gt2glmpowue.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2tsgxymkd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2tanbmgvz.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2groidcvt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2mtxrsipv.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2mpvxrzvx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2arovmdez.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2dyoormoj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2hggwknll.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2vbobtkan.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2ipqmwzpd.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2owanbgac.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2kgmdxqwn.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2cszlufog.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2mydimzwf.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2jrslcgke.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2yzxeondf.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2wppkzgwv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2emarcram.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2rxcrxigl.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2vcrfyttb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2huwisicz.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2unzepqdr.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2rymgbyev.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2gflrnkkz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2nevcdfed.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2nkhfxpex.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2gwjlnuax.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2srrgetpj.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2tfmuvaom.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ektgqsgw.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2yafllsrj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yivxthjr.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2rxcyfnnd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2aeatncga.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2xmwehuon.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2rekholjd.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ttnlrqzx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2spcrqkgo.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2kkeladqp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2jgspgczy.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2usufvjgl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2kqkvijzz.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2culrcokj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2laysmkpx.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2kdcuuvjn.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mcecisrn.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2cxcpeoob.html


<!-- 参考信息 -->