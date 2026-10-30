代发 wailian999

Py:   if __name__ == "__main__":
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkymogib.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrlaaswf.sHtML

JS:   require.main === module
来源：http://baike.fanxiaobao.xyz/Article/details/gjqfgvhil.sHtML

TS:   require.main === module
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggapkovme.sHtML

Java: public static void main(String[] args)
来源：http://blog.fanxiaobao.xyz/Article/details/gebtytknr.sHtML

Go:   func main()
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzbukqmf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fanxiaobao.xyz/Article/details/gugnokuex.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfaoonmy.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fanxiaobao.xyz/Article/details/gmlxxxjqa.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcqhwzrz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtxwbdls.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fanxiaobao.xyz/Article/details/gicuysdab.sHtML

TS:   process.platform;  process.version
来源：http://baike.fanxiaobao.xyz/Article/details/gpkwhfvfx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgbbfhoi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fanxiaobao.xyz/Article/details/gowpfvhpm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fanxiaobao.xyz/Article/details/gdipiuigt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqbutide.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gcszutlqv.sHtML

N. 数据结构与算法
来源：http://www.share.fanxiaobao.xyz/Article/details/gwefxemoe.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjcybvaf.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdvazxxn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwnltxzg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzzbhixj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fanxiaobao.xyz/Article/details/gepqqfmuu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulxlqjfj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyltschgv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fanxiaobao.xyz/Article/details/gdlazpqam.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzicclzyq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkpsohop.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fanxiaobao.xyz/Article/details/gaxmlpdce.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjoapdmpd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gjlgpldpb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fanxiaobao.xyz/Article/details/gdovozrvp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpnlgbcq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fanxiaobao.xyz/Article/details/gxnxpyqcp.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/grjmxieyw.sHtML

Ruby: arr.sort
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfdigawa.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fanxiaobao.xyz/Article/details/gsfvuusgj.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrcxwzir.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fanxiaobao.xyz/Article/details/gayrsxvfr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fanxiaobao.xyz/Article/details/giwphagxw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fanxiaobao.xyz/Article/details/ghhaluruy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fanxiaobao.xyz/Article/details/guyakfuiv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fanxiaobao.xyz/Article/details/gndjozycw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsmfflom.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fanxiaobao.xyz/Article/details/ggaylpvic.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fanxiaobao.xyz/Article/details/gamvtmgro.sHtML

[N04] 斐波那契数列
来源：http://read.share.fanxiaobao.xyz/Article/details/glvaxtkys.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gglzvbmhh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fanxiaobao.xyz/Article/details/gygfageyk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqivfluo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpoqztey.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fanxiaobao.xyz/Article/details/garyscbef.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fanxiaobao.xyz/Article/details/gsvebytfn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjzdczih.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnhcyayv.sHtML

[N05] 最大公约数
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpripyfj.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fanxiaobao.xyz/Article/details/glxiowkih.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fanxiaobao.xyz/Article/details/grkmfqtox.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glbjaofyf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdjkkedia.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamnrjxwz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpbnpmxq.sHtML

Ruby: a.gcd(b)
来源：http://baike.fanxiaobao.xyz/Article/details/gnfyeurlz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fanxiaobao.xyz/Article/details/gvueoghcy.sHtML

[N06] 判断回文字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gaasdpomd.sHtML

Py:   s == s[::-1]
来源：http://baike.fanxiaobao.xyz/Article/details/gxfpoifww.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnykitsos.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzwokzjk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzszntkec.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fanxiaobao.xyz/Article/details/gieweabkk.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsbatwvl.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcgcfvqa.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fanxiaobao.xyz/Article/details/gstyjjmuv.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fanxiaobao.xyz/Article/details/groluoemq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpxdkqee.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fanxiaobao.xyz/Article/details/gneiaiejr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fanxiaobao.xyz/Article/details/gsltayvgp.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giaixvbxp.sHtML

