代发 wailian999

TS:   process.platform;  process.version
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzdkqdlg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fanxiaobao.xyz/Article/details/gimixqgug.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fanxiaobao.xyz/Article/details/gayzettxl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fanxiaobao.xyz/Article/details/gebahfsqs.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fanxiaobao.xyz/Article/details/gsteztkkt.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gbursmbvo.sHtML

N. 数据结构与算法
来源：http://wap.fanxiaobao.xyz/Article/details/gxxtiubqb.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ggedlfnqf.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/glxjibwho.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfmglcjv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazsucfje.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fanxiaobao.xyz/Article/details/gqjvgfrcr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fanxiaobao.xyz/Article/details/gokozceqk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghylifpka.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvwsrutf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbzjmqxh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkzzausw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fanxiaobao.xyz/Article/details/gqhajjbbs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fanxiaobao.xyz/Article/details/gbefqahfh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzhgihyc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/gxereamyv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fanxiaobao.xyz/Article/details/gklnbgtsi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixzgryiy.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gujmmavjk.sHtML

Ruby: arr.sort
来源：http://www.share.fanxiaobao.xyz/Article/details/guitvoljg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fanxiaobao.xyz/Article/details/gdxomfrmf.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fanxiaobao.xyz/Article/details/glsgfsple.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fanxiaobao.xyz/Article/details/ghjddblpa.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geyfsbtrk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljhkeqna.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fanxiaobao.xyz/Article/details/gqfwaozqy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbgawafn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbsskzfl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fanxiaobao.xyz/Article/details/gxrqormat.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fanxiaobao.xyz/Article/details/grklktenp.sHtML

[N04] 斐波那契数列
来源：http://read.share.fanxiaobao.xyz/Article/details/gexkofeqp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/glldoszkr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyfwcjla.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxiqnegfl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpczvoay.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmujckfj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fanxiaobao.xyz/Article/details/gpmgqblro.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fanxiaobao.xyz/Article/details/glolvbeqs.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmamsourm.sHtML

[N05] 最大公约数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmxedomq.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmbbawyo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpndseexr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gemkbnbyt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gixielsbr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gagjttlhl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fanxiaobao.xyz/Article/details/gnbfxfdug.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmrxrlzu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrrviqxx.sHtML

[N06] 判断回文字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gduaxwlkw.sHtML

Py:   s == s[::-1]
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvxhbovn.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fanxiaobao.xyz/Article/details/gifntyzcp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgonxtap.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcuhbyqqz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fanxiaobao.xyz/Article/details/gtqbctcjv.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fanxiaobao.xyz/Article/details/gcmytyklf.sHtML

Ruby: s == s.reverse
来源：http://baike.fanxiaobao.xyz/Article/details/gfqxujcye.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fanxiaobao.xyz/Article/details/glalbizpv.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fanxiaobao.xyz/Article/details/gqbrmqcja.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhieovgp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fanxiaobao.xyz/Article/details/gavxpucfy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fanxiaobao.xyz/Article/details/givlhqxpb.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fanxiaobao.xyz/Article/details/gepcrauaf.sHtML

Java: // 手写 HashMap
来源：http://read.share.fanxiaobao.xyz/Article/details/goiztuqan.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fanxiaobao.xyz/Article/details/grywpgpah.sHtML

Ruby: // 手写 Hash
来源：http://baike.fanxiaobao.xyz/Article/details/gvxktexph.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fanxiaobao.xyz/Article/details/grecalvkb.sHtML

[N08] 生成全排列
来源：http://read.share.fanxiaobao.xyz/Article/details/grcasjecu.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gzixbgbll.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksyldiwm.sHtML

JS:   // 手写回溯递归
来源：http://blog.fanxiaobao.xyz/Article/details/ggvrgqzjm.sHtML

TS:   // 手写回溯递归
来源：http://3g.fanxiaobao.xyz/Article/details/gtpwoqjfr.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzsttpuw.sHtML

