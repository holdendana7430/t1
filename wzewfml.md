代发 wailian999

TS:   process.platform;  process.version
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyawropb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyiebpir.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fanxiaobao.xyz/Article/details/gjphgrptf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fanxiaobao.xyz/Article/details/gxkjhikfq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fanxiaobao.xyz/Article/details/ghcrjgbkq.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gafkwqvjk.sHtML

N. 数据结构与算法
来源：http://mobile.fanxiaobao.xyz/Article/details/guuooylnm.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gikbvacsc.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/gfiwxtzuv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/glswfpumt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbjsvkev.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fanxiaobao.xyz/Article/details/ggowzswvu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnphklzh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbyvqrpe.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuscnqdv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fanxiaobao.xyz/Article/details/gcectqshr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/grkwsosag.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fanxiaobao.xyz/Article/details/goiwfpvsa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqodalir.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gjztntsjg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcngxrqlu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqhvwydu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmumgjqfw.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gszxijqct.sHtML

Ruby: arr.sort
来源：http://mobile.fanxiaobao.xyz/Article/details/gekohotjc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfqdmrac.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fanxiaobao.xyz/Article/details/godpzgkit.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fanxiaobao.xyz/Article/details/gzumujanv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fanxiaobao.xyz/Article/details/goepuirkm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fanxiaobao.xyz/Article/details/gmrdaremz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcshbsab.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fanxiaobao.xyz/Article/details/grvkzvyke.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fanxiaobao.xyz/Article/details/gbcmzkjtn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fanxiaobao.xyz/Article/details/givqizfft.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fanxiaobao.xyz/Article/details/guxnvgyii.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkbupdse.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpxtacms.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrpntpaz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gypluigml.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fanxiaobao.xyz/Article/details/ghrlhkelu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnahetcm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fanxiaobao.xyz/Article/details/gypinnzkj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gfecyushm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklgwsrvt.sHtML

[N05] 最大公约数
来源：http://blog.fanxiaobao.xyz/Article/details/gvapznsrc.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpkejfwq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwmlyspyo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fanxiaobao.xyz/Article/details/grdebxmth.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsauyevqn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fanxiaobao.xyz/Article/details/gdfqazwfj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fanxiaobao.xyz/Article/details/gutquphax.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlvijuvf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkphvjxkq.sHtML

[N06] 判断回文字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gjbxxiayu.sHtML

Py:   s == s[::-1]
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhezvagc.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fanxiaobao.xyz/Article/details/gztflncve.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdskjeiv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyuysawa.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fanxiaobao.xyz/Article/details/gnypxymkf.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdeuganp.sHtML

Ruby: s == s.reverse
来源：http://m.share.fanxiaobao.xyz/Article/details/gsijezvei.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fanxiaobao.xyz/Article/details/gawrhyhpx.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fanxiaobao.xyz/Article/details/glesltpyc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fanxiaobao.xyz/Article/details/gpaaofmag.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgliwtsx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcifgjufe.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fanxiaobao.xyz/Article/details/giqforvhz.sHtML

Java: // 手写 HashMap
来源：http://read.share.fanxiaobao.xyz/Article/details/gkewjxswa.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fanxiaobao.xyz/Article/details/gssnbiwre.sHtML

Ruby: // 手写 Hash
来源：http://baike.fanxiaobao.xyz/Article/details/ggouoijlj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxwzeqke.sHtML

[N08] 生成全排列
来源：http://3g.fanxiaobao.xyz/Article/details/gbykjwtmc.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/ggunxnudd.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxmrbghh.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/glymcqccf.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwlhqgua.sHtML

Java: // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gldfddywz.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpqinsnv.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fanxiaobao.xyz/Article/details/gaycwehdm.sHtML

C#:   // 手写回溯递归
来源：http://blog.fanxiaobao.xyz/Article/details/gacddtakj.sHtML

[N09] 栈与队列
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyjcmuzd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjpsldjv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fanxiaobao.xyz/Article/details/glhorfgav.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fanxiaobao.xyz/Article/details/giuuhszok.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fanxiaobao.xyz/Article/details/gepblboom.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fanxiaobao.xyz/Article/details/gbxaaqnrt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fanxiaobao.xyz/Article/details/gafpohccd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fanxiaobao.xyz/Article/details/gddrcvkww.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fanxiaobao.xyz/Article/details/grrsgjhvw.sHtML

[N10] 链表节点定义
来源：http://baike.fanxiaobao.xyz/Article/details/gsytmfkqt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtfdfyto.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqrndqla.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlyrearx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gbmthlbdu.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcuzkmkhm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fanxiaobao.xyz/Article/details/gdqdupdkv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fanxiaobao.xyz/Article/details/gchovzivh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fanxiaobao.xyz/Article/details/gynbnfgbu.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbmvhcov.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzizjuox.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gergafjdx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvksbzsh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fanxiaobao.xyz/Article/details/gussqmdok.sHtML

Java: // 手写递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gycqesnlu.sHtML

Go:   // 手写递归
来源：http://3g.fanxiaobao.xyz/Article/details/gxsqahmbp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtivuzzd.sHtML

