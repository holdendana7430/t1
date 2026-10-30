代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzvawhzo.sHtML

[M05] 设置退出码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtbyhidk.sHtML

Py:   sys.exit(1)
来源：http://blog.fanxiaobao.xyz/Article/details/grwjrjxar.sHtML

PHP:  exit(1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsjqwgoe.sHtML

JS:   process.exit(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhvoxdvw.sHtML

TS:   process.exit(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehkfmfxq.sHtML

Java: System.exit(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfdcpqaw.sHtML

Go:   os.Exit(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gspnvrpxi.sHtML

Ruby: exit 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gorjwwjcm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujmflumj.sHtML

[M06] 向标准错误输出
来源：http://baike.fanxiaobao.xyz/Article/details/gnevndhmw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/gqbifgeni.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fanxiaobao.xyz/Article/details/gvndphgkl.sHtML

JS:   console.error("err")
来源：http://blog.fanxiaobao.xyz/Article/details/gijhzwdnf.sHtML

TS:   console.error("err")
来源：http://blog.fanxiaobao.xyz/Article/details/ghukshifp.sHtML

Java: System.err.println("err")
来源：http://3g.fanxiaobao.xyz/Article/details/gcaskmwmm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fanxiaobao.xyz/Article/details/gcaaztlvf.sHtML

Ruby: warn "err"
来源：http://www.share.fanxiaobao.xyz/Article/details/gecbthzoo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fanxiaobao.xyz/Article/details/gykwmsrsb.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fanxiaobao.xyz/Article/details/gabukinie.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fanxiaobao.xyz/Article/details/gkxptwpdw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fanxiaobao.xyz/Article/details/gatzjbdoy.sHtML

JS:   require.main === module
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gviqcllsw.sHtML

TS:   require.main === module
来源：http://m.share.fanxiaobao.xyz/Article/details/gkizhgmxy.sHtML

Java: public static void main(String[] args)
来源：http://baike.fanxiaobao.xyz/Article/details/grthzkzgx.sHtML

Go:   func main()
来源：http://3g.fanxiaobao.xyz/Article/details/gigscefjc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkkvcprh.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fanxiaobao.xyz/Article/details/ggbxsjkvm.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fanxiaobao.xyz/Article/details/gkeedhtdk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakgrcctk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fanxiaobao.xyz/Article/details/gjvfdfdsw.sHtML

JS:   process.platform;  process.version
来源：http://3g.fanxiaobao.xyz/Article/details/goslwrqie.sHtML

TS:   process.platform;  process.version
来源：http://blog.fanxiaobao.xyz/Article/details/gmzezfhda.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fanxiaobao.xyz/Article/details/gmrjyevdc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhhxvrvy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fanxiaobao.xyz/Article/details/gwruxuxsx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmrszmzu.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkvcaiyd.sHtML

N. 数据结构与算法
来源：http://baike.fanxiaobao.xyz/Article/details/gwkowdaes.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmyqywdc.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/glzrbrthv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fanxiaobao.xyz/Article/details/gvkremvcd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fanxiaobao.xyz/Article/details/gwvlrkgnt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fanxiaobao.xyz/Article/details/gwqyvybpr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fanxiaobao.xyz/Article/details/gboobrkuk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/gwzvchsda.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzjidwbc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxphlfksu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fanxiaobao.xyz/Article/details/gbeeljnei.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fanxiaobao.xyz/Article/details/gfaqiyjwx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fanxiaobao.xyz/Article/details/gzxlykdjx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/govozmipm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmniputz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdainznm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fanxiaobao.xyz/Article/details/guzzhkxnh.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/ggangmxwf.sHtML

Ruby: arr.sort
来源：http://wap.fanxiaobao.xyz/Article/details/ghdurynof.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fanxiaobao.xyz/Article/details/gagolrmip.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fanxiaobao.xyz/Article/details/gitahmbyj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctkynwty.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyzhkxty.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxjqcpyb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsjmwhyo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fanxiaobao.xyz/Article/details/gokxayxxb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fanxiaobao.xyz/Article/details/gqcfdwlaa.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fanxiaobao.xyz/Article/details/gmiwexnze.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fanxiaobao.xyz/Article/details/gbafartmo.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvozzjap.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwaidtpt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfvrvnkj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gjkzyyyqt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/giixnnqve.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gagpbkhux.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fanxiaobao.xyz/Article/details/gfjgepzxl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/glwhrvapk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmemfygkg.sHtML

[N05] 最大公约数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxuuzlrc.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmieueme.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcwltclf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtyxoubrj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwugocmlx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmryziby.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fanxiaobao.xyz/Article/details/golqelhhw.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkcddusk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxghlfbu.sHtML

[N06] 判断回文字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzmhtiim.sHtML

Py:   s == s[::-1]
来源：http://3g.fanxiaobao.xyz/Article/details/goelaovoq.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gajorjepo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fanxiaobao.xyz/Article/details/geqaagemt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmiqmxfaq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrijjsur.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fanxiaobao.xyz/Article/details/gwpiircmk.sHtML

Ruby: s == s.reverse
来源：http://read.share.fanxiaobao.xyz/Article/details/glnhnwagu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkhtvqxn.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbibjffq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fanxiaobao.xyz/Article/details/gksglphuz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhioozaq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fanxiaobao.xyz/Article/details/grzngqyne.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fanxiaobao.xyz/Article/details/ggwcmgobd.sHtML

Java: // 手写 HashMap
来源：http://3g.fanxiaobao.xyz/Article/details/gawudiuzr.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fanxiaobao.xyz/Article/details/gyswgsovn.sHtML

Ruby: // 手写 Hash
来源：http://blog.fanxiaobao.xyz/Article/details/gacjbwipi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fanxiaobao.xyz/Article/details/gpekewvyf.sHtML

[N08] 生成全排列
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfsepzom.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdoeulhx.sHtML

PHP:  // 手写递归交换
来源：http://baike.fanxiaobao.xyz/Article/details/ghfinropp.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fanxiaobao.xyz/Article/details/gjczikpig.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmynxvkr.sHtML

Java: // 手写回溯递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gitogqvye.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzblcxuk.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fanxiaobao.xyz/Article/details/gxaowjalc.sHtML

C#:   // 手写回溯递归
来源：http://baike.fanxiaobao.xyz/Article/details/gtvrognnl.sHtML

[N09] 栈与队列
来源：http://3g.fanxiaobao.xyz/Article/details/gqkehrbez.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmoqcuscl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fanxiaobao.xyz/Article/details/glgnppngu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fanxiaobao.xyz/Article/details/gsvdspvrp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fanxiaobao.xyz/Article/details/gbykkovgm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fanxiaobao.xyz/Article/details/gvioztgma.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjizxabck.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwtabxgq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fanxiaobao.xyz/Article/details/gubfptkwk.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhsjxwvw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fanxiaobao.xyz/Article/details/gydmrmmyz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjugfvfh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goufokuhs.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvxsnpaz.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlkayfhn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcxfxvlk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxorahiz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fanxiaobao.xyz/Article/details/govnkjsif.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gxugxukyj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fanxiaobao.xyz/Article/details/gewmxfacl.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzubtlshh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkucjzau.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqyuxanp.sHtML

Java: // 手写递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefrclioa.sHtML

Go:   // 手写递归
来源：http://read.share.fanxiaobao.xyz/Article/details/gugbnntdk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fanxiaobao.xyz/Article/details/gravviwze.sHtML

C#:   // 手写递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezupupbc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjkbftjy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fanxiaobao.xyz/Article/details/ghxsxqngc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fanxiaobao.xyz/Article/details/gmsyrefrd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fanxiaobao.xyz/Article/details/gmreqljlj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fanxiaobao.xyz/Article/details/ggjovjkwd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfidfakx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gftvoavhw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gzxhpjlpa.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fanxiaobao.xyz/Article/details/gwyzfmaju.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggejaijem.sHtML

O. 并发与异步
来源：http://mobile.fanxiaobao.xyz/Article/details/gmprwltrs.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gdlbyaygb.sHtML

[O01] 启动一个线程
来源：http://wap.fanxiaobao.xyz/Article/details/gqazgyxxo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkenqfjai.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsslrzslf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fanxiaobao.xyz/Article/details/gqwuijeoa.sHtML

TS:   // 同 JS
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvxtnydj.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvgjkcta.sHtML

Go:   go f()
来源：http://wap.fanxiaobao.xyz/Article/details/gqtdmjglx.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzfvhsno.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzygnhiut.sHtML

[O02] 使用线程池
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmxobktn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fanxiaobao.xyz/Article/details/gwjilfiun.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgbjwift.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fanxiaobao.xyz/Article/details/gstcuqlod.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fanxiaobao.xyz/Article/details/gilfvudiy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gmivcakmf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fanxiaobao.xyz/Article/details/gncthlhdl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fanxiaobao.xyz/Article/details/gzryoufcz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttmzqxex.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsqptwaf.sHtML

Py:   with lock: shared += 1
来源：http://3g.fanxiaobao.xyz/Article/details/ghuzbazeo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmgwahen.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fanxiaobao.xyz/Article/details/gyoxertiv.sHtML

TS:   // 同 JS
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvtcuxxf.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpavsatm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwqocilq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnlhridk.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/garkfvrpx.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gayikqmvw.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fanxiaobao.xyz/Article/details/gyubokrye.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fanxiaobao.xyz/Article/details/gtnvxdlmn.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gidmmddil.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gekbmsdvn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fanxiaobao.xyz/Article/details/geblaxhqr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnfxkhlw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fanxiaobao.xyz/Article/details/girabaebu.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gpwxgbmvk.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpfvqvpp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakbmcxbe.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fanxiaobao.xyz/Article/details/gorvqzzlw.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fanxiaobao.xyz/Article/details/gdwpxozjo.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefqkwkte.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fanxiaobao.xyz/Article/details/gmvvtfobc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fanxiaobao.xyz/Article/details/gwrjwebza.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fanxiaobao.xyz/Article/details/gqropbzmo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjekemwo.sHtML

[O06] 使用进程池
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvigvvyx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fanxiaobao.xyz/Article/details/gighupwjx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fanxiaobao.xyz/Article/details/goaczewog.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkekqanbg.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fanxiaobao.xyz/Article/details/gibnwahie.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fanxiaobao.xyz/Article/details/gwwaqnpzb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fanxiaobao.xyz/Article/details/gbfdbgnau.sHtML

Ruby: // fork 块
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoznvywq.sHtML

C#:   Parallel.For
来源：http://baike.fanxiaobao.xyz/Article/details/geexslfyq.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmztabncz.sHtML

P. 常用工具函数
来源：http://3g.fanxiaobao.xyz/Article/details/gbuyikdbi.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gkgpxoaol.sHtML

[P01] 生成 UUID
来源：http://blog.fanxiaobao.xyz/Article/details/gbnmrdcdq.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fanxiaobao.xyz/Article/details/gziqrzmkn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fanxiaobao.xyz/Article/details/gikefuwwa.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpbgyiif.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/gjbeiwrnv.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfwotadh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fanxiaobao.xyz/Article/details/gbuovcdej.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fanxiaobao.xyz/Article/details/gplzoequu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fanxiaobao.xyz/Article/details/grcedzcbq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fanxiaobao.xyz/Article/details/grbcisvge.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fanxiaobao.xyz/Article/details/gjwlghphd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmcilcpe.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fanxiaobao.xyz/Article/details/guddovppz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsnfylab.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fanxiaobao.xyz/Article/details/gpvqkqgpx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjohhwey.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmitvzmcl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gseyaxqyp.sHtML

[P03] 生成短随机字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gshbkjggg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fanxiaobao.xyz/Article/details/gaobtcyum.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fanxiaobao.xyz/Article/details/gcwedbxgb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/grwlbsqnq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhwumikw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fanxiaobao.xyz/Article/details/glzrzbdqu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fanxiaobao.xyz/Article/details/gcqacbjth.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guguyquur.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowhxghhs.sHtML

[P04] 求长度
来源：http://read.share.fanxiaobao.xyz/Article/details/glbhsadot.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fanxiaobao.xyz/Article/details/gblpboeuh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfnvejje.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbrvjotm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fanxiaobao.xyz/Article/details/gypjmftse.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fanxiaobao.xyz/Article/details/gzinavnic.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsenjtqky.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fanxiaobao.xyz/Article/details/gibbfcxms.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwvahhli.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwiwgxky.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghplokvfo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fanxiaobao.xyz/Article/details/gqhtvlrlc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmxnbrxz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasdogexd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fanxiaobao.xyz/Article/details/gyuooyjdd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkqhhrdr.sHtML

Ruby: a == b
来源：http://3g.fanxiaobao.xyz/Article/details/gyswnupxv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fanxiaobao.xyz/Article/details/grrcryhyu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gtevzywrb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fanxiaobao.xyz/Article/details/gsiewhdaq.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwrimetd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmitzchy.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsxjocjz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gwditrveq.sHtML

Go:   if x == nil {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gkskyvjbm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fanxiaobao.xyz/Article/details/gwklrzqcp.sHtML

C#:   if (x is null) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gzjriauli.sHtML

[P07] 防抖与节流
来源：http://www.share.fanxiaobao.xyz/Article/details/gtaryaohx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fanxiaobao.xyz/Article/details/gvlyxnwrr.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvikhwdai.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjhyfppb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gxywduqnl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzeztwmfe.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fanxiaobao.xyz/Article/details/gjcfasdue.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaaqgjwwu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fanxiaobao.xyz/Article/details/guxzbsmyi.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fanxiaobao.xyz/Article/details/gfcvvfppe.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fanxiaobao.xyz/Article/details/gioyvnuur.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqmrbccd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaejojcyx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fanxiaobao.xyz/Article/details/gpggbqfmg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhaevwru.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fanxiaobao.xyz/Article/details/gsqipuktt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fanxiaobao.xyz/Article/details/ghussjbxo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fanxiaobao.xyz/Article/details/gomlunsjp.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gstebpden.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fanxiaobao.xyz/Article/details/gzlkpiluv.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gnekybhwn.sHtML

[Q01] 创建表
来源：http://mobile.fanxiaobao.xyz/Article/details/gugqjmblv.sHtML

CREATE TABLE users (
来源：http://3g.fanxiaobao.xyz/Article/details/gmyuvncuw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fanxiaobao.xyz/Article/details/gndtykwyh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fanxiaobao.xyz/Article/details/gicgiuoyq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fanxiaobao.xyz/Article/details/gsyfnrhsh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fanxiaobao.xyz/Article/details/ghizmcvlj.sHtML

);
来源：http://blog.fanxiaobao.xyz/Article/details/gidxktuct.sHtML

[Q02] 创建带外键的表
来源：http://3g.fanxiaobao.xyz/Article/details/gsyzyuwfm.sHtML

CREATE TABLE orders (
来源：http://baike.fanxiaobao.xyz/Article/details/gkzrpbxes.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwurtgsv.sHtML

user_id INT NOT NULL,
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwnnxwkm.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlnrdevb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fanxiaobao.xyz/Article/details/gjtihudys.sHtML

);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkmnezra.sHtML

[Q03] 增加列
来源：http://blog.fanxiaobao.xyz/Article/details/gcmcpgcuh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlhofxwc.sHtML

[Q04] 修改列类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmoutekc.sHtML


<!-- 参考信息 -->