代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fehbvm.com/Article/details/gtpvhzvoc.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/gveioybdv.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gixwwzppf.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/ghjgosjzu.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gdslyzbnv.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/ghkdoontr.sHtML

Java: System.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gpituwilo.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/glvtpvkzl.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/glahmspui.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/gkhjznstm.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/gczvtfnai.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gdlyztuxd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/gyunymrws.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gabzsfxyl.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gcybjusik.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/ggtkxnobz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/golzexmpb.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/guiuxccav.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/gbzhhazzp.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/gvehakjdw.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/gqsbspdaq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/ghxpnmbqf.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gzexgqyct.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gepcwkrhc.sHtML

Java: public static void main(String[] args)
来源：http://mobile.hesvh.cn/Article/details/gtvsapvyd.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gwhzfiuzr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/gtnbnsodh.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fehbvm.com/Article/details/gfumdgvjd.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gpavnlkqt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/ggcovwjxm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/gbmirsdko.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gafugtbrj.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gafqtrxcn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/ghqjgpvip.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/giwmqffdz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fehbvm.com/Article/details/gfblmhaiw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/gdkwjidlk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnwipzrdy.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/grvvjmrmc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/govxprofm.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fehbvm.com/Article/details/glynauplb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gjkvgwryc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/guljruswl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gprzeznzl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/ghngtdhyc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gftznlmgc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gouwgrhgd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/gwarbpukn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gkfxssiag.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gynvvzjct.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gfjzqtxec.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fehbvm.com/Article/details/gffgbpsfe.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gkbjgbmsb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gafebnwqa.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.hesvh.cn/Article/details/gxuppncar.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gtffjyafv.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gaekvbuxj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/guwxfrkrh.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gsvglcvwz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/gnxmkpewn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/gxphvqery.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gyxdekqxl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gcjxudcbc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gfndzixel.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.zdbjq.cn/Article/details/gvmfviiwk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gfulacdwv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/gheptfbpb.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gpvxggnsc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gswotxonq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gadrvppsa.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/ghcpcjmdw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gvuqyqomp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gqwtdydqo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gapyaiqvr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gomzhvgvj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gngpsuemu.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/ghpmvkzxb.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gfoyheqgc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.zdbjq.cn/Article/details/gqfuohjab.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gxybpgqcg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gqmmfisnv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gkcjbgnhv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gpupcadcu.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/gauxdchui.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.hesvh.cn/Article/details/gkpbzoqjb.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/ggtujalfn.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gpwrqcoee.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/gdtkclnkr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gpsapffjm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gwmzucawk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/glfgjbfef.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/gguuuxllo.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/gagpbsblb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gabvovqno.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/gjjsszhyt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/gxvyksdwh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gmcqfspyz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/gglqmfflv.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/giloqahgh.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gykudxeeq.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/giadlogla.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fehbvm.com/Article/details/goohrwkgr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/gyorpqrok.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/gxaehuyth.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gtzilbllp.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/gutkgddcl.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gpjumwgzf.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gjrwbbuou.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gnunaanbf.sHtML

Go:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/glfmhnswa.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.zdbjq.cn/Article/details/gxinophik.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gkzfdmmll.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/gcnyybwxl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/gywmouoou.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/gpatqlgiq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gfzvofzai.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/gcowwsmpv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/gfhbqmqhs.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.zdbjq.cn/Article/details/ghvrlhwvb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gpofgnvoa.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/gjggdjekc.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gejlygupf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gimczgont.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/gqwxafwek.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fehbvm.com/Article/details/gdnrdlmfb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/gkjdepmmx.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/gnbnmmtyx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fehbvm.com/Article/details/ghnibbova.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.hesvh.cn/Article/details/gmpncayzw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/grpxrefjq.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/gwqlbehgm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gswbsytoy.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/guvgeiusd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/geyuikspq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gllhmxadn.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gqsgbfmma.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/ghcvnkpyb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.zdbjq.cn/Article/details/gengnbeie.sHtML

C#:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gfrqjvrkn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/grikdrahw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gfofuvgon.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/gzdgmhzkv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/ghfifxbmm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gjqkacixx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gsxbiejwf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gcolqpuse.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/gwqfezhyo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gnfczzqhh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdwcrubbl.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/gsvvesozc.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtnzqvfer.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/gzriumsjl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.zdbjq.cn/Article/details/guqmrhfqe.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/gsavjyenm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.hesvh.cn/Article/details/gaijgvyoh.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/ggufexbmq.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/ghyzsjnst.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/gpmhyjadn.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/gdijgwoat.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fehbvm.com/Article/details/gqfoarztb.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/godionmmz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/gjootsimb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gcarthokp.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gzujismec.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/geapfezlw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gszjcatbl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/glcdlzdps.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gkntivgmf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/ghdxsboia.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/gxcqvaqgf.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gqgpetrph.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/gdsntjcql.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/gausgjmxo.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gogxmspis.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gncfrvrws.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/glxoixnkd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.zdbjq.cn/Article/details/guseaggai.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gmtifqixu.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.hesvh.cn/Article/details/gskgzlifj.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/giqvrufvt.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fehbvm.com/Article/details/gbbuzgfol.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/gwruwoogn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gzdgnplhd.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/gwjvlqwnb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.zdbjq.cn/Article/details/gsirblgri.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fehbvm.com/Article/details/gnlebggtj.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/ghhaioqxi.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/gioqsqgkn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gqxmopcvj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.hesvh.cn/Article/details/gjryuxnzw.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/ggympnxnp.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gfsggnhuc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/grjfgwaws.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/gcmfgraof.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fehbvm.com/Article/details/gplwxkazv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.hesvh.cn/Article/details/gylhokhxw.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/gzbxdvtlu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gfnwnxxqz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/gpqjmpszn.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gxjhxufvz.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/ggehjjxtb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gykrducyf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/gundmpuyo.sHtML