Java: // 手写 HashMap
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsokihmz.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fanxiaobao.xyz/Article/details/gcswbvmqa.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgsfvsyj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fanxiaobao.xyz/Article/details/groiwtdit.sHtML

[N08] 生成全排列
来源：http://www.share.fanxiaobao.xyz/Article/details/goakvknnh.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjgenrio.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduajetsu.sHtML

JS:   // 手写回溯递归
来源：http://baike.fanxiaobao.xyz/Article/details/gjjyddubu.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gasfqlzeo.sHtML

Java: // 手写回溯递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gogccaegl.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjtrsayn.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fanxiaobao.xyz/Article/details/gwbylpgoo.sHtML

C#:   // 手写回溯递归
来源：http://3g.fanxiaobao.xyz/Article/details/gpsloqdhe.sHtML

[N09] 栈与队列
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnskkclf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxhdzzyp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fanxiaobao.xyz/Article/details/gxloyomor.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaiurwucb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgpgxdpb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fanxiaobao.xyz/Article/details/gtzubypof.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwaufacl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gedjglkxs.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fanxiaobao.xyz/Article/details/gneglxbgs.sHtML

[N10] 链表节点定义
来源：http://blog.fanxiaobao.xyz/Article/details/gqzwhkahs.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fanxiaobao.xyz/Article/details/gdjhdgpgf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpuuabbz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fanxiaobao.xyz/Article/details/ggoybzqxf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvknrbkwh.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fanxiaobao.xyz/Article/details/gowaseodo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fanxiaobao.xyz/Article/details/gksixvnli.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fanxiaobao.xyz/Article/details/gptxlucmu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyfpzabp.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/grswdegls.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdrcwecn.sHtML

PHP:  // 手写递归函数
来源：http://baike.fanxiaobao.xyz/Article/details/glvtggxcq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fanxiaobao.xyz/Article/details/glgrrvtsz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpyhlbgw.sHtML

Java: // 手写递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gvweohvbu.sHtML

Go:   // 手写递归
来源：http://read.share.fanxiaobao.xyz/Article/details/gggheqlay.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnmvjnke.sHtML

C#:   // 手写递归
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkaxycxj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fanxiaobao.xyz/Article/details/gpznducgq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fanxiaobao.xyz/Article/details/gwvebhwjh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fanxiaobao.xyz/Article/details/gjiypeihs.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fanxiaobao.xyz/Article/details/gkvmxktto.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fanxiaobao.xyz/Article/details/gateuzbbp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fanxiaobao.xyz/Article/details/gguiofgoc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fanxiaobao.xyz/Article/details/gkwvrgqhv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzafgzyjr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fanxiaobao.xyz/Article/details/grrelgstt.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/goetgvqhp.sHtML

O. 并发与异步
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrjhpaza.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gywwsehkx.sHtML

[O01] 启动一个线程
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjhlnxrf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fanxiaobao.xyz/Article/details/gislmcvxp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fanxiaobao.xyz/Article/details/gcyzosnkp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fanxiaobao.xyz/Article/details/gpjjryzwv.sHtML

TS:   // 同 JS
来源：http://baike.fanxiaobao.xyz/Article/details/gmskneogv.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fanxiaobao.xyz/Article/details/gsfnpredw.sHtML

Go:   go f()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhbhtsor.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhdgaxel.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fanxiaobao.xyz/Article/details/gcskmrchj.sHtML

[O02] 使用线程池
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gooxmtqnz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fanxiaobao.xyz/Article/details/gbvvhphgc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvhfmwko.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fanxiaobao.xyz/Article/details/gsnsjcedq.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvnkdkoj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fanxiaobao.xyz/Article/details/guhpwfljy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fanxiaobao.xyz/Article/details/grwyrljcr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fanxiaobao.xyz/Article/details/ghaqpwtox.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fanxiaobao.xyz/Article/details/gakrpuovi.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fanxiaobao.xyz/Article/details/gtsygalxf.sHtML

