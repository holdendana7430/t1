代发 wailian999

Ruby: exit 1
来源：http://blog.zdbjq.cn/Article/details/guoweapmo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/gdsjfeyuh.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/gkdyhidqk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gmwxetdaf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gkmjfdbch.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gzhdsompi.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gosmyksdq.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/glnozylnv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gkkwtshvz.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gydvhwtch.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/gvpsyttxi.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/gjqnrwrgo.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fehbvm.com/Article/details/gvbmpnphy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/gsxvbifti.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gadnaoupq.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gsskhmsgg.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gkjibdtha.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/gbvsdxgvv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.hesvh.cn/Article/details/gftmgqgfh.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gzojztkff.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gecusimkx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.hesvh.cn/Article/details/gholoswxe.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/givoymatw.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gueepvwlt.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gnsveiomc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/gspfvonau.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fehbvm.com/Article/details/gwkfccoqn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gmplfibyo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gxhpmjakl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gsybmesyx.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/gnsqxqxba.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glxdtkouj.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.hesvh.cn/Article/details/gujkxilun.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gskllqcux.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fehbvm.com/Article/details/gltcqmsnq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gftkgvuov.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gvdypdhuu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gnpzyfejv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gyteoxejn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.hesvh.cn/Article/details/gufvkiwmm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gulvcimoj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/gcgpvduwu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gnmlpzsrm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.hesvh.cn/Article/details/giodafvup.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gtaeiltpm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gmpokjzvu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/gtpnulwyx.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gqazhkbuw.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/ggyynvztl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/gahqmosaj.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/geyeqivan.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.hesvh.cn/Article/details/gmggdwmzk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/gfmggcahq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gedghjaop.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/ggjshyrcx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fehbvm.com/Article/details/gbmpisjjp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/goegdakeh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/gtmujxdcp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/grjbxoekh.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/gaeupldsg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gdshhlhvr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/guibeyjga.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gccwpoksx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gcdbycsdm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.hesvh.cn/Article/details/gkqnmhapb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/gjngktlnv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/glhpfbkby.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gqbycgvpw.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/gjqbsuyqp.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gipctfsmd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gscywxthw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/grcueqsvw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gbyhfnwuj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/gwfaxxqfb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/gigykjxni.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gbjgmdlvq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/gflsdebpq.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/goiqfmbhc.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/gbqjqdlsq.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gdadkmzcw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gzpqoywzf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/grmivjdon.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gsjisbrfm.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.hesvh.cn/Article/details/gbacrbzqa.sHtML

Ruby: s == s.reverse
来源：http://baike.zdbjq.cn/Article/details/gnisrskbl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/ggtivdcdn.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/givvuzszw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/gdizynnoz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.zdbjq.cn/Article/details/gsedgyerk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/grcnskfji.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/gulmxdyyu.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gkrgngiyf.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/gsgetesuu.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.hesvh.cn/Article/details/gfdocamso.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/gvoyifbga.sHtML

[N08] 生成全排列
来源：http://read.share.fehbvm.com/Article/details/gcbjtiesk.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/glnprvhkd.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/ghkaepann.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gqxeogegn.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gltcghtzd.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gplbkctpy.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/ggmgocgjh.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.zdbjq.cn/Article/details/gxahzewwl.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/goiqizjgu.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gjuoouvij.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.hesvh.cn/Article/details/gzhqybwfo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gmeudmsyt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/goijccygv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/glyfxynsy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gwgveafnn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gljuwzvnk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gscxmslui.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.zdbjq.cn/Article/details/glpzwqqgv.sHtML

[N10] 链表节点定义
来源：http://baike.hesvh.cn/Article/details/gkdmmtpvq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/gghrnaiuz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/guslzqtpc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/gdrgcvlne.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gldauhqqf.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/gmeweewst.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/guihlzmqh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/gmfnwdqip.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fehbvm.com/Article/details/gblxotste.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fehbvm.com/Article/details/gydrfgyaa.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fehbvm.com/Article/details/grpyxtavl.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gjvgcygjk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gwsexpsxi.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gecrhoeit.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gdgsvdtjp.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gpfhuxosj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/gnthhskhz.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gutclqnaf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/goeutbyap.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/gjfhqeerj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.zdbjq.cn/Article/details/gzgaqewno.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/giqsbzbzu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gkmjqndnm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/genmlrses.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/ghnubdxir.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/guidsjmol.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gulksrsqh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkyavwegy.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/ggdtbxvml.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjobuczdy.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/giezfsdyh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.zdbjq.cn/Article/details/gmksbdoxq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/gyndvhjyy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.hesvh.cn/Article/details/ggekncade.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gafsdeovy.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.hesvh.cn/Article/details/gpyskavdo.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gyzwodpwc.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/guovaxhca.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/ggchavrjl.sHtML

[O02] 使用线程池
来源：http://www.m.share.fehbvm.com/Article/details/gtusdxsdj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fehbvm.com/Article/details/gussadrcc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/gmxyvihzd.sHtML

JS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gadgoerbd.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gjjafegkq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/gotexkvhe.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/gikycfwih.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gtadswlwg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fehbvm.com/Article/details/gsbghqakx.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/gprsizpmv.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/glacwlbir.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gqstyidtl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fehbvm.com/Article/details/ggnlzjplt.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/guldvrsam.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gpotdozkb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/gcgylyebx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gqlgwxiny.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gdluyqqyj.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/gospobvwo.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/gontoczwm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/ghdhesojh.sHtML

