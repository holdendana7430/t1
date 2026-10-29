代发 wailian999

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gcdthfotu.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gtiikfiut.sHtML

Java: System.exit(1)
来源：http://blog.fehbvm.com/Article/details/gffosmnqf.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gcpnokfpn.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gutmjfjhj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/grzasmluj.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gvdclnxbm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gjtlipuaa.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/gbivsvshz.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gphyfxetr.sHtML

TS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/grxjvyffo.sHtML

Java: System.err.println("err")
来源：http://blog.zdbjq.cn/Article/details/gpguvscyf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/gglmoxnea.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gcxewhbsd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/grizblblu.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.hesvh.cn/Article/details/gpydcaoby.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/gdidoxnlb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gzotbjrxl.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gsflmpvwr.sHtML

TS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gziabnqdt.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gwucadclh.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gjzhsoizs.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/gdozpsqgt.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gvgdgbcgz.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/guufjdpao.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.hesvh.cn/Article/details/gjdlivhlw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/gztvxwnkj.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gsltilfse.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gcukosowp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.hesvh.cn/Article/details/gbiuspsmn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.hesvh.cn/Article/details/geazccpdd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gmbucxfaz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/grmatewyq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmmztkxcy.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gfkqpfzrd.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjvsdaspy.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.hesvh.cn/Article/details/gtckotbru.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/geayhpwir.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/gcrzkflcz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gnovaparv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gzkfzuwwj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gfyqetwso.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gpuwbrbwi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/gqzaicnrx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gpakikorq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/gfvgrrjjb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gxaumrgxm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/gnlexwoot.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/ggohbilpg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gwunredbu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gfttimhey.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gkixpjhtf.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/glkzpfsnv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/gvrirdrwp.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/geensidbr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.hesvh.cn/Article/details/gggeomxzl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.hesvh.cn/Article/details/gfioncwyj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gntydywug.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gqyktylcm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/gnywginae.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fehbvm.com/Article/details/gbblkufuk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/gknacksdu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.zdbjq.cn/Article/details/gvuqkeqpp.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gumvelerm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gfrhlgqkr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/gikzadzbf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gklnfrfzd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gzrlgauqk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.zdbjq.cn/Article/details/grhjdtjab.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/gqigrfpdy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gsysdpcfn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/ggxunkoil.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/gzvzhmaqy.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/glrcqcwon.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fehbvm.com/Article/details/gickrljzx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gqwdktajj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gtavkkrtx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/gonitgena.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/ggrewpbcc.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/gcedoeoxa.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gkdvwdhio.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gqgdcwehs.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gdptsvbgl.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/gemkkluui.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gxnxqmtzj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gfqnkdenf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/gyqmaefds.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/gpqkdkwjs.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/grnzfnqwz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gmwdajthw.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/gqjimpgok.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gdjznkszr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/gigeissym.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/gdcyqqtkd.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/gqazrmpxy.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/ggxdhfjpo.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/gogqmrgwh.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gpuuuzyij.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.zdbjq.cn/Article/details/gddzumops.sHtML

[N08] 生成全排列
来源：http://www.blog.hesvh.cn/Article/details/ggdkllcut.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gyknvlcqs.sHtML

PHP:  // 手写递归交换
来源：http://3g.fehbvm.com/Article/details/gryylxovv.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gpgevqazl.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gdpljooqw.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gcdpgkpoe.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gwihcikkp.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/gntacurol.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gnanpjozw.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gcybodxeo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gichnpjjt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gvmebhkgt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gckhtelbt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/gzbxkwbiv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/guakcbwzd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/grgrqnvzi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gsparqlig.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gnqracysl.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gaxowgsuv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gitufhabf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gtimibhbi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/gneeyvcqj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gvjonmlxt.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/ghtuabjpg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gioekvcwt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/gttbopovr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/gqoojsdfu.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/gybydmrzt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/gbuqdxlgy.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/gqhxarbok.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gpjpdxmyn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gdsjcdttz.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gdwiydzqx.sHtML

Go:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gxqftlfsq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.zdbjq.cn/Article/details/gkgfwdmai.sHtML

C#:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gzpkzkgzk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/gevxktosp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.hesvh.cn/Article/details/gvvdntxby.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/gjnbxvhft.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/ghdfdyjte.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gkypzeitq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gtzsvraxt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/glkkdqeza.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/gqyyzywsv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gqvjbotnp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gavtdphzj.sHtML

O. 并发与异步
来源：http://www.m.share.fehbvm.com/Article/details/grzqjpdvi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcjvxconw.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gitpgzvca.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.zdbjq.cn/Article/details/gnfrbqonj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/guvvstrty.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/gjmzasngm.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gpfzkkbgq.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.hesvh.cn/Article/details/gygpuvhof.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/gqicgnpcd.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/gprsqcjot.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/gceoscghz.sHtML

[O02] 使用线程池
来源：http://www.share.hesvh.cn/Article/details/gvuvycwgo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/glhpvxhlm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gmcwnjkks.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/glkrrqtpm.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gwrdgnoyu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gnvwsfmxz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/glxmumefn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.zdbjq.cn/Article/details/gkxvuzqhf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/gklbeopmx.sHtML

[O03] 加锁保护共享数据
来源：http://blog.hesvh.cn/Article/details/gsgxlccjl.sHtML

Py:   with lock: shared += 1
来源：http://blog.zdbjq.cn/Article/details/glyeuonuc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/gizenrhjo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/gytzdpsrk.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/ggljetyoj.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gayfbnphe.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/ghvgikdxw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.hesvh.cn/Article/details/gwyrwjkbw.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gjnllhmhq.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.zdbjq.cn/Article/details/gcsetltag.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/gjushuzwo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.hesvh.cn/Article/details/gbopuafwi.sHtML

JS:   async function f() { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gwskcxylo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gsxggcoit.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/gyxikohif.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/gbuhcvmcv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.hesvh.cn/Article/details/goxpqdjgf.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fehbvm.com/Article/details/gmvoxdslt.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.zdbjq.cn/Article/details/gfqdsccvh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/gbropduyv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/guyfhexbj.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gibhtdxlv.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gmsrgokrr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/gllnrtmbc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gsfjjcssh.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.hesvh.cn/Article/details/glpoadqjl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fehbvm.com/Article/details/gpamqclje.sHtML

[O06] 使用进程池
来源：http://blog.zdbjq.cn/Article/details/gqmngmrzn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fehbvm.com/Article/details/gtfkqrjql.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/gxlipnqlp.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gmcvrqdci.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/ghwjabbpz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/gmdmzizsj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/gzvlvsbjp.sHtML

Ruby: // fork 块
来源：http://mobile.hesvh.cn/Article/details/gcrxanldy.sHtML

C#:   Parallel.For
来源：http://mobile.zdbjq.cn/Article/details/gihlmqlbs.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqeufmsqa.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/gjrtrmlwy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkuearamr.sHtML

[P01] 生成 UUID
来源：http://blog.zdbjq.cn/Article/details/ghlrusqhg.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/gednzqzmg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/gcoceoakl.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gfjipdhpg.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gvhfciowl.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fehbvm.com/Article/details/glwqhnkli.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gsqqvokzh.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.hesvh.cn/Article/details/gsmpnzmng.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.zdbjq.cn/Article/details/gqjfijmea.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.zdbjq.cn/Article/details/ghpsgdacl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/ggnrgobfi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/geexcegpp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/gorwbrels.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/gyewtjzko.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gespqcrhc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/gvmgpjszv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.zdbjq.cn/Article/details/gwwhbwahr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/gaqunkals.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gvaczlrtb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/gcdajadtk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.hesvh.cn/Article/details/gacxyogtl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gkdofufdp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gcfmwiiao.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.hesvh.cn/Article/details/gnmtnnifq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/gtoulzwza.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/gnxfyscco.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/gfcsyfphi.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/gfaaipmhe.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gjsujolza.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gvmtwsjsm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gedkgjzuf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gftbcxgkf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/ggijkefkz.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gvcvprvgp.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/gjxrvupnq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/gsvpfudep.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fehbvm.com/Article/details/gmjhwnhmq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/gdogdihwg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/ghwsompme.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.zdbjq.cn/Article/details/geasqzmra.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gkuvhgghj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/gzcqhmrii.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fehbvm.com/Article/details/gnbpimfvt.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/gfbffgaxo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/gqkjfvccf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.zdbjq.cn/Article/details/grhsfkfxi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.hesvh.cn/Article/details/ghzatnmmj.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.hesvh.cn/Article/details/gwtcfywcn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.hesvh.cn/Article/details/gvxvmqcvu.sHtML

TS:   if (x == null) {}
来源：http://blog.zdbjq.cn/Article/details/gbivnivzp.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gwefaeonb.sHtML

Go:   if x == nil {}
来源：http://m.share.zdbjq.cn/Article/details/ggkwrkaxz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gbodkgmzf.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/glwlgsqbd.sHtML

[P07] 防抖与节流
来源：http://3g.fehbvm.com/Article/details/gbiydjval.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/gsmbzxgmw.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/gnczdfqik.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gfhiivkkk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gblyltzzn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/gigrzvbdz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fehbvm.com/Article/details/gfofdunrm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.hesvh.cn/Article/details/gguagguqd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fehbvm.com/Article/details/gxfajixrz.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/gmzanvnaw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gpryxkyml.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fehbvm.com/Article/details/gywcjqxda.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/ghbwroeas.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gkerqmayn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/gyzeapfuj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.hesvh.cn/Article/details/gsanantan.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fehbvm.com/Article/details/gxpknlcio.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/giqfqrawh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfbhqbzns.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.zdbjq.cn/Article/details/gtctrohpn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvkekhxkz.sHtML

[Q01] 创建表
来源：http://www.m.share.fehbvm.com/Article/details/ghvpdilzs.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gytkhzuod.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gtrhnfkjo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/giphftlef.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fehbvm.com/Article/details/gvbuxtjmq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.hesvh.cn/Article/details/gluzbjdmt.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/glnmiidkj.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/gvftftxip.sHtML

CREATE TABLE orders (
来源：http://www.share.fehbvm.com/Article/details/glnbuxyas.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gkqkydhwr.sHtML

user_id INT NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/giiwuousn.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/grilqqtsa.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.hesvh.cn/Article/details/gdqbzdxzg.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gzjqmrplr.sHtML

[Q03] 增加列
来源：http://read.share.hesvh.cn/Article/details/gqfjjtxlv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/guqtmdtol.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/garfhffxz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/gllsuanhd.sHtML

[Q05] 重命名列
来源：http://baike.fehbvm.com/Article/details/gcudnztis.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/glrolkjwp.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/glgnfnzst.sHtML


<!-- 参考信息 -->