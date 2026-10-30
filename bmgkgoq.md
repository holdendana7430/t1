代发 wailian999

Ruby: exit 1
来源：http://www.m.share.zdbjq.cn/Article/details/gwxrrwkqq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.hesvh.cn/Article/details/grccijphy.sHtML

[M06] 向标准错误输出
来源：http://mobile.zdbjq.cn/Article/details/gphhqgllg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gqaqjafcm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gojztryni.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/glpwyielb.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gwibcmmcr.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/gyyuiambo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/gnapkucmo.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/glendqxuv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/gpbqmtmxx.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/gvrtsdpch.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/gzvxpdjdz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/gayrvuhji.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gwnotzqxa.sHtML

TS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gbqhthbdp.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/gzxzdnepx.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/gjwcgaiok.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gqkfxrzkf.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gtmrdtbaf.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gzwegvbdt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/gsmvpzxgf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/gwvyshixf.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gisfjbiul.sHtML

TS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gnvfwlqjx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/gqnzftyie.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/glwjtynke.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gnntfrjps.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/gmriknwjz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvlpqivvn.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/gglccytzk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gutpmcrva.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gljymofda.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gyswyttmr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gkwrmxdxk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/grrkfwfyr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gbbzgttcf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gsgwbipcl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gspcwissh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/gnfwhxhnn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/glhlodopp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/gkmexgtif.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gpzadtkdk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/gbawlugjm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gdapsxbtw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gbffhcawf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/glptgjzjh.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gdkwhjjbg.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gyhxerrea.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/gttmsrxiz.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/gfyohzoph.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/gysqfhcgl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/gdzadkadh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gzgmnlqfi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gflpgmlwp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/gtivmicvk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gcmlrgqiq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.hesvh.cn/Article/details/grrpvkggk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/giqzdglqa.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/ghkhucdox.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gdvuvldia.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/goykthkrm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gxdzpqscn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gpceimvrq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gkrvksbzq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/grrskuqvb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gqyvvjkvs.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/grmtplauj.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/gnunkirst.sHtML

Py:   math.gcd(a, b)
来源：http://blog.zdbjq.cn/Article/details/gxvplyxjh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/gqwyfrvia.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gjxnvkaid.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gtabyggwy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/gfawouxtz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/gzqgmhdbr.sHtML

Ruby: a.gcd(b)
来源：http://m.share.hesvh.cn/Article/details/gyjkwzjeh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/goqflbjuh.sHtML

[N06] 判断回文字符串
来源：http://www.share.zdbjq.cn/Article/details/gxywhyrrt.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gautdhvhb.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gxfuuwmbd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gtakloabs.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/guocebiki.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/gktzcrmfb.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.hesvh.cn/Article/details/gnqxcplzg.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/gzisxawik.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gqmgvzdja.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.zdbjq.cn/Article/details/gmqnmdkid.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/gquttwncj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/gmkvrakkg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/gjgcxjcml.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.zdbjq.cn/Article/details/gzyychktc.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/gzirbmrrf.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/gjsaonxed.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/ggwqvjhbe.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.hesvh.cn/Article/details/grmqxqsns.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/gtvesivgk.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.zdbjq.cn/Article/details/grvcncsqa.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/gpxavktpe.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gfpkmvzgq.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gvupqdivq.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/ggvfrvhtb.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gtcwscfxe.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/gjhycyjmb.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gnkdmdepr.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gfudjamjs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/grcjxrisy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gullfwidg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gnkzcyzln.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fehbvm.com/Article/details/ggnbwqlcg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fehbvm.com/Article/details/ggfcwqoqr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/gjvjeihgo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gqglzzait.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/gbpllduna.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/gehzsutoc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/ghzcbgapb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/gqtkrayjn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/gntijvjcs.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/gmneqthtr.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.hesvh.cn/Article/details/gvajfsvdh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.zdbjq.cn/Article/details/gcatmpmdj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.zdbjq.cn/Article/details/gtzjzfwjt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.hesvh.cn/Article/details/gfimsirjp.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/gshrbknfj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gistlwlfr.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gmjnjchfr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/ghqdfxhbd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gmbbugpww.sHtML

Java: // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gcigbtrze.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gvximkqys.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/gewtndpnx.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gsuhtkowv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fehbvm.com/Article/details/gazyhietg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/gidiiblhn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.zdbjq.cn/Article/details/ggngnaepr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gumcfsvdz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/giwklplgm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gsjzotout.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/guwtrfeau.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fehbvm.com/Article/details/ggeqozokn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gelrcjumt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grgfufjog.sHtML