Py:   with lock: shared += 1
来源：http://baike.fanxiaobao.xyz/Article/details/gtkkptbni.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhzifdzv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjhenipo.sHtML

TS:   // 同 JS
来源：http://read.share.fanxiaobao.xyz/Article/details/gggmutaxe.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxtmqnsz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fanxiaobao.xyz/Article/details/gbxeqhikv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gkerenovs.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjuksdwyn.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gywjylaqg.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfacbzcc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fanxiaobao.xyz/Article/details/gvxbtuxuk.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fanxiaobao.xyz/Article/details/grxoqupla.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqluhorim.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fanxiaobao.xyz/Article/details/gdncfqave.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuldscwm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fanxiaobao.xyz/Article/details/gmmccufrw.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gckoyfbmv.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fanxiaobao.xyz/Article/details/gphvqoiva.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fanxiaobao.xyz/Article/details/gqhlktsve.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fanxiaobao.xyz/Article/details/gbiqipuwj.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fanxiaobao.xyz/Article/details/gkwpyvwql.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxmytnae.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fanxiaobao.xyz/Article/details/gjjwpwggw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvwphngk.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxviswaaa.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fanxiaobao.xyz/Article/details/gvchezqxp.sHtML

[O06] 使用进程池
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkttvseb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fanxiaobao.xyz/Article/details/gpolloyqx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcsfzfxn.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fanxiaobao.xyz/Article/details/gbaskrjux.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fanxiaobao.xyz/Article/details/gufbocagc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fanxiaobao.xyz/Article/details/gwwhaljpx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fanxiaobao.xyz/Article/details/gsazbecib.sHtML

Ruby: // fork 块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsemchwzi.sHtML

C#:   Parallel.For
来源：http://wap.fanxiaobao.xyz/Article/details/gmcjphonn.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxqdonfq.sHtML

P. 常用工具函数
来源：http://baike.fanxiaobao.xyz/Article/details/geszzdult.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ghprrdupj.sHtML

[P01] 生成 UUID
来源：http://blog.fanxiaobao.xyz/Article/details/gfmcckwyl.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fanxiaobao.xyz/Article/details/gijfocrdo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fanxiaobao.xyz/Article/details/gdctktoaa.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gktgyazid.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmclxkdlk.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fanxiaobao.xyz/Article/details/gfvfgkgug.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzafljnu.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsrjkcra.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsorwouj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fanxiaobao.xyz/Article/details/grhrcxpxg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gieglikso.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfiwikkox.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccxaflmi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlgogeri.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrlowacm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gflbzsggx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagcwryyl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpguwxusa.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/goobbtqwy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fanxiaobao.xyz/Article/details/gxdfainls.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfdgzmhy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggofzaatb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/gornerlas.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnkiocxl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fanxiaobao.xyz/Article/details/gifuujqpk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fanxiaobao.xyz/Article/details/geycmhqlm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsjuyaud.sHtML

[P04] 求长度
来源：http://blog.fanxiaobao.xyz/Article/details/gaigsmptx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnlfbpmz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fanxiaobao.xyz/Article/details/gwfvdihbt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fanxiaobao.xyz/Article/details/gbbrxcjei.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fanxiaobao.xyz/Article/details/gluehadgw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fanxiaobao.xyz/Article/details/gqthemtau.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fanxiaobao.xyz/Article/details/glnzslcjr.sHtML

Ruby: x.length;  x.size
来源：http://blog.fanxiaobao.xyz/Article/details/gciqjcpvf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjvwvpyj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fanxiaobao.xyz/Article/details/grkdfmnvx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grylfozkh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfhqjjgy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fanxiaobao.xyz/Article/details/gttcboyez.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/guedquipw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fanxiaobao.xyz/Article/details/gsaywvrvh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydndshwd.sHtML