C#:   // 手写递归
来源：http://wap.fanxiaobao.xyz/Article/details/gnwsnvmhd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fanxiaobao.xyz/Article/details/gxygllnna.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfpitihz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfpomrmm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzjuavui.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fanxiaobao.xyz/Article/details/gokvyhsxj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gafoydjno.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fanxiaobao.xyz/Article/details/gvqktugki.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gbufmpmox.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtznlswl.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuwdmtiu.sHtML

O. 并发与异步
来源：http://3g.fanxiaobao.xyz/Article/details/gymwziexp.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gshuowwhq.sHtML

[O01] 启动一个线程
来源：http://baike.fanxiaobao.xyz/Article/details/gnwxeaagj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzwmxtxz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fanxiaobao.xyz/Article/details/gqfnwpgtu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmdjeyei.sHtML

TS:   // 同 JS
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbfqlknl.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtjvbwrx.sHtML

Go:   go f()
来源：http://3g.fanxiaobao.xyz/Article/details/geuxizgfz.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fanxiaobao.xyz/Article/details/guhahiewa.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fanxiaobao.xyz/Article/details/gofgrczzq.sHtML

[O02] 使用线程池
来源：http://wap.fanxiaobao.xyz/Article/details/glxnxfapu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fanxiaobao.xyz/Article/details/guebivrng.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fanxiaobao.xyz/Article/details/gufwkiixl.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghofojkql.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaujdivuv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fanxiaobao.xyz/Article/details/gdnqxzdcc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdniaqii.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxpdsszs.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fanxiaobao.xyz/Article/details/gpaxmhumb.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fanxiaobao.xyz/Article/details/gowcxbpcd.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnydtuss.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fanxiaobao.xyz/Article/details/gmqjqzbsc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grymtexlo.sHtML

TS:   // 同 JS
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcrbhhkb.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gabibzodx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fanxiaobao.xyz/Article/details/giiccmsft.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gwojczxnz.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdbiimvxj.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/grglxzwhy.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fanxiaobao.xyz/Article/details/gydocbwhn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fanxiaobao.xyz/Article/details/gfheyrjex.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gieprvhxn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/garzeuafh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnznztbi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fanxiaobao.xyz/Article/details/ggsxkhwjo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhzfarii.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/giuihdgmd.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fanxiaobao.xyz/Article/details/gstfddvao.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpvvxqcd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fanxiaobao.xyz/Article/details/gtesnwdlr.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fanxiaobao.xyz/Article/details/gqcldopmj.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fanxiaobao.xyz/Article/details/gdsyfcrsm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fanxiaobao.xyz/Article/details/gxpdsjpko.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdmnpdql.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fanxiaobao.xyz/Article/details/ghtuikppb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/galwjfwul.sHtML

[O06] 使用进程池
来源：http://baike.fanxiaobao.xyz/Article/details/ggnuriium.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fanxiaobao.xyz/Article/details/gtimomjdt.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gxoijwvub.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhalaoje.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbzooipg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckyxizum.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fanxiaobao.xyz/Article/details/goukiubnf.sHtML

Ruby: // fork 块
来源：http://3g.fanxiaobao.xyz/Article/details/gkjbxzmqb.sHtML

C#:   Parallel.For
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxpcwwvk.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhfwsowv.sHtML

P. 常用工具函数
来源：http://blog.fanxiaobao.xyz/Article/details/gybzhodaq.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayciunui.sHtML

[P01] 生成 UUID
来源：http://3g.fanxiaobao.xyz/Article/details/gzjwluchd.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtcbjqxu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fanxiaobao.xyz/Article/details/gwlvewjft.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fanxiaobao.xyz/Article/details/gpruddjyp.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/gghxgfnec.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzrlmfrb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fanxiaobao.xyz/Article/details/gticwyvbu.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fanxiaobao.xyz/Article/details/goaryeihr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbumjikd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fanxiaobao.xyz/Article/details/glnewuwib.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fanxiaobao.xyz/Article/details/gxhnliwgw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fanxiaobao.xyz/Article/details/gahtafrnj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fanxiaobao.xyz/Article/details/gnrqkaayh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaunvjmor.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyucnblx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fanxiaobao.xyz/Article/details/gspiyulkx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzifheqt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmgntopn.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybahrnvu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fanxiaobao.xyz/Article/details/gwpqdgrne.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganxcfyoz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gkfjznozr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyovmlpvu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fanxiaobao.xyz/Article/details/gdcsttorm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fanxiaobao.xyz/Article/details/gprdxhmgw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fanxiaobao.xyz/Article/details/grdntxppk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fanxiaobao.xyz/Article/details/gtibeinlk.sHtML

[P04] 求长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gheczfwpz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fanxiaobao.xyz/Article/details/gaumeypkd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fanxiaobao.xyz/Article/details/gsylytinn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnzglxjc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fanxiaobao.xyz/Article/details/gthytgvyk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgagpgtd.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fanxiaobao.xyz/Article/details/gbbxafege.sHtML

Ruby: x.length;  x.size
来源：http://wap.fanxiaobao.xyz/Article/details/grtgbvsky.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fanxiaobao.xyz/Article/details/ggfeeeevf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpimkhoz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fanxiaobao.xyz/Article/details/gaqrvxkqd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqbpgsyr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnjczpdk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gmyjjvgmq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fanxiaobao.xyz/Article/details/gydehpoix.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjybmaac.sHtML

Ruby: a == b
来源：http://blog.fanxiaobao.xyz/Article/details/gmlfylfjy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrolglwb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fanxiaobao.xyz/Article/details/ggsmzzkpo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fanxiaobao.xyz/Article/details/gaanrpdnq.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbmkxjlr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgqhnjlh.sHtML

TS:   if (x == null) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxoacxnm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fanxiaobao.xyz/Article/details/grgsooeva.sHtML

Go:   if x == nil {}
来源：http://blog.fanxiaobao.xyz/Article/details/gtlhrmsxw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaodopxgm.sHtML

C#:   if (x is null) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/grrlaigsn.sHtML

[P07] 防抖与节流
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvblfkqk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fanxiaobao.xyz/Article/details/gwipaufto.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fanxiaobao.xyz/Article/details/gsepuhuog.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gcpgyjvmg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmdzsuyj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfoduydm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fanxiaobao.xyz/Article/details/gzeaitshy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gorggrdpe.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fanxiaobao.xyz/Article/details/gukbdbnjk.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcwxiqfs.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsylggunn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmaqoxbbl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fanxiaobao.xyz/Article/details/gwavoajvd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfakhgrjg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpwasxup.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fanxiaobao.xyz/Article/details/gxurpoola.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbuqsfab.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsdfmzqi.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/garjfvnew.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvrdemam.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gzqhvyzbt.sHtML

[Q01] 创建表
来源：http://www.share.fanxiaobao.xyz/Article/details/gpljtqpbs.sHtML

CREATE TABLE users (
来源：http://3g.fanxiaobao.xyz/Article/details/gsmvyyrnw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflsjnulp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzjbkvnd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fanxiaobao.xyz/Article/details/gehvjufpu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fanxiaobao.xyz/Article/details/gczcfwquw.sHtML

);
来源：http://blog.fanxiaobao.xyz/Article/details/gxhycpvbg.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxjxsdij.sHtML

CREATE TABLE orders (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzyhjnstb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fanxiaobao.xyz/Article/details/gwdejcihb.sHtML

user_id INT NOT NULL,
来源：http://mobile.fanxiaobao.xyz/Article/details/gijuxtlzy.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqjkpfhw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fanxiaobao.xyz/Article/details/gafzucmkz.sHtML

);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrjhpxsy.sHtML

[Q03] 增加列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfihtazfm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcwummxo.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehkcywba.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fanxiaobao.xyz/Article/details/gwjpvvzhz.sHtML

[Q05] 重命名列
来源：http://blog.fanxiaobao.xyz/Article/details/gchcfaapy.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fanxiaobao.xyz/Article/details/gvolppcrm.sHtML

[Q06] 删除列
来源：http://baike.fanxiaobao.xyz/Article/details/glnaavlib.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghaawjvlc.sHtML

[Q07] 删除表
来源：http://mobile.fanxiaobao.xyz/Article/details/grrghqxis.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gibzilbkn.sHtML

[Q08] 创建普通索引
来源：http://blog.fanxiaobao.xyz/Article/details/gslyiyuxh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fanxiaobao.xyz/Article/details/gigimaizi.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gqertpbae.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fanxiaobao.xyz/Article/details/gfqpgxqwt.sHtML

[Q10] 插入单行
来源：http://wap.fanxiaobao.xyz/Article/details/gxuljctrf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gyfydabfu.sHtML

[Q11] 一次插入多行
来源：http://baike.fanxiaobao.xyz/Article/details/gyhuasvpy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gvkfnjwur.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fanxiaobao.xyz/Article/details/geggbmzpq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fanxiaobao.xyz/Article/details/gyteqpvky.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsnncxtj.sHtML

[Q13] 忽略重复插入
来源：http://blog.fanxiaobao.xyz/Article/details/gdcjyxhkr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gbbegjwzu.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fanxiaobao.xyz/Article/details/gicubvbkk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlaphkyx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fanxiaobao.xyz/Article/details/gqlidrhlj.sHtML

[Q15] 查询全部
来源：http://wap.fanxiaobao.xyz/Article/details/gmespahrt.sHtML

SELECT * FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbclnzet.sHtML

[Q16] 查询指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gdpdnmrde.sHtML

SELECT id, name FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gfeagfahr.sHtML

[Q17] 条件查询
来源：http://mobile.fanxiaobao.xyz/Article/details/grzafadav.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gwimuaclz.sHtML

[Q18] 模糊匹配
来源：http://wap.fanxiaobao.xyz/Article/details/goopwneai.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmhpjrnx.sHtML

[Q19] 范围查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvozikgzj.sHtML


<!-- 参考信息 -->