JS:   async function f() { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gofdtoidh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gndebokst.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gmkmcgloi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/gcgqvikbm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gzinspqup.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/ggigxcxub.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/gugzweojp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.zdbjq.cn/Article/details/giatphrcz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/gazknlcow.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gzrkkfgoq.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gokvixjdh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fehbvm.com/Article/details/glpfdcrpa.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/gadvcinls.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.hesvh.cn/Article/details/ghscnqgpx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gkfynpnlt.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gmjlbqxmk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/gaiojpfri.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.zdbjq.cn/Article/details/gyjsxuafs.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gxhqqerkn.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gzoobqliv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.zdbjq.cn/Article/details/gciqgrvia.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.hesvh.cn/Article/details/grcakwkbx.sHtML

Ruby: // fork 块
来源：http://www.m.share.zdbjq.cn/Article/details/gdpnyisnl.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/gzhtohhbn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggycvxklj.sHtML

P. 常用工具函数
来源：http://www.share.hesvh.cn/Article/details/gbsqzjewi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gccfzgfle.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gsalqobou.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/glvpnnfzp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gbfsswlgl.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gdzokqbqh.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/grybqepsl.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.zdbjq.cn/Article/details/grdsqirfy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.hesvh.cn/Article/details/gbdrwjhsv.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gnbcpencz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.zdbjq.cn/Article/details/grqpyhwzc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gpievqmhq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gcyciwfcr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/gcuobhpma.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/gsymghewp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.hesvh.cn/Article/details/gqvgfzghp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/gbbobvtqz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/geirchyjx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/gpbtwlysg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/gqulmthzo.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/ghyueuynk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fehbvm.com/Article/details/gbumdsjhc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/gorvhfdte.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gswpmtrvi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gwvjgtwec.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fehbvm.com/Article/details/gifhwakze.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fehbvm.com/Article/details/gethkhojd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/gizyraseh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/gjizqxauq.sHtML

[P04] 求长度
来源：http://www.blog.fehbvm.com/Article/details/gbugsjdvo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gmvdzrybb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/ggqkalbha.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gknvybppm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gxqgfilru.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/gratmipop.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/glfzxghxu.sHtML

Ruby: x.length;  x.size
来源：http://wap.hesvh.cn/Article/details/gdyhpwdhv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/gaswxfrwk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gudnapiyz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.hesvh.cn/Article/details/gellccrmn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.zdbjq.cn/Article/details/gogevmlau.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/gmhzuzsoy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gpnjyfugh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/gbjgouqxy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.zdbjq.cn/Article/details/ggcktyqbv.sHtML

Ruby: a == b
来源：http://baike.fehbvm.com/Article/details/gxjmhyypq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/gjayyyhpu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.hesvh.cn/Article/details/ghduiextm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.zdbjq.cn/Article/details/gwebkpbhm.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fehbvm.com/Article/details/goswoouru.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/gxekgsxeh.sHtML

TS:   if (x == null) {}
来源：http://wap.fehbvm.com/Article/details/gdvjqepwa.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/ggccoalmh.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/guxmoizat.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/gehurqxdl.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/glicrmjtd.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/gzyhfkgoc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.zdbjq.cn/Article/details/gzumuqcfd.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.hesvh.cn/Article/details/gklbgxtnh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/grjnvyrkv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gpwqqfboa.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/gpufiygzv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.hesvh.cn/Article/details/gsgdzdmhd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fehbvm.com/Article/details/ggaoxgvpa.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gyrnbqorj.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/gurnezcgn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.zdbjq.cn/Article/details/gornznfih.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/gmpalwcdj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/gwsxdpksx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gngorixlc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/gsqjxzegs.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/ghdcwdtui.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/gdiobakce.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fehbvm.com/Article/details/gotbplwqs.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gznpkdbir.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.zdbjq.cn/Article/details/gcumsdjlj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvlsnqwxu.sHtML

[Q01] 创建表
来源：http://www.share.fehbvm.com/Article/details/gfyxgjnpe.sHtML

CREATE TABLE users (
来源：http://wap.fehbvm.com/Article/details/givsghver.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gsizgbiqo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gnaqnyadd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fehbvm.com/Article/details/gbwcrcbko.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.hesvh.cn/Article/details/gepkrzmjj.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gupkdpwpw.sHtML

[Q02] 创建带外键的表
来源：http://www.share.zdbjq.cn/Article/details/gtbjsyltx.sHtML

CREATE TABLE orders (
来源：http://www.m.share.zdbjq.cn/Article/details/gpzdfjqpq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gadxfpqnp.sHtML

user_id INT NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/goyxfgymt.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/gskwajuxy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.hesvh.cn/Article/details/gtcxqkqtp.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gywmrlcvg.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/geglnlwio.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gfpphesma.sHtML

[Q04] 修改列类型
来源：http://www.m.share.hesvh.cn/Article/details/guhvzgbyn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/gljzqsiip.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/gsohonrdt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.hesvh.cn/Article/details/gszaliskn.sHtML

[Q06] 删除列
来源：http://3g.zdbjq.cn/Article/details/gfzizrfhl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gcwteryyp.sHtML

[Q07] 删除表
来源：http://baike.hesvh.cn/Article/details/gymhlczeg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/gzecbclpr.sHtML

[Q08] 创建普通索引
来源：http://read.share.fehbvm.com/Article/details/gjdpeaewy.sHtML


<!-- 参考信息 -->