Go:   // 手写回溯递归
来源：http://baike.fanxiaobao.xyz/Article/details/gywtarrxr.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fanxiaobao.xyz/Article/details/gslcnzxyy.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzagsnsag.sHtML

[N09] 栈与队列
来源：http://3g.fanxiaobao.xyz/Article/details/grxdjsriv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gomgimqcy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvlhhjvo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gexqpgrdt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fanxiaobao.xyz/Article/details/gqqqctgnn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fanxiaobao.xyz/Article/details/gikpepcnl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhjhscbz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fanxiaobao.xyz/Article/details/ggqdoatua.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwirxzjb.sHtML

[N10] 链表节点定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gboevhark.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fanxiaobao.xyz/Article/details/gknpyhmco.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfokwajec.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gqdmqrici.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gndsthksd.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fanxiaobao.xyz/Article/details/gruwjiqyz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fanxiaobao.xyz/Article/details/gqllgjtjv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fanxiaobao.xyz/Article/details/gpfkoutgr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fanxiaobao.xyz/Article/details/guoqwdlxq.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gmspztcco.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fanxiaobao.xyz/Article/details/grmvdlpxa.sHtML

PHP:  // 手写递归函数
来源：http://baike.fanxiaobao.xyz/Article/details/gmdqprfzo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fanxiaobao.xyz/Article/details/godrqxdwp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fanxiaobao.xyz/Article/details/gszpiqlua.sHtML

Java: // 手写递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazwsofkj.sHtML

Go:   // 手写递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gelpfgmor.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjlccrrf.sHtML

C#:   // 手写递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjwzdebf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fanxiaobao.xyz/Article/details/gsfotdzcn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnxiffwq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fanxiaobao.xyz/Article/details/gfkqvdxqd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fanxiaobao.xyz/Article/details/gtsokifss.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fanxiaobao.xyz/Article/details/goooywzfa.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsivpugtu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpwmiyxg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmfciwtt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlzjdany.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhiphtqk.sHtML

O. 并发与异步
来源：http://blog.fanxiaobao.xyz/Article/details/gqpgjbaht.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/glcfazmto.sHtML

[O01] 启动一个线程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjvzrkkx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fanxiaobao.xyz/Article/details/gzkrhwhol.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fanxiaobao.xyz/Article/details/gypohljyu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fanxiaobao.xyz/Article/details/gtkbfxppj.sHtML

TS:   // 同 JS
来源：http://www.share.fanxiaobao.xyz/Article/details/gltlojxyh.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhbsqddy.sHtML

Go:   go f()
来源：http://3g.fanxiaobao.xyz/Article/details/gqubdykbp.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fanxiaobao.xyz/Article/details/gixmdunly.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fanxiaobao.xyz/Article/details/gstcbarmi.sHtML

[O02] 使用线程池
来源：http://blog.fanxiaobao.xyz/Article/details/gstyyjfqq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdgakrsp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkkamnen.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsblnuswu.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fanxiaobao.xyz/Article/details/gcincsngm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtwumhee.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fanxiaobao.xyz/Article/details/ghwachbpp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fanxiaobao.xyz/Article/details/gjthygmhc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fanxiaobao.xyz/Article/details/gjpiprwgd.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyqrhkyv.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuvcytrd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fanxiaobao.xyz/Article/details/gwirjvjte.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fanxiaobao.xyz/Article/details/gewjoznwi.sHtML

TS:   // 同 JS
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdjhoyhe.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwazicwnn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fanxiaobao.xyz/Article/details/gmyvppwjt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqifsyspr.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmxhkgqc.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxbogkwb.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrueggdl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fanxiaobao.xyz/Article/details/gcloebnco.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geyegxrop.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqlmnfkz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fanxiaobao.xyz/Article/details/gpyxivtav.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fanxiaobao.xyz/Article/details/gypqswuoe.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fanxiaobao.xyz/Article/details/giggdioso.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsgetyqj.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpobrnhdj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fanxiaobao.xyz/Article/details/gofkcwobi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fanxiaobao.xyz/Article/details/gwhtdomhd.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fanxiaobao.xyz/Article/details/giuyuvzqb.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fanxiaobao.xyz/Article/details/granaoriw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplmvruda.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guyahoszr.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fanxiaobao.xyz/Article/details/gwwogifbu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtaulrps.sHtML

