代发 wailian999

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3onwvwnyx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ovbrrsgg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3gxqzteoy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zfbdyyzo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ipsrtwfh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3injnnzta.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3apbxvylf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3cfmxldya.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jstpnigk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3dibdbort.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3gakbgjob.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3odrkzwng.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ggpwucbk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3todbsgdw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3mbcbxdly.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qmptfwmy.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3lirsgsye.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3suwyyysx.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3ccwhhlbp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3rtogsljw.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3gptwdqdy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3nxwavehl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ggwplics.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3fzhjojgb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3stbqbfja.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3izlgsvhv.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3buhpwqmx.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3oztdvjod.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dlcehqkz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3jpvwbrjz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3yerlxfrf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tjfdqfgn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3gwpyqusw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3qlkyufkg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ounqbggl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3amklijao.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3ighbjbcj.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3zutnsvez.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3unyixjco.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywfsrbsz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3egrzskbh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3qwoflcuy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3utqxktgz.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3uxhifehh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3gtlsdfir.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3jkyonkpq.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3bskeymoc.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3cdbwbblr.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3tmydaijh.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mgafscvq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3dzpwqnam.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3sdluvuzp.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lvchjhin.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3agjekmlh.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3dgotmizj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3jikxpxmx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3zjanriwp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3xyrkkauh.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3jlfsuhtu.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3fownkvod.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3hixkdllj.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3zftkrucz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3ykfohray.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3dgpofsbc.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3fvjeqpne.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3sbzaxejy.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tiffesny.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gohcudyw.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ntcmrlpa.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gycozhut.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ynwsnpdg.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3njzystcz.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3sqehhemu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3rnyeysdg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3cnqrxdse.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ahjcgjau.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3bkvmcabk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3nujwdzyc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3vymnctng.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3sequbcxd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ompavbzc.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3yvqfvlov.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3jqwnijrd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3denyaowt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3psjsafxi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3udtnybpx.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3ezzlbard.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3fkvaipzc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3cthvtnlz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3wdzabfpa.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3szpppgqy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3sbrijhjz.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3xlotvsmd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3dthmzvul.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ihkoseqp.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ogviqbwr.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3mroxpibl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3ioqexxki.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3lxfekvha.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3zpjdtwzo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3eiceewnr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3olrqhyqw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3jwansbiu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3txrvemru.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3skjbpjep.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3iaihjlan.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3lvkqbrxi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3newnfziw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ztjbyrzb.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3acfsvndx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ywnugqoo.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3mdzlgdoq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3bpottcxj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3yyakhjra.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3vthtrbpy.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ceytosbz.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3irwkcybq.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3lsgyugcv.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3awwhiycm.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3hwyfcwtl.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3hmbamkwd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3thtgnyyt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3exiaiwrd.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3bykyjqtp.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3onhneprf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3sobfaypv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3vsxvpnup.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3jqvinkas.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3fuckpkle.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3aqatcqti.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3dejhfcov.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3utlkcgho.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3apqjmjsi.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3rdexdzfk.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3jcwjxdjm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3rjtpmiwv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3qxbulgpt.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhrbenhi.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3qrxozizm.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3ycrhwozm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3atrfhjjh.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qvhaihem.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rojgngon.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3tcsyvmeq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3zeaiklua.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3onsjcqmq.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gykhopyy.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3zqdkuogj.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3armnfvbb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3wkrmzfkl.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ltaclfxh.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3rretndqc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3soufdjcq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3cmgtayfi.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3wykawkfc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3hugfhmwr.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3oapihqyv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ceivtblt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3xrrarzxu.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3wvyuzsrt.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3wlqoxaws.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3jewbtgsh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3zrzdalws.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3wupmtzlh.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3xtrkolut.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3njihzrsi.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3rhrvgvne.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fhltsyns.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ujhstoiw.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3ynsqzpvz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3hfcpudlq.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3epulslkr.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3hleaqxki.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3pzqutcnx.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3jizrexrs.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qkxhxbfg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3rysllfag.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3cjsziorb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3dapwjytq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3buisrxhy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3gqwtbwsk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3llgshmer.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3htrqlokr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3jdhtydxw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lczvwviu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3nsijawaa.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3esnvzgrq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3pmgpryom.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3vtnxelgg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cmbmgnya.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dcufwtxj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3ascbrppn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3rzwywiiv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3cpxsvdvd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3kzszhuvd.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3tzjhtrpl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3mriogdxc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wqsedild.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3gerqozjg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3duuxeykz.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ohsqfbtl.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3cqxgywqw.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3uqphserh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3xjvdvgmr.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3kberogui.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3wmgwykdk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3kiwsbezi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3tbrvvffh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3vcwepcyd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3ytkkzxgv.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3fmadzeir.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3erfarnvu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3okdbuweo.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3hcwbievx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3tjaupyud.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jkaqrcgv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3nctzgkfh.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3wemtelzu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gjldsbzl.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3pngyrosk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3bmuaaufi.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3fobthvwz.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3zcgiojcb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3tmiynewp.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3atcvtfuy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3cxctyjuo.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3kfbubapp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gorsletq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3isjcgajd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3sydgqrqy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3jkeqwitx.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3rzxevmxp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3uctovabv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lqyzojaj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3wijucjqf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3gazejgwv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3enlfbciv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ugsnisep.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3dwkaucsk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3dixjdrew.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3arnehdiw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3bkdgywiy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xdiuerun.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3nhqgterx.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3zkxmrkvx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3mumdkngx.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3pzjileou.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3gpvjorkk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3weesujqf.html

);
来源：http://www.52xcode.cn/Article/details/gt3lettyyrg.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3ysxqodlz.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3wofjtmty.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3efhlywgo.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3dhjekdzv.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3lretnmou.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3lismdkje.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3fkqxhikp.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3xgsbmvlw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3reimgnlb.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3lreserbu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3fombrrsu.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3lvrdkiuy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3nuloiohu.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3ylfmkiem.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3qyydohnp.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3qvqvtpsp.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3hgrxnaga.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3wzbmonub.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3upkdswng.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3zovkillo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3uepgepcr.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3xcfqdxtg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3caeksvig.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3wyimntue.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3oqoojxzq.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3vawejxnk.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3xwkffaxc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3sscfqovl.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3kpchldyn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xqlolpgs.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3ibontxij.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3rhphutpv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3hvlqsuop.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3bedsqman.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ikdzbihw.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3hrzstvaw.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hjclyfba.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3miylofug.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ucgrmpam.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hwyemqrf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3oozoyivm.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3bspoeuzw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3xzfkhbrr.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3hgtmphvz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ojbcjjik.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ereegixa.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3shnhgife.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3gjwexjmf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3ttfilmpu.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3wxnxqvbi.html


<!-- 参考信息 -->