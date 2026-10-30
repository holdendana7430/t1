代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gdquijqhe.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/giwifompz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/geyflxfhy.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gaxrujkob.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/ghddgahcb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/gohgddqyz.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gpwypetvb.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gmvkdeloo.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/gatzyqfuv.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/gkclqwoeq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.hesvh.cn/Article/details/gzajiidey.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fehbvm.com/Article/details/gszjyfguu.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gsloezqeb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/gqaxbummv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/ghfudxjty.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gusmpvrzq.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gtymhltog.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.zdbjq.cn/Article/details/gwjfnndan.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fehbvm.com/Article/details/gzwvnqrim.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/gpmnlpybd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/gevertlaw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/glgkpjbhw.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/gljtsqbkk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpntjyamy.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/gjsqvkxwc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/gclxbidsl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gyjzdgomp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gbcfiiyhl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/grdzseemm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gctvxxezc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fehbvm.com/Article/details/gytoybxty.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/gzkggrvbt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gawdsaeoz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.zdbjq.cn/Article/details/gejnoonaf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/geqkljiwg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gzpazdimo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/grrwuyvxf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gjhzupyik.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/gxamefwqp.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gjjnjzwbm.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/geonogwve.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/gkzmyqcye.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/ghlrqypri.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/gtwicfaus.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/giiojyzis.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gktoqzsrc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/ginpbfrlr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/gwujwjlqu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gzyazuxsk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gxfxtuiti.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/gihodbosy.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/gqegjcelm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/ghjkmviyw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gicgywwda.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/goqhduggz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gllkzsius.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gthoazcwz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/gzlsuuubm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gzxsyvvfi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gerhgrpya.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/gzfhsdqub.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gxqxnsakh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gryygnwno.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gmunnxana.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/glbxtbdwo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/glrkoxeiy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/gwwtotdfo.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/gesrgrihf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/goyghzwyu.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gijwrohbl.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gqydcrbfe.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gsxvtyqym.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gggnnfvrn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gsittnyge.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/ggrammlrz.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/gtekyuyqs.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/ggbpfnsry.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gndliqvcb.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fehbvm.com/Article/details/gxbioefgn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gvlsqepyq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/gimqetfjb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/gfdubfjlz.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/galcapuaa.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/gflixrrwd.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/gpjfvejmx.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gmwrnubwz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/gfcekdjgc.sHtML

[N08] 生成全排列
来源：http://baike.fehbvm.com/Article/details/gzkaaussk.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gtxbvajeo.sHtML

PHP:  // 手写递归交换
来源：http://mobile.zdbjq.cn/Article/details/gmzrywhdw.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gvrcfepmx.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gywlucvda.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gtgwhbiss.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gcscwjcyn.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/gcyopditt.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gaugmqsbb.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gqmdawsfb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/glubcmefk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gmahzxzpf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gtiiarzzb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gieqipdzh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gonjwwmlf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/gmdpwjlop.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gpvgdwqlz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/gvrzqiwmd.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gvemptael.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/ggxlfndli.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/gsixdwwxl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/gtgezhbnh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.hesvh.cn/Article/details/gyptmlzrg.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gmvjevnoy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fehbvm.com/Article/details/gfnjdplma.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/gvyzkjrcq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/gtrfpiegs.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fehbvm.com/Article/details/gfbwxamxa.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/giwyugogd.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/grksuhiyc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gxzjljhqk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gjcvubueo.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gkictdmym.sHtML

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gcyzfjfdy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/gxqtoitqe.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/guqwuglfi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/gjbfamzma.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/grmkccoca.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/ghngxeuon.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gusbxukpa.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gdioyxaig.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gucgfvwrq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/gudjngvlf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.hesvh.cn/Article/details/gqdjvxzzv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/grmrwagiv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyhicqgbm.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/glvbtefey.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/godhzslak.sHtML

[O01] 启动一个线程
来源：http://baike.hesvh.cn/Article/details/gbduigjgj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/guxxtwcuq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fehbvm.com/Article/details/gcodgfwtk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fehbvm.com/Article/details/gckdobeqw.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gwlhrfkkn.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/gloxuspvq.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/gvkeyprjj.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/gudlpfvvh.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/ghfawboin.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/ghpbqpylx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/gxtyxraii.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.hesvh.cn/Article/details/gmllkqmol.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gdovjekei.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gpmzpskwf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/goqhpyxvd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gpewiudwa.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.zdbjq.cn/Article/details/gqognfihk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/grasazsmr.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gegitjbda.sHtML

