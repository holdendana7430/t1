代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3gxdvhjxq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yoozglsj.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3zwndtpqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nxfbngdu.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3hjymxplj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gmpszjnu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3hqrpjcte.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3mzohlwbl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3wsldqjlo.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tdkdvbdh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jhtgmgsd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3nyrfthcd.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rklucaks.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3dprrrmqg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3qqzjhexh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3gewesfls.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3uxjcpuqe.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qaenjtos.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3mwxjsqjv.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3fdbvjtvf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qrzcxnxo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3lmmgjezz.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3vnyzrthj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3hjhhwjjn.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3hmwbmgiq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3vvngkdmk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3djtwulmi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qelyzzan.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3cfxjoijy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3unhgxvxi.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3xpavogeh.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3uxdmixhd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ouratceo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3dhtztyeu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3knayfymc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dnxhczop.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ehogzhno.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3zmogiufq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ezhrkzdg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3eunigxxb.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3ohevnpuu.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3imwlvtvv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3akituavp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3uqfywmlb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxzdumyc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3lhzpjzit.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3hudkcrlg.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3ccjslvfy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3bvsnhguq.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3krnuidub.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3gvvmzdnr.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3tqmigcsn.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nrrlplbq.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zvcmtfzm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3mppjqsyl.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3iplznzft.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mwsfjmgz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ijuztqrg.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3hogvpztn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3wdnhmiwu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3kniznfee.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3texeuosn.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3zfgdvqvt.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3mueazxkv.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3yokojbtr.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3nmvxkvvl.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3aepqogys.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3skphgsjg.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3tamrxilt.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3jkwkskub.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3idqendmf.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hqtrsszw.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cnvyhudl.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mcglwxio.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3zbynddym.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ricwcqkw.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3xxrwvllq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ydgnvnww.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3olpdxond.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3rtryfkol.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3kqilnjas.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3oysbagvj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3gbxlekgj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3uzzpmezu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3fucxjurr.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3lsvniokx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3utwrpgmz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3rhbvisei.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cdpqpmnm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3nwzjiwpg.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3jrmmeyln.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3oitmndfi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3pzjczekv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3isouyydb.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3afaeaigo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3jhjpqbfe.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3gwptlimt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3paazvmeb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3eanqjhcf.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3dfotyicu.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3bmuefdwe.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3ojjxoqch.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3bpaotvdo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3djrqbecc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3kuokbiec.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3fzrcfxux.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3afmlimfg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3mhoklhrg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3depfjicf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3yecqyyar.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3uaisngvw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3bucfhuul.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ancivgkn.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3tbapzufb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yokqnqsg.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3jpcmdzmb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3zfpwsdsd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3pkrnfiah.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3yqilscwc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3inhqrazx.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3wibumtug.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3xfnxidwn.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3aqjmatoe.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3fawfttew.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3tcsgfjsf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3zbgqhchb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3tqejkyeu.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3nblvexnb.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3wbhhzedh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3owovajnj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3mdssmrrn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3mhbmghub.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3ddmqeggc.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3urfpqgqh.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3fplckiat.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3pkhwwptg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3ekajklne.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3zcghtdvb.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3iifgdiny.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3vomqmdyw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3brncetow.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxkdllev.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ebjkztzv.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3ytkqcsnt.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3coatbzze.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3scqosyif.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rhkluwmt.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3tsxncoae.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3eeomyzju.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3oixcoliv.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tdaueagx.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3loufugqv.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3reqtafoi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3uvnwzdvu.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3fgafposx.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3dgtigfdv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3tgghjjvf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3uxefvmmc.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3dkvqxuvi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3ckoebqvo.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3vmvdhijp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3pkjwpofr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3yfotnucl.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3shzxnsar.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3medwbabw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3bfhmrflo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3mzaysdfk.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3vnoxnrwo.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3wrkixrdm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rtbsnnwh.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3shhaqmet.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fghewkow.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3odbcpnhh.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3dghtqnri.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qztdynbx.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3pqqnduih.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3sjqvifwj.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wxipjmie.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3gyutwhlv.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3twdkmesu.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3acdxkgld.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3qwtqotls.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3ntahsoxv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3ackzsxbr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3qtmgzamn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3ltmtmcjt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3sumudxqk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3vtpnzcgz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3veersppe.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3moqxsjak.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cgznlewa.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3begewlpm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3jppepyyj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nndralby.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3kendmxmx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3yzfirdam.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3eqdblfvg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3nvsncues.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3ncmadgaw.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3kdozypfe.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3stfqincs.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3onqvqnhn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3tdvfarnv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ktnlwqqf.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3mceeetys.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3oazbumyh.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3nubdgfwn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3jxiyonke.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3brqmjstp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3eowphmuh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3mjjhyfiv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3iwmimnme.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bcbnpnbd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3fwlogkfp.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3dgocgbnx.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3ljgfthab.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3nkycffij.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3qiwqsdkx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3jxvztwsg.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3fwancjdm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3fvsuavsv.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sofonsft.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gqtmneio.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3gknrhigb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3hotefynu.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hizrkxpb.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3juwhcusi.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3pfmzmaeu.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3rslcwcbs.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3gyxwwzvg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jjlulmyu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hjzswnpb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3mqhhrivq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3hdfpojlu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3bunkvksf.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3gxobepir.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3dxqluaaz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3waeznzsy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3jswwvgyp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3zdkagzjs.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3gbfbppsj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3ixwofvko.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3rwxhfgnk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3ihkaabbj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3humouofl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3kkkvtpga.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dipvwmwf.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3sumuzaxc.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3qbdqybzd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3cwhhdzhs.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3uwjasbww.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3wpnzwfqg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3uzbhzeqh.html

);
来源：http://www.52xcode.cn/Article/details/gt3nhvpfpyf.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3fwblzopf.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3wwqvasgk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3eietezrl.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3mhsredra.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3oifwtgch.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3xtvefpne.html

);
来源：http://www.52xcode.cn/Article/details/gt3ghkhzojq.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3wjuuqsac.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3lrhvjhpw.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3twyvhuhs.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3aucseash.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3xselbior.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3hjsxtmbq.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3nklrrazo.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3ddjnqogk.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3xwbibtia.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dfnacssm.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3qlgvqfkz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3kzdzpxem.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3qnyzdugk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3vppcwfgp.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3ymycvgee.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3gwhexzuk.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3vzjfnkob.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3efzoskrt.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3wojybevs.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3zrdmjctq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3ccorszjb.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3krfnrxde.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ruwidpea.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3iwyvhcha.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3jgcdjjzk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3gmqajnin.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3wwxdpwpc.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ogyjlpyc.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3hjrercpz.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3axaeqsnt.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3rcvxszwu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3xaodpzim.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3rnbljfbx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3snboqapj.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3eelfdsre.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3kivesstg.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3bnxbvyhu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3bkkmzuam.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ovrrqmxh.html


<!-- 参考信息 -->