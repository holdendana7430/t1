代发 wailian999

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gqovjwmgm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fehbvm.com/Article/details/gvxmhzeoq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gqzxqksli.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gctgkfdcq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/gaebqetno.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqbdlzyuu.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gkcxbqyzr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gebluxdtr.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.hesvh.cn/Article/details/gjyotbgck.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gqvujwljh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gduowaanc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gsxssylsz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gtxzdcwjr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gxvatongo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gsdrgbqkx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/gqnpllwsn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gorrfrmuv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.zdbjq.cn/Article/details/gehpdmdgf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gyoksnvka.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/gdfivskgl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gjbxkangk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gdcrsueda.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fehbvm.com/Article/details/gojnkjpht.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gwlfuarof.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gfztynplz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gmdzkyvlm.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fehbvm.com/Article/details/gybclxuht.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gbwyhpgyr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gqngjggsq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gvxqiyept.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gryixzhir.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/geslntjxb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/gidoylvrk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/gfmtsskty.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/gleiinfxo.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/gbraqjdqe.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gqrbtgmag.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/gtqffvtac.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gbgguvlhf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gfcdgbqju.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gtzgzftbk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/ghamhozzm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gkoyislnn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/ggpnmvzbo.sHtML

[N05] 最大公约数
来源：http://www.m.share.hesvh.cn/Article/details/gszgjbssb.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gjndusjbd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/gewbdphed.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaeouioww.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gxqddzaxh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/goaowikea.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fehbvm.com/Article/details/gmisvghrl.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gsyiygusq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/gsqfpjoht.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/ggxebbhil.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/ghslydmgd.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gyjusmyrx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gbxxuczhf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/ghtcldjqv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gndmjhecn.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/gkkgjmftn.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gxfuymsyv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/ghhxrrcuw.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/gvgecjsfp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.zdbjq.cn/Article/details/glwtgilpe.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/ghbdbhlmz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/gbvvpnrjd.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gtqscuuhy.sHtML

Java: // 手写 HashMap
来源：http://mobile.fehbvm.com/Article/details/guebcvinz.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/geluxhgvg.sHtML

Ruby: // 手写 Hash
来源：http://blog.hesvh.cn/Article/details/gyhxixhtb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/gvlajzlzy.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/ghgizsntu.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/glntiljys.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gqvekhvzh.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/grzkkkmcw.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gsdezxnjh.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/ggxyyfayy.sHtML

Go:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/glugsnwvf.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/gfnummpzx.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gzybwvrbe.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/gyqfrnogg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/gknsegcum.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gnbovujub.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gypkdlvlk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gcnmftyen.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/gepatsvdt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gvkjrzqra.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gxfnaeroe.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/gfwsmenon.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gymgebgqh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gcrxmdjki.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/gjmdptvms.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/gsbivaozd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/goqrxmiqa.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/gggoaqoeo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/gymamowdh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/gdvzctpxh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/grqpwgmxs.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/ghmcrswtu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/ghrhxtwbu.sHtML

PHP:  // 手写递归函数
来源：http://www.share.hesvh.cn/Article/details/gkbubswwx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/glenleszw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/guvobyohw.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gbdpnfyud.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gqvmmvmyb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/gnvffzbpy.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gtajhteii.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/gvswapzwi.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/gzkrbplik.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/gucpasogy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gmnjsrtuc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/ggxliwnpz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gocskoeop.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/gdwojltwj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/gcxmpxhvi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gpnxowpjr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gucknytvz.sHtML

O. 并发与异步
来源：http://www.share.fehbvm.com/Article/details/gsxxgeabn.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gszawfgkc.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/gnkhhugbb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/gjlyfwzcj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gwjmxhltj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/gnlfnguum.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gpwuqnizk.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gnrpjqscv.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/gvrbyecli.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/grmkujdnk.sHtML

C#:   Task.Run(() => F());
来源：http://3g.zdbjq.cn/Article/details/gmydnrghb.sHtML

[O02] 使用线程池
来源：http://read.share.zdbjq.cn/Article/details/gaqkjmsgs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fehbvm.com/Article/details/gxnatappx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/gtlieiswg.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gqxkkplcm.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gmhoqovnc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/gsulfpgud.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/gbowecxlb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.zdbjq.cn/Article/details/gykczuuor.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/ghvzjrghm.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/gysxpuhzw.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/ggwjipugw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.zdbjq.cn/Article/details/gskzoegxu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gthzlszrv.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gfrlptwpi.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gntzwyceg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/ghjeklwsq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/gqwawzwbn.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gxdwbkrzp.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gjtqrwczv.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.zdbjq.cn/Article/details/gabtzforc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/gwrorfwih.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gwhmafpah.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/ggpjrxapq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/gccytczcn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/grbqbgjjc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/gpzgrvjze.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/gkqgbguws.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/gjuvwcyum.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gpqvbuhxs.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/gdkknkeuf.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gnfdkribp.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gvmpivfmu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/ggygfetzz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gzapassse.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/ggfxgngxv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.hesvh.cn/Article/details/gdtllyqzo.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/gugeexdyc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/gegbhnjhg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fehbvm.com/Article/details/ggtseehro.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gjdretnaz.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/geyagsiyn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gxdaudomi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/gdvgdykse.sHtML