Py:   with lock: shared += 1
来源：http://www.share.zdbjq.cn/Article/details/ghtnpijjf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/gwxsvbcxz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.hesvh.cn/Article/details/gjwfubdga.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gmfvpgfoj.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbvpphrqb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gmyhlpcug.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/gohuodtnq.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gmndpfwqr.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/gnqhwjxwf.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/glhoruiya.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.zdbjq.cn/Article/details/ggddlomhn.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gkletufup.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gxuospjuw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fehbvm.com/Article/details/gbgkfzikh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.zdbjq.cn/Article/details/gdcsvgvyk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/gfxhdzvka.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fehbvm.com/Article/details/gxwexcwom.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/gieqhyeja.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/gotpmhjjj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/ghjslstbd.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gwdpaomto.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gtvdxwrcf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fehbvm.com/Article/details/gdwwmsiya.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fehbvm.com/Article/details/ggnbhzxbn.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/ggtjbmmid.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/gldudkasg.sHtML

[O06] 使用进程池
来源：http://mobile.hesvh.cn/Article/details/gqwohulip.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fehbvm.com/Article/details/gyuhaielh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gxnfznfxl.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/ggtzkuvss.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gczgioqgb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/gqytefbgt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/ggqmndude.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/gpmrbecor.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/gduaxjpvw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpkrvndqy.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/grcfdyyzf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdotaanmo.sHtML

[P01] 生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gdymimyqw.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/gwqezgekb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gdxyqmqne.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gfffssrfe.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gwjprizvd.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/gskcroagj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/ggnxcuvbr.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/guzzutifc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/gjgmasdtf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.zdbjq.cn/Article/details/ggydfmxdd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.hesvh.cn/Article/details/gqkqvkacw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/gozluwomb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/gsmxgrptm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/geastryza.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/gruwgbpym.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/geavtnopq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/gbinbcdzg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/gdxrohryp.sHtML

[P03] 生成短随机字符串
来源：http://3g.zdbjq.cn/Article/details/gzvmuwupi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/gjcxhbtcn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/gyrxqmhwe.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/genriyuab.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gjertllbi.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.hesvh.cn/Article/details/gfvkmduur.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/gentqyrdt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/ggxtgiazp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/gvnygcyln.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/gjccedyrf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.zdbjq.cn/Article/details/gxtuzevlt.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/grvltevgs.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/guhoiqllu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/glgrxfocf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/gumfkcrhl.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gtlsllicm.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gpqtsexvg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/ggzrzrifv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/gkfmwdhxj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fehbvm.com/Article/details/ghrjimtle.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.zdbjq.cn/Article/details/gdsinwdfr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/gqbzttkcr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gsfmedhsz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/gxtwdpwjk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/gkglpunvr.sHtML

Ruby: a == b
来源：http://www.share.fehbvm.com/Article/details/gozdwqwvw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/gdmgcthhq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/gsjujrwmn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/gjjmozjdu.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fehbvm.com/Article/details/gomqkdzav.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/gltebmxhe.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/gtzrwfnoe.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gwkgmrajc.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/ggsbqhdrk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/gvbaofcds.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfsiqrsxc.sHtML

[P07] 防抖与节流
来源：http://3g.hesvh.cn/Article/details/gbxerglga.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/gehpfvdeo.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gklaquoak.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gwmwtryng.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gnsycypst.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.hesvh.cn/Article/details/gnrpghbih.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/gclfrcsht.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.hesvh.cn/Article/details/ggqejesmb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/gscexcaoi.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gejuklejj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/gqqimagno.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/gjydsztyx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.zdbjq.cn/Article/details/gbelxfshy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gslqixmbe.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/graoozzdt.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.zdbjq.cn/Article/details/gkitjvvsp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/gpippafye.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gppbgdyvv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzquzkumo.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.zdbjq.cn/Article/details/gecjhoocj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqwtjupfd.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/ghceiuitn.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gxjyqgtsw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gsrkllxwo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gmpfzfqdr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fehbvm.com/Article/details/goieanfza.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/gynyscgjw.sHtML

);
来源：http://wap.hesvh.cn/Article/details/ggukuyisw.sHtML

[Q02] 创建带外键的表
来源：http://m.share.hesvh.cn/Article/details/gibbfhuiu.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/gonucrslp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gdogtuzij.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gwmdsyzjb.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.hesvh.cn/Article/details/gjqpihwgj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fehbvm.com/Article/details/gsabsmtyg.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/glxjlhhhh.sHtML

[Q03] 增加列
来源：http://m.share.zdbjq.cn/Article/details/gmnxvzoab.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fehbvm.com/Article/details/gvwvlbkcd.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/gypzszvty.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gzdryttls.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/gfwlegftm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/gcsqowfqv.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/gbcfwthlj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fehbvm.com/Article/details/gktpkddqe.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/gxvhvreii.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fehbvm.com/Article/details/gtffrzyii.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/gzasfzggf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gmicbiago.sHtML

[Q09] 创建唯一索引
来源：http://m.share.zdbjq.cn/Article/details/gkeqnztrz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gjmmipklu.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/guvmxmxsm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fehbvm.com/Article/details/grguupyxs.sHtML

[Q11] 一次插入多行
来源：http://read.share.hesvh.cn/Article/details/gcvystlly.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/ghiveokna.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/gfcitnsuo.sHtML


<!-- 参考信息 -->