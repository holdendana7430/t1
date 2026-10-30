代发 wailian999

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/glxgvsjpf.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/gelnblqvx.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/gtkpemtyf.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/godtyvclz.sHtML

TS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/godsygjcr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.hesvh.cn/Article/details/glymafylc.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/gzmhoksgr.sHtML

Ruby: Dir.pwd
来源：http://www.share.fehbvm.com/Article/details/gxgrzrkbo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/gepmjmtwb.sHtML

[M05] 设置退出码
来源：http://baike.hesvh.cn/Article/details/gpookoyxa.sHtML

Py:   sys.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gkxoshfey.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gbukvjhpj.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gyvrsdcaz.sHtML

TS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gyltgngdt.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/gffhifrkc.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gpmwndiar.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/gomkendqk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gflsnshfx.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.zdbjq.cn/Article/details/gtsmhbbja.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gdeggyake.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/gbiwpelen.sHtML

JS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/ggeiseisx.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gyryhsmzb.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/giooonutq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gryrzskga.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/ghoiiktlz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/guwbigqiv.sHtML

[M07] 判断是否为主入口
来源：http://m.share.zdbjq.cn/Article/details/gdjzsseiv.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gejqrzcnj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gpacupfhw.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/guytiqrrk.sHtML

TS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/ghdswhtio.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gcqhvtwyc.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/gyzzgwqsx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.hesvh.cn/Article/details/ghtvpycjz.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/gjoefssrb.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/grcsozzrk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/gsghqipku.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gfppozpyo.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gwyfzhpwx.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gtkefmazx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.zdbjq.cn/Article/details/gqpgualrt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/ganjaxziy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fehbvm.com/Article/details/gwycqosqx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/gerswcict.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxxgnxoqt.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/gxeyxacjf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gebfhdsrs.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/gfibterks.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gtuvbxnxq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fehbvm.com/Article/details/gstuyiiho.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gaodsneil.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gwhmkbwsl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gkpegeizm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gfqafaylw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gyqujnfgl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gvqxnguin.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.zdbjq.cn/Article/details/gzjencmrr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/ggtuvdkgd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/gzginpkjp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gfkknxuix.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gvglqldcy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/gqceknicy.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gzegigsfn.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gsiuizowv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gokyoapth.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/grjaercob.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/ghmwjomos.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/gaaczqhko.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gwlubnmun.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gsfahkjzc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gskwuouqd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/gogfcqkco.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/ghexxfcxr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/gsmwkukax.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/gncmlreoz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/glcpbwpgr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gtulxowkc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gkdhfloyc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gakccyjgx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/ghoaqvyqp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gzklxrvue.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gfzsjgort.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gxdlsvxkc.sHtML

[N05] 最大公约数
来源：http://baike.hesvh.cn/Article/details/gqvvoyjoz.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/goctbuibr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/gibravlps.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gghlfirqn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gblgvzirj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.hesvh.cn/Article/details/gygcpreye.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gzjfrjptb.sHtML

Ruby: a.gcd(b)
来源：http://mobile.zdbjq.cn/Article/details/gpdfnrree.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gfhcofqdw.sHtML

[N06] 判断回文字符串
来源：http://www.share.hesvh.cn/Article/details/gnhnfkgyu.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gtjfqqgkb.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gpphbzmom.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/grxrmekxj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gucuuswom.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gvccwjcnz.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fehbvm.com/Article/details/gbnuvqnyu.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/grawitmmm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gppmxhhtk.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gvjshgpyr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/gkzdohonu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/grvkiimzt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gqttqonbr.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/glfckkgym.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gsbxunowc.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gjnwudpks.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gzqzzzftb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/gxodybwev.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gkanranby.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fehbvm.com/Article/details/gxzohcqby.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/gvyhchpyf.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gsqxvndgq.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gyandtzpw.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gsmctbvuj.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gntlirknj.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.zdbjq.cn/Article/details/gytblebzp.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gfarncxan.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/ghfhidtcg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/ggxqqmczo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gawratyxl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gftjrsdtt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fehbvm.com/Article/details/gsoyisqdd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gheyqufcj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/gxpjdwyrc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gfhdnamgj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/grechlyok.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/gcbpcikst.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/gfhvmyvwv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gtomakpxv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/guqltyzxs.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/gxtduglls.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpcnywwkm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gsmtquxqc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gzjufjwrd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/gytewirza.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/gbozncdpx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/gjugnvydg.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/gznuasldk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gbcxetyth.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/guvwnbaym.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gdkhabxbo.sHtML

Go:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gfkildbnc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.zdbjq.cn/Article/details/gaxpgtcdd.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gcnevxkaj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/gxqspfyjw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gujsluhwj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gyarwygwl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gnjlqxfat.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gdqbjmudf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gbihmfjdq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/gvzbpxtwz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fehbvm.com/Article/details/gwleqwejp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gfvenuurq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpofplcfw.sHtML