[O06] 使用进程池
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnjyugnf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fanxiaobao.xyz/Article/details/gqscjgley.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gpixuaekz.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fanxiaobao.xyz/Article/details/gdfkqyjjg.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fanxiaobao.xyz/Article/details/gqaerbugv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fanxiaobao.xyz/Article/details/gpadbjods.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fanxiaobao.xyz/Article/details/gpndfsyni.sHtML

Ruby: // fork 块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genfppgcj.sHtML

C#:   Parallel.For
来源：http://www.share.fanxiaobao.xyz/Article/details/gupbpanmy.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gkinfomhw.sHtML

P. 常用工具函数
来源：http://wap.fanxiaobao.xyz/Article/details/ghyaehgjt.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/grewjsixu.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsznkiauo.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fanxiaobao.xyz/Article/details/glusenltz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fanxiaobao.xyz/Article/details/gyozlojxx.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulplbgpm.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/gvbutdikk.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwfelayz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fanxiaobao.xyz/Article/details/gthhpdlri.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fanxiaobao.xyz/Article/details/glhvlglsd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fanxiaobao.xyz/Article/details/gpszfedpo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fanxiaobao.xyz/Article/details/gemkhmhex.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpiciwss.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwzzgsnu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fanxiaobao.xyz/Article/details/gfznoagzv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fanxiaobao.xyz/Article/details/gxjvtwzwx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fanxiaobao.xyz/Article/details/gzpsnlonc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fanxiaobao.xyz/Article/details/grmqfruhn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fanxiaobao.xyz/Article/details/giodwoutt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyeahohwp.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/garakvjsr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fanxiaobao.xyz/Article/details/gzozsfxnr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fanxiaobao.xyz/Article/details/guufrfpbl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gzqhoxqcw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fanxiaobao.xyz/Article/details/goshjbjfs.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbmzdabk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fanxiaobao.xyz/Article/details/glehtogfn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbmzatau.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjoweflp.sHtML

[P04] 求长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehlqmzqb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyxvnncj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fanxiaobao.xyz/Article/details/gkuhpgkbk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbtgsbvf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fanxiaobao.xyz/Article/details/gcpnaoqti.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fanxiaobao.xyz/Article/details/gszpgspne.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fanxiaobao.xyz/Article/details/gropzpsql.sHtML

Ruby: x.length;  x.size
来源：http://wap.fanxiaobao.xyz/Article/details/gvytuiuqz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fanxiaobao.xyz/Article/details/gniklwdsz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxoqxfaoc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fanxiaobao.xyz/Article/details/glpmwjmbi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fanxiaobao.xyz/Article/details/gznzvbwna.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fanxiaobao.xyz/Article/details/gwppfppwr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fanxiaobao.xyz/Article/details/glsgrlkjb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnpcoihu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fanxiaobao.xyz/Article/details/glzoxvzqe.sHtML

Ruby: a == b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcuxmilot.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fanxiaobao.xyz/Article/details/geonovwso.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fanxiaobao.xyz/Article/details/ghlynuczg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvouyvffo.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvgcrwuu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fanxiaobao.xyz/Article/details/gyplcfjoe.sHtML

TS:   if (x == null) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gkdpugyhz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gubzukfzn.sHtML

Go:   if x == nil {}
来源：http://wap.fanxiaobao.xyz/Article/details/gldivclao.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fanxiaobao.xyz/Article/details/githormwh.sHtML

C#:   if (x is null) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gakorwypc.sHtML

