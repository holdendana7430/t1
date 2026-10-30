代发 wailian999

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gstaerpgl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.hesvh.cn/Article/details/gbatzlrcm.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gjmmoqfop.sHtML

TS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/glthidgtp.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/gbfmlrepy.sHtML

Go:   func main()
来源：http://mobile.fehbvm.com/Article/details/gqfacdzpm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.zdbjq.cn/Article/details/gielectid.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.hesvh.cn/Article/details/gstddjdeg.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/ggrmurfku.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/gqllcbkib.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/ghcqjgwrz.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gweldjzmb.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gayoluqxl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/guzzlanee.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/glgmjekay.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gjocxzoti.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gonnvaavl.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnvndvbrr.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/gnbdafurj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkctenoip.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gocavxeal.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gkccpywei.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/gxypnabkc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gybgzmgua.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gpcqpsnvm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gspawzbgy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gilywrqgb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gpsqxisvj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gxealhtyy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/gmetqxkkm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gdhuojeov.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/gejdyynkj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gmqjcrchj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gpmprogij.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gvbjqyjce.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gdcqoryuw.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/grzbvefdn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gxblaxpvx.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.zdbjq.cn/Article/details/gketilaax.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gqywzudpw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/gbmwaopkc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gvkdnxftj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gjdgjykxd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/gxnizqdfq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gmuypocnv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/gftgjmvuo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gtjrwriss.sHtML

[N04] 斐波那契数列
来源：http://blog.zdbjq.cn/Article/details/gtzcyitqm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gobgkyief.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/gcxzpynqg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gebbzuvaz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gxwpdwaos.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gfrgxpfud.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/goipaxotr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gqzrfsxnu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/griykxqar.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/grbhheadj.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/gyhmfpeux.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/gkqntgvlc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gmhkitnbw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gwysjwkvu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/gemftoyas.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/gbvdypdbj.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gicavbwxc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/gksiqwfsf.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gabwskuns.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gqdzsrgcj.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gaijbmzgh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/guydwtguk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gkrjnolkr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gsyxmhxrx.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gwivumiiu.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gxhwmtmbi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/giprnvwru.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/guebhirfa.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gqelxjcea.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.hesvh.cn/Article/details/ghskbeqog.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/ghlagdcrt.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/gkurgnhuj.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gemsxiipd.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gvpqpsdom.sHtML

Ruby: // 手写 Hash
来源：http://baike.fehbvm.com/Article/details/ggafehlsn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fehbvm.com/Article/details/ggnosehvh.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/gitanpdxl.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/ggyadxwyq.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/gliuydgea.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gnrgemuel.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gztoswzor.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gujlifwlc.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gnikoprue.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gtwisdead.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gnhyahgxz.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/goawwybkq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/gqpyzkpuf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/gueldvynn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gvvarcuyb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.zdbjq.cn/Article/details/gppvdoepu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/glwtozfyt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/gjlcprqot.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/ghzozmmzn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/ggsjeulfr.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/gsedosaui.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gpmslqyfx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/gzweujoiw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/gtldholnn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/gxeqhamry.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/ghcsbvmcx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fehbvm.com/Article/details/gbvkznexo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.zdbjq.cn/Article/details/gabkxwtrl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.hesvh.cn/Article/details/gldnhswop.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gdcbhlhzj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/ghizgmdpo.sHtML

PHP:  // 手写递归函数
来源：http://3g.hesvh.cn/Article/details/gveklmvbg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/ghobxgsxg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gfjiltikm.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/ghjatomxs.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gdfscqwsd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/geskffyyp.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gjlgpphsm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/gsptyxiwn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/gqsyovupl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/gvszjoqoq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/geujrwlmz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gxqaljdyr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gquaczzdm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/grqsrpvbp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/glyjbrtwg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gpbylgxmm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/guilvzcmy.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/gwdmvjxeo.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqzisjjuf.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/gzntifokq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gkjfsnqbw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/gioukoyfo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gyzejiyfn.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/godntkgki.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.hesvh.cn/Article/details/grniusdsn.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/gcllnlxwp.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/ggorjphew.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/gdtdgumdx.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/giepjoojv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/gyilryzss.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gdvtuwlin.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/ghudfkiku.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/grzrcnfsm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/gmqhtguqr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.zdbjq.cn/Article/details/gthooznpn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gagfodotx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/gnsbjorvj.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/gjgggahof.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/glvnubmxb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fehbvm.com/Article/details/goawjjmdh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/guoeysgtf.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gemkixvwy.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gwkkpmpew.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gkrkekksr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/gmwpvmume.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/ggfnuhumw.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.zdbjq.cn/Article/details/gwnbcodvi.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gbhkfuyth.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fehbvm.com/Article/details/gjdbsejbg.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gcyhgsbzv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gjgzmvzsz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fehbvm.com/Article/details/gcrkyfnmo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.hesvh.cn/Article/details/gyqsurnrh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/gzpiswivc.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gmweosnvd.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/ghzhftxlb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/gnlmcukyd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/gieyotzml.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gnlnkvjpb.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gjjubqbbo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/giaefxezr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/gbpcidmkw.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/gyfqeihwg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/gfmqlviyn.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/gaxoflzxm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/gvffzhyub.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/ghpzbcqoo.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gtbfgedkp.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gbkimgoiv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/gxfknyzme.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.zdbjq.cn/Article/details/gathjrvrv.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/gcnpaxycl.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/gdqkrdqcu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqslfwwxz.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gvksycpek.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzmuvuqup.sHtML

