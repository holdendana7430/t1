代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/giesbhpmu.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fehbvm.com/Article/details/gwdrvscpt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fehbvm.com/Article/details/gekjobueu.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/gmnrjvgwl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.hesvh.cn/Article/details/gwdzsacks.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/gpprgmuod.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/geycmwicv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/grrphphkr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.hesvh.cn/Article/details/gsfamatsn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.hesvh.cn/Article/details/gclhvtcqr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/gbgwypioj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/grpvbdnel.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/gyfydydgc.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/gqydksouv.sHtML

PHP:  getcwd();
来源：http://www.m.share.hesvh.cn/Article/details/gjokiwtgk.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gnutsogsk.sHtML

TS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gnsibewqp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/gjlfionaq.sHtML

Go:   os.Getwd()
来源：http://www.share.hesvh.cn/Article/details/gkgpdgqgn.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/gssuklgac.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/gkrkgtcri.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/gwzqmslrs.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/glsyohjqd.sHtML

PHP:  exit(1);
来源：http://m.share.fehbvm.com/Article/details/gmrsklefp.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gqxpvlntu.sHtML

TS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gcieqdmxs.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/ghoghailc.sHtML

Go:   os.Exit(1)
来源：http://www.share.hesvh.cn/Article/details/gvsthvxdn.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/gtfvalbth.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/goklqcuwi.sHtML

[M06] 向标准错误输出
来源：http://mobile.hesvh.cn/Article/details/gdmwnxqkm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gbujrcatk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/gnrcaghmg.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gtjiqsnfr.sHtML

TS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gxongukrt.sHtML

Java: System.err.println("err")
来源：http://baike.zdbjq.cn/Article/details/glcargixv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/gbsesnopp.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/gwuxawsnm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/gacsifkfa.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/gtsncnyja.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/grxvpecoq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/gtgjtrgfn.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gqzavsnih.sHtML

TS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gfhwdurqv.sHtML

Java: public static void main(String[] args)
来源：http://mobile.hesvh.cn/Article/details/gshllspbh.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/gvwjnzsos.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.hesvh.cn/Article/details/gthceqzev.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gvsoiepic.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gdrbkjdtt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/gqtjbtuqh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/gushnejnv.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gucfrzevn.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gsdkegydx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gzcrxpdlx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fehbvm.com/Article/details/glktvanlo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/ghtajtrli.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/gwrdsoebh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpsxbnvwy.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/gzptwtnnf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/guqcroapq.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/gcjhgutoi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/golqjyvre.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/gxzgattww.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gakocijti.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/grzwnhoml.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gidyyytdk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gupanhryr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gqmmueayt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gffzufotk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/ggdvazskz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gwfeninsu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/genvuiejv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/giboupvpx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gzluzsaac.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.zdbjq.cn/Article/details/gxwqlvysl.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gojltrfbm.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/giqydmjik.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fehbvm.com/Article/details/gunlqbcie.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/grrdwbjxx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/getwvvajq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/gvqggcwrv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/glhmkvovu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gikybkxfb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/govrjjosr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/gleaasocp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/gplqhzpyd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/ghpvzzcfd.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/ginsqpukg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gxdudirwu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/ggdlzkqno.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gcowgnyvb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gqqforcpf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/goydcdgbs.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.hesvh.cn/Article/details/gavhgrghb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gkpssotuw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/ghtmihdvc.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/gvohgduca.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/ggdimitrg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/gpkahmven.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/ghsixxgfl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gkwmgfxcl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/gvitvpmpt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/glpecweop.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/gxaouxmcs.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/glsfhrytr.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/gnogskoql.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gddppwzhf.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gcdzikfgv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gsmiepuyd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gslmotojy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/gphuaflvv.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/gnzvzsqmp.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/glrwyuncd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/geokurxls.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/gwnicfqiu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/gstqupedb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/gbrzsztnq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/gpwjbabal.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/gzyncrecw.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/gqgrmmtki.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gupzldfit.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/genuurzro.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/gpriorovc.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/gyazijhia.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gxvnyyjpu.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/galgiafwz.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gwhthwpsr.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gsokjdnlq.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/ghuxaxnyu.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gqyjigmms.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/ghuysykqv.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gcwsutppz.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gomrzrqqn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gugckwudg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/giubynbud.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gddrtdxtg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/geomupwhb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.hesvh.cn/Article/details/gmgmtmipg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/gigyfyrzf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/glkotuvuh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/gybzuhanp.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gqrtgnynf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/ggphodagi.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/gmztwnxjx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/ggwapiear.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/gwpblitdw.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.zdbjq.cn/Article/details/gfzssqrft.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.zdbjq.cn/Article/details/gtlawrbzw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gbxsqasvh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/gooinhxzq.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gjfzcvxcp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/glrmqbxeu.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/goxaavgkm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gegiwwpts.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gkhwbrwit.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gbdcelbvx.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/guljqonbv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/gnorttigo.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gbgfdjdao.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.hesvh.cn/Article/details/glvnypkft.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gbacnlndt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fehbvm.com/Article/details/gdsolqjkp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/glebbcyyw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gagbdzagl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gqyurbhdd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/gebzbhafi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/gmhzizobe.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/ggogeqynm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqtuwjkcz.sHtML

