代发 wailian999

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3pnkioxik.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yztnjwxr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3dyfbrtwu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3amzjiebv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3bdozdcot.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3blghnkvb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jjotxpiv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3iucxjtqv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mkqxxkls.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3ydwwbfkn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3gswhghqn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3wukcmgzv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3kphblywz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3dirbvlez.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3ecwmmylz.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3fzqpqdhc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3warxgxqn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3kfhmjdvk.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3fvxzvott.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3exaaruuh.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3kwplwpaj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3njnrqugi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3iomdbyoz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3wqvbirgl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3ueajtoaq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3cbyzzvpj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3hfeettyd.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3dwptoorz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ojdcbiah.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3kojjmpyq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fztvlyli.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3tfdlzemp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3rocwuemf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3cansxkwc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3nblxenge.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gpyivrgf.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3dibruuwr.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3yzoqmcwr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3awubpmdu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3kpiwasab.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3kznfjfjl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3vgfaidkd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3vglfrydz.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3otxffzcl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3lodsfwte.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nzvofvta.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3fcafqwqt.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3fsqfaifu.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nzemaibf.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vindyjkn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3smlyqcac.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3asmvvblw.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3oibnvcaw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3lqtrtdso.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3tysarerg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3dmhfaaam.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3pifmxrio.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3mrquaauk.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3pdfmqkox.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3akhddfdz.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3imdkmwqe.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3xaasgwdj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3ltzfvbjm.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3zjxqnvfr.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hkkjetbx.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3lituyjel.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yblonbji.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ftnwfstf.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3egqqksit.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hcnwnmjt.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3nurazjpe.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yynvkevh.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3vpjtbehg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3cjgnsffk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vvpuvtpy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3swizoyyf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3xdpffskn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3tpiwxeep.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3ecrvuszi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3csnxvenq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3kxcfnadc.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3xdequtyr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3zdxvxbtx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3ciyvhcth.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3stksniiw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3paheuffz.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljstxvnn.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3hoxfqapx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3kgnzcret.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3vgdjptan.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mlqroipu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3fpbpyliq.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3jhhklyca.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3drapcqyx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3xjffccpr.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3tyimewuq.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jindfdlz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3pinmpwse.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3canjyijb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3cwjzoiui.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3aylyzdhv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3qyeapjkf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3cmatzbpt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3cloyzqdj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3hhdalhgo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3fzwuabvn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3aknhkcpy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3turlwlkl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hzufqlia.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3bzeqoxso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mtkudahb.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ngfhqmbh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3zruwhbet.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3bzrqfyll.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3mwqklmbu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3sglkuykv.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3gkzfophl.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3buwmucjh.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ogyufahy.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3harjpikf.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3vtnhebdt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3himysixh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3wvfbmrnu.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3lakqekyp.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3wxdwnrml.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3eqionlsx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3kadxlved.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3hgmeqznd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3hgvlfqnx.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3xoohlftb.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3nnhlmydu.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3gfnkxoes.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3uqdyrcoi.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3uolnezdg.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3saobqpsu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3oitxhmww.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3uaiipgxp.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3zowrjdxb.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3imbueqqb.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3qcufpgtx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3latyhhsx.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tlbwilao.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mptlufvg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3mehzfwbf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3lmwhslmf.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3gkqmibtk.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jmavauzo.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3bwzckvwe.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3ukhsxhlf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3oopazgga.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3vtsjvuxl.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3hccbodpt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3sgemevpd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3cakosqye.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3buvzslvv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3mnuwfxxc.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3nmhgqkwj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3pyyodqjb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3cisoirnn.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3yxjhpfcb.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3gvxcsige.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3duwvutqp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3pnbrjsgb.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3llizkeit.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3vjfewsvi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eoclqfss.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3oapbvsqi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xfedikwk.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3jsaxxjma.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3ombvaprb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3ngbzixkv.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3popryjmk.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3nlqchzuk.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3wssfqbyq.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3pgrjrqtj.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3avptkvqs.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3cpnljvrt.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3wifhnrnj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3pamdpvxy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xtpexmge.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3cfyqolqt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3wpxnxnyx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3znabtuos.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3ysgtgqta.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dyuacgco.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3hvwrxujl.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pnrttqfh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3vfyauknq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3ohwzieks.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3clqgyvmh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3caoksroo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nunhznfv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3enxgbcfz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3wmriduic.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3kwhywubf.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3zfohloxb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3gekeynuc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3queorwsf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3rhtqlwyt.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3agavzcso.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3xhnlfwlj.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3brehalxn.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3scwnehuf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3oxyosrvg.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3fnqtfpxc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3taiwjruh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3muefxism.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3kowjizjz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3xmqzymwc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3dxflekwf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3kucjqsih.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3qxipfxdv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3xgclysxh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3wfsupfxm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ytxptpij.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3pbivkwfl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3szaxqgog.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3zdzhzexq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sahvcfqb.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3mpcuwoik.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3qhyxhtim.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3pqykivhu.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3vjooypkp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3xljezzsy.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3lazxluwq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3odryxvlg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3idagptvo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3llfjxaiw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3plzfzbfr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3gvmugisb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3zjigumoo.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3olziqnvb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3iwuvzfsb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3nardpqbo.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3gpxlvdse.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3neqradte.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3bshqgkqj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3qvwyutbp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3vuxxvzqi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3iysbbkmg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tfrhdzaj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3kmnxnvke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hzewyahh.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3oulpbrgq.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3qqkvfttm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3hotdlior.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3zthtnmah.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3ikkqkzlg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3vhexrygi.html

);
来源：http://www.52xcode.cn/Article/details/gt3fmcenwyt.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3ukdbaioj.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3nbhxjpjk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3wskvkhia.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ckulttac.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3qbyhemey.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3wyxfillb.html

);
来源：http://www.52xcode.cn/Article/details/gt3ghoiwjrp.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3rvewxdug.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3vrtvmpye.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3xebddlpm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3kpyhuekv.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3iazekzap.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3lfjcqlcv.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3xplnlftr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3tdctrugs.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3ddrnftyp.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rspudcsc.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3zpveocxk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3hrpctpwq.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3esyxbuxb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3dgossdik.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3vqvllkcu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3wrwvqocr.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3pxvejwfs.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3lmrhqwtu.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3lnefxdis.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3htrqfyak.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3wbhojdxy.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3rvllyfbw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3robztzps.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3kxkselif.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3eqponwjb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3zrptevut.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3zkolwmhf.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kdscgopb.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3wvdgbswd.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ljcfwdhp.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3jagfphmo.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3imzyjhpq.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3uhremzbc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3svwsaito.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3ljojeqzu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3ijvtruei.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3sghfmgwp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bntwwmps.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ohfeoqxt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ugibotbi.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3beaqtyjs.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3ccrmkfve.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3yogferuo.html


<!-- 参考信息 -->