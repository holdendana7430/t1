代发 wailian999

Py:   if __name__ == "__main__":
来源：http://wap.fehbvm.com/Article/details/gkgfkgrcp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/gozgsxano.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gtvnxqvnv.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gklqrenut.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/gxslyncme.sHtML

Go:   func main()
来源：http://mobile.fehbvm.com/Article/details/gvjnmnuuv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.zdbjq.cn/Article/details/giloarzmh.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gvoukksby.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/ghpurhpyl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gdphxgpcl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/ggbdkkfgz.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gakgbtcwx.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gojeqnyzo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/gqhggvixq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/gscbbujvm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/ghytpmgwq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fehbvm.com/Article/details/gdpeonhiz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjujgoszh.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gcxqezjuf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdwojykqz.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fehbvm.com/Article/details/gilemmpui.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/gunapaanc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/glllhfden.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gyktddshw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gdgoydygz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/ghystjdfs.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/glkqdiuvl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/gzddiijwv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gljkziugv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/gcnpyxsvb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gctiibmre.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/gbhkctail.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gpivxplme.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/glufvrkhl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/gauhtnhde.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gdowldaoc.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gujzlfgbc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/ggcpmecur.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/glpdqyrxr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/gsztlgrdc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/gmqbdbyls.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gnacemcdi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/grcrcncxl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fehbvm.com/Article/details/gqafybkob.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/gekrrqvvq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/gacadeqao.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/gazlksjlu.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gpnfqxoct.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gyzfwvqwi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/gqvjxlabc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gggsnpbho.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/grypjmwfw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gpgtmbrco.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/gsjzqkeae.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gswwoubfy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gumucmzmo.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/gxsucidud.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/gtwaslpcg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gdaiwvzdf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gkzguckza.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gioinrrbz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.hesvh.cn/Article/details/geturiuba.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/giurmpopr.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/gexxobjcf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/ggacbpgyl.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/ghlinuwbc.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gahiltbog.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/goygxrker.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/grabuzbdz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gcitypgff.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/gwxaowxgk.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gndtcbtrc.sHtML

Ruby: s == s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gggryrxhl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gfklhmcxa.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fehbvm.com/Article/details/gkzrqpszy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/guxwbgwpe.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/gyuajjybu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/gdqopmgrk.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/gagihgwzk.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/glaiaxjhk.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/gifuikkif.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gmuqgqarz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/gifnhqqmz.sHtML

[N08] 生成全排列
来源：http://www.blog.hesvh.cn/Article/details/gsjdzjtoz.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/gbyzbyqrt.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/gjdpmtzqh.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gdewpqcet.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gciiqdvji.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gvaclboin.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gqgrhrtwn.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/gsxzxikyn.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gzxshtvto.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/gefvdpitf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/glgjmqbln.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gpjjjdwcf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gamjsqwqs.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.hesvh.cn/Article/details/gsvnxhiwq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/gesfqlfey.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/gkiumizmp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gcwvdmqpg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gwkjxiume.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gurmcwtzy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gdgsnfeho.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gmcwblhyx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/gxekkggax.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fehbvm.com/Article/details/gdtdkioaq.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gdvtifspe.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.hesvh.cn/Article/details/gntfkpklf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/gyzlwlmck.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/gqontoypq.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/ggogkxfth.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/gfnojchye.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/gvellsfhd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gokqgjomx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gswoepwvl.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gghrwaxzu.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gtqipfzii.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gwamvvzeh.sHtML

C#:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gqcuezltx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fehbvm.com/Article/details/givastskd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/gkgirsaeh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/gkgoqosby.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gvfepmeud.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gzhbgkpai.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gqrmykqru.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/ghwoymmot.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/ghdutpjoc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gemvdgzat.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/glumiajet.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/guuwtnzno.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqkpyekwq.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gopaxrcel.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.hesvh.cn/Article/details/gkiwwprff.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/ggdjckqua.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gdgryzhst.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gokoldjxh.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.hesvh.cn/Article/details/gljrryvlo.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/gylwgryar.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/gygwxztqc.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/gozzcxrlo.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gzaexhjuz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fehbvm.com/Article/details/gyticaraa.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gsxtnxqgo.sHtML

JS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gneigxnmm.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/ghnicevdv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/grgmnwiyf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/grysupyyx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fehbvm.com/Article/details/gpctjctvi.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/gziygvyqx.sHtML

[O03] 加锁保护共享数据
来源：http://blog.hesvh.cn/Article/details/gmlcihckk.sHtML

Py:   with lock: shared += 1
来源：http://blog.fehbvm.com/Article/details/gofmwtmhs.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fehbvm.com/Article/details/gjofopojh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/gnrwdwccf.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gsohwyiiv.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gpahcdisg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/gjqxjxzeq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/gtunzyyvy.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gbqgngnfh.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/gnhrfoafm.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/gdnhhfkox.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/glqsiwaon.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gyimhykle.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/ggdjnoryp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/gdadiytsm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.hesvh.cn/Article/details/gkvhujmwy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gzjgxuxjv.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gkahuehwr.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/guxeeecjw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/giaxnamnp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/gueehwbaa.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gvipbueyb.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gwrxxlalr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/gbyouppta.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.hesvh.cn/Article/details/gmwdlijwg.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gyrcvkgsr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/goceblkhv.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/gsoxvmhwr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/gxbkpaydd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fehbvm.com/Article/details/gchmegbnu.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/geaotdtif.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gqmklvgvs.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/gixngltyq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.zdbjq.cn/Article/details/gzqzlfwny.sHtML