O. 并发与异步
来源：http://www.blog.hesvh.cn/Article/details/geqcqjclx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggbpdnpvp.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/gyeghmxqp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.zdbjq.cn/Article/details/ghmsznglp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/gfnjabpes.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/gbmajphjo.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/glcetfced.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.hesvh.cn/Article/details/gaqlarkwm.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/gpvqfbbzv.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gvztmivyq.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.zdbjq.cn/Article/details/gfbgiodyf.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/gikocqdoy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/glaljiaia.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/gcrtfcido.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gffjatxbl.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gpczdsbiq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/gbggyacpv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/gmovvjbqr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gewobjsdm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/gbnxhlmbr.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.hesvh.cn/Article/details/ggpkehhrg.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gzxfoekai.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/gwcozjsed.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/gssbgjwjq.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/giuzlqxch.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/ggymkqpbk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gtkjubktl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gcbyiiqsz.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gdpyfsyqp.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gsnihytff.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/gdyctydkx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/glyzqussl.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gvpeazvvf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gynjinuhy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.hesvh.cn/Article/details/gusyadxvd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fehbvm.com/Article/details/gtetsjjav.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/gegnnmbdb.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gzzouvbdh.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/gotuztlqy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fehbvm.com/Article/details/ggfilanei.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/gpnqvujhr.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gkgxleshp.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gnhbvlowx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/gpnrtevav.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.hesvh.cn/Article/details/gxgqotjmv.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gczyfsgtl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fehbvm.com/Article/details/gkqawhney.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/gkytruocq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/grzuumovi.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/ghukmcces.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gogbuwzir.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gxqeullyu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.zdbjq.cn/Article/details/gvhbxafab.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/gpqvhltap.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/gahvowafc.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/gbguskfmo.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gyihcluhx.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/gwpppwkre.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcxlwbvqt.sHtML

[P01] 生成 UUID
来源：http://blog.zdbjq.cn/Article/details/glablxvhn.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/glsexarpl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gvoagcquu.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/guqbswldr.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gvnjiaosu.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/gxooqrgvy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/ggbdewjrf.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.hesvh.cn/Article/details/gqygicius.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/gxivmniop.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/gntevgchn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.hesvh.cn/Article/details/gvdyhjoun.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.hesvh.cn/Article/details/gwueszxlt.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.zdbjq.cn/Article/details/gjugedrrs.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/geornypnl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fehbvm.com/Article/details/gyzdrzdyk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.hesvh.cn/Article/details/gnneheobv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gwbtfmryg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/gyhdnfjpp.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gyjhmiuce.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.hesvh.cn/Article/details/gbgwztpva.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/gmbwxacnm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gtfkaihmy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gpgjsxvnf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.zdbjq.cn/Article/details/gieecnuuq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/gmlsfmhww.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/guksfcblt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/grkckoicq.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/gxuehrhsv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.hesvh.cn/Article/details/gawpwqbvr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gbkonzcmi.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gvrzkmhpn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gtuzzxqao.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fehbvm.com/Article/details/gtzazpcys.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.zdbjq.cn/Article/details/gjqmpteku.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/gbckmnsna.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gbirtfkuv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gwsrcsbjt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gcwwhpmss.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gkvgcknab.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.zdbjq.cn/Article/details/gliztxqne.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gfolickgn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.hesvh.cn/Article/details/glkeizyvu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/gotpiqxre.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/gswzlcprm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.zdbjq.cn/Article/details/gdefcsimi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/gmqhrvdnh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/gicpfsinl.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.zdbjq.cn/Article/details/gwjppnqfe.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fehbvm.com/Article/details/gvjrulvzp.sHtML

TS:   if (x == null) {}
来源：http://mobile.fehbvm.com/Article/details/guxihbxld.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gpyhujfyq.sHtML

Go:   if x == nil {}
来源：http://baike.fehbvm.com/Article/details/gdnlauzkp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gmydvcugj.sHtML

C#:   if (x is null) {}
来源：http://3g.hesvh.cn/Article/details/gmvrbhiii.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fehbvm.com/Article/details/gzvwcopfk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fehbvm.com/Article/details/gjtxatmpq.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/gidpxrbtk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gmwowicki.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gfmnmpoxk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/gobemisjx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fehbvm.com/Article/details/ggcdjjssp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/giiasmlyr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/ggvujfkmu.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/gdhwycrxn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fehbvm.com/Article/details/gyshbisme.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gjqocmdnz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fehbvm.com/Article/details/gqzowgppz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/grevklhfw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/ggxcykjzk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/ggriozvak.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/gxxqgqnuu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fehbvm.com/Article/details/gsrwhygqz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggjnkorsh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/gjtxnwmph.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghfurtppw.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/gxpsxjkcv.sHtML

CREATE TABLE users (
来源：http://m.share.fehbvm.com/Article/details/gziixyrsj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gktrpyqph.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gazufaouy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.zdbjq.cn/Article/details/gzxxjxxrz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.hesvh.cn/Article/details/glctbszry.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gomuqcoya.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gnhqpguky.sHtML

CREATE TABLE orders (
来源：http://wap.zdbjq.cn/Article/details/grpipdfyp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gqvimskur.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gkrhbhipa.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gpopreuph.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gnroasnxb.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gzqbfelqf.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/ghrawzqjr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.hesvh.cn/Article/details/gpmzdgwvb.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/gasrryknp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fehbvm.com/Article/details/goxienphb.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/gxsiktgzq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fehbvm.com/Article/details/gvnjwzeae.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/geczzyvrb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fehbvm.com/Article/details/glzfvkebu.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/geimoaeml.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.zdbjq.cn/Article/details/gesgphmpg.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/gvkjpvbmw.sHtML


<!-- 参考信息 -->