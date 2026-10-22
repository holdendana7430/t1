代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2crznixrt.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wyirubpu.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bfzhjzec.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2dqkwdvuf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2aknjcwxx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2xtkwkmkp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2mhbbtbxo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2nmlhdzgf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2qojqoqfv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2aommcauh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2aoglfjax.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2kkhnogxc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ptkifkfq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2xjtqfzaw.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2oqgivpeo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2mxzfquor.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2cwgfrljn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2mgfptlks.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ilmorfkz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2cohkyfqa.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2wszmcrcc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2xrulsqjf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2jlftzxcu.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2pagzxiop.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2evynysbz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2dormadfq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2kuooflhx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jjlyfdno.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2jietctxn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2cqdudlrf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2fockhgyn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mzfvuokb.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2zwlfetfm.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qygaymlm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2mcbknpfg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2lizsvlpc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ccytrdlo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2jafoiixq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2ulhtkbjk.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2kdekrfmy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2igbrhupc.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hohvwlos.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ivoqciyw.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2hlbcgfkq.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bbdzvyfs.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gjnraksm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2fcezckax.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2kakjwvke.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2aswmmwvm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2whrfyumf.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2ukixvdbn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2xifhfcwd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2cenrghit.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2njvbtyjr.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2hbsobgxy.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2xfqfbrlr.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2refsovhd.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2dyyymeqe.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2ipcdnfvn.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2vivcylxa.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yggdfwlq.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2rvnshtpn.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wmdelfyn.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2odvgmedq.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qwklgrqv.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2itboscjf.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2knuyesrk.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jlbxkzhb.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2hmezunbo.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2qhxbctal.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2omkltdqa.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2zeazffmg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2puonkgyt.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ghtqpfqb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2vddpahgx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2eocxyyky.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2qmcykymy.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2gohgeemg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2pqmjngzm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqhzpyqe.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bfdibgpg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2ilhfnfvm.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2dvkszalk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2aettcnzk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2dwhilyed.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzmhxebk.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kuwrgxyc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2uhhgvovm.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2vweuyrdd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2bkmytejh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ltttujql.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2juyxzpcp.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2bzujvykh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2pwyvgplv.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zubxtgia.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2pauwuhvd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2tczwjgkc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2xijdipeu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2drwhspka.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2qbipqqry.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2yexqppmn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2ffthmnqs.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2izkiujmm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2sbgzsgwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2srosnefc.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2efzlojsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rzpoypai.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2akeixhhn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2xikedyjf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2jdobxtja.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2xrgecxrz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2tnzrvoxx.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2nhutwdcs.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2qhpaldes.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2nqncdwot.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2bppfsdao.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2iftdukeg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2gjrwminc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2xabwerrb.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2nucenlqj.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2zhbzbzoh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2vhkpcqdl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2nuvdinnv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2ybyxapgq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2vbwfrwuy.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2frvblrgg.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2lzsnudqr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2kjjlwogs.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2jkgfsiho.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2sselxexl.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2odwyqlcp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2dwfmexbo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2sqrbjjrh.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2kdzncpbu.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2zrrnebgn.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2ucqagoks.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2heufggzc.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2avewximg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2eeeohkzz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2eyhtsxxf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2vbeeharn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2dgnxhxxv.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pyshibtm.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2uguvwbut.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2cudqvgpn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2jroeziax.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2vpwagbxb.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2fxpxakfu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2igketxnk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2qxdfvxft.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2rgryclmz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2eafcgmbz.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2pvjatehh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2eiqgejny.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2sbxdyjfl.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2dkgvnklc.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2coxyllfb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2ovjoxuzo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2gmkgyfic.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2qeglfhyj.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2ohfaxzec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fisnziha.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2uoetewue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hhnbeyyx.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2pkdlzras.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2ojoheixq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2egyucdib.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2dtnowlqt.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2cztoizwf.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qyzchgfy.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2emepojqj.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2bhkzntkt.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2yraoeeol.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2kivstdmm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2fmlamxfp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2ubtytvsq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2twhexxta.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2hdtyfwmb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2nswzrylt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2rcetsywc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2ikkzlxep.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2pbmymdcd.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2knarpjck.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2zgtlnfng.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2ufvblipb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gkzemfoh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2zoqjwcoh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2iqnokkhf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2cgfeqczw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2magrgoti.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2rpedysil.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2siycbglv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2isowvukc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2cxqwlswf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2awkhtbqx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2wzgywsmv.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2plogggbm.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2reefqiba.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2ustmnzkx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2fgxpdkrm.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2owuqflff.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2dhztjfdg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2offlbcae.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2fulmkqzg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2htxksblu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2rxsbtnen.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2foxqyfjl.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2zccwpyql.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2tfocsppb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2fucjdflv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2iggrednr.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmvyaqom.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2vpcvwzik.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2gjjrfmqu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2klaahxsj.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2xxrhqfra.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2hvjtigvc.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2smabsvch.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2jkgbngsz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2wgwmhbxl.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2wgihdbih.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qwhcwwjd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2fftrdxad.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2efwybxje.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2wihusgba.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2rpqahgkb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2vvbrfiat.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2marrdgtx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2aodcgtmt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2deuslkhx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2atmmvmfr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2kkymlxmh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2hdzrhdqr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2cpotxnpt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2hghaaifu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2abmusmyd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ugagoebb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2bypmdizg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vqrtimhe.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2bwdivifd.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2yoikgiuv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2pdyamuyo.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2dukwffxj.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2gebypouz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2uuschhpm.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2bxjwbmhh.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2qgtvvjyz.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2nxvfgcoe.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2djuwajjt.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ybcuqbyu.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2akpippdg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2czkfjsok.html

);
来源：http://www.52xcode.cn/Article/details/gt2jdwxjzjq.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2zejvwtje.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2vsfkketo.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2tqerkzgk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2hxjioelf.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2pcjwthgh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2huxztzyy.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2agxpiyea.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2oaeyjata.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2gnyjdalp.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2uaaayuci.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2snlzcnwq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2jmonqwar.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2aezfzqxr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2jatqsqbe.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2sbmyvccc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xtelbrpi.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2jpritraq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2vbarzccr.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2iqvekknt.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2qdymusvg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ieydkuao.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2gqmbszza.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2qjocloxx.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2tdqlhirr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2ohfulibd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2eiebrlff.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2fxhwtyyb.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jnttkgli.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2vsssrtxy.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nsehlhmr.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2duselmvr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2brplmqzf.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2yzjocscs.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2tsjmadli.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2gngeuyeb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2oywgiigr.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2dnjxfwcg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2tozjwkoy.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2budbuqmn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2rhdxnxul.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2jphjwxfr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2cvirdjdd.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2rrvnvuoh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ecensksk.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2sspuzobf.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tfzctvwc.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2nfbewvqz.html


<!-- 参考信息 -->