Ruby: // fork 块
来源：http://m.share.hesvh.cn/Article/details/ggkuruyfy.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gctqygslf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghhhvtkrj.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/ggqgvjpmd.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnmkfniau.sHtML

[P01] 生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gfecbbiew.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fehbvm.com/Article/details/gbmbfnzmq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/gsgibnqpv.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/ghvaspchk.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/glfnmwamn.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gzzsqcora.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gqawzeags.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/grljilutm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/ghrgsouer.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.hesvh.cn/Article/details/gjnfgfxne.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/gvczvllbt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/godjrewho.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.hesvh.cn/Article/details/gxwjubyka.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fehbvm.com/Article/details/gneasipjn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gzbpqzdqa.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.hesvh.cn/Article/details/gswmbzvvd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/gguvaclfu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/glfktdzgh.sHtML

[P03] 生成短随机字符串
来源：http://blog.hesvh.cn/Article/details/gyaqljmhp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gepucxnmm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.zdbjq.cn/Article/details/gjlsdbmvl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/guupsvzju.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gqzlfrayd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/gmhfdzoed.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/gzyifjcsb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/gwcktjpss.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.zdbjq.cn/Article/details/gxwtzdlgb.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/ghgqmnmkz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gwjkijtqp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gmrelprmt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gykpkoves.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gjlsujdlf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fehbvm.com/Article/details/glaljxage.sHtML

Go:   len(arr);  len(m)
来源：http://3g.zdbjq.cn/Article/details/gpwnnbrqi.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/gexbptjcg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/gdlfcvvus.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.zdbjq.cn/Article/details/gnmocnvlk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fehbvm.com/Article/details/gxrcweseb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/ghykkddiu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/gjlmalino.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/ggayozgms.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/gprngevyy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.zdbjq.cn/Article/details/gkujnzowg.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/ghpovsrzz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gtnejqsmy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/giuenqpdo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gncbcelqg.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/gegybpdyl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/gdmwykuji.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gcnoxcirt.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gbmcoxxcq.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/gqpvahnol.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/gbbpqqdbq.sHtML

C#:   if (x is null) {}
来源：http://blog.fehbvm.com/Article/details/gwpoxbevs.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/gnfyuhiye.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/gviucydwo.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fehbvm.com/Article/details/gymzwgflm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gqlxknyxk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/glwuaxseb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/gvvlgqbfg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.zdbjq.cn/Article/details/gthlsyeqe.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/guxgvwjdi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.zdbjq.cn/Article/details/gnrymdbdi.sHtML

[P08] 处理浮点精度问题
来源：http://wap.zdbjq.cn/Article/details/gkizopwfb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/gttlmzxmi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gfrkjhwok.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.zdbjq.cn/Article/details/gfvdebken.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gqefxgvzp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/gtuuudbig.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.zdbjq.cn/Article/details/gggufswcc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fehbvm.com/Article/details/gbeexnmnp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fehbvm.com/Article/details/glergbghl.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzgxccplk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/gudkndrcu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gagqsddjb.sHtML

[Q01] 创建表
来源：http://baike.hesvh.cn/Article/details/gifhpyxpw.sHtML

CREATE TABLE users (
来源：http://wap.zdbjq.cn/Article/details/gwmtnebjk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gkozrmntp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gdewnrfye.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/gfspavkzf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/gonefsoxj.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gzfsxghpu.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gnhuzulfa.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/ghzwmvblu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gylpfstvl.sHtML

user_id INT NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gzdcjqmle.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.hesvh.cn/Article/details/gjvxkyleu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.hesvh.cn/Article/details/gxkcxhgmk.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gyoicgnyr.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/gimremyuw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.hesvh.cn/Article/details/gsstnrffj.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/gnligckeh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fehbvm.com/Article/details/gywjaxicu.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/gwflfwxyc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.hesvh.cn/Article/details/gzpfxhibw.sHtML

[Q06] 删除列
来源：http://mobile.hesvh.cn/Article/details/gnbydhcjw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.hesvh.cn/Article/details/gariwlyoa.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/gmighaneu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/giyxeyfcc.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/gabgclwqa.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gxiammzur.sHtML

[Q09] 创建唯一索引
来源：http://blog.fehbvm.com/Article/details/gqpanuykp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gjlqxdnxt.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/glefwgoev.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/grbfqaquq.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fehbvm.com/Article/details/gpafhapnm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gfumgzand.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/gbcmibmea.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.zdbjq.cn/Article/details/gayugpwrb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gfsstbssy.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/gejszfnmp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gnxkjogec.sHtML


<!-- 参考信息 -->