Ruby: a == b
来源：http://read.share.fanxiaobao.xyz/Article/details/gplqdxrku.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fanxiaobao.xyz/Article/details/gkltzedyt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fanxiaobao.xyz/Article/details/gnuofvtvp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fanxiaobao.xyz/Article/details/gfjgevgwq.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gkdacuxsm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgdpnata.sHtML

TS:   if (x == null) {}
来源：http://blog.fanxiaobao.xyz/Article/details/ggvymqdjv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzycoznuq.sHtML

Go:   if x == nil {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gorqtsecg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqxwfhyn.sHtML

C#:   if (x is null) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzsswbix.sHtML

[P07] 防抖与节流
来源：http://m.share.fanxiaobao.xyz/Article/details/glptyqaqa.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgxmglpb.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fanxiaobao.xyz/Article/details/gmjqdmufr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gacwjnfxa.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gvjerbarg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpocabcyc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasommzre.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gvksnvdhj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fanxiaobao.xyz/Article/details/grszuledv.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fanxiaobao.xyz/Article/details/gjgelgbvv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqruvtmsx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggcnazzx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fanxiaobao.xyz/Article/details/grvplpjaq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkeyutknm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fanxiaobao.xyz/Article/details/gqzhafzfu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fanxiaobao.xyz/Article/details/gvobbyegv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghupcljpl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnsheiuq.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxjmaeig.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fanxiaobao.xyz/Article/details/gobrxzgzz.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/groxuizgo.sHtML

[Q01] 创建表
来源：http://read.share.fanxiaobao.xyz/Article/details/gxofephfa.sHtML

CREATE TABLE users (
来源：http://baike.fanxiaobao.xyz/Article/details/glxrktyut.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fanxiaobao.xyz/Article/details/glaooruhz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbyylaac.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fanxiaobao.xyz/Article/details/ggalbxyfu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fanxiaobao.xyz/Article/details/gwjdkpzbt.sHtML

);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhierrnv.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqgbgwvl.sHtML

CREATE TABLE orders (
来源：http://3g.fanxiaobao.xyz/Article/details/gqkqizpws.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fanxiaobao.xyz/Article/details/gdebdsijc.sHtML

user_id INT NOT NULL,
来源：http://baike.fanxiaobao.xyz/Article/details/gbdyvhajk.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fanxiaobao.xyz/Article/details/gyuqyyotn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fanxiaobao.xyz/Article/details/glsxqxpqd.sHtML

);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givpdhcta.sHtML

[Q03] 增加列
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjlobsoa.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmylkzvu.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcsxmtxl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxijzfvr.sHtML

[Q05] 重命名列
来源：http://3g.fanxiaobao.xyz/Article/details/gsamytagr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fanxiaobao.xyz/Article/details/gexptbpss.sHtML

[Q06] 删除列
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpwfntwf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fanxiaobao.xyz/Article/details/gcuejsypi.sHtML

[Q07] 删除表
来源：http://3g.fanxiaobao.xyz/Article/details/gpgkpufgj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxlusyjs.sHtML

[Q08] 创建普通索引
来源：http://blog.fanxiaobao.xyz/Article/details/ggivtvzow.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fanxiaobao.xyz/Article/details/grzzbxvus.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcznvkuvo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fanxiaobao.xyz/Article/details/gxisjwbnj.sHtML

[Q10] 插入单行
来源：http://read.share.fanxiaobao.xyz/Article/details/gntrretnh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/guzvuomvx.sHtML

[Q11] 一次插入多行
来源：http://baike.fanxiaobao.xyz/Article/details/ghqzlbocl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gjtbevxyt.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fanxiaobao.xyz/Article/details/gibpdfamq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhypgboz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fanxiaobao.xyz/Article/details/gddzisfvh.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fanxiaobao.xyz/Article/details/gjajtwlrc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/gylaupqpe.sHtML


<!-- 参考信息 -->