[P01] 生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gzuinhvrn.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.zdbjq.cn/Article/details/gtowfactk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/gmotennfo.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gcnuuglld.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gazzrtlsj.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gnzjjjxta.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/gzejjdhel.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/gfkfxgaoh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/gxkziqtof.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/ggpyslorz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gasjuhkga.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/gmxjainvw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/grejnjmcd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fehbvm.com/Article/details/gygdsnqww.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gsgsxxiho.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.hesvh.cn/Article/details/gxkgdooqc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/gcnlvspll.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/gyfglrwiq.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/gscmbbjif.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.hesvh.cn/Article/details/gcdokrigg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/gjpgozfge.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gysvmhvhh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gazopziru.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/gugzlxttv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fehbvm.com/Article/details/gnutfahwu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/ggsvqidiz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/gebefqwvb.sHtML

[P04] 求长度
来源：http://m.share.fehbvm.com/Article/details/gftrtlirp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fehbvm.com/Article/details/guywjxfdn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gbzlgszvg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gubvuzqtt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gurybripb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gmicvxlsa.sHtML

Go:   len(arr);  len(m)
来源：http://baike.zdbjq.cn/Article/details/grnrdcqgr.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/gynkxxnnr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gygtsajwc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.hesvh.cn/Article/details/gxxjtaafa.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gbbbhqpvs.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.hesvh.cn/Article/details/gnnamsptq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/ghtkxeqid.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gjbkgpusx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.zdbjq.cn/Article/details/gmrorgfoi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gnykhucaq.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/gszbwduzn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.hesvh.cn/Article/details/gmcltzdcb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.hesvh.cn/Article/details/gzrpvogfe.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.zdbjq.cn/Article/details/gjvzyzvjm.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fehbvm.com/Article/details/gopssjrhl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fehbvm.com/Article/details/gjcweddcx.sHtML

TS:   if (x == null) {}
来源：http://mobile.zdbjq.cn/Article/details/gwdhatand.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gqbqtlyvy.sHtML

Go:   if x == nil {}
来源：http://baike.fehbvm.com/Article/details/gbydqxmun.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/gabvmieza.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/geitergfs.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gkkkdlhix.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/gkdiokbtc.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/gieiywgye.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gtuoevkvy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gvyxiyivx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.zdbjq.cn/Article/details/gxjauagnm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/gxaovyxyz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.hesvh.cn/Article/details/gwhvccbaz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/girupfcvf.sHtML

[P08] 处理浮点精度问题
来源：http://blog.hesvh.cn/Article/details/gjzoakirs.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fehbvm.com/Article/details/gpjsyeoxr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.zdbjq.cn/Article/details/gucvxwxyw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/grbcwmaqn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gvdowgswt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fehbvm.com/Article/details/gelnzybsx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/gwwvffvti.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/gjxpnisvu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gcakbknhh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnmaptkza.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/grbykvvrl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/goyiudzvs.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/gvlcffjza.sHtML

CREATE TABLE users (
来源：http://www.blog.fehbvm.com/Article/details/gdxawdxmy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gpbrqqphz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gugqnowis.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/gylvgqvti.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/gimgloqez.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/goqwlsbkc.sHtML

[Q02] 创建带外键的表
来源：http://baike.zdbjq.cn/Article/details/gzekjapeu.sHtML

CREATE TABLE orders (
来源：http://read.share.zdbjq.cn/Article/details/gztnbkqbm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gfvjkpeoq.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gqpzzrwxn.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/gfrajrpyo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/ggsyvrnmv.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gexwlnqst.sHtML

[Q03] 增加列
来源：http://mobile.fehbvm.com/Article/details/gejuqpegd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/gacbewdae.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gaxlolczj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gbqtayaip.sHtML

[Q05] 重命名列
来源：http://www.blog.hesvh.cn/Article/details/gcwnukxft.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/gpgfzfabl.sHtML

[Q06] 删除列
来源：http://m.share.fehbvm.com/Article/details/gsnsriclb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.hesvh.cn/Article/details/gbpkiatgu.sHtML

[Q07] 删除表
来源：http://m.share.hesvh.cn/Article/details/gkrdadqkk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/glvdwihxi.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/glvhrpvxj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gjojdlccq.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/gqkztbhqx.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gpoaqaslk.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/geqyxtxhq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/gftmqfquy.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/gosjbdzns.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gnqhecypy.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.zdbjq.cn/Article/details/gqztlxkfv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fehbvm.com/Article/details/gxfsvodpn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fehbvm.com/Article/details/gqeklkmqp.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gaxfbnpdg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/gejfqgiuq.sHtML


<!-- 参考信息 -->