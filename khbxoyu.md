代发 wailian999

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gnuqbhuru.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/gbguonmvz.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/gzgwuhavl.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/gmpcskfne.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/glmwmpdex.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/gvvqoqmcu.sHtML

Py:   sys.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gcjxwmhka.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/gjtinasdz.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gyykvchgf.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gylxgwemr.sHtML

Java: System.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gqyhzpnyp.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gmpjfmheu.sHtML

Ruby: exit 1
来源：http://blog.zdbjq.cn/Article/details/gwgijrpqj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/gbtxxmhlt.sHtML

[M06] 向标准错误输出
来源：http://3g.fehbvm.com/Article/details/gvfhqnyye.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/ggfvqyknt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/grvanajwc.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gfdtrfzxc.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gpoapvwvz.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gsyqnkmmt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fehbvm.com/Article/details/gyugetshr.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/gjnyaunxo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/gepctsrzo.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gspujwkiy.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/getbmaznr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/geuavwuee.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gaeiqhmuz.sHtML

TS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gtfhztxpw.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/gyrdfmkkh.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/gweymlblo.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/gquadtmyj.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/gvfojocws.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gfnsdqeay.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/gmmlvrjyy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fehbvm.com/Article/details/gfxrzvqet.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gqqrvacrk.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/geboctcgn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gmexoqmeq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/grajhbcmd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/gzqhmtilv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/gndlasbxv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gsyoqjigp.sHtML

N. 数据结构与算法
来源：http://m.share.fehbvm.com/Article/details/gexkofpfu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gczfjtjtb.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/gfvvorcaq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gnvgpfxsp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gzujuqqme.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gliviljfj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gsmnvhiyk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gtmybvxzf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/gicgpcgwh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/goptqrcnt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gsjhqaxon.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/gogfzrbpe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gdbkcqsuh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/grqjjhpzw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gcsibnmhi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gxzxromoy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/gnstrmyzg.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gbydkyzdy.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gfkkyilus.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/glkvccqyb.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/gxyxcalef.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.hesvh.cn/Article/details/glodqjfnp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fehbvm.com/Article/details/galcfeibg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/greothbhv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gcqbcgpue.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/gujfwkdbp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/gmwvwkuwh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/gcoypzfkk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/gmwjsiyfc.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gnkhuxdzw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/goqxvuwud.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gblhiuidd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gkaeiqzoy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gzvuhldzk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gmcrvgjyf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.hesvh.cn/Article/details/guaeifqxg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gzdtcsoqy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gprcathqa.sHtML

[N05] 最大公约数
来源：http://read.share.hesvh.cn/Article/details/gzfmyqavn.sHtML

Py:   math.gcd(a, b)
来源：http://3g.hesvh.cn/Article/details/gjdqzourn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gwhchxeco.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gchhqgzhi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gfzldobkh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gvfdmigou.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.zdbjq.cn/Article/details/gikfgdjjs.sHtML

Ruby: a.gcd(b)
来源：http://baike.zdbjq.cn/Article/details/goylhjtov.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/golorqatu.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gohslkvvn.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/gswyyyvej.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gxqveelwp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gprlpuxmy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gqjzbrjai.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/gqbyxomzc.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gsdfcfqjb.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/guylnmwoz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gdsvggjio.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gqqlhhivj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gtxtlnysu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/glmowzzfn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/gaoksmzli.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.zdbjq.cn/Article/details/gpruudjkz.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/gzzmamklj.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/ggntsidvb.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gidcfuguz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gkpvmtukn.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gnyjiorkn.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gombnbwep.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/gqlqxjztf.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gzibjzaac.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gvghkrkvj.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gokicsmof.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gtdvnwdea.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gixlzpnfw.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/glzfhqcdc.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/giskddkad.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gxuzvfnzl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/gcnlcxzaj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gkzssqnji.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.hesvh.cn/Article/details/glkxtegpg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.zdbjq.cn/Article/details/ggetldarq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.hesvh.cn/Article/details/glvzrmwge.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gjrkxlhrf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/gsvadxxun.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/glzqlrcwa.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fehbvm.com/Article/details/gmsmoyhxj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gtbslovol.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/geqdeztuu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.hesvh.cn/Article/details/gbrslwqui.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/gxkhpsxaw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/gauygirsj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/gvfzodytn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/gsenqdmry.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fehbvm.com/Article/details/glvttbmpe.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/gmypaadcm.sHtML

PHP:  // 手写递归函数
来源：http://3g.fehbvm.com/Article/details/gtqnodehb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gntrwuror.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gvznvznea.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gpjwhblnh.sHtML

Go:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gqjduimdx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/gsuddmncf.sHtML

C#:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gfiddjufa.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/gtkbeaycb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/goclrjkff.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/gbvoylzlj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gisrjdaci.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gfiabctyr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/grzrcnxoz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.hesvh.cn/Article/details/gqvhxyaop.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/gdztxninh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gfpkfhpne.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmgwthsxo.sHtML

