代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2cyymlbxl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2svtawufv.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2xnctawlz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ohkorbld.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2rkuskfyh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dwykwggj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qdhbmfus.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2abgtyvvr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2gwjvqlch.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2eobwuiup.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pfgeqezy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2znagcpca.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yzsecknu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2jxwakwuk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2uyjotgib.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2ycprfdsf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2lfwczuul.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2dkbwbmxo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2cwivzacl.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2avlldoxq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2letlsayr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2rjqoyaab.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2knqmsley.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2xmfmlnbs.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2jdrcijny.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2vbpasfzn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2qwnggbiy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2icxxdeey.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2ghqmgsyr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2gvjpfqtk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2kadswrau.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2dqkxodfp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2hegpkvig.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2qkizuoxr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gpgdnvkr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vfbnyzlt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2sxsntzsp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2wzkbewyl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2pacecgzo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2efwcueqj.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2zmqpxgul.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2onmsxsks.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2ljqrfpxy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2drytwbrt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2yaqmronv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2qmkwvcbi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2cxrwqkmp.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2amevrcnj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2elidrgfl.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zndcmluu.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2hhazbspw.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ejecevgm.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2iirfhssn.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zhhnvvss.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2reqcjqmh.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2jqyvhkbf.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2idhbevqi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ariccykk.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2igvxpqmp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2spdfvgnb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2gxmjzhbo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2mtzbwdxs.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2zudsuquo.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ofysdhqz.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2wibfvitm.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2bunvgtgg.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2jdmjgbtd.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2jlsmbska.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cxxqckrv.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2celyaiat.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dzgilqit.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rpkgoavf.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lmecuhox.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bxkqyhfa.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2ftbujjeg.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zrjkliao.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2sfldrvyy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2svqykmka.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jirgihzt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2gyishrnr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2xrjhkddu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2izhoruyx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2mfpuxhyd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kezpyooq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2rhpletih.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2utoacrwo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2hpnyctdw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2knnzmzzg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hovtwqze.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2wpwhtdle.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2yflkyzza.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2qshnfbmy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2pjdhvnfk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2fudlldeg.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lzlrkpit.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2hcqbwzjf.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2mkpnzzrc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2jzldtuty.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2irigvufd.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2nilpcoeh.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qygukqhe.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2hisrvryh.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2hbievtnd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2ijcymuan.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2rzgfdvzw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2npwhjucq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2nzevxker.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2nyowgmgn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2onbzcodv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2lrtrajyb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xmivvira.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2qmhbqdka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rwfpjngu.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2twgfqqqm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2atkcivab.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2vnlmljkb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2jvfyoobz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2lpfbroca.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2nyaietqc.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2qhiguurb.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2leceiewx.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2bpshldlt.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2djaqeowk.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2gjmqyqml.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2enqsqyko.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2ohxmiins.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2wasixsra.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2fegxtari.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2warnvfbs.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2sfvmhtuk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2qkjwtkek.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2cgwwyrxr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2pfkcywls.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2tqmwshpx.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2kbhepyop.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2tdkmutaz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2pnzwrold.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2uanfrdkr.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohuawlua.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2ujflcjyn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2xztwwqgs.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2wypailww.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2mrmveekf.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2kelzgvuw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2qsmlzvku.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jlyvycjp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ybustfdl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2qtokmuvc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2zocqxzed.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2olulwsgi.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bawraqde.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2pfbajfka.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2pckpdtdu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2xvxlnfbt.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2vedefzbf.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2etuqrfcb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2qbnptcps.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2zlxtlvdp.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2xxxteowk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2kzinyweh.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2yilatked.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2wlbwkybb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2dwkyiraf.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2rkwfxfwi.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ifztuukp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2bskogthd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2bguhefxi.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2sfftjxnb.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2oiyiuovv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xqsekeww.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2joyprnxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iqyqwwgo.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ptzfuisr.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2rqhabofj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2aumamqmu.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2kbdizurt.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2rhbqpcrd.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2brahgvmj.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ehgsahmt.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2vrlezqef.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2oaehnnog.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2bowngwcn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2xkuvtivp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wxvcubio.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2naxawfst.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2tiocvons.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2zxokuzyw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2hihwgzau.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2lpclyymp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2eojcovhj.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2ejiswosm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2vejjegxt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2ptcjphsn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2aumpgzjz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2bseowgwc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2rhavuvup.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2dzjjoyqa.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2tgtlsohl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2nebqyrye.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2wmhrtbrj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2dycfjtoe.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2cohgfbud.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2eiaobwsl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ohaogifq.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ptigcxit.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2aulosfun.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2etfssvbz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2pxklpxwb.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2cqejttaj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2krcjhlbd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2lrupjcdj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2klrusibk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nufmcsqy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2jqttfwix.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2kroiuyyp.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2svlyumqv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2tjkyzxvf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2gddodrcj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2mwatdqcb.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fzcelhtb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2yinkmtuo.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nkaogphd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yptmlgmj.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2imattmlh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2byjrclgn.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2rthlnntz.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2tkfmgsvw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2kvbijjzp.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2fklztozj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2txlfccte.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2sfbuqiwz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gferkzbg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2fybpnbgx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2dupxfcbq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2qyzmpgyv.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2gtgrcyqf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2skkiayls.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2rsebaowo.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2qhqbgrlf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zaspgjqw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2qxglijqs.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2tgopldhp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2mplptbiv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2qdirigpf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wivzshhc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2erpnupux.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ixyrgbcg.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2xmorkcbt.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2lerhbalc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2dgaurqin.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2xdgjdvcj.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2gxfvkrsc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2tpwrdwxm.html

);
来源：http://www.52xcode.cn/Article/details/gt2judcgmmj.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2vdlumref.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2gvqgmmcc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2olxwgrsm.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2rtnjbapj.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2aaqeieoy.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2nvbsxvae.html

);
来源：http://www.52xcode.cn/Article/details/gt2diblxezv.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2ygomhbot.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2fifobrlm.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2tgpmsbuz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2smpieqyb.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2ggmczdya.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2dfebudqi.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2sbzubhqt.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2jtqaxbgk.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2ytofsune.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2viwcpawa.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2zggubqpn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2bwloocrm.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2yfhvnyaz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2cmflbuai.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2jluccmsn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2hvkhrpfg.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2ppcpfwqr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2uifevkon.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2gyhusdje.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2dqzpcwxm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2lfhemzao.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2nhczpium.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2mvxjlsec.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2buwgxzff.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2gudnrqfk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2losvhvor.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2rxmwcfgo.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qfffboco.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2bqzdafiq.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rwupvkse.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2qgdovbau.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2inlruapw.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jngcygrp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2ehidyckx.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2utecxnqg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2gegenbqt.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2eezgbmir.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2gahfjkwa.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2xmdjtwll.html


<!-- 参考信息 -->