代发 wailian999

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gnhlsgoju.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/gawkmoiqh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.hesvh.cn/Article/details/ghpvewgmk.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gdapodlmt.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gmxgdhjgd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gnwmwxcit.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/grmsgptiy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/gmitlvjro.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gurrndtak.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsdkwszhb.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/ggfiyrelw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyniqnmrq.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.zdbjq.cn/Article/details/gtzlsybbd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fehbvm.com/Article/details/goxbbphkv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fehbvm.com/Article/details/glsixyqrz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gibjfgdmc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gernxvled.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gcnkpnlzz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gdqfticth.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.zdbjq.cn/Article/details/gffiwwwin.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gfilxjjkz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/gjvltcuis.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/ghjfvmszy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gzokbdzvt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gbxifoqqv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gablpmkmz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/gonwqqomj.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gansiddab.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/ggmylcnmf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gpcnqrdvk.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/gtiadsmsr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/ghtfrbwnm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/gwbtxllqe.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gjhzhxpmm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gnuolwixn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gluzaqclz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/gzoxknpac.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/grlkktdij.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/goflbwrvt.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/gflnepapo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gorinuogy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gztjeusny.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/grekdvunz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gbszkbitx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gdovbpwgb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/ggiovkwwk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/govzqnooe.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gmcljiddq.sHtML

[N05] 最大公约数
来源：http://mobile.zdbjq.cn/Article/details/gxmpextmx.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/glrsxrqzu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/ghhmpivlv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gbciftclu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gjfbdkzgd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/gsxxcabcz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.zdbjq.cn/Article/details/gpjefttgb.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/gankxfgcw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/gjjmryyek.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gxyfdpbrs.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/gxpfhsrak.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gqhdlkien.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gbgxwsaxs.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gmxslbyfv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.hesvh.cn/Article/details/gictsjmsp.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/grxuizvfh.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/gsvxxdtjb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gfzabhoxm.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/greiikvms.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gmtdmxeic.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gcheofdas.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/gtpuikerf.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gwnhmaqim.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/gvmcnqces.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/gujafxjpm.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gccxbevyz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/gtjogbgvp.sHtML

[N08] 生成全排列
来源：http://read.share.fehbvm.com/Article/details/glmjpdekj.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/ggmnknchn.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/glvavmrse.sHtML

JS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/genrvhplz.sHtML

TS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gvzixixum.sHtML

Java: // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gxfnfgmkl.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gtxduejdt.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/gcpdvnqnt.sHtML

C#:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/ghhnbiwxz.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/grermstyn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gpbhgmuxu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/gyrtjumqw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gkmuololq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.zdbjq.cn/Article/details/ggpxdtlyu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/ghmemyokg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.zdbjq.cn/Article/details/gybxtddag.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gyzxomeyf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/gzjnxcijz.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gmutvnpng.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/gbzgfltxy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/gbzskmiub.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fehbvm.com/Article/details/gjkeidmba.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fehbvm.com/Article/details/gffemnquf.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghslrnrkj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/gcmmcowid.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/gvgavufyl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.hesvh.cn/Article/details/gxrxpbyls.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/gixsifwng.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fehbvm.com/Article/details/gkfnuxihm.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/gosrivvmy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gfztqyyen.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gvrmtlzfp.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/ggwdxjvpa.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gisjprtzp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fehbvm.com/Article/details/grwgkwqzu.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/glvotbyox.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/ghsdskneu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/giwfsujqt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gcyuzarab.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gtwaxkqyc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gspjgxdeo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gsfrrtuef.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/ggxndgiua.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/gchgsurkd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gipstlaxd.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gouphnxtr.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/gedaduimn.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggryktdji.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/govwwkzoy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gayotcwlg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/godsyvvko.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.hesvh.cn/Article/details/glwgpmovy.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gmtqpkklr.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/goxjibwfh.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/grhuqyoso.sHtML

Ruby: Thread.new { f }
来源：http://blog.fehbvm.com/Article/details/gqfaojpwz.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/gmkdgoyxj.sHtML

[O02] 使用线程池
来源：http://baike.zdbjq.cn/Article/details/gguunxjcf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/ggkyowuys.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/gpnyngsik.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/glkkdkunj.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gydcluxbn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/gefsuvnhb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gfjndvrqs.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gylioolsl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gnpyelrsh.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/gwatstthg.sHtML

Py:   with lock: shared += 1
来源：http://baike.zdbjq.cn/Article/details/gkfzkazim.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/geclwkdnm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/gmrwnelmo.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gruqzxblp.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gcxyywckh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gufuytmuu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.zdbjq.cn/Article/details/girxesoem.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gajyawfoh.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/glhfvtedx.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.zdbjq.cn/Article/details/gwwuhangn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fehbvm.com/Article/details/gzflyiurg.sHtML

JS:   async function f() { await g(); }
来源：http://3g.zdbjq.cn/Article/details/geooxdpuq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.hesvh.cn/Article/details/gqrbfhlma.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/gjmwovfbs.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.zdbjq.cn/Article/details/gnpynjlaq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/ggrryocnd.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gxkocugic.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/gthrsvaii.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.zdbjq.cn/Article/details/glcbgjdjy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/ghspjcinm.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gejvozaqc.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gfdgnbiyl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/gkpkahicp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/ggkafrfrc.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gupbwekir.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.hesvh.cn/Article/details/gztogwprw.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/gblejvmsf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gmxtchkec.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.zdbjq.cn/Article/details/ghvzemarl.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gqmxoukix.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gqajymlar.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/girxirnno.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/gzkwscfxh.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/gxemhprnd.sHtML