O. 并发与异步
来源：http://www.m.share.fehbvm.com/Article/details/givbjzhij.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glcqtsdxe.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gafmzljyj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/glijpxeul.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.hesvh.cn/Article/details/gxhhkduvh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/gklwdqhfg.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/ggqesrfre.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.zdbjq.cn/Article/details/gxogvnwkm.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gcqzrfgrw.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/gcvgifqyg.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/gjphpnfjl.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/gxvmhxozh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fehbvm.com/Article/details/gcrfthejj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gyfyrxdtf.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gddfdzcny.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gwgzhliem.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/gfoopstbi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/glhlbgpuo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/gryqdkigr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/gdevyrirg.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/gejnbdmnb.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/gpuutowau.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fehbvm.com/Article/details/gfxfidjio.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.zdbjq.cn/Article/details/gznwwhrgs.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gyjogkzfd.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpyirvqss.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.zdbjq.cn/Article/details/gzidoucwh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/gargoanhv.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gsjjibaxp.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gloivpyju.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/ghrufjied.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/gokaxhcpt.sHtML

JS:   async function f() { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gpqcsraut.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gmcphlcfd.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/gvhflmivx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fehbvm.com/Article/details/grxfbexqa.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/girthzxgn.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/grwkiedxb.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.zdbjq.cn/Article/details/grsmtpcsf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/gmiiehwat.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/gtvgbzdjw.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/grudjurap.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gcdnaijev.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/gowdzoqha.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/gyufgtxxu.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fehbvm.com/Article/details/ggllrwatr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/ghimznxfn.sHtML

[O06] 使用进程池
来源：http://wap.hesvh.cn/Article/details/grhedoxeb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/ganhthxov.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/gxulffygf.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gedxxkcix.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gdvwdgumu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gkofldirj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.hesvh.cn/Article/details/gndvskyhw.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/gavytqeve.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/gewnfnrnd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdngtvovr.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/gwohfilcy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpnrddjmj.sHtML

[P01] 生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gybdpereq.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.zdbjq.cn/Article/details/gpwexycxx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/gcwfiaiql.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gartxxprm.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gzlbjerot.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gwwhzbbij.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/girjpyqsk.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/ganupmsff.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/gxvtjawlr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fehbvm.com/Article/details/ggnyxjmxs.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.hesvh.cn/Article/details/ggghgbtsa.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/gsdxywuny.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.hesvh.cn/Article/details/gqxgjmbbu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/gwsgpkeif.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gcrtclaig.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/glirnpnba.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/gkqcjgakl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/gilcjztgn.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/gmarlxpnc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/gcsvkwsep.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/gykoisrxq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gfwzocnhq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gesydhufk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.hesvh.cn/Article/details/gvapbajri.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.zdbjq.cn/Article/details/gceungviw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fehbvm.com/Article/details/gqfpzzfem.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/gcgwvrrxq.sHtML

[P04] 求长度
来源：http://read.share.hesvh.cn/Article/details/gyleogvti.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/gwgwfecpc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/ggzbwhulh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gxhywcxwf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/goxectlos.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fehbvm.com/Article/details/goyusvnwg.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gypefennv.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/gunvegnxr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fehbvm.com/Article/details/geutvdnal.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/gmteftijx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/gdqumznkz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/gqmwulqdh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/gkgfotbnb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gtqxslppm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gekguanev.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gsaqhaeei.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/geyhyqihm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fehbvm.com/Article/details/gnwbopeqp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fehbvm.com/Article/details/giljlmrpy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fehbvm.com/Article/details/gqptlofxq.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/govycfolj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/ghrbvtykj.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/gpmfnggwx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gyqakyvcv.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gbeicvuat.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/glxzqshfl.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/gitltmcsy.sHtML

[P07] 防抖与节流
来源：http://www.m.share.zdbjq.cn/Article/details/gmsdyopzn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/gncstocvw.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/gyudqwgvt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gtrhnqvmg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/geyafxbns.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/gtgndgczn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fehbvm.com/Article/details/gkioptiej.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/gvsvrryvn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gbfupezep.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.hesvh.cn/Article/details/gtwyhkunc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/gdudmxoow.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.hesvh.cn/Article/details/gnwdvxnvu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fehbvm.com/Article/details/gmiebovni.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gzzhkstnv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/guimmjnhl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/gvuvoohwt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fehbvm.com/Article/details/gatjvwcbq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/gdposizyx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtlgjduqp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/geirrjpuw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/glmlxitby.sHtML

[Q01] 创建表
来源：http://blog.hesvh.cn/Article/details/gepxwdyqw.sHtML

CREATE TABLE users (
来源：http://www.m.share.zdbjq.cn/Article/details/ghfgxbdyx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/galoxrija.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gqylnzshq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gtwlvgimk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gpyubujun.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gqdqjnbpb.sHtML

[Q02] 创建带外键的表
来源：http://mobile.zdbjq.cn/Article/details/gozbwmdwp.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/gscirhmnf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gmeqhhjeq.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gdebezglp.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fehbvm.com/Article/details/gksvnxcnz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.zdbjq.cn/Article/details/gysbuvpyn.sHtML


<!-- 参考信息 -->