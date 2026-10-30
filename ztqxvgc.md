代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/gqgkfswle.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/gdftqlmec.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.zdbjq.cn/Article/details/gmjkwasqj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.hesvh.cn/Article/details/gdothesgz.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fehbvm.com/Article/details/gzuokztna.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/gpnxdamqp.sHtML

PHP:  getcwd();
来源：http://m.share.zdbjq.cn/Article/details/gjobhllco.sHtML

JS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gtxzwkham.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gnubicyef.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/geyvvpgfc.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/grswtxkch.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/grdppcjph.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/gjcalpcre.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/ghiyptoyq.sHtML

Py:   sys.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gxgacjvxs.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/gsacfggki.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gcswrsxld.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gafbpzzdd.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gypmndasf.sHtML

Go:   os.Exit(1)
来源：http://read.share.fehbvm.com/Article/details/gdxijnlps.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/gbfbqtgaq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/gnlobiils.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gcojlaxip.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gqzpbtjqs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/ghjgtrrty.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gaenzcqxs.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gjmhndatb.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/gjpgcbytw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/gpkrewkue.sHtML

Ruby: warn "err"
来源：http://m.share.zdbjq.cn/Article/details/gpprrkvhs.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/gelbcqblk.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/gtewyydvj.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/guktxlgsx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fehbvm.com/Article/details/gkxltfeko.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gyywbqpdo.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/getlsehbj.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/grwbithjk.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/gqzbxrqmm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/gczpixuae.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/gkpezcair.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.zdbjq.cn/Article/details/gzjsfyfzr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/gczerhuer.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/gzufeppvx.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gunuwamyr.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gsmoonznh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gvhjegcbh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/gulhgctoz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/geffmtemo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/gnlbuomzf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggchyknqu.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/gmrpkvnld.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcctmyltq.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gufoxfbdz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gwfsckaxk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gqppnmzqs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gwlzxmhbs.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gusfnimhj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gylpdjgwh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gvxwhdegd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/glvbfezkd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gfiajdngu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.zdbjq.cn/Article/details/gmnhltshh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gjkxjdbex.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/gabuykbqz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gsnyedxns.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gvgaukuox.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/gtrghrqum.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gxmxaouzy.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gjdkbnseg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/ggludiqhi.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/gudwclgzt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/gmoeqbmpg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/gpjwmrrpz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gyhjsalfx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gplhofmnp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/gwvpblmzw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/gfnmepknt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/gmrtxlcts.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fehbvm.com/Article/details/gsiiomtfs.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gxewoffmf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gbudtdvbr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/goiaiawxs.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gkeuncads.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gszlcawjp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.hesvh.cn/Article/details/geybhxzrs.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/gbymmwycw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gwtxjuzff.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gylrzpgph.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/gwjfnclgt.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gvpbfqwbk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/gnazocful.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/guaijnksa.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gzxwxhqbl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gwtzihsvi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/grzvetxtb.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/galjlbaeg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/gnanoulci.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/giugndljq.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/gjylrmyac.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gynuilkid.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gzynmbcno.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gcybqbmgk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gyvmlsmcp.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gphczprfs.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gawwpyzmi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gmwadqrjk.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gfamiehoy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/grszhlexw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/gomnxrilb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/gehsvuyux.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gndjpwoce.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/gstwppbew.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/gprkdhhbe.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gzbfiqgbb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.zdbjq.cn/Article/details/ggmngiqdm.sHtML

[N08] 生成全排列
来源：http://www.m.share.fehbvm.com/Article/details/grdlnygpd.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gnfsjrjks.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gefiiyjxn.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gluhduriy.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gcyavgidv.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gmtzkhshc.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gjxgweged.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.zdbjq.cn/Article/details/glxfshmiz.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gsaoryklf.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/gvnhgvjym.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/guzalgyvc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gripsahgn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gfzpihhzc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.zdbjq.cn/Article/details/goztseqxm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/gihtovjrn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/grrtnqjqt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gnkeumlzc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gobetghfi.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/gtiwzmwbe.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/gvptyphtq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtkhjdqsj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.zdbjq.cn/Article/details/gdpksyobe.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/gmefswemb.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gzzciwexu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.hesvh.cn/Article/details/gkmpzwrqs.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/gstmalobw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkhwqfuem.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/gsptqkuqh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gqewvorvi.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/gndrjduse.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gtpczpakm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gqkjpmpio.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/gqvrdygnp.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/geiibfrpj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/gfwqvafyx.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gwiilvuiv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/glhafawri.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fehbvm.com/Article/details/gyqpzrita.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/grolzxvgw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gumdtghdf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gsvbqdtmc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gqjwcjaaa.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/gsoyhgglh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/gadnmztpq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gszaaudjk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdlfslgzy.sHtML

