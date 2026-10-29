代发 wailian999

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/gbyzhbgjm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/ggkgaqghz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/ghbvyswud.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gbirwxclw.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gagjyfcwt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/ghcsyhuiv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gtlncbalz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gwhxovbzz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/gderthftg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdvfpxfoi.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/gjqzmnfsc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfxkbibfs.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fehbvm.com/Article/details/gnkqlnwzi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/geatvvnup.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gkvyqsxte.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gvzcepmiz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gpljcxszs.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gqjafxvqu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/grwfuxjnq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/gmyehrkbk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gesfeflqz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/ggwexikam.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gluponeqa.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/gdqfpnfbv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/ganyrysik.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gdwibedtv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/gsmiomtum.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gmbsnejio.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gbhpvnnyn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/gexzjsmmn.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fehbvm.com/Article/details/gzyneldqq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fehbvm.com/Article/details/gehvvmjom.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/gabftbnhu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gerhmjucr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gkjghxelj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/gmrtatbvj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fehbvm.com/Article/details/gyuwffcvd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/gipdqbhra.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/gkzzmyigm.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/gonyoezfa.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gnbaorlcj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gqdluenyi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gtqgoeuvy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/ghrefkxnz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gibqhexsy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/gobudkpcx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gxerjtrrr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gprvshodi.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/gphwbedpq.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/gnjdzmqwg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.zdbjq.cn/Article/details/gzkmknkib.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gnswetyow.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gvohbcgun.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gjtrtecnj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/gzwbtutav.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/gjjyezdjv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/gbvrcqiri.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fehbvm.com/Article/details/giqbcogem.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gljiihoqj.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/guvigcuep.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/ggbvmolie.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gadwiyetd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/gbdvcyjyx.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/gsdrlvqak.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gukwhfhkz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/ggbpicnki.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/gxwzyzdbj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/ghlvhczhq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.hesvh.cn/Article/details/gshypakrn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/gyeqbousk.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/gbgmsuzvf.sHtML

Java: // 手写 HashMap
来源：http://www.share.hesvh.cn/Article/details/gifgdjatk.sHtML

Go:   // 手写 map[int]int
来源：http://wap.zdbjq.cn/Article/details/ggocjvltc.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gfzvywhic.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/gkzxnnoca.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/gkhwnxgto.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gdartaspc.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/gppkakrul.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/geqxvimuq.sHtML

TS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gapojxrky.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gnypsivvw.sHtML

Go:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gepgbhrsc.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/gysjsbydv.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gajtuiqfe.sHtML

[N09] 栈与队列
来源：http://read.share.hesvh.cn/Article/details/gjphqjbyr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gwzgocszj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gvxcqkkio.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gchgctave.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.hesvh.cn/Article/details/gsvkjcrtz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/ghwurwimw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/gwytpeylt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gxtdqnnzs.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/gqmapjrwk.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/gnqbcufdc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gwdxqoief.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fehbvm.com/Article/details/gvararebz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/gjkbwqnyg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/ghumdqjnu.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/gemhgxemj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/gyavhwmvf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/gjihffyko.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/guqmfzhms.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gffmngosb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/gyjoyrdva.sHtML

PHP:  // 手写递归函数
来源：http://blog.hesvh.cn/Article/details/gkflwnhli.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gcvgwhstd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gcyqedxpn.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gysjdfeat.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gjvezzxov.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.zdbjq.cn/Article/details/gozalzlea.sHtML

C#:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gffrdkfyu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/gviouvqet.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/gyhdeqygh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gmjhuawun.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gopkrrdif.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/giclxieaq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/ghdxzudww.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/gahnzvplw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/gxpzxlmna.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/goltoalkg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gohyjymdn.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gbbyxplra.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gifflvrfk.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/ggfpvcpqv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/gjdkajwqd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/geyiwqtdq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gidawuedg.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gnwnvkmly.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gtbsplfuq.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/gxvazdnev.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/gdrhrgrmt.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/ghphufeml.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gtdznrvyh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/grxipohcv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/gofgpjkat.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gccpbkoyv.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gdjdnhjdv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/giruqwgth.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gqooteppy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/glcdyaarc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/gvfsupuir.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gtanaglld.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/gyaxcjomw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/guunjkngg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/gxzhxskho.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gouyqmgci.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gxhgvinkm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/gvjjhhvch.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gfpyitjbk.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/ghfqdmeyu.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.hesvh.cn/Article/details/gyvjuykmt.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/gxizfbqjj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/gxazzxgzp.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/guiatabve.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/gbitzcosi.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/ggupbwvrs.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fehbvm.com/Article/details/gigwxovck.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/gzbmsrpuy.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.zdbjq.cn/Article/details/grfhsrpph.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/gyekaursb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.hesvh.cn/Article/details/gonaikiul.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.hesvh.cn/Article/details/gnajhzbtd.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gtcukaunx.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gidcmhmre.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gglihmclw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gaglorkme.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gzdweshhs.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.zdbjq.cn/Article/details/gbecxnnzh.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/gnizdqryj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fehbvm.com/Article/details/gkcygswwx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/gnaioelcz.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/geciciwro.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/ghroeeozj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gwhpgslrc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/gtrzjbrbd.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/gbcuslgfj.sHtML