[P07] 防抖与节流
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpzxwdmy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fanxiaobao.xyz/Article/details/gqiwgprix.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gksztkqjt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbxyiaft.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gerjgxnwf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gbsnvehxt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fanxiaobao.xyz/Article/details/gubnldnhy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fanxiaobao.xyz/Article/details/gjsxxcgoo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxcxflyo.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvfkapxk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fanxiaobao.xyz/Article/details/glryqkgwr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpfdhyib.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbhpiaph.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcterkpvp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fanxiaobao.xyz/Article/details/gclagbqww.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fanxiaobao.xyz/Article/details/gprgvxrir.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvmgrpch.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkbsenxz.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicdrynmr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fanxiaobao.xyz/Article/details/gongcfbte.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrjtpiig.sHtML

[Q01] 创建表
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlerxvqn.sHtML

CREATE TABLE users (
来源：http://wap.fanxiaobao.xyz/Article/details/gdntlyucg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fanxiaobao.xyz/Article/details/gqrjufoxu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fanxiaobao.xyz/Article/details/gscwarale.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fanxiaobao.xyz/Article/details/gumnkkfqa.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fanxiaobao.xyz/Article/details/gkesnkfjc.sHtML

);
来源：http://3g.fanxiaobao.xyz/Article/details/gllmnsqlp.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fanxiaobao.xyz/Article/details/gicuavkmq.sHtML

CREATE TABLE orders (
来源：http://read.share.fanxiaobao.xyz/Article/details/gahzparxb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvatfzcp.sHtML

user_id INT NOT NULL,
来源：http://wap.fanxiaobao.xyz/Article/details/gnownoenl.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdhasbzz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fanxiaobao.xyz/Article/details/gkmtmynok.sHtML

);
来源：http://blog.fanxiaobao.xyz/Article/details/gemlnuzra.sHtML

[Q03] 增加列
来源：http://read.share.fanxiaobao.xyz/Article/details/gazavnfdq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsquqqgx.sHtML

[Q04] 修改列类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbdfyylk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjjefkza.sHtML

[Q05] 重命名列
来源：http://m.share.fanxiaobao.xyz/Article/details/gknjrlowl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnkknhfq.sHtML

[Q06] 删除列
来源：http://blog.fanxiaobao.xyz/Article/details/giyekgrbe.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fanxiaobao.xyz/Article/details/gqqvumppi.sHtML

[Q07] 删除表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfvlpcbc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fanxiaobao.xyz/Article/details/ggkrwlbxg.sHtML

[Q08] 创建普通索引
来源：http://blog.fanxiaobao.xyz/Article/details/gghftasyq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvdsmpet.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gxirxryag.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fanxiaobao.xyz/Article/details/ggbkmgzzt.sHtML

[Q10] 插入单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwtrrnss.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/gvtyeizdl.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqmhzbqv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/ghobbiaoo.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fanxiaobao.xyz/Article/details/gbgsyophu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fanxiaobao.xyz/Article/details/gimpzrqlt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fanxiaobao.xyz/Article/details/gomooksnw.sHtML

[Q13] 忽略重复插入
来源：http://wap.fanxiaobao.xyz/Article/details/ggquejaby.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gaxymdkcx.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fanxiaobao.xyz/Article/details/gobxtozoc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fanxiaobao.xyz/Article/details/ghaurqpzu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrgulqbh.sHtML

[Q15] 查询全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjznftoo.sHtML

SELECT * FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlarumjh.sHtML

[Q16] 查询指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjhvvzlq.sHtML

SELECT id, name FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gwzkoyrsn.sHtML

[Q17] 条件查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyytwvxkj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkghuhrjx.sHtML

[Q18] 模糊匹配
来源：http://blog.fanxiaobao.xyz/Article/details/goyfpllhd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fanxiaobao.xyz/Article/details/gzyvpltbg.sHtML

[Q19] 范围查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtklxjarm.sHtML


<!-- 参考信息 -->