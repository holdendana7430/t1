代发 wailian999

[M04] 获取当前工作目录
来源：http://www.m.share.fehbvm.com/Article/details/ghuqgshqf.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/ggcrzmmov.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gitvddvwi.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gpxsavbco.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gideatkqa.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/gvpdtbhop.sHtML

Go:   os.Getwd()
来源：http://m.share.fehbvm.com/Article/details/gkiofjtyr.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/gervnivdt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/gqrtvatnr.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/gbetenrnd.sHtML

Py:   sys.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gqlgekfpo.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/grkddjhey.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gdvkrvpix.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gihlvtlpc.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gdxzoxzrp.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gxhkmxoty.sHtML

Ruby: exit 1
来源：http://www.m.share.hesvh.cn/Article/details/gascqbahz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/gpzmjqmfn.sHtML

[M06] 向标准错误输出
来源：http://www.share.zdbjq.cn/Article/details/garcnjwkb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gnvhjditw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/gmzxfjyws.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gbsbwrofs.sHtML

TS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gnidvnyvo.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/gwglmnjah.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/gofsydboz.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/gtxvcknjn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/grdaqpicb.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gnuuqzshz.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gnudxdifl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gevlaeykz.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/guealjdpu.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gxggliohs.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gfsrfzzbe.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/gkwoyuljp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/gwgezlxjh.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/gzcyhozwk.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/ggwrlfdgh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/gfihzbbjj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/gaykmawfl.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gwksinvvo.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gtvjtjozz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/gvdbbsahx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gxntgtzsw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/gruoaasyn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gjxwmkjfe.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glpwgzjcs.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/gcpxyxwtm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfigrmodb.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/gydpxqpjm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/ghjdxcgrf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/ggchsrgqv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/grcsaepje.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gvowneijw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gqbcolctr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gpjzgjkrv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/gmyypkevl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gdbfbmezo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/gyrqofseo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/guyogsidi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/gxisbjryy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/ggpsanhgm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gspmqeggu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gavgpysjd.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gyhrfpuyo.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/giesvwahn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/gmgsnuttd.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/gugdxorpu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/goqzefxej.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.zdbjq.cn/Article/details/gkmbrhugc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/glsuzcmbn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gdkbmhmrl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/glxtvdedo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/gdkvhnxxn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/gacrgkrab.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gdzelzodc.sHtML

[N04] 斐波那契数列
来源：http://blog.zdbjq.cn/Article/details/gubveldew.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gzmrcbkaq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbjetskjc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/goiozsjyl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gxfbwyzsz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/gzwkkcqou.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/gzfkzvkrb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/ggmjaurvd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gukvdpooy.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/gacazjefq.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/gweqltpxj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/getggfssn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gfxblnqwm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gtgugpval.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/gfyabccfb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/gfstyyuzp.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/gyedyezwf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/gskzpdeag.sHtML

[N06] 判断回文字符串
来源：http://www.share.hesvh.cn/Article/details/gzwkjibyf.sHtML

Py:   s == s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gjawbsfzg.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gsqgdvlzk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/ggmyylhxy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gycvnlhsu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gvdwlrolx.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/grkgzpxno.sHtML

Ruby: s == s.reverse
来源：http://wap.zdbjq.cn/Article/details/gwwnbpqov.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/ggpsvqpcg.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/gjuauepgu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gbaoqwmsb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/gscpmjymh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.hesvh.cn/Article/details/gcrvrynvz.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/glcklefxq.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/gmpjcoupx.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/ggdllczcq.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/gdvnlunmi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.hesvh.cn/Article/details/gkueacvhb.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/gboxcmvsz.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gyiocsycl.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/grjhweghm.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gbrjtoxat.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gmvaefmis.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gjtoidala.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gdduyyuxy.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/gwvudwrmd.sHtML

