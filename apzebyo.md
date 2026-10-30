代发 wailian999

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/gxqqanqpd.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/gwuscjzoq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.zdbjq.cn/Article/details/gdbwiedsh.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/ghyhbkpjy.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gtiuuierk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/gkdoxndpu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/guvwperkx.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/geuflfhxn.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gugbvszwa.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/gjrjssnfb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/gryguanjl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fehbvm.com/Article/details/grfhvpcpn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/gskhnrqbg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjasabinx.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gwtbwdija.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gshsjwjct.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/ggixnqevi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gzivfcslh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/gfrbyocvf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/grgcajhop.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gswnkzgop.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gczxqgsdr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gropnjvwt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/gbwrctpdz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gkjqsrxvv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/gbltaghhr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gedmwjclx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/gdcfmogmj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gwgjhbxwz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/ggqtuzydz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/gifdgftep.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/glxmjpslj.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gxwkeeyit.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fehbvm.com/Article/details/gtkokkoau.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/gqrteufik.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/gyvurjvdi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/gxapapdoq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/ggpxluhde.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gpnfqfabh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/gabptajte.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/gxkzwgmjl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gbgatesna.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gvhqbmgoq.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/gnvrjhivo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gfjcyrvde.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gidbwhtwx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gwbsmavej.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gsxvvwgja.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gckzifkex.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gfrjfcwdg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/ggwjikovo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/giqgsoqbp.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/grvxzkfbe.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/gnrouuxlo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fehbvm.com/Article/details/gpdpowzcy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gqsudjgra.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gpkuwqisa.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/glpyrujhz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gumkoyiqr.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/gyszgvnip.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/ghalawbcs.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/giwnumqid.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/gstfsfsmt.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/gutvdlmwm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gxueuqzoe.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gtphhwbug.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/gyavbjbvm.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/gdglmgmvg.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/gwaltvuti.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gyijyxntf.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/gvilafxsh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.zdbjq.cn/Article/details/ggdlcghch.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gnzvdkejl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.hesvh.cn/Article/details/gogqvttin.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.zdbjq.cn/Article/details/gtqmzuoxh.sHtML

Java: // 手写 HashMap
来源：http://www.share.hesvh.cn/Article/details/glmvxzntz.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/ghdfgzold.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gszuofrvq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/gzjgvgnvj.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gyvuxagem.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.zdbjq.cn/Article/details/gnmmbvyyv.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/gxjdkfzht.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/ggdisymzp.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gzdxkxtew.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gtvwqknrw.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gzfkmyheu.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/grwnamulc.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gwiibbqyd.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gumjwlhhw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/ghfvimgnk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gmvmnpwqs.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/givlcomnv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.zdbjq.cn/Article/details/guudvrtze.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gplinhqpu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gtmjheznj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gotaalgun.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/gxkgzqfue.sHtML

[N10] 链表节点定义
来源：http://3g.zdbjq.cn/Article/details/gqvjjwjup.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/gjqlnxgul.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gflgcqhhs.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.zdbjq.cn/Article/details/gieemgbjo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/gtikypmfo.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gtwbyjomt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.zdbjq.cn/Article/details/gbtimvvwc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gtoqldabx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/geofflmjc.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gikxgzmws.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gxntvywog.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/guppxcnbl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/grjsdligy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gakafhfke.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gwqjyfenw.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gsmlxfkdu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gxbjgrieq.sHtML

C#:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gnalaqnzm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/ggfekozwp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/gptpbddwg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fehbvm.com/Article/details/gzvrzabgo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gsvllsosz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gkefwxssl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gggufraoo.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gctzwwxzb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.zdbjq.cn/Article/details/gmhjofcqg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gykjkswmo.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfjkuktcn.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/gffbauapc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxwtszvrn.sHtML

[O01] 启动一个线程
来源：http://mobile.fehbvm.com/Article/details/gcjfqknri.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gljntgxce.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/gnyfrnqck.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/golstmlmr.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gmiahrjqi.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.hesvh.cn/Article/details/gubekvcjd.sHtML

Go:   go f()
来源：http://baike.fehbvm.com/Article/details/gtfearbhe.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/gzxapueyd.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.hesvh.cn/Article/details/gboyhdreb.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gkarxpfww.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/gbkgwrwmh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/galfilfsd.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gzyvrnnhy.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gojtzmpqk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/gjmfbcsum.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/gnbtkvgpx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/geyxcngrf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/grucpdvti.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/girjkpssz.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/gpubyshsk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.zdbjq.cn/Article/details/gtjqlzeqn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gcwfrzifc.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gweddqtyx.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gggngzcls.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gcorsmoku.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/gqffogupb.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gdvvruvpe.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/gzncikdtt.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/glvqojoqb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/gfhcumxke.sHtML

