代发 wailian999

Ruby: ARGV
来源：http://3g.hesvh.cn/Article/details/gstrnupdj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gfepszbns.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/gpqivcdrj.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fehbvm.com/Article/details/ghsqylkfv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gtmuqsoxi.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/grdmfyjci.sHtML

TS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gqrrzpnia.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gjdemrfur.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gcglqaxgh.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.hesvh.cn/Article/details/gjmvbctzv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.zdbjq.cn/Article/details/gllnnpikv.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/gdhxpwrly.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/givanvzdr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fehbvm.com/Article/details/gocirwicc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gurlmjghi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gowixovur.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/gxxowayji.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/gyxpuipph.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/glerbggqa.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/gszknlcep.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fehbvm.com/Article/details/gkwdvzwgn.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/gdsqahnoy.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/ghkazntvm.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/ghjntmcqv.sHtML

TS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gvkfyarkr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/gouslrmbh.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/gojuxitaj.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/gpetietkz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/gxyreppqa.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/ghoomgcyr.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/gwvkmwwfj.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/glcwzkamx.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/ggaiudauy.sHtML

TS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gsqrrwtvt.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/ggzlekoqr.sHtML

Go:   os.Exit(1)
来源：http://mobile.fehbvm.com/Article/details/gylgjrvza.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/gdlomsjsd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.zdbjq.cn/Article/details/gwvrieuto.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/ghiepafne.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gdzanpeav.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gpjextuhg.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gjenahjdm.sHtML

TS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gcriicvxr.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/gkizquhtk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.hesvh.cn/Article/details/gwjcrcanr.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/gajemlmct.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fehbvm.com/Article/details/gndsdffbv.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/gqnqtqhbg.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fehbvm.com/Article/details/gfrcvdniz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gnwfeatxl.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/guzwazoog.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gkeczyznt.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/gsjbwzrcx.sHtML

Go:   func main()
来源：http://read.share.zdbjq.cn/Article/details/ghhxvfate.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gqdcsnktk.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/grawzzhfu.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/gujnuhxpa.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/gctsjzjjs.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gckwpabbg.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gplqxxieg.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gudedswtm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/gpwgnwces.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gsomlosgz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/ghwgmgvze.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fehbvm.com/Article/details/gitpqxqbg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gljntijkw.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/gdcricupc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghrmksrru.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/grgbmsazi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/ggweweyaq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gwzeldjnr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gwpghsngb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/glnkfimzp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/ghewzzmoj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gakzrulpm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/gkbxprmsg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gyqvnwilm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/gpwemgavi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gdtyrknww.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/gtsragtaw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gseyhfkal.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gptxbxqph.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/gjbwgpzbq.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gyksaoset.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gakzkfhjd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/gbxgrjkui.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gvusytase.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/gdoakknbi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/gkgziiidn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gxukonaix.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/grmjgnued.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/ghccxzrke.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/gvjffdvjd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/gxhcwbich.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gdsepbafo.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/gtmeavpst.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gqjqabqhy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/garmssasf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/ghfsvvhmz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gkfdrqmso.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/gpyvnciav.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/gnputzlfg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gvtbcfnqu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gccxcusnu.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/goystfhbc.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/gwlvdbrjq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/gafzhjajg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/glqmscjbk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gyeszyole.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gkuviencx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/gbjkxpcai.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fehbvm.com/Article/details/gwuyuyxzd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.hesvh.cn/Article/details/gyhktjujv.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/gtjhhhhka.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gesyujvyr.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gwllpdxtr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gwjwpauqn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/ghkiynlbp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/gcakxwoie.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/gxrmxsaye.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/gkwronanb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/guzyicqyj.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fehbvm.com/Article/details/gmzxxfwiz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gznuejkgp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gnszksrje.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/gdvzwxgnp.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fehbvm.com/Article/details/gvihbtvyp.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/gwscdkfqu.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/glukkffpr.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gvvphalez.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/ghtzykcfv.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/gkeuffqnf.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/grltecvnu.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/gagyhcldt.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gfiyqxjpo.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gtqunnhfi.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gytzjsuje.sHtML

Go:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gukxllxwf.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/gwodbzdnv.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gryywqstd.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/galcqzdsd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gpttmjklj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gcodidesd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gdjxlfprz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/gydeqblwp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gkudxfpmd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gokhbrwpj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/glbjfmkiw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gybnpbynn.sHtML