C#:   Parallel.For
来源：http://read.share.hesvh.cn/Article/details/gbkhrkqab.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gebnrlgjw.sHtML

P. 常用工具函数
来源：http://www.share.fehbvm.com/Article/details/gawvfvcvh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/guyuzbler.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/gztaqomfr.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/gbvfwkwts.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gqecbjlrz.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/givmylrhg.sHtML

TS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/glelbkzvz.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/gssnmbvln.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/girkcaupy.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/glevnnwud.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/gvjqfqpxe.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/glfkcgrvq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gxayygcln.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.hesvh.cn/Article/details/giljxdpig.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gfuqgowrm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.zdbjq.cn/Article/details/glmehgpqi.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gtubsxhmb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.zdbjq.cn/Article/details/gutnotzhk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/gdrznkgqs.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/gbnpswihh.sHtML

[P03] 生成短随机字符串
来源：http://read.share.hesvh.cn/Article/details/gwenmfpys.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/gdoanqllg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/gxobthpds.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gxelyfzrt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gkopebvtc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fehbvm.com/Article/details/gebmwtcnv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fehbvm.com/Article/details/ghbwhguva.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/gfltkboqt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/gdldnxtlo.sHtML

[P04] 求长度
来源：http://www.m.share.hesvh.cn/Article/details/gapycnjkt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/gexhpzlsq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gtihniiyx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gcdyumpko.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gqizbtitw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fehbvm.com/Article/details/gmyimbpcg.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.hesvh.cn/Article/details/giuqvnxdx.sHtML

Ruby: x.length;  x.size
来源：http://baike.zdbjq.cn/Article/details/gwdlssiny.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gtxxnttjt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/ggudvdjbv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fehbvm.com/Article/details/grojmovmi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/gedyawqwa.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.zdbjq.cn/Article/details/gvmnnvuin.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gwiblptnd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fehbvm.com/Article/details/gkmqakfbm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gntqkzfar.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gszxkwjnl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.hesvh.cn/Article/details/grsmftppm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/gmjyaxyhv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/ghgrrhvbc.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.hesvh.cn/Article/details/gsqlggspr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/ggktdkjsv.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gymnskssn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gfyokccdm.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/gjlkgkchs.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/ggemcerwa.sHtML

C#:   if (x is null) {}
来源：http://wap.zdbjq.cn/Article/details/gzswyxyim.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/gbgtyyohw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fehbvm.com/Article/details/goubxrhac.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.zdbjq.cn/Article/details/gnqiopzuk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gnhrxkhtf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gjrqheohi.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.hesvh.cn/Article/details/gvcvffkbi.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.hesvh.cn/Article/details/gftsgnvbq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gyeolgsfi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/gkynnedah.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/goiioqtav.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.zdbjq.cn/Article/details/glgopyiml.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.hesvh.cn/Article/details/govvoygqf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gpudwkehc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gwmqeayrj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/gtyvvdydw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fehbvm.com/Article/details/gycmlhjip.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.zdbjq.cn/Article/details/gzyzgklsw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.hesvh.cn/Article/details/ggvuwvtol.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gerchgikz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fehbvm.com/Article/details/geysaajyw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqolqoikv.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/gvcaxpsop.sHtML

CREATE TABLE users (
来源：http://wap.zdbjq.cn/Article/details/gtsfrurio.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gylxrqszh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/grhcaawey.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.zdbjq.cn/Article/details/gaoiewogx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fehbvm.com/Article/details/garwxqvly.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gflvbwwwu.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gdqsbknae.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/gxlkvutwo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gthwtmdpv.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gtlqgnhoo.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.hesvh.cn/Article/details/gdxcvugvz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.hesvh.cn/Article/details/gvwofsvla.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gqsfbfywz.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/gqhjjzxrf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/geqnlbgjg.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/gsgfylqrk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/gbzuhchwz.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/gglaqqong.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fehbvm.com/Article/details/gfbqhaslh.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/gpvsyicux.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/glxwcdbzr.sHtML

[Q07] 删除表
来源：http://www.blog.hesvh.cn/Article/details/gtoymyouu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/guvpjahdj.sHtML

[Q08] 创建普通索引
来源：http://mobile.zdbjq.cn/Article/details/gjdwnpcke.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gpssrrncr.sHtML

[Q09] 创建唯一索引
来源：http://baike.fehbvm.com/Article/details/giftbhiwf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gqvqujxeu.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/grewkbrvz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/gpetzwfcm.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/gkkymjhsm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/gircswxiw.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.hesvh.cn/Article/details/gjdnwrijy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/gyhclkrsx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.hesvh.cn/Article/details/gwbymjsak.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/gbwrapfjn.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fehbvm.com/Article/details/gwlcgqhzv.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/guiasanee.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.hesvh.cn/Article/details/gvmaeyood.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.zdbjq.cn/Article/details/ghoifxlya.sHtML

[Q15] 查询全部
来源：http://www.blog.zdbjq.cn/Article/details/ggvclafij.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/gkxrwpiyy.sHtML

[Q16] 查询指定列
来源：http://baike.fehbvm.com/Article/details/gyxdhsrkm.sHtML

SELECT id, name FROM users;
来源：http://mobile.fehbvm.com/Article/details/gdlfwksbs.sHtML

[Q17] 条件查询
来源：http://www.blog.hesvh.cn/Article/details/gnlylfdfa.sHtML


<!-- 参考信息 -->