Ruby: // fork 块
来源：http://m.share.hesvh.cn/Article/details/ghuzariju.sHtML

C#:   Parallel.For
来源：http://wap.fehbvm.com/Article/details/gqbydpfwm.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gywocyqiy.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/glaimdywy.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtnpgkjhq.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gzrylqgcg.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/ggzwbzsia.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/gwpxakyhk.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gxwyybbip.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gddtdftxs.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/gingbsysa.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/gekzcpgas.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gbjwhfsyt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/ghdbxtkjb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/gyqycqehi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/ggygiitui.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/gstmezkwn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.hesvh.cn/Article/details/gqwxobzmt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.hesvh.cn/Article/details/gpmubibpo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gzvtkqlwt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/gfnwqdbnj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/gjyhmhmna.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/ggfrnhugr.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fehbvm.com/Article/details/gycofvgrf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/ghpqotxjn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fehbvm.com/Article/details/gcmwspkyj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/grfvucmgb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gpmqqkmru.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gvkobhber.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fehbvm.com/Article/details/gixyayypz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.hesvh.cn/Article/details/gvuwjcdnh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/geybelkso.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/grqiezbmq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fehbvm.com/Article/details/giaglwqst.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gdnumudts.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gwayddadm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gmglvtjxu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gjowsyuue.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/gvfgrsygt.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gytqoxeuy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gacfvocxs.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/goxgqvjwp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/gwwpybsxa.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.zdbjq.cn/Article/details/gjgegvylc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gzuhbnlwo.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gxiteqsax.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/glvzvgbex.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.hesvh.cn/Article/details/gugzvsicq.sHtML

Ruby: a == b
来源：http://www.blog.hesvh.cn/Article/details/glmwrvjbl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/grhqxsdor.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/gzbtgiucx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/gnctiqebh.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fehbvm.com/Article/details/grssaclbf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/gdnwwzfzu.sHtML

TS:   if (x == null) {}
来源：http://blog.zdbjq.cn/Article/details/grminusos.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gbwigfape.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/gmeyfmbcf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gxppsawss.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/gdcmqjnrw.sHtML

[P07] 防抖与节流
来源：http://www.share.fehbvm.com/Article/details/ggunbpvsd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/gdrcfmezu.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/ggomxruah.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gxnmueeqb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gdglyfwjd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/gikxqcvdi.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.zdbjq.cn/Article/details/glqwyegah.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fehbvm.com/Article/details/gihinhjvc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.hesvh.cn/Article/details/gzysnneza.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/gtbbrgusz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gsbzaorqo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.zdbjq.cn/Article/details/ghaflkidl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.zdbjq.cn/Article/details/gwuftmynq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gnawyzipx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/gcfxnnlnq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/gearoyslj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/gfserrqft.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gfdgvqqfz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggzngpjaq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.zdbjq.cn/Article/details/gsunkcnal.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/goqymeezr.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/gockxtuyn.sHtML

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/grnztickp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gwypefuhx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gjjzhabyr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/ghvbkbjws.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/gkgyhfjyg.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gldgufegu.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fehbvm.com/Article/details/gpzorssjs.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/gazsrijdh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/ghlzikjri.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gzfsivokm.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/glgfalhtu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/gmwlvgliq.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gfhndjlig.sHtML

[Q03] 增加列
来源：http://www.share.zdbjq.cn/Article/details/givffucbb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/gggbmkzjy.sHtML

[Q04] 修改列类型
来源：http://read.share.fehbvm.com/Article/details/gqdqucwvt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fehbvm.com/Article/details/grferwytl.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/gvwausekv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.hesvh.cn/Article/details/gugwbshzh.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/gxnfnyvbm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fehbvm.com/Article/details/guhcvohvf.sHtML

[Q07] 删除表
来源：http://www.share.zdbjq.cn/Article/details/gqmqqimnp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gnxtbfxlo.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/gmxbggfet.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gdkrketeo.sHtML

[Q09] 创建唯一索引
来源：http://baike.fehbvm.com/Article/details/gnpyxcruw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gpuuiziuu.sHtML

[Q10] 插入单行
来源：http://m.share.fehbvm.com/Article/details/gqjxhglsk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/getfebolx.sHtML

[Q11] 一次插入多行
来源：http://read.share.zdbjq.cn/Article/details/gwdizblgf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/ggfpivesj.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/gyntvhodt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.zdbjq.cn/Article/details/guihefuet.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/gmhasyiao.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/gwtgnldtv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fehbvm.com/Article/details/goluotrpo.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/gflblwdhz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/gloegdsye.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/gdjjnmqub.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gtbkozlhq.sHtML

SELECT * FROM users;
来源：http://3g.zdbjq.cn/Article/details/gomobrasl.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/gnhcrakeg.sHtML

SELECT id, name FROM users;
来源：http://m.share.hesvh.cn/Article/details/garmhsiii.sHtML

[Q17] 条件查询
来源：http://read.share.fehbvm.com/Article/details/gdqdxbppw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/gbfprkalm.sHtML

[Q18] 模糊匹配
来源：http://wap.fehbvm.com/Article/details/gyridhytz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.hesvh.cn/Article/details/gcfkykgys.sHtML

[Q19] 范围查询
来源：http://baike.fehbvm.com/Article/details/gdvnjgrqi.sHtML


<!-- 参考信息 -->