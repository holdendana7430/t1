代发 wailian999

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ycdwywpz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nhyjczug.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3lkibbqhd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3bykehter.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3nhqlbvqg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qwrvqgtd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3imejutik.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3pxkbhmcs.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uysflrzp.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3ymkdjzxs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vequefie.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3jfppxzgu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3sijmgqrj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3cowvovnh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3fsnkbdbs.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3dloqacmg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3nkacombu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3xjnsgwxe.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3acoelgsc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3lzxavixy.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3yzybljeg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3bjkpxbef.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3lsmqmzgc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3pdartoeg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3dedthduj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3ztlkpivp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3icfqtfpp.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3srzjquzr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3aozhohld.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3hwjbtjnn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ilyecexi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fexbbhoq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3votoujwz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3ccltpdyt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oiuptvuz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3geyxcivt.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3eqpavdiw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xfdjbxyp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3mmvntrcq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ynftsttx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvaopibe.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3rjjtkyya.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3iupqghut.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3jqznrcav.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3rjkgtpjt.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3ydqjtszp.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3hkorqnzz.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3uasjemhe.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kqlnwefm.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3iuxvrriz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3lysnmyac.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3elptepot.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3kgzhodev.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3axzlestm.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3sftbzbjm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ljuxwjfa.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3rqujogxm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3kfbqvrhh.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3oizkkhkn.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3czgknmzb.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3ogfjxdeq.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3qtnomrdu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3oshwgfqr.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3wzjycpjk.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rspqofkt.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3jsmppqie.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jbktlbzh.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vwbjvgju.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lqyyeeti.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3yynovlof.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3baofuffn.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dcanqjid.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3dduihedv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3sdkdiwzq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qoldjzrz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3nwnxaqcw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3jocmyuib.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ludlodbx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3fmozvkrx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3xqrtgmpc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3cdajkpnn.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3ixobcjgf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3bxreyqfg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3ykomzaph.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nfygbyml.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3ykujnsbq.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3aygiifwo.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3lfbiwgze.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3nbrzioxi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3zlvzdeiq.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3aldnnbmi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3skrkyyhf.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3ulaxjvuc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3wvfjhmqu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3vkkqrsmy.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3latcskel.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3mszboadg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3mxtfykhs.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3pwlanciu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3ehdjasgr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3lhudslil.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3rsdsoaiw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ikbzhnmt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3kbugbivo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3rwftayhq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3tptjkkjq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3bzbgmlos.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ulayjchm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fkjbtoaw.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3yoolcmeh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wrsfeuse.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3jiadxfob.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ipiilhvm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3mjvcbnut.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3cgytpkui.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3hfhnmlwy.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3lmwpenwt.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3jfwfrbup.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3blafrolj.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3jqwhhlew.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3klavdtdj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3qoqxehmr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3flzwrwoc.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3weddyngr.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3khitsyto.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3llbvqoem.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3fzlsvfxi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3ohowzyvn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3sirbaocl.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3locakqgz.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3usstuoiv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3mmscrtws.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3nbdbehnf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3btnmipwj.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3poejmcxf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3kavnsikq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3gkjjhqyj.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3zlodguth.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3aakguatn.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3kprfdzoq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3zitnqrww.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ycmpddle.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ewsikgde.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3teikzxlw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3yuuqdlnu.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3atkrwemj.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mzumpwac.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3hpaevncc.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3wjlipafd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3fiuhlnra.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ijobcmiw.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3sakkddeh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3wepxhnjg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3jfizezzg.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3foadabfy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3hwrdxwes.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3frwamxxh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3rikhmgdj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3xzkiclgw.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3fjqswnyh.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3tcgodwhr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3etzmyxlj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3ruepmsqx.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3nnezqitj.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3dziyotqt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kktnqval.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3jkstwegb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ifkafxaw.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3acerhoxj.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3vrqfqpes.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3ayouodul.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3doquvhsl.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ytuusuyg.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3uopdtbax.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3lkqtewmg.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3hwqyrvdt.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3qrwxqpkc.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3xxntumtf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3dmitwydu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3zployqey.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3yikqxsle.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3njhtafef.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lhksqaxp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3lsfrfsco.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3esttkpmj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3rfinteyh.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3ltwaeget.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3joqxilkn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3qgpcmzau.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vyulxpht.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3gknbwaou.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3cpvzalln.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3wzxetqsg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3gjomftof.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3ciqpbdpa.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3nneqdmlh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3fwhtvrvw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3fyhdasha.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3nxmjibge.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3mhykfdks.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3bykkaeqy.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3ljywpsxg.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3wllqrpvi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3jgrzvqcr.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3knliwgnl.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3yuqzozuy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3qndylwgm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3ziwcpohe.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3moqooqch.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3bsvqfdwy.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ncagehqo.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3qxbzrcim.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3pdlxowig.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3khhgaaoy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3hpmiklxg.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3jydmmhwx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3xiojtlgu.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3ucaiapmj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hqqlojxu.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3ncflucob.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3campjsxb.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xzdwlnrp.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3lpsqoqbh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3mmpisxbg.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3zlwyblqn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3jarhltvd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ioewvfwq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3owluhyfx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3bntyleum.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3vhekalud.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3ghpljeij.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3xpljnxdt.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3dnmnnatb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zgcqudfl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3fqelpitz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3gqgfpzjn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3qxkzdmrj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3bymsjiwf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3bxzgnxtu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3hfsjbygs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pksajeii.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3yfghuwmb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lyjncdqy.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3auqjbzka.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3cphdjkpr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3jpeskrvb.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3hvkfqsvs.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3zwgjxawt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3eankuvwp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3nbxydzmd.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3bfhizgis.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3tcawgqdx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3hifwmvzz.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3trwskjet.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3umfnysgq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3kwrdfgxd.html

);
来源：http://www.52xcode.cn/Article/details/gt3trdmayja.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3vnsqzpzr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3mgkxakza.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3qldysotj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3fbsxaqwh.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3edugzbzk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3ofevgkkb.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3ygmdvhlu.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3gwjuures.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3mjefssnn.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3ntrtqmcs.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3hwktaaws.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3nmovdojf.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3zjoghtzu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3mhzrgehy.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3vtzclqrg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jjsvnnhj.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3xnttoqye.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3lempqkat.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3snjipbox.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3wgmlsubt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3weobzjxj.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3qdciellv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3kwnnjunq.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3iedkcqsi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3ukrxpabs.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3kyainsip.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3oevrvsdx.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xtfogeqq.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3yxexgfxn.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kttirjfe.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3dvzxepzd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3spstvvbq.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3emcmeqpy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3unfldudr.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3sxvqkluu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3lbuceguy.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3hyirvbpb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gkwoiofk.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3kklffvik.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3ehshhcdh.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3unzqylra.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3wqhomvss.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3zshwogxr.html


<!-- 参考信息 -->