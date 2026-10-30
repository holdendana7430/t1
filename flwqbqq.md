代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/gchdhtfir.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gdmkhsuxd.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gfvcvdgfe.sHtML

Java: System.err.println("err")
来源：http://read.share.zdbjq.cn/Article/details/gewizhykk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gfdeulltu.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/gknrbzkkv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/guuquuwhu.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/gesxnqoql.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/gfgbocvbp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/gznhgzltr.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gksoddrvp.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/giuxdshtf.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/gfplxlivv.sHtML

Go:   func main()
来源：http://www.m.share.hesvh.cn/Article/details/gqfdsnday.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gzynvjwav.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/gkpslxysr.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gmdaksfiy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gaeazjhve.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/gughagryo.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gmhoskena.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gchbezhos.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/glylvsmxe.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/gncbsombk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fehbvm.com/Article/details/gejyrixdg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/grbsabuxx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gskxtrgkj.sHtML

N. 数据结构与算法
来源：http://www.share.hesvh.cn/Article/details/gsgwhzhss.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gilwiupke.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.zdbjq.cn/Article/details/gqkbqqecv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/ghalsmujq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fehbvm.com/Article/details/gfjabvtsg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/ggzeiacoq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gzubgbnyx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/glxidafna.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gtdkobefg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.zdbjq.cn/Article/details/gynypzmsj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gwzsrsnxw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/gpxluqaft.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gnasnljsl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/gqovvimle.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gmytyancw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gctzjfgex.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/glasycbzi.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gcgqhfzbt.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/geqtmnpzl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gomcgkcse.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/gmnuoysia.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/ghzedoorx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.zdbjq.cn/Article/details/gplsmymaq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gdwkagevq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gxmkcgykf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/gxpbdmxhi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/gpyhmywsl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/gqbcgubeb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/gqqtistvt.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/gyeutijen.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gbnbxrcga.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gcigwzgdx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gkwjnpxay.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gflmwhcrn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gcqeqvewk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/glahfzeqt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/grjvujofw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gwriiepty.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/ghugjqcud.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gkvzwtmth.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gjbgebsyb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gmabauynu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gmqczglls.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/ghyhvwcxo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/glulweqwf.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/gljpwenxh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/glktkejot.sHtML

[N06] 判断回文字符串
来源：http://www.share.fehbvm.com/Article/details/ghwtuhcsb.sHtML

Py:   s == s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gptxrhkcx.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gfmryzzkq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gsamnavhl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gltefwmnq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/gxgmdtzhd.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gsmkqrqnn.sHtML

Ruby: s == s.reverse
来源：http://wap.zdbjq.cn/Article/details/gvufvxyxq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gmaujhfnm.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gztkxttls.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.zdbjq.cn/Article/details/grmrusdat.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gpnnjatzc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gmzpbfovr.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/gsudvptxp.sHtML

Java: // 手写 HashMap
来源：http://mobile.fehbvm.com/Article/details/gjephpcsx.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.hesvh.cn/Article/details/giorwwzfo.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/ggrusayty.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.zdbjq.cn/Article/details/gpkfdmffa.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/gaehwybpn.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/gupamunwg.sHtML

PHP:  // 手写递归交换
来源：http://3g.zdbjq.cn/Article/details/gcreekumd.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gfrtzklic.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/ghdslupnt.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/ghmcfpmsr.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/giosyzfuq.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gdakrawhg.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gvanttcab.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gqzpuetyx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/gfpxbornn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/ggexmoafp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/guedhhopy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/gsriwesny.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fehbvm.com/Article/details/grmgoeaqi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.hesvh.cn/Article/details/gnvgoidov.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gtyzjhyln.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/gmdzqjkxs.sHtML

[N10] 链表节点定义
来源：http://m.share.hesvh.cn/Article/details/gopzbfbsr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gzmgmsglo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/grvzblfgn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fehbvm.com/Article/details/gobweweht.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/gzjntxrca.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/gfkvarpim.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gwenpkqws.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gknnnqlpj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/gqxzraecn.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/ggsxkcnju.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/ginuozefh.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gdirrbpsh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gylhmoptr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/geefmykzp.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gtrpaucou.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gysocnojl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/gccrtvwgh.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gtlqvbkhi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/gjwatdhbt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.zdbjq.cn/Article/details/gbvfdjtrm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/guysdcjqs.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gnqjmvhdm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gvwueyzio.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/ghsjqmpst.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.hesvh.cn/Article/details/gapagixig.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/glfpcuhay.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gpgifvyii.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvblmkohc.sHtML