JS:   async function f() { await g(); }
来源：http://blog.hesvh.cn/Article/details/gsvkdctzo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gagamnvjw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gguydiwmd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/gptsabefw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/glfrhdvvm.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/gvnbhhivr.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.hesvh.cn/Article/details/guuvmcbhe.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.hesvh.cn/Article/details/gokpqppgm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/gmsxerayq.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gvgwdbrrc.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gdmtkpfrc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/glgsclqau.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/ghwwaskki.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/gsicgatzh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/gjfnoaxqc.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/gsjaongme.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/gdvwbhwid.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/gueajtoxx.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gjvdwccwx.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gujzvjjcp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/gfaurbxqu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gklmckqcl.sHtML

Ruby: // fork 块
来源：http://www.share.fehbvm.com/Article/details/gsjpxssfn.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gebkakoaz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gehcafcmx.sHtML

P. 常用工具函数
来源：http://mobile.fehbvm.com/Article/details/gfcqftdfi.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grhggohuh.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gqlhcjlln.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.hesvh.cn/Article/details/gmnicaurv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/gddydmohq.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/ggnumdeaj.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gkbpyzdff.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/ghfempnlm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/gnddpcozl.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/guxpaupcd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/ggszzjirg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/gawhnmwwt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.hesvh.cn/Article/details/gcnxzztjd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.hesvh.cn/Article/details/gepialqqu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gbiynlppu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/ggntkvayt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.hesvh.cn/Article/details/gnicnpbdv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/gfawirhck.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/goriamtnz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.zdbjq.cn/Article/details/goqcfmooi.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/gwtnlftys.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gkoizzxnc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/gvpummznb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gyvpvxkgp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gtfzekeeo.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gwhjvfpdg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/gnkhsxgwk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/gipcgmvrv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/gdwgkqkdu.sHtML

[P04] 求长度
来源：http://m.share.fehbvm.com/Article/details/ghckgaksz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fehbvm.com/Article/details/gtrwdpjmh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/grfeazggp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gluoivlul.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/ggfchaqrb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/gzkzgkqly.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.hesvh.cn/Article/details/gszqfvwzq.sHtML

Ruby: x.length;  x.size
来源：http://www.share.hesvh.cn/Article/details/gkkyenfop.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gjkfpuwnn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/gcgeuapcp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/gqxgbnmow.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.zdbjq.cn/Article/details/gcthwdkhu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.hesvh.cn/Article/details/gefhjhxzz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gxovichit.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/gpfhywiki.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/gvwgwdfrt.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/grxakhlvs.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.hesvh.cn/Article/details/gqgbkfhju.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/gnpeqmwxi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/gvetprfgl.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fehbvm.com/Article/details/ghxetgsgw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.hesvh.cn/Article/details/gdqneissi.sHtML

TS:   if (x == null) {}
来源：http://mobile.fehbvm.com/Article/details/gsdnartnv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/goerhieey.sHtML

Go:   if x == nil {}
来源：http://wap.hesvh.cn/Article/details/gkqmxexhf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gmqdhwebl.sHtML

C#:   if (x is null) {}
来源：http://read.share.hesvh.cn/Article/details/gygbgjdiz.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/grcrhgalv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/gzxilchyd.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/gjksspsuu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/giwvdtksr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gcyiqqohs.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/gsztkfptk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/ghsinhcys.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gvmzzyxvd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.zdbjq.cn/Article/details/gyaihvjjb.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.zdbjq.cn/Article/details/gwnmgzjdi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/gythycqyl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/gqsxgovnu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/gwbvwjgvv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gyxmuhyot.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/ggxquyxzt.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/ggrewvmif.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/gitdymrxm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/gdxwhgcjp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcufzreej.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/gdvfkodpx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjsoxmyyr.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/gglhsonee.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/gkjcdodpm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gqcvjprbr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gbmhalpsj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/gmzalnosx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.zdbjq.cn/Article/details/ggdajbiya.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gbwblsniw.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/gqzmoafmw.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gpkhwnqkt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gxxdquygu.sHtML

user_id INT NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gawgxwwik.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/gtpeolnzj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.hesvh.cn/Article/details/gxloqbenn.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gfvayytyx.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/gzlvdwoxi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/gpgzwlfwl.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/gstxfssvl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/gwpcswlcj.sHtML

[Q05] 重命名列
来源：http://baike.fehbvm.com/Article/details/ggtaymbta.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/gqllwhhjm.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gvhqxtmhk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/grmfvvkhv.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/gvqdbmaub.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.hesvh.cn/Article/details/gvgfdsrpw.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gqxwyxriz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gevjscwwm.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/gwnrkdjre.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/grpniggcg.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/gzowqxjlx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/gtmhlejmg.sHtML

[Q11] 一次插入多行
来源：http://blog.zdbjq.cn/Article/details/gzfvyotpw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gnyvvmbdr.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/grsergavu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.zdbjq.cn/Article/details/gnbyavelp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.zdbjq.cn/Article/details/gknoukgyx.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fehbvm.com/Article/details/gioewucud.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/gjphhrnja.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.zdbjq.cn/Article/details/gwrbmyutz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.hesvh.cn/Article/details/gghtnnjcn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/grfazkthx.sHtML

[Q15] 查询全部
来源：http://m.share.fehbvm.com/Article/details/ggmpodyxo.sHtML


<!-- 参考信息 -->