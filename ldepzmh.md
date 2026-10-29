代发 wailian999

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/ggpxpbptc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/gwkqwaeox.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/gkwnyktsd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gbvdegjjg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.hesvh.cn/Article/details/gifvurnkk.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/ggidxbpse.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/golcdbfss.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/gjzdgqbvp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.hesvh.cn/Article/details/gsuaislij.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/gykiycbxt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/gdkuzfgmf.sHtML

[M07] 判断是否为主入口
来源：http://blog.hesvh.cn/Article/details/gbeiyrkmv.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gallihuwd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/gqjltfsvd.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gkxcycwjs.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gvwngaesl.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gnyvyrrth.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gkwpqgncj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/gunexyefw.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gwkzmzyhq.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gxmszblnh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/glqmkfype.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.hesvh.cn/Article/details/gcmppfhvy.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gwtvvdwpd.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/ggwbwthjn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.zdbjq.cn/Article/details/guatyqliz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/gdlyuramb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fehbvm.com/Article/details/gpjofwgwq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.hesvh.cn/Article/details/gojnnslvl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpfgdnfmz.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gtlgdzvkd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxdpsehuk.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fehbvm.com/Article/details/gnnncxpng.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gcjhdeksa.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.zdbjq.cn/Article/details/gepjgtmcc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gqdwzbvvu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gawkjvoge.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gklrthgxy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gtdnzihni.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/gjfgvgavx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gknvhjazd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/gxtkfvllg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gdhbxppgl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/gpbkjxvnz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gixodkinq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gbusdfypa.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/gdvjievyv.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gdvogkiwc.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/glexthvqy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/gzprmirtn.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gbxtlpvaq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gsetqjhgu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gsdjjjcpr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gsnfglzmv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gkihjmzbc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gyikdqfoh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fehbvm.com/Article/details/gulnydsdh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/grauykgdw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.hesvh.cn/Article/details/gvuajuwav.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gevdyqzex.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/geokttrdy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/giismvrhm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gvuvxqvup.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gabryrxpw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.hesvh.cn/Article/details/gazxpvccf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/grtqwbidk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gzqwswhpr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gjqgwltwj.sHtML

[N05] 最大公约数
来源：http://www.blog.fehbvm.com/Article/details/gksvyjoqg.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gvdirsldd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gtygvodls.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gyviikgzh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gqamjoyyq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.zdbjq.cn/Article/details/gvharcumo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gdksenigb.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/gbzmnxyic.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/gkgkbslon.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gmbsrhsat.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gauarzoai.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gqkftjdbn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gzzmjrilc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gvocclzza.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/golfenfrc.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/gtaqsxhly.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/gjqgjrmfd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gtahpevxs.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gheeozlfl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.zdbjq.cn/Article/details/gxguqvizu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/gpymtjyij.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/gjcocvdas.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/guiaxbhyo.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/ggmsxxfak.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/gfmhpdxui.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gncrqnrld.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gebcbbhdh.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/gbdokgexu.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/gaxkkebae.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/gclphcxzc.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gilhmkbdj.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gscnyxzfo.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gyynpfgmv.sHtML

Go:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gxxihzobj.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/gbucfaede.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gfarpdjlq.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/gyanwmoog.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gevkgijrb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gceluvowh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gnjvixzlu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gxdctdyyj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/giukiyfhs.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/gznzsbzoc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gliagnbto.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gxeuuekdk.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/ghtcxsqdx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/gvmmathct.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gifarfvfk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/gmhhlmotp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/gtzbwemkk.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fehbvm.com/Article/details/gqusdkccl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gcjfaxfdh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/goxmhkwvr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/grwqleqfe.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gxjkitwzg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/gvoswwzbv.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/gcvinboof.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gncuwhfpe.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/glndjweok.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/ginvfwxlq.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gqyelzbpa.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.zdbjq.cn/Article/details/ghjgnimsj.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/glwvcrncb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gzsztxgcp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/gzhfytmzh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/gutmlfwux.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/grttqziwy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gxtyazybb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gcudqhpft.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/gfcurvvay.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/ggkelgjnl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gtdrstkjo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcsujcmla.sHtML

O. 并发与异步
来源：http://read.share.zdbjq.cn/Article/details/gjhuvrfdw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbvvvugda.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/glvvjzwzv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/gkfountbh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/gogetvnak.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gugxfwvwc.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gfdljpcdg.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.hesvh.cn/Article/details/gohwgbosb.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gjeggkrqd.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/gwlyucpxk.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gqlirhuxq.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/ghligftsy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gplgvyexa.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.zdbjq.cn/Article/details/gacvuqbkp.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gxdoebdak.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/ggltxdvhn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gzwamxnft.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/glqzmatag.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.zdbjq.cn/Article/details/gwzexdxcz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/ggdbdfuyl.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gmbqacesv.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/gkmqsxfuf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/gjxuzbupl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.zdbjq.cn/Article/details/gnocutfij.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/grgqbxtnk.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gpmujxqrz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/gvecvwdrs.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/godzqkzqp.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gsucmokiz.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gaewxviic.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/gxzxsxwzs.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/gauhjgojk.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gshsietbt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/glsnbquzy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/geetntqtz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/gvddbvdtz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/gzatgkbtj.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.hesvh.cn/Article/details/gvyirynsy.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/gwboioqho.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/gfhhlaxpj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/glukldvge.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gdnpuduew.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gmalwqnvy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/gvuzubmsw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gkxoovgol.sHtML