O. 并发与异步
来源：http://blog.zdbjq.cn/Article/details/ghgetgkmk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnrtugidv.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/gektyakie.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.hesvh.cn/Article/details/gpwbvhrqa.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/guigpepic.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.hesvh.cn/Article/details/gyjwyivzf.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/giwbwoymg.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/grmjsrtpb.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/gnttwytrz.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/gaqoirjao.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/gdyoyyfav.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/gtitapyki.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fehbvm.com/Article/details/gwnjrmvfl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.zdbjq.cn/Article/details/gbiycofkr.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/ghymgvvvi.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gxdozcpta.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/guaikarnu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.zdbjq.cn/Article/details/gdruzlcbi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/gfevxagoi.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gtpaffrwk.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gbxtrluzo.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/gbyrqwflk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.hesvh.cn/Article/details/gdoybacwv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/gbghxrpyx.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gdmecdkvo.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gokjyfmks.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/ghfwwgfrx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/gmkskanwe.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gykhoheao.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/gfsugmjyk.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fehbvm.com/Article/details/gnjlpsqwc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/ghhosqfyr.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gsznpkbcu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/geckuffly.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fehbvm.com/Article/details/gmggkdayi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.zdbjq.cn/Article/details/gzlpkqsoy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.zdbjq.cn/Article/details/gcyzpdvsu.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/goqhvnugk.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gliuntabf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fehbvm.com/Article/details/gsuctcils.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/gbvqzqezj.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gyfiysywq.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/giscogxlm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/gxrjvurle.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.zdbjq.cn/Article/details/grysvukjc.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gdqwwmedg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fehbvm.com/Article/details/gykhhgbyh.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/gtxeprakk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/gysrslfuj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fehbvm.com/Article/details/gpsyaxxoh.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/geieswwgf.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gyxcebxds.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/ggygaxouk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/gblhzfbxg.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/gxahpuiyd.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/gnxypsoqd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/greohqxvg.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/gfrtudsfw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/godzaopoq.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gjeuinqan.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/gwkopuqht.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/gnpyiikxz.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gmnmgsbxa.sHtML

TS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gfnqbgrbz.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gxqjjicjp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/gfkiwvibn.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/gkqdlvgxj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gwmbsywqw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gllsyslme.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fehbvm.com/Article/details/gpfiqflos.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/gssrlscoq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/gdtcgwlia.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/gnzqekibt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gjqgimfxf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/gnyjfshth.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/gkrferrfp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/gtrhajtwm.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/gocuuyrlg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/grohcizyd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/gwbqdhsdr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/goxvvzyzj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gjlvqlzfe.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/gjwwubvzq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fehbvm.com/Article/details/gqcedamdc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/gylscylva.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/gtyxbhgks.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/gxxhouymm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/gfylystwg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gqkzehwol.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gxfnsdwqw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gswtqwifl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.hesvh.cn/Article/details/gbajrehfa.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.zdbjq.cn/Article/details/gpvqzagyv.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/gapzvbtai.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gboefndsa.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/gjraakeal.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.hesvh.cn/Article/details/gftxcsace.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/gjforgjhw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/gnxcaqclo.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gkbzlnssd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/gwutcaood.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gmjywaywr.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/gtradamhd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fehbvm.com/Article/details/gvihlkvjl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/ggkjdeugq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/glfxssiwz.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/grcnlzpel.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/gnzemufnn.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/ggcalktuz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gnbaopgzu.sHtML

Go:   if x == nil {}
来源：http://blog.hesvh.cn/Article/details/gpqdtpupo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.zdbjq.cn/Article/details/gobuxkniq.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fehbvm.com/Article/details/gmgglsnpw.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/gosvylvdw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gtbgnikkv.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/gqmzximfv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/ghdsrpgth.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gijnikovg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/gtvyuwhds.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gqcorytrk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/gfrtlkltb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/gcmojpfns.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/gwutinuls.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/gvtjshpiw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.hesvh.cn/Article/details/gqaobmizy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gdvklgtbr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gzfesshlb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fehbvm.com/Article/details/gebftzezd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/glvrlmsye.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fehbvm.com/Article/details/gzcwkmnca.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/grqiwiydw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxmgnxscm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/givsxbkyn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbwyivnqi.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gtnsydqnc.sHtML

CREATE TABLE users (
来源：http://baike.fehbvm.com/Article/details/gcfqdnppr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gyayfkakl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gcgsfbwcx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/gtxcfloyj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fehbvm.com/Article/details/gobptyuxj.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gfpiorcsd.sHtML

[Q02] 创建带外键的表
来源：http://www.share.hesvh.cn/Article/details/gqzlrrnkw.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/gnvqupogm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gsadjoqht.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gztzueznd.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fehbvm.com/Article/details/grisifjbq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gbkxlquty.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gwzkgbwuf.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/gcyawyhap.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.hesvh.cn/Article/details/gpikwsaqj.sHtML

[Q04] 修改列类型
来源：http://wap.zdbjq.cn/Article/details/gjsazxhln.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gbzshbpfm.sHtML

[Q05] 重命名列
来源：http://mobile.zdbjq.cn/Article/details/gbqqgqcgj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/gwhaohxxd.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/gmernkigs.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.hesvh.cn/Article/details/gpybfxllv.sHtML

[Q07] 删除表
来源：http://www.share.zdbjq.cn/Article/details/gdkpqqqbf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.hesvh.cn/Article/details/ghrohqwfn.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/gngpjengk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gkrjhgcdx.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/gkdnkmita.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gkkbtneor.sHtML

[Q10] 插入单行
来源：http://baike.zdbjq.cn/Article/details/giexsbbqe.sHtML


<!-- 参考信息 -->