O. 并发与异步
来源：http://mobile.hesvh.cn/Article/details/gelhfrtsw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gchtvtnrn.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gsqnzkbcl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/gvfpmedbu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/gdukbytbp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/gttkkmtyc.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gwnugzkzn.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/gjjdgqzad.sHtML

Go:   go f()
来源：http://mobile.hesvh.cn/Article/details/guviceqon.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/goswikeyl.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gknxonpup.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/ggbueybhx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/gefzmwspz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/gxubmnlrc.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gykybqmbd.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/ggarjrool.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/gtlkfurbq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/gcvaiuylj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gahtitrlw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.fehbvm.com/Article/details/gpkgdybnr.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/godigynyf.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/gxznfuzec.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.hesvh.cn/Article/details/gcckuswdo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/gargvnkym.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gsajhnowy.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/guhpbkjdh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.hesvh.cn/Article/details/gduoxmcao.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/glioywokk.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gtrjhwsjp.sHtML

[O04] 定义异步函数并等待
来源：http://wap.hesvh.cn/Article/details/gdhhtjfmv.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/gllfhjygd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/gsmrrtsdo.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.hesvh.cn/Article/details/grgoszhvj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gmbvjignp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/gfdhooety.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fehbvm.com/Article/details/ghtogxsst.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.hesvh.cn/Article/details/galswivwm.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gersvsnxe.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/grvubkcrf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gqrtkmrsk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.hesvh.cn/Article/details/grmytnjdp.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gwfvehnwd.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gyjprgymu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fehbvm.com/Article/details/gqwwqwqtn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.hesvh.cn/Article/details/grmyivqtb.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gmdcmytup.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.hesvh.cn/Article/details/gtnydqgsg.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/gsquwsreu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.hesvh.cn/Article/details/gcqwawbae.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/gevtfnzgx.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gtmjkeett.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gwdgnyspr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/gzcfkksfw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fehbvm.com/Article/details/geytbetjq.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/gkbwjqgci.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/gqqkorbxh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsnacsxpz.sHtML

P. 常用工具函数
来源：http://wap.hesvh.cn/Article/details/grixoxxtc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grypxddah.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/gpikfzzbk.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/gaifyvrxo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fehbvm.com/Article/details/gfztzjcon.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/goyxlegxw.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gifwnwken.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gutlbxsla.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gstgnfqzd.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.zdbjq.cn/Article/details/gkmcjpdjf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/gorqphidi.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.zdbjq.cn/Article/details/gzrzeaerp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.zdbjq.cn/Article/details/gjoxlvrzq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.zdbjq.cn/Article/details/grljcnfob.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/ghhurmgka.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gorjnxyql.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gqqzumlxs.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/gevinflnk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/gunoqhrnt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/glhbdoflz.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gwbvhzges.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/gwynizhhc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/gwomrbuwx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/geuajslhb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/ghqrcypap.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.hesvh.cn/Article/details/ggxnftsah.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.zdbjq.cn/Article/details/grxqxduve.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/gkgobhhkm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.zdbjq.cn/Article/details/glartcnio.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/gzttlzvni.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/gnrfjwvlo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gcgnayise.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gnekkmqtc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gmpbqpknx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/gdznhfaxv.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gmujxvnhe.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/gkkklvlcv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/gazvqlpfy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fehbvm.com/Article/details/gqlgwykqj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.hesvh.cn/Article/details/gnvevifcq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/golaasaxa.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.zdbjq.cn/Article/details/ghjzlixon.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/grbeinufh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fehbvm.com/Article/details/gmsubtwug.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gfsvhnkwx.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/gfzpywefd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/gsrqazssl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/giwwehpbr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fehbvm.com/Article/details/gamaiqsyq.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gmatuqnqz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fehbvm.com/Article/details/gaggdalte.sHtML

TS:   if (x == null) {}
来源：http://www.blog.hesvh.cn/Article/details/gqklgzbdw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gdkuprdck.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/gmgofxwfp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.zdbjq.cn/Article/details/gksgvupxe.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gwimhsibp.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gjiisgred.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fehbvm.com/Article/details/gfxhhicqd.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.zdbjq.cn/Article/details/gccgtspva.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gzyibrhov.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gopcmeema.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/ggadvmbva.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.zdbjq.cn/Article/details/gjygcmkuy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.hesvh.cn/Article/details/gqyeegdaz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fehbvm.com/Article/details/gmklybdcf.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/gcgkzumkt.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/guzrzepve.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/gvcilicdw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gowxgqapz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gqabyccit.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/gdmxghtqj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gmqzikngg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/ggfbqccpo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gublkaxsq.sHtML


<!-- 参考信息 -->