Ruby: threads.map(&:join)
来源：http://wap.zdbjq.cn/Article/details/gnseijhcq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fehbvm.com/Article/details/glqyvkvgk.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gmbgbycuf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/gjfktgnis.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.zdbjq.cn/Article/details/gzpjibdcd.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gmcywnmwl.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gzgwehuxn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/gxkqtunhv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.zdbjq.cn/Article/details/gkpklnxog.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/gytteihtf.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/gteognoaw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkqgoskka.sHtML

P. 常用工具函数
来源：http://m.share.fehbvm.com/Article/details/gxlakybem.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/guozitycs.sHtML

[P01] 生成 UUID
来源：http://wap.hesvh.cn/Article/details/gqifvtoix.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/gtrmrbpus.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/gqmuxgayq.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gejwvrwtf.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gybxuyexc.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gbvgrvdey.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.zdbjq.cn/Article/details/gogmjsjjw.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/gauvollob.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fehbvm.com/Article/details/gbrsbaido.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/gdcocfqup.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.hesvh.cn/Article/details/gsshewwjy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/ggugdhymj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/ghqfxxgxp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/gibqzowwg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gpaljrfix.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.hesvh.cn/Article/details/gxayuhfwo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/gmtpvcttj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/gmqcosnax.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/goghpymnv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/gkervqook.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/ggmarrtwv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gjhzbehvl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/ghyecakjb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/gokzddkpm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/gtsvvsqdt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.hesvh.cn/Article/details/gdqvdoket.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.zdbjq.cn/Article/details/gajmeupwm.sHtML

[P04] 求长度
来源：http://read.share.fehbvm.com/Article/details/gqsrbzzrk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gbimhnahc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gmfgsfmky.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gqbmhkqlt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gswwimdbb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gkhcuxtmg.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fehbvm.com/Article/details/guoncggpu.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/ggiizdlkz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/guuqgilms.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/gawxdspio.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/giwwvudxw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/gwizslsta.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.zdbjq.cn/Article/details/gdqffthwy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gmxuqmmjh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.zdbjq.cn/Article/details/ghwdxerst.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.zdbjq.cn/Article/details/gatdcmgwr.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/gpynvmood.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gwmioclzr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gcablskgu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.zdbjq.cn/Article/details/glettpjnu.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fehbvm.com/Article/details/gbycsbnmm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/gfviffupk.sHtML

TS:   if (x == null) {}
来源：http://blog.hesvh.cn/Article/details/gkxqikneb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gmmlfaowx.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/gfdkrnnkh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/gzazuxbam.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjxvsrcdx.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/grntfpytt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.hesvh.cn/Article/details/gfloncerf.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fehbvm.com/Article/details/gjxxinbol.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gjczazmeb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gjvpcbllx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/gydraextz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.hesvh.cn/Article/details/gptbeeilo.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gvburwfda.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fehbvm.com/Article/details/gfmjmwklm.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/gowzbyrqz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.zdbjq.cn/Article/details/ghmqjmkra.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.hesvh.cn/Article/details/grwpxvptf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/gmdubybvv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gaxqanmlq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/gpsteflfy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.zdbjq.cn/Article/details/gtlinxkbh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/gvughshzv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.hesvh.cn/Article/details/gpborwvut.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gcfbcokkq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gxlihepfs.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ganhcjztm.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gqquywrno.sHtML

CREATE TABLE users (
来源：http://blog.fehbvm.com/Article/details/gbazxdhfl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gpulqzcei.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gyddtgrua.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/gxgushgqo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/glsoatxqi.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gndfisens.sHtML

[Q02] 创建带外键的表
来源：http://www.share.hesvh.cn/Article/details/gzgoxlwln.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gndgixkan.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gwbrhfyaz.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gqviagrtd.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/gjqhwtibx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/gkpsrulnq.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gjxuwkskf.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/gsnxyvslm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.hesvh.cn/Article/details/gaamrgpww.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gdghkroed.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/gqyizmkao.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/gqyffitwg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/gjmyzvxuw.sHtML

[Q06] 删除列
来源：http://wap.hesvh.cn/Article/details/gqkqpffgj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/gkevekvwz.sHtML

[Q07] 删除表
来源：http://3g.zdbjq.cn/Article/details/gdnznmokl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/gtgdfeawk.sHtML

[Q08] 创建普通索引
来源：http://baike.fehbvm.com/Article/details/grdijefjq.sHtML


<!-- 参考信息 -->