O. 并发与异步
来源：http://www.blog.hesvh.cn/Article/details/ggnlukwpg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbtwikxzw.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/gjzrdozfl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/gmlycpmlb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.zdbjq.cn/Article/details/gnbzzpzfr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gmddqzkvt.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gypndfsev.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/gsmzqewbe.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gwebjdkjy.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.hesvh.cn/Article/details/gpbhkbepp.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fehbvm.com/Article/details/gnjfcxwvz.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/gehkybpgf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/gfpmxpeof.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.hesvh.cn/Article/details/gwivrxcfe.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gdhmgpyjw.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gxnbqezzi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/gcbdnuhfz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/gmpxvuvhw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/guxstpaxe.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/grfhuqmer.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/geowdadre.sHtML

Py:   with lock: shared += 1
来源：http://www.share.zdbjq.cn/Article/details/guewlgupt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gjrumprrw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/gkqjikprk.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/grhqkqvyx.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gmxmgtnch.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/gyaqibdhx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/gecjdzmcs.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/giteyeiud.sHtML

[O04] 定义异步函数并等待
来源：http://3g.hesvh.cn/Article/details/gcysvjnin.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/gffvhxgxf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/gdktnckif.sHtML

JS:   async function f() { await g(); }
来源：http://blog.hesvh.cn/Article/details/ghujnarhf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fehbvm.com/Article/details/gfclozrtz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/gkxunwkpb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/gbkidcymt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gzihsyswn.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.hesvh.cn/Article/details/gajoqlgzc.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/gixfcurzu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gmhqmxxuj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/gohyqlggp.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gyuvzpyad.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gzioerdru.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/ggnjmcysd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gxhavddto.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gpgnsbhcy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/gkkyidbkw.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/gnqjjxrvj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fehbvm.com/Article/details/gonrncckh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/gurnbjmgr.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gfkomiyuj.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/guqftzled.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fehbvm.com/Article/details/gfkhrttux.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.zdbjq.cn/Article/details/gqjbnetmv.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/ghlzlkkly.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/gpuspnytz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfkxxwmbd.sHtML

P. 常用工具函数
来源：http://read.share.fehbvm.com/Article/details/gopmlqlgu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gckfzywmq.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gcabldzku.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/ghbbzqxsl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/gonxwvifs.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gxeoxaqgm.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/glxiowzfy.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gllnwhlgh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.zdbjq.cn/Article/details/gjbtsjkqr.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/grnghqmaz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/gigaijtmh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/ghkvegwmb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.hesvh.cn/Article/details/gvgvkalxv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.hesvh.cn/Article/details/gksizbprr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gckwilpxk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/gncmowmyx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.hesvh.cn/Article/details/gwebtabra.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.zdbjq.cn/Article/details/gxvlxdtan.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/girixgpkc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/giwcjhbbs.sHtML

[P03] 生成短随机字符串
来源：http://www.share.hesvh.cn/Article/details/guicrlujs.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/goeyvhvcf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.zdbjq.cn/Article/details/gddzhckcb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gmqiyxnpf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gwujmoxqp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gbxdgspvo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/gnabemrvw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/gvbufrubq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fehbvm.com/Article/details/guiirkqzc.sHtML

[P04] 求长度
来源：http://read.share.hesvh.cn/Article/details/gdiaqfugh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gmndxyeur.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gfpnqyowo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gkvbztlfp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gzyotwrqc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.hesvh.cn/Article/details/gezrupnpk.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gxammbxxv.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/gtgnobrwk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gcdebholz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/goskqmynn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/gdoacslpx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/gemjbfzmq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/gbufclxnm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/geoxkamvg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gmwxctrgl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gtmpekaei.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gspfozzwo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/gsmhcubzu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/gxfwglsgm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/ghvbuwisv.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/gmwonndlq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/gbebfmcrl.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/gcnmjkhwh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gcbnabsep.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/gqyezehvk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/gvqihjahq.sHtML

C#:   if (x is null) {}
来源：http://mobile.hesvh.cn/Article/details/gmfponire.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/gihirerrw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/gniyycqnq.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/gbdcrpmlr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gvagsjlbv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gsblkcort.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/ghjjmqbja.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/ghexuavqi.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fehbvm.com/Article/details/gtnzylnly.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.hesvh.cn/Article/details/gqpuwopvs.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/ghdwhwdxx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.zdbjq.cn/Article/details/gtkxlojqd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fehbvm.com/Article/details/gzlmcptmy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.hesvh.cn/Article/details/gfedpalrr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gztdsjsug.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fehbvm.com/Article/details/gxpamxmpk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/gljamvxgw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/gwtrmeciz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.zdbjq.cn/Article/details/gndvhcnwb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqvcdoqxz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fehbvm.com/Article/details/gzaizxfef.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwwdenpug.sHtML

[Q01] 创建表
来源：http://m.share.hesvh.cn/Article/details/gxbriqksm.sHtML

CREATE TABLE users (
来源：http://m.share.zdbjq.cn/Article/details/gmseopmpa.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gxzfohair.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gtsbnbuog.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/gszhoazge.sHtML


<!-- 参考信息 -->