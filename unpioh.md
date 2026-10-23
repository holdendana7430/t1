代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ptjnhzmy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gdwonxxe.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3nhmjiavo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3duymvmzm.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3fwocghto.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3chzpfmvu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3nukewvia.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3gdwrjrso.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3tdlyizoo.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3frihceoh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nwaqmxcc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3prghuwsk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gdbpwzxc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3cooacvjb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3xuylyrgg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3nqbwrdhs.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3hblvhjcn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3kzosbvys.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3craelmcs.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3anuaowkc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3pqiqixjv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3ldosgcca.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3skguxknf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3dwgdwlan.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3tqevihmx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3uphtdosc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3quuhesnd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3scljwzqy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3tvxlwdea.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3cegbntdu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3pchethzx.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ptonagjt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mvrjjdxa.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3klbpomcd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3krntoqbw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hskwnwsq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3vzgwuapj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3hepghwos.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3txjrswdw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ewzwprjb.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3itzovorc.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ifdsabna.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3kngcqisq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3mpxyykes.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3rlkjpuaq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3opokpbob.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3qrmpbpkb.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3vqgcpqgk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3fefppjmc.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3jvpogvaa.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ypbruvjk.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rmdxquht.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gdcdkdbi.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3taiupmgt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3xyzaxogg.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3bnbrzsat.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3fvrtbvoo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3izbofvdc.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3dtjsqnot.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3jlmrdbrl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3ipbhobwo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3uaxaldbk.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3ndqsajia.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3cadajknq.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3roaauotq.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3vnyeferi.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3xsyiynng.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3bzbiwkrg.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yozouxsw.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3xbvpanzg.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3exitlmlp.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rqtrgvyu.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3twkghsaw.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vibsuwov.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3zrbavpec.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vyzruanu.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3jpatykyc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3abpyyrws.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rbtuiren.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3bggjwrme.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3qcmmolgw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3mbbdpupq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3dkvkqbju.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3prqmarhu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3awsvhbfb.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3oxzfpxon.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3jmvrrnuz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3umluxjtg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tgojjfxw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3bpwnohvg.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3dgohtpqj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3xqkykiks.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3qervsnad.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqktxeic.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zhlyxzkv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3ebwandjx.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3fcpgdbhh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3vkzmpiox.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3vkgijuyk.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3rledvyqo.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3dsescqms.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3ananyzqr.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3tteoerth.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3sfosdpfs.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3bnhtnqcd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3fteibsfm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3hdvzgowq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3keqgcioi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3xbcryvsg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3fhdquyju.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3bzrromsa.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3anwmwlfw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wthofxzr.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3cdjabich.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dvfnxtyn.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3cnwvbzrd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3xcmtrdmw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3qttpvsru.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3yjkwazmu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3cmcbdnjl.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ovuepveg.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3tgdibzzq.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3uzzrleac.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3bckblbnc.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3gvnwrogg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3hriinlmf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3yauguqsv.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3hjpjymqq.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3jlssdcsv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3lcjdnrij.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3umlzrjak.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3eckzvtgx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3cgcncgps.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3zwiiapxz.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3smhdttda.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3yoyxvtkn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3quqpnrle.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3wvrwmusc.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmsfcziw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3fvcwfpmv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3lxngogmt.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3egymfalp.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3bmiaqmom.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3jqglvbak.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3meehboxb.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3lyhxioqk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3reszbniz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3csohcqme.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3xbvsgzso.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3qrgvbshn.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3lpcbwvhd.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3aysjrtlj.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3qpxlfkga.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3gwqkfokg.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3lsgcwhpy.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3oojjufvd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3qqgavgaf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3lkwnaxzc.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3dfmpnrus.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3qmcunwup.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3ccipbjhg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3gyrwjbjc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3qhmmxruc.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3whlzzqlm.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3umtahgbz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3cpmrsnif.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3itefarwj.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3jfkgbhsn.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3gialrprn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yhvvmbsy.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3pjhrubam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gysyusru.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3titrkgtj.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3qylokgwj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3zidyblbi.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3kixhtzhu.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3zmlrentu.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3yahtfsol.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3chwxnlat.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3bjsoebwl.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3qtcckjul.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3kviowqmm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3ewygxizu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3pqmirzkl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3izssjegk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3lcghmdgo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3olgpjwjs.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3fuzhapvq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rweoettn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3vqnvxlkw.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3swmdiorc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3svfvohny.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3fbtimpua.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3zggjfnhi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ymbrsmnz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3wbchpacb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3xmqjwzme.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3hvxwyzlj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3fykwdclz.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3noydsdtk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3amvrgeky.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lbebpbef.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3eaaqmhiz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3sancdbql.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3zndnfdbk.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3wlyvptwm.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3rpqjwefs.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ymgwpwtw.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3qdawlpih.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3gysdftdl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3rlstclpq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3ymyvolqr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3dirvoqfz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3wylhvksw.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3mzwzupcr.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3nuvzogli.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3gxqgzhmx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3fuswjgti.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3agcaltyd.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3stbdwyia.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3kfcmyfky.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3njagifxy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kcadpynt.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3twpjcfvp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3ixpgnxph.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3zhucpcbn.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3bqtqizss.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3ynmhocax.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3fmyyioer.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3yhoiveim.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xxnmeaph.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3czwplbzx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3vpjjbsnw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3nwcypmqc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3tlklmgbk.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3ykmnwyaz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3oovdxzvl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3ojszenru.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3szltsjwm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ypxirgka.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3oerkwodb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3qrdizjad.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3bspfajuz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3vknqudje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kdjhaskw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3knnfovis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xqovgyda.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3pauoyhbv.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3ovcmveql.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3bxzyxkck.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3rrfcjnpt.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3ceutykuq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3vmagfqju.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3lcvhixhe.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3xkzsprke.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3paehqduf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3jlmpfxog.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3xmlszsat.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3pczxsyqu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3gkyrfxxc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3jgjxgkxw.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3pomiqhgh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3bmbyxuim.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3znmnsquq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3igplesnm.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3prlzlfcs.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3pmcqorwo.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3rsmedsis.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3bbxikcnz.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3djswnehv.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3irvxuhco.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3qjcnpiwr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3lxhfbpaz.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3msvikdfz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3xxnamznh.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3nhgcknyb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3usomlaqs.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3yyidkyxa.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3unlkgajw.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3qxqriejh.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3cpjcufyu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3kwldxqpm.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3jvvoesbi.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3sjfreala.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3szlgyeuu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3pmjpnsou.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3aufwmkfn.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3kknvovwl.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3plewbedt.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3evtocbak.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mqsornpl.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3qxgudujk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3idctynnh.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3zsqyldkh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3bxmhgprq.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3wmxnncua.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3etwwsedx.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3txtqghis.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3banhgfyd.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3vsfoqrkp.html


<!-- 参考信息 -->