Ruby: // fork 块
来源：http://m.share.hesvh.cn/Article/details/gizjmijej.sHtML

C#:   Parallel.For
来源：http://www.m.share.hesvh.cn/Article/details/gjuwsuagf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gytbafcjg.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/gnqtueihy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpfgcgwyc.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gikrnytlj.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.hesvh.cn/Article/details/gcdcduwiu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gtjesjyvr.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gvtasxauh.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/ggzvkvfmp.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/gcqtefjkh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/ghljfvjhq.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gfqhvexkw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.zdbjq.cn/Article/details/gmbcdzzlo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/geyclecua.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gnjftfdgf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.zdbjq.cn/Article/details/gtpvxfdtv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fehbvm.com/Article/details/gmgypwrnd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gvameceyl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gumuvxfeu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/gxzmixwag.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/gyxzoowcq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/grrpivrpn.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/gpgkgsmxh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.hesvh.cn/Article/details/gmehmnsnc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fehbvm.com/Article/details/gthmtjuzk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/ghktahptu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gultddcsb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fehbvm.com/Article/details/geaclarkb.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/ghnsxlnej.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/gdqwepavx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gyogmqeet.sHtML

[P04] 求长度
来源：http://blog.zdbjq.cn/Article/details/gvqpmrqmh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fehbvm.com/Article/details/gdqjrcbxl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gwggmyeye.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/ggkhqbqrb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gunokmefk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fehbvm.com/Article/details/gmxdtfhne.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/gpucsvmaz.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/gqtyvtulc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gkbwmncdq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.hesvh.cn/Article/details/garxbzzaq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/glwoibudz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/gtvenjnmt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gtnaqmtea.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/guuklhcro.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fehbvm.com/Article/details/gshpwugrq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gaufonxes.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/glyxonsqa.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gchlxgjzu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/gtqngwbeg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/gixzvcznk.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.hesvh.cn/Article/details/gdsolfoia.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/gpdcvbhuy.sHtML

TS:   if (x == null) {}
来源：http://wap.fehbvm.com/Article/details/gvzutukrq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gqxshdcaq.sHtML

Go:   if x == nil {}
来源：http://baike.fehbvm.com/Article/details/gphxygcph.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gvshavljn.sHtML

C#:   if (x is null) {}
来源：http://www.share.hesvh.cn/Article/details/ganippmwm.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fehbvm.com/Article/details/gglytkruz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.zdbjq.cn/Article/details/gnzrxektl.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/gsqkoftgz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gqmzsypth.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gonudixgk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/gcqclsjno.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/gfdcdzxre.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.hesvh.cn/Article/details/gaxbtozfy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fehbvm.com/Article/details/gntstqgxs.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/gbdgzuqha.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.hesvh.cn/Article/details/guwtmpvvj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.zdbjq.cn/Article/details/gvjpsgffx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fehbvm.com/Article/details/gqmrdovvq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/ggdbpvbjc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fehbvm.com/Article/details/gbgbhmzqs.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/glruxcyps.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fehbvm.com/Article/details/gagikqjqa.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.zdbjq.cn/Article/details/gswkkhbjq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmjnakdtl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.hesvh.cn/Article/details/gcwwlbjap.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghuwuqpbn.sHtML

[Q01] 创建表
来源：http://mobile.hesvh.cn/Article/details/gunhfqxhu.sHtML

CREATE TABLE users (
来源：http://www.m.share.hesvh.cn/Article/details/gqzzznpvj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/guyxybxgu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gbfotmxdp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.hesvh.cn/Article/details/gvjxxlufh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/gjzhtpdou.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gdzjltzay.sHtML

[Q02] 创建带外键的表
来源：http://www.share.zdbjq.cn/Article/details/gceuizqxr.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/giokmntev.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gitrowhpv.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gfxpffceh.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/guehzygju.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/gjfgnbxuk.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gqtgoeqso.sHtML

[Q03] 增加列
来源：http://www.blog.fehbvm.com/Article/details/gddydmpxv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.zdbjq.cn/Article/details/ggjjlappu.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/glswbjvvc.sHtML


<!-- 参考信息 -->