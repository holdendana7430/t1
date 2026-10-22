代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2bmkaexiw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zangjlhf.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2fifubcjp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tcgqmikz.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2tgwihdvn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qnfgnbrj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2txdhcjzz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2sruelttl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2mfkedcsn.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fnfpoqwb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lmnpcvqr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2hbejxkzw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bzrnmdej.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2qyhiecor.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2gerrgfkq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ffwpboet.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wchykwfp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2shrhciuq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ecfmpxqa.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wlnldqdt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2kiuguldx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2cwejeeha.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2yadzkfoy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2tygxtbnm.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2ebulgxyv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2xtzwyrtq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ajcpgohm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2npczsnts.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2bggbukuy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2nkczicjl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2vadqjvwr.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2pfeaahmx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2pnkwiihg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2lpymmixc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2jvkinqrg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hoihhogs.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2gsiskkel.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2bdjxrado.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2teaztafx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nmwtzbuo.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2vtjlmyvu.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2pzklmwdl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ycvvhvle.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2sqfmymfl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xnmngrin.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2tohuvvgk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2tbiucjds.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2ipoczchp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2mlxamjem.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2rumjwjea.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2xxduzjlh.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2guzugnxt.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2arjucplt.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ryrjolly.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2gybpzwgs.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2wwjwztyu.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zwejfgcw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2xfhzhuqg.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2zgbahldn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2mknmzlwi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2nltifcds.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2phesvyxw.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ngrqyaww.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2krautath.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2ieianwjk.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2pwpxjadh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2amijypmf.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2wwqujvcl.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cgopscso.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2lmjiogbz.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jklxqpss.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vbpgzmuu.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cjbqshyf.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ixdavtey.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2rzkjgkmc.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lcjmtrrx.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2jrsdsenz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2araqrncf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2uqefaeix.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gaifkhfq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2zqrcunsx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2gncevtbi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2embbxwbj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2sqymqgou.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ojeskvri.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2bmjbagpg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2pkjmtdlq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2ryxfwmyg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2fgvaijdc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2lqbjujkl.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2qummwgcp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2roixbqev.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2tselwvdf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2xkzncugr.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fooccbvl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2jqeviihi.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2crxwpabo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ibwlpijr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2kcrkkchb.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2baywwizu.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2gzzwdyyw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2crsddgpi.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2reokpuen.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2qajcwmqz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2llbgmplz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2xzvqwhup.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2wuqzqpcy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2tzdaxcrw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2hwtmkido.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2ilayvtti.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2lnhcwurh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2szsfhrbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vuuqbauj.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2qwygfihi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rzulvehh.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2skvzfvpl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ppaurbxo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2rjkejsls.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2xcrrsamk.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2zcvjmffy.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2gndrbnhj.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2fgdzqcyw.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2fvszkucx.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2lhihwepy.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2aptuahqh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2scjtkgpl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2huhesvin.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2tigjyjqb.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ujhujorh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2vbjsxzgt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2djuyeoum.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2njrssbzy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2jnbczban.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2zopqnymw.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2lyonjtld.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2hgdbarhu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2npxmaxyk.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2pxyvdcyn.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2tutxufsc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2gomhimpd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2odsafrfz.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2vulepfcb.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2vgtwndfo.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2ckeptcfr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2raxptogz.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mtklzsmq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kkzmywrc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2sqjoobuh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2tpqprfmx.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2ztoyrrpq.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jqmniwbo.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2lsebkiwz.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2kbiosfgd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2ougfnapa.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2empqlkbe.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2jvjgcdiq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2etlcxtqd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2btwzlquy.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2pnbljlru.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2parhjkjx.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2tlrxzbkf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2awbwsqvj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2srtyigso.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2pewyreyx.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2qwhkwlct.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2nbskmbzt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2xzlrlmxb.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2dvgwrsnk.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2cehpxakb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iwsjszne.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2brpxwhgt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ljnggswp.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2raurabfi.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2eashvrvb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2wmiggslf.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2eeszfolx.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2csdtfeft.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zomlodht.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2dqcjnvrr.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2pvutozzm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2phgvcjry.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2mxgmxtve.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2dsopvoen.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2kgvmxjnf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2oknytumz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2xphklpgt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ningemcw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2hxsmvczc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mcyvczfl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2aupobfao.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dgeowdqn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2gsftkzin.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2qzmfmqgz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2wdqkyxtt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ntrbkyjz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2pxvcndtf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2sssklluv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2odvdoodz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2rotlbrpy.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2akbdsrtb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2yyjhdbrl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2szcfyxqd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2fdclxjtg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2airatrxk.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2pvzgdxby.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2smkgzpla.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2ouhrryhn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2jamilfnf.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2lzeifgyo.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2afqdbhch.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2qroiofju.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2ygapdswj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tuwsdjxz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2mapyffob.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hsibxxvt.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2cllbtdyf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2jkemldpf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2wtdvcvlr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2vnhfkhbd.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2felbrcmw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2wybwgapr.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2mfsmkxrh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ymbzwxtz.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2yhdgypic.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2isflqhcz.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2gabrqefm.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2cnpkbgnq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2kgcxmixc.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2pqpnpfcc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qhrqdjwb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ynyjtuet.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sczikpbi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2wmxmmklh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2facmgncb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2ppxsyivy.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2ywrwktdp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2symxigmw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2cdmefnci.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2fbfdbtlx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vywozasx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2bettzhbq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2xptmjlke.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2jldmxzgy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2btzqlfve.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ajzatokf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2ffwezvre.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pmzwtcsi.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2srdmutgb.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2qwhrwchd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2gxuzfpcy.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2lsomaldw.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2bggcoonn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2cnohydlg.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2azjlbinm.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2bwedthcq.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2ppremisq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2pknhpicg.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2tazgvxht.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2ongakcgn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2huxhmeki.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2feypzcfg.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2caebsryj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2dtincfes.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2hvssuwzw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2uylmwybg.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2jvvscmum.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2aducslmq.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2rblengja.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2fouerzpt.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2tuzceufv.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2cdrxpjcu.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2tafoqmsd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2glgtyrtj.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2tqikhfnn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2babvaqau.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2hykyomlk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2udlajqwg.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2gyomqdxl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2fhdbvvgz.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2rqoexwyi.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2epmvkhjz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2gkvmwihb.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2nqsvgjeg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2qevqipqg.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2jzgvwauy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2hnqrkxee.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2btnyvsot.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2ddcsgqqq.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2azgpufei.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2wxdgqkxn.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2runimotb.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2gqwgtdnp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2kojdksgn.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2xsetocjv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2sqwiadri.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2teiilpfo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2hbflbupv.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ggbonxdk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bhprzhal.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2fmvbkqcc.html


<!-- 参考信息 -->