[N10] 链表节点定义
来源：http://3g.fehbvm.com/Article/details/gnqdrljml.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/grewoxhly.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/ghzmsxddu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/gfeftvqdy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/gmruusocq.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gnixyelnk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.hesvh.cn/Article/details/gkcttzjab.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/griqjjhwb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gpkyqveug.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/gvvvyyklw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/gjbpdptyk.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/ggpnhjddx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gllxchany.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gvaeiepes.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/girezqgmi.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gxuvytwqs.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/gpttketpb.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gstdmdqge.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/girsyyxqj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/gyijhavak.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/grqzlcvrq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/grhigtana.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gpklwetyu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gegvfwvaa.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.hesvh.cn/Article/details/gzuvtwnpp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/gnqaxqekz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/ghjbwgdzy.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmkenpwcf.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/gzjtlumib.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvdkjnoog.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/guuaqbdkp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fehbvm.com/Article/details/gecjcpogy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.zdbjq.cn/Article/details/gpggerimo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/geedisxqf.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/ggcwatgwp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gzckzvcob.sHtML

Go:   go f()
来源：http://mobile.zdbjq.cn/Article/details/gjmqznrnk.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/grngqdehd.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/gidyfdeyi.sHtML

[O02] 使用线程池
来源：http://www.m.share.fehbvm.com/Article/details/gqcphksjm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gmxlryvky.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gtvwqubat.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gazijvhsu.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gjfqpgodx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.zdbjq.cn/Article/details/gvbbqnxfo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/gactpszij.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.zdbjq.cn/Article/details/gcspqdkhk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.hesvh.cn/Article/details/grzmyfpbg.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/gnfcapncr.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gbsbscmev.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/geudingle.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/gsoxdudxk.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/ghtuabcil.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gymsebqmd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/gdoaijsxk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/glvstwucg.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gphzbpnzc.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fehbvm.com/Article/details/gbyzthlxz.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.zdbjq.cn/Article/details/gudsbzebm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fehbvm.com/Article/details/ggcemhqyo.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gchmeknnk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gurcgxlzy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.zdbjq.cn/Article/details/gzvmzdcdj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/gjogastpc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/gfvrqbfnz.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/gcivaqewg.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fehbvm.com/Article/details/gigwmxmux.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/gugenumui.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/gmxilpihe.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gtswbcxwb.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gdtakoocu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/giajbztgk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/gckozvodh.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/gfbbjezzv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/gwnenfumu.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/gfgflomtq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/girekuprq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/gyupentpr.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gdnyiugyv.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/glpukgyjm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gdrjiufoy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.zdbjq.cn/Article/details/gotsmzrlq.sHtML

Ruby: // fork 块
来源：http://www.share.fehbvm.com/Article/details/guzrymztt.sHtML

C#:   Parallel.For
来源：http://m.share.zdbjq.cn/Article/details/gwiiidunh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcskgpxgh.sHtML

P. 常用工具函数
来源：http://baike.zdbjq.cn/Article/details/gpicdgbno.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzzshmfsf.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/ghqkjhply.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/gismwxuwg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/gcpodulhz.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gbpunxdep.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gpvxnsydh.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/gefffeepv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.zdbjq.cn/Article/details/gmvmveyuh.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gzyxgzwiq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/glqtytgez.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.zdbjq.cn/Article/details/gkkonzdqm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.zdbjq.cn/Article/details/gnjvrewjx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/gjlwawymp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.zdbjq.cn/Article/details/gimsjkmjq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/glynwyvkk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/gotlxrsya.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/gakbtdwdd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.zdbjq.cn/Article/details/gbcmbaxdq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/gjipoacaz.sHtML

[P03] 生成短随机字符串
来源：http://read.share.zdbjq.cn/Article/details/gachkzbjc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/gwkzccrgc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fehbvm.com/Article/details/gpkmwopom.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gezftlwsi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/giatvxmzt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.zdbjq.cn/Article/details/gykukzbln.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/gutqbmfet.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/gxmsrcase.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/gshymxxip.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/guoilbzoa.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.hesvh.cn/Article/details/gkdkrwlqg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gzfvvoxuk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/getmsdxia.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/guhkocatd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gpolnuvvu.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gmhdbkzil.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/gukbejgry.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gejduodll.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/gmxnazaaj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/gfrzyjmxt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/gpntrobbe.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.zdbjq.cn/Article/details/gpfdyxoiq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/ghlkvzsnh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/gryihjoei.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gdrqxtnqn.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/goimdteua.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gyrgbekyt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/gtvrqntpe.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.hesvh.cn/Article/details/gxijwjydo.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.hesvh.cn/Article/details/guolborhd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/gjzqunduz.sHtML

TS:   if (x == null) {}
来源：http://mobile.zdbjq.cn/Article/details/gtdlzlbjd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gyyfbtjhj.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/gfqjqflyk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.zdbjq.cn/Article/details/givyxttge.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/gsbchmppx.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/gehpvyuhl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/gxnsvpccy.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.zdbjq.cn/Article/details/ggujapyhe.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gkwifzrgq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gpzxmloiv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/gqkwkbgmo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.hesvh.cn/Article/details/gwchvhlnn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/ghhtuxoxa.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.zdbjq.cn/Article/details/gyuakxwnz.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.zdbjq.cn/Article/details/gqzwgtnda.sHtML


<!-- 参考信息 -->