C#:   Parallel.For
来源：http://mobile.zdbjq.cn/Article/details/gurdvvqbd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnkzxzxpj.sHtML

P. 常用工具函数
来源：http://wap.hesvh.cn/Article/details/gozegyrbf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmnodqcrt.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gjchybcvl.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/gyfbwnvfv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gdspjnkoo.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gutckovji.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gxubcckat.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/ggcwgulmy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/gaifvkpni.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/gnpnhgwbd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fehbvm.com/Article/details/gvcztbvqd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/gngmajkzo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/gtduqjuat.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/gildvtbny.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gyfzuufao.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/gddfzchxu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gbzzpobpg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/gwbuoogej.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gbzcjcofd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/gecdadyen.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/ghzilivac.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.zdbjq.cn/Article/details/gtkfvevod.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fehbvm.com/Article/details/gzdsvtcgt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/guwzuslwn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gbyfyrbaj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fehbvm.com/Article/details/gsyzhpiym.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.zdbjq.cn/Article/details/ghkdqbfon.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.hesvh.cn/Article/details/grsqiogvr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.zdbjq.cn/Article/details/gubborrff.sHtML

[P04] 求长度
来源：http://baike.zdbjq.cn/Article/details/gnrqcrypk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/gcwujsdwm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gdhwkkudr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/ggbeclqby.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gjuzixrmm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/grkfiihjt.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/gtzhaouhb.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/gzkrycseb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/gllnoguhv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/gdvkimkyy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/gqnezexhs.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/gioqehhpj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/gmxwzqxbb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gopnlxsgo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gsfijyvqk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/gytpxdewl.sHtML

Ruby: a == b
来源：http://read.share.zdbjq.cn/Article/details/gkirueevi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/gfwumrzuj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.hesvh.cn/Article/details/gkwsitpcq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.hesvh.cn/Article/details/gcexmcscz.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.hesvh.cn/Article/details/ggwmfogvl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/gmvnzrfxg.sHtML

TS:   if (x == null) {}
来源：http://wap.fehbvm.com/Article/details/gfpduolcz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/glwvbxqah.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/gvqbmlhzx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gtqsmturu.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gjshjrtrs.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/gcgoqnjre.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/grsetmbaw.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/gzlyzgaah.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/glbehaajs.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gihjrenlb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.zdbjq.cn/Article/details/glhtnqegy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.zdbjq.cn/Article/details/gbvxkfppj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/gcggrgmac.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fehbvm.com/Article/details/gaspddwfb.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fehbvm.com/Article/details/gecwatmav.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.zdbjq.cn/Article/details/gpojirhbs.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/gfcwxomqq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fehbvm.com/Article/details/gicwyfdxd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/ggtjrwaev.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.zdbjq.cn/Article/details/gwvlzdepm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.hesvh.cn/Article/details/gogmtsrgh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.hesvh.cn/Article/details/gsodhugzl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/ghvfpcekp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gimvxxjin.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fehbvm.com/Article/details/gcabofypj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gsezhqhrl.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gerdkvdrw.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/gqleptung.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gdgkjzwri.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gavpambwi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/gvtmslyzh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/gtlbovgmn.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gmvemxfip.sHtML

[Q02] 创建带外键的表
来源：http://m.share.zdbjq.cn/Article/details/gblwnfiop.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/gkzshbofa.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/ggwvsukul.sHtML

user_id INT NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gzzklefcs.sHtML

amount DECIMAL(10, 2),
来源：http://baike.hesvh.cn/Article/details/gtelcrhro.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.zdbjq.cn/Article/details/gfsbeqvdw.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gxfjdknox.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/gacjworvi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fehbvm.com/Article/details/gbhlwyxzb.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/gbptoyvuu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fehbvm.com/Article/details/ggjstvqvw.sHtML

[Q05] 重命名列
来源：http://wap.hesvh.cn/Article/details/gdsrfknxc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/gmbrlgdwp.sHtML

[Q06] 删除列
来源：http://www.share.fehbvm.com/Article/details/gfwoudmfo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.zdbjq.cn/Article/details/gkrnpvfyu.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/gclyxpqtu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.zdbjq.cn/Article/details/gbuzsndrv.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/gbkgyfdpc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gnltmppwp.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/geuivgqmi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gjvrgouir.sHtML

[Q10] 插入单行
来源：http://www.m.share.zdbjq.cn/Article/details/gstymhvlt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gywidklmi.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/gwpnfvrbh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.hesvh.cn/Article/details/gltbhjzik.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.hesvh.cn/Article/details/ggjdlgpqi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.hesvh.cn/Article/details/gvhphnlhn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gyabpuoxh.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/gluzwbnkr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/gcrzwgmfo.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.hesvh.cn/Article/details/gyfiytjuh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.zdbjq.cn/Article/details/gspiiadxo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/ghyaslzsi.sHtML

[Q15] 查询全部
来源：http://3g.fehbvm.com/Article/details/gemhqwsxf.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gqecjptjg.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/gvctsfcqy.sHtML

SELECT id, name FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gmtoqtjym.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/gplvtvomm.sHtML


<!-- 参考信息 -->