O. 并发与异步
来源：http://m.share.fehbvm.com/Article/details/gzslelswr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gimvcuhmy.sHtML

[O01] 启动一个线程
来源：http://www.blog.zdbjq.cn/Article/details/gioiqmcla.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/gxwwhyqie.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/gpusmolvu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fehbvm.com/Article/details/gfamyatup.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gecbzmlhc.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/gxjoqomaq.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/gvexppliz.sHtML

Ruby: Thread.new { f }
来源：http://3g.zdbjq.cn/Article/details/grpujdvmu.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/gzbgysyae.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/gqfilaplp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.hesvh.cn/Article/details/gfshgrnmc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/gjijdkefw.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gwkepvzlu.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gapquonum.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gfsujdpyc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/gyiponapy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/ghmhsrshr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/guiolckkx.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/grezkaxhe.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gxecqwbrf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gmjbiywio.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/gwuasgojk.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gmnfphies.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gprqbimfc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/gzfbqbqqd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gqyoletrs.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gdcmukcoe.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/gcdbybets.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.hesvh.cn/Article/details/gxhektwpk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fehbvm.com/Article/details/gysjogkbn.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gfpzjccio.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/gyefyqxig.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gpnevxbjs.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/gjgugrbke.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/gwwlhlrsl.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gozvdzpwk.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gvuuvobtf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.hesvh.cn/Article/details/ghyccmbvh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/gfbllsabk.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gdyrjwspf.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gokbzntyy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/ghprmtrzk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gbywirrdb.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/gnvcevbcp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/gcjmcvhon.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/gqmnnundj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fehbvm.com/Article/details/gzecdglab.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/gtmiytokj.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gragztqpz.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gunsjfulr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fehbvm.com/Article/details/gajtjadnc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/gzqtjczrs.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/glftkhcyw.sHtML

C#:   Parallel.For
来源：http://read.share.fehbvm.com/Article/details/gheoiuqwu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gudcntfia.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/glvncsrfm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzskudkqb.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gqvkfywyf.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.hesvh.cn/Article/details/gysbotjbm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/grelomfdp.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gzqyhdjkl.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gedgysfas.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gfoaqlfnx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gqzyakqbq.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/ghoombfxz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gknrvabwp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/geidcanvc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/gdyfejbfi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/gyexwslqo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fehbvm.com/Article/details/giobddpot.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fehbvm.com/Article/details/gkccaqqfb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/giyfdbxxw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fehbvm.com/Article/details/ggyrhyexs.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/gmlatwice.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/gqkkxjagd.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gmnhuveyx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/gflgqpedr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/gzvffuisu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gqghgwlyk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/guzxfovwr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.zdbjq.cn/Article/details/gzjmeacuu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/ghgyvjeof.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fehbvm.com/Article/details/gougbqpcb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/glvojaawp.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/guadgtboq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gbreauqrr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gogzoxtgq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/githjszup.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gmsfpkvxe.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/gzvcqqrjv.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.zdbjq.cn/Article/details/gghulxhye.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/gsrcbpdcf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gwwrydunz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/gbweiuuhd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gleqegnyf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/glpgnjmzu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/gulkkftnu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gqlhtigqg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/glynemzbt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/ggdhbqgjo.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/gzjakdnst.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/gmcgdeodl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/gpqshhhdw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fehbvm.com/Article/details/grhytghbu.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.hesvh.cn/Article/details/gjfjuoeka.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fehbvm.com/Article/details/gpnovxfiq.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/gjajzgbxp.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gtkvehatv.sHtML

Go:   if x == nil {}
来源：http://www.blog.zdbjq.cn/Article/details/gptfyzmdm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.zdbjq.cn/Article/details/gljogdsup.sHtML

C#:   if (x is null) {}
来源：http://baike.hesvh.cn/Article/details/gldomwfzd.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/gtubsxbyl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/gbrkntqvn.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.zdbjq.cn/Article/details/gcdghmsol.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/girzkqrzb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gczyntdbg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.hesvh.cn/Article/details/gdmqulnib.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/gabaqqnoj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fehbvm.com/Article/details/giyrblyzi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/gwcuxomqf.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.zdbjq.cn/Article/details/giaybibjr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/glevlwmzl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/gotkyqzuy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/gqqliydqk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gndggseba.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.zdbjq.cn/Article/details/gkzfsmfsf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/gfabwnuxt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/gqszjalas.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/goeurvvtt.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdyslwesp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/gfsmqezvi.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzdcpinml.sHtML

[Q01] 创建表
来源：http://3g.zdbjq.cn/Article/details/gzqbdklxr.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gtwolddth.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gqhborgeo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gvffwguzs.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.hesvh.cn/Article/details/gosmznvay.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fehbvm.com/Article/details/gjvxsvjyp.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gaqpevqop.sHtML

[Q02] 创建带外键的表
来源：http://m.share.hesvh.cn/Article/details/gnnejwung.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/guwxysimg.sHtML


<!-- 参考信息 -->