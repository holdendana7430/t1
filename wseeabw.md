代发 wailian999

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gljturmvi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.hesvh.cn/Article/details/gtjbmaxpv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gtrqkjzxz.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gnumzrodt.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gkqsssqwa.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/giechojpj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gepklrrvt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fehbvm.com/Article/details/gmbtpmclh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/gxrqjlirx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gaiivdkrq.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/gnovqxboz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gizbjrrzj.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/glpwypbro.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fehbvm.com/Article/details/grrppgmcd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/gqvkyrztv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gxubhgfks.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gdczvnekw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/ghpogaree.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gwpeeciim.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fehbvm.com/Article/details/gzeqxpprx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/giwfmcwro.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/gplqvoadj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gasrufgsl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gydyahbyn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gnexvpsmh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gufbpwglu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.hesvh.cn/Article/details/ghwucgfod.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/giecmssda.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gzfzzlbwz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gyjjtovyz.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gymuxncef.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/gfgfnczfi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/glbmfygxq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/glrrapqgp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gfiixxyku.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/ggqtygnru.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/gbaxejzqa.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gdoxavqzk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fehbvm.com/Article/details/gnpwstvlk.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/gygmunpxz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gwrjllbnp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.zdbjq.cn/Article/details/goszjwcpi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/guihydtnu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gjpevbfyp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gkasxxpbv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/gxmtbdkip.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/guqsipdgf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gbeufegqe.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gsihkmvwt.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/gyoaaqphj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/gcfmvttas.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gmgmktsba.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gbmnwlzne.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/gejgwnews.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/gjgrtglgs.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/gqftsqmnd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/gbgwbvpcz.sHtML

[N06] 判断回文字符串
来源：http://blog.fehbvm.com/Article/details/gamdozzjh.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/grbfunokr.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gneogeucu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/ghbbuofxy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/ghtdpnnoh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fehbvm.com/Article/details/gbgjxjmdz.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/gxlslvsvx.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/geccildwl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gxeyumrju.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.zdbjq.cn/Article/details/girzypjqo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.zdbjq.cn/Article/details/gqhvigkfu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gkwcqyslu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.zdbjq.cn/Article/details/gdtzkrmgd.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/glwugnisq.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/ghdoggzce.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/gsslbpvyy.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gziywhhmk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gkdxbbfiy.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gsymujdgf.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/gwkjlywyx.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/gmkitclmk.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gnazromyi.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gjorfmzwx.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gmgkocqny.sHtML

Go:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gtnbwimxy.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/gnbfbuotr.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gfwxubeme.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gkgncpmos.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/gjcxojher.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gypomiqft.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gtllpswph.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/gdcytyclf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gqpqidwgm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gorcxrsuz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gqfzfbiou.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/gjffetdrk.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gqcauyrju.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/gdsoaodbb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gyvottplw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/glejqnvie.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/gxrqsrady.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/gilkwrzsy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.zdbjq.cn/Article/details/ghyvrlzjj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fehbvm.com/Article/details/gjsyicund.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gmmntfcep.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/gdwctlxyd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/gpjjpnwlk.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/goucfjdgl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gdyjqphjy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/ggxlxgbpg.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gvfjujmoa.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gnrftmxry.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.hesvh.cn/Article/details/gbelaevuh.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/glflajmdr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.zdbjq.cn/Article/details/gahfykfgs.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/gcdskitlr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gzoawbhmk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gdezimscv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/glqcxglxo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gvbueoubf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/gsbmuxdlw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.zdbjq.cn/Article/details/gzqbljaqp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gztetuupx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqflkiztn.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gzfhnimmf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/guzbrossm.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/gelduerrx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/gzbmatlhn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/guqiipnqu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.hesvh.cn/Article/details/gpkzvgboq.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gxlvzxuuz.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/gznoihznp.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/guyxtalfg.sHtML

Ruby: Thread.new { f }
来源：http://read.share.zdbjq.cn/Article/details/gcazcwoiw.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.zdbjq.cn/Article/details/gevayipau.sHtML

[O02] 使用线程池
来源：http://www.share.hesvh.cn/Article/details/gixqosysn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.hesvh.cn/Article/details/gogzlrkcz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/goibqevlq.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gzszhgkix.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gwytrlexk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gyukvraer.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/gtrzkiwab.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/grdjregpc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gftmxcitf.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/gtaufhtel.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fehbvm.com/Article/details/gpqvgyrdh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/glzejwjsy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/gkjccftco.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gulcvsxxq.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gctqaalev.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/gpmeiztll.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.hesvh.cn/Article/details/glndepnhd.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gzumzsonk.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fehbvm.com/Article/details/gvujjgnav.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/gactvrjxr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/gtbhydxlw.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/glidwpuxu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/glbrgptkc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/gpyzqgxgg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/gdhblfufw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/gzzwvmpok.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/gxzpqhaib.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/gjnykrfsd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gmknmasog.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/gkghycxps.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gnaarxgkk.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/geuvxwqsd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/gdbdoybcx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.hesvh.cn/Article/details/gvjyybflp.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/gywphlhjj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.hesvh.cn/Article/details/gmorqxkno.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gmcniyntq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/glspjxqpx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fehbvm.com/Article/details/gowqtrbie.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gakhbecio.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gapaituss.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.zdbjq.cn/Article/details/gecwrewug.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gnqtrisnh.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/gsqyzbcfo.sHtML

C#:   Parallel.For
来源：http://wap.fehbvm.com/Article/details/gmuwsxzzf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxfbyplrf.sHtML

P. 常用工具函数
来源：http://www.share.hesvh.cn/Article/details/gnqqdijlk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghgyjadvc.sHtML

[P01] 生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gjnlxckht.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.hesvh.cn/Article/details/glzfdeqbl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/ghgybsmxw.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/givupyjkc.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gsszyosph.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/gqwnitbhd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/gnmhoqrkb.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/glftwhhqz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gdqwxlkwi.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/gpsbwrfcy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.zdbjq.cn/Article/details/guxfdzbvp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.hesvh.cn/Article/details/gatubmjsr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/ggcywouyn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.zdbjq.cn/Article/details/gofinqotq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gsgmxppgu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/givfpqbiv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.zdbjq.cn/Article/details/gfgklmdwn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fehbvm.com/Article/details/giizlrnmz.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gdyuvprpa.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/gmrfuudqz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/gidcxgqwp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gfitkiygx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gkbgglgdw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gscwuapri.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/gsiscvwtu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/gayjmzlmg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.zdbjq.cn/Article/details/glyrqwrig.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/geajnbrsd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/gabzowgsm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gazjndhsl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gqrqogbbh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gdaxpefwi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fehbvm.com/Article/details/gxijgidxg.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/gyeocjete.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/gukhklhoh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gqcgcqvmy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/gmbsgtena.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gmjvnewfx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.hesvh.cn/Article/details/gyoqhrgyz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/gyropntac.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/glmxkihwq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.zdbjq.cn/Article/details/gdydluaks.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/ghwdcjhwd.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/gxyfcummv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gndnnrmwz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/gsfclowaf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.hesvh.cn/Article/details/gntypoujw.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/gvfadahqc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/gurrxntcq.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/gtcaxtboe.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gvvlpeais.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzlyizmah.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gkwhsghao.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/gedikmlmn.sHtML

[P07] 防抖与节流
来源：http://mobile.hesvh.cn/Article/details/gthlsefnt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/gjijsqlew.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/gbzguriab.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gqfraucfu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gxurbzhxi.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.hesvh.cn/Article/details/gvdpiidmr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.zdbjq.cn/Article/details/grzuettgg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gokbluuzt.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.hesvh.cn/Article/details/gmutumyvu.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fehbvm.com/Article/details/gzepszaiw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.zdbjq.cn/Article/details/gvrgfenlu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/gzasnntyu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/gsajeutnw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gqizdnhxg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/gpzyvbedf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.zdbjq.cn/Article/details/gkihsqbdx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/gzqcetjam.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gloghpetu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzocwzres.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fehbvm.com/Article/details/gvbklytlc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfazugwkh.sHtML

[Q01] 创建表
来源：http://3g.fehbvm.com/Article/details/geybbsrys.sHtML

CREATE TABLE users (
来源：http://wap.hesvh.cn/Article/details/gvkzasbqb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gecdhpirc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gplqjstfm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/gulppzwwg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/gvimnxnrn.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/guhgpgvio.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/gvgnpeiuf.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/gcrwodoqb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gtnjefzef.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gqqhvsval.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fehbvm.com/Article/details/gnuqfjlwl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/gttztufoc.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gsdlgswbt.sHtML

[Q03] 增加列
来源：http://www.m.share.zdbjq.cn/Article/details/gvdzyxcta.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.zdbjq.cn/Article/details/gunozjxyc.sHtML

[Q04] 修改列类型
来源：http://wap.zdbjq.cn/Article/details/gyvsvbrgc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/gzqyydavn.sHtML

[Q05] 重命名列
来源：http://3g.fehbvm.com/Article/details/gedaurgxj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/grifdmilj.sHtML

[Q06] 删除列
来源：http://www.m.share.hesvh.cn/Article/details/gmefjzrzl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/ghqijcclx.sHtML

[Q07] 删除表
来源：http://read.share.fehbvm.com/Article/details/gcguyutgl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/gvgsxxhmd.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fehbvm.com/Article/details/gtmboehsp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/ghafesgjh.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/glwiaansv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gnjcujrny.sHtML

[Q10] 插入单行
来源：http://www.share.hesvh.cn/Article/details/greytyssk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/gngqgivmd.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/ghqyqmbpt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fehbvm.com/Article/details/gugxccrsv.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.hesvh.cn/Article/details/geageaxti.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/gfjkhakfj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/gsezxmbmz.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/gxqnzmtau.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fehbvm.com/Article/details/gixligdrw.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/gzwvkxfmo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/guovmdwne.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/gliuqhdem.sHtML

[Q15] 查询全部
来源：http://mobile.fehbvm.com/Article/details/ggwnmamut.sHtML

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/gylzbdmdc.sHtML

[Q16] 查询指定列
来源：http://3g.hesvh.cn/Article/details/gaxdmhydu.sHtML

SELECT id, name FROM users;
来源：http://wap.zdbjq.cn/Article/details/gtvncgqbm.sHtML

[Q17] 条件查询
来源：http://m.share.zdbjq.cn/Article/details/gtqyuaooo.sHtML


<!-- 参考信息 -->