C#:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gkmzmaawm.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gkfovnuqq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/glosvokjm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gnouuobzh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gkjwjydxb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.zdbjq.cn/Article/details/gbcfcppyy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fehbvm.com/Article/details/gtnwbhint.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gckoczzjj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gukuyttyc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/gneexucef.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/ggyvwrber.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/gnhdqssto.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gaplktzki.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.zdbjq.cn/Article/details/gbqbztkkj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/gwhctedxt.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/gqqqjlyxx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gjjdewisy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/gzzcmsixq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/gfxdplhjs.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gugsutkzd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/gwjctgqos.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/gfrtuzodr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gflsmdbwn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gdkooxnls.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/gttapskha.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gxhztxeqw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/gcyijjdyt.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/garctwfpx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.hesvh.cn/Article/details/gckxeqivk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gcknxweet.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gyzfcatec.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gpexddnff.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gizoypxdg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gwpsdvwvy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.zdbjq.cn/Article/details/gzpiqdazw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/guntrvlbx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gkreshlre.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gebgwzrpl.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/gbixtavms.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzxyfbjuc.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/gshgyqswz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/golvqmspx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fehbvm.com/Article/details/gnfihoiyh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gazbqfpul.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gvstihnoz.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/gqnmpeymx.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/gaxptzyax.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/gjwzaaeji.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/gwvjuljly.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/gxmdqfanu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/gmhogpaya.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/grcavdasn.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gczedufpx.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gpptftocw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fehbvm.com/Article/details/glfjqthgx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.zdbjq.cn/Article/details/gfhcewtdl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/gqzquawky.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fehbvm.com/Article/details/gyfbgpbot.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/gwphccxqj.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gyzqrdqvd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.hesvh.cn/Article/details/gensmvgjj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/gvaecnnzb.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gpfrspbtw.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gcujhlxer.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.hesvh.cn/Article/details/gqtqlwfyf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/goemogwgb.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gffynlxhg.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fehbvm.com/Article/details/gtsrqkvte.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/gplgqgobq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fehbvm.com/Article/details/gkrwcmrge.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gvvhwylbg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/giseymhzt.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/garrbzkji.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/gjsayhftl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/gcezpopkx.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.zdbjq.cn/Article/details/gyexosfkf.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/gkfgikjec.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/gimtoqujn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/ghtknxgnw.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gtwzgwncv.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gdfkkpqza.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.hesvh.cn/Article/details/ggbcbdypy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/ghxyacvqd.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gzxyfxyjc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/glnkwqama.sHtML

[O06] 使用进程池
来源：http://3g.zdbjq.cn/Article/details/gihhbteax.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/gtidhjodk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.hesvh.cn/Article/details/gjcofwctn.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gsxepzfod.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gpsoxaxzk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/gzfyxmfrc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gskqfhcwz.sHtML

Ruby: // fork 块
来源：http://3g.fehbvm.com/Article/details/gtkbzzrrw.sHtML

C#:   Parallel.For
来源：http://3g.fehbvm.com/Article/details/ggivekclp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gakuahrtx.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gjqmmrauw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grrcsmyiu.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gcxflbpsp.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/gvufpgvzf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fehbvm.com/Article/details/ggychdljk.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gedrojoyi.sHtML

TS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/grhjrkkqt.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/grpnysujg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/gteqptuiu.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gbawouwiv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gzwsmpliw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/gejbeolgr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/gjytczqar.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.zdbjq.cn/Article/details/ggqyyuglq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/gsyfrekzw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/gedosdtsi.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gsjohwonr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/gpclguevs.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/ggctwwapx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/ghfyuuhxl.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/gyfjioecf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/gwoylgodb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/glyknuywn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gjgoekmzb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gnhanoxyr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/gnqpfsanl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/gfccsmmyl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/ggszuncxu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.zdbjq.cn/Article/details/ghwfhqfyu.sHtML

[P04] 求长度
来源：http://3g.zdbjq.cn/Article/details/gkyvlkxkt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/gmniidrvy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gcrkvcjsr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/goabviycj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/grxnbsrak.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/gzpbestye.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fehbvm.com/Article/details/gojjhatou.sHtML

Ruby: x.length;  x.size
来源：http://mobile.zdbjq.cn/Article/details/grdzcmjxg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/ggpjmlngu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/gcuwaidjv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.hesvh.cn/Article/details/gnhrmxukr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fehbvm.com/Article/details/gtqcetpfb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/gpvdizdbo.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gugeichkc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/gwqffluii.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gkztrpyyg.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/gqsgtjpqg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.zdbjq.cn/Article/details/gnhbutdvf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.hesvh.cn/Article/details/gtnjuduhx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/gkhcgvxih.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/gsvytooat.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.hesvh.cn/Article/details/gbvjxzetl.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gxgcohvlx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gpgpfesgw.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gsbgufnrt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.zdbjq.cn/Article/details/ghjbfabhv.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/gvbvelkvv.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/ggdmxgqer.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/gyjirotku.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.zdbjq.cn/Article/details/gvfwbqbhq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/grjlzddnc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gldmrvmpw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.zdbjq.cn/Article/details/gqwuguldb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fehbvm.com/Article/details/gqcnavsra.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/gyfugukot.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/gslxpmhgp.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.zdbjq.cn/Article/details/gfcbqvtwv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.hesvh.cn/Article/details/gnzuyplqv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/ggeqxcawf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/gwojfgwmi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gvtrfibpt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fehbvm.com/Article/details/gqnarcwhi.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/gfcibnpls.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fehbvm.com/Article/details/gxmukuwko.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.zdbjq.cn/Article/details/girdsyaip.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghsiyigyv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.zdbjq.cn/Article/details/gyxigdhhc.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjqfisfpv.sHtML

[Q01] 创建表
来源：http://blog.hesvh.cn/Article/details/glljemcmp.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/grcvbuono.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gthflxxgg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gxjcrmqol.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fehbvm.com/Article/details/gxotbxzri.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.hesvh.cn/Article/details/gleinjenx.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gezgegepq.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/gyttfscun.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fehbvm.com/Article/details/gdpuojdgu.sHtML


<!-- 参考信息 -->