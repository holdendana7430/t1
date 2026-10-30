代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gwftlpdbp.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.hesvh.cn/Article/details/gbbnvstaz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/guemwnsux.sHtML

[M03] 执行外部命令
来源：http://baike.hesvh.cn/Article/details/gstizjayu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/ghpbdpwjc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.zdbjq.cn/Article/details/gfdlrpvsy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gtyvplchv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gjpizxtld.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gyubevlqf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/gdborlvly.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/guyrwlvdb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.zdbjq.cn/Article/details/geqzavixc.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/giyteegnl.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/gjvrpfgfw.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gwhoyicao.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/ggfpqozdz.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gfazfeynw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fehbvm.com/Article/details/glsphigvh.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/gefpvnndx.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.zdbjq.cn/Article/details/gadfzpqgx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/gdchnsokr.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/gmhqrrhcx.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/ggxoxrzcx.sHtML

PHP:  exit(1);
来源：http://m.share.fehbvm.com/Article/details/gfvhbxjrx.sHtML

JS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gaqctqokg.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gilzsezrh.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gdviylepb.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gexpiylqb.sHtML

Ruby: exit 1
来源：http://blog.zdbjq.cn/Article/details/gmpbsebao.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/gohxjxolq.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.zdbjq.cn/Article/details/gmwvmxdxy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gyulmwagt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/goushbwes.sHtML

JS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gxgwsrgls.sHtML

TS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gorjferin.sHtML

Java: System.err.println("err")
来源：http://m.share.fehbvm.com/Article/details/gryvweuwn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gdgrxecvq.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gfbsngofn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gubueqspn.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/geaebdarw.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/gfmojpmla.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/gmgyvrgvy.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gizrappse.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gujhnogvz.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/gcmbwpuvs.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/gshvasjwt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/giqfryqzl.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/gfimvulzu.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/gnteypcjf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/gpiezukei.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gfbdjgbqf.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/grdscplud.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gqxfgtfhj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/gejrfiqjo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gcfihjoiu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/ghzoehqpo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/gukuiebsx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjailrrif.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/gjhiowgqj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gaxzlmjbb.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/guipjsqfr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/garagepqn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gwpnwgawq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/godiugmig.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gmhynldjf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gawwtaceh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gxmdtaqif.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/glsnfbzmq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gwfeajvyu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/gctpyvcvh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/ggedewiek.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/greenauio.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/ggujeohxa.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gvpiwobjn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gywwdmrby.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gbfxrtwqf.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gultcqrfd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/gvheishqt.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/gszfsscem.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fehbvm.com/Article/details/gbthutrqy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/gyxbqfyrq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gytgsgoqu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gbjhtkpyq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gsmergrpg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/gasmaeakx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/gkadabrxr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.hesvh.cn/Article/details/getzgtvkp.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/gnxpvlxex.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/grsvmczce.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gmadomtfe.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gwprgvtvy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gphfyhbpl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/geeehaoff.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.hesvh.cn/Article/details/glgpzeyuc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gnsxuewlt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gpmvslyyo.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/gmwdkwvzn.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gtqqctqaz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.zdbjq.cn/Article/details/gfbipitbw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gelqzrsud.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gfokfpxun.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gtpmsdfmt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/gswyfxoyu.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/gijsnjfma.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/gekhxgfjp.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gxfizrdqg.sHtML

Py:   s == s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gbyifnksv.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gsmfeszwg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gpfplvznt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gvjcygyfp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gxjtbaubx.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gaskhytxo.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gqfegjlfb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/goikinnee.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/gmaqzdpcr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gzldalede.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/goicgweog.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gtblrvkmc.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/gkjnmhngx.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/geawfdfke.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/gsdusuyal.sHtML

Ruby: // 手写 Hash
来源：http://baike.fehbvm.com/Article/details/gnennftcp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/gvsteqgrn.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/gcqieqgjc.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gytdtacil.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/guovfavwm.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gpgbebjdi.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gyulpiola.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/glzunmpuq.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gvezdhgqd.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gpkyykita.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gholuyrrq.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gmcfhyfiq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/ghtaqvour.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gerxsupfn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gnbrhmshc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/ggezzdwlf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gzmmieiec.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/gyaypcyry.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gkunvxtff.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/gtygiqwfp.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gumbbjbck.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/guzcawerr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/garvnxusi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.zdbjq.cn/Article/details/grfwqdbky.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/ghmwwqrzb.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gcjpdmyos.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.zdbjq.cn/Article/details/gfcmepzim.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.zdbjq.cn/Article/details/gmvtvqofu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fehbvm.com/Article/details/gttvwzeci.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/givvfcgux.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gptivsccm.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/gqmxvkdbu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gvmomexdl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gwedxwmop.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/gkpzmmbgt.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gnsiaoxse.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/gumotlblm.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gsafkohgs.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/gocyakbda.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/gmttabeta.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gmtnidtov.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/grtixxsui.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gpizghimn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gyrrgstbs.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/gfupjxbzb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.hesvh.cn/Article/details/gibrkezob.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gtvezypcs.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzhfplniw.sHtML

O. 并发与异步
来源：http://mobile.hesvh.cn/Article/details/gzbazdnsd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gguvuybsj.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/grjikqdlm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/gycpbswep.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/gtbslaspb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fehbvm.com/Article/details/gwipwefzi.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gedawhrdj.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/gmucddmcg.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gxuujemft.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/gyujmfjng.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gbwhrmbyb.sHtML

[O02] 使用线程池
来源：http://read.share.zdbjq.cn/Article/details/gwtyuoikx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/grkcnrkzs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.zdbjq.cn/Article/details/gzfdxjtku.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gwmxcehnm.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gyiqrcyeh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fehbvm.com/Article/details/gnlktstos.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gwqjroaac.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/gvcnxuzlk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/gqtximrzf.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.zdbjq.cn/Article/details/gimjrxoop.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/griaiowob.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fehbvm.com/Article/details/ggfhifqtz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/gaxeynlhq.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/ghhkfzkjy.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gozutgnzq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fehbvm.com/Article/details/gneaunsaz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gfvzsfrwc.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gazkamtoh.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gosnerfgt.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.zdbjq.cn/Article/details/ghlumcbaf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fehbvm.com/Article/details/grwvvngns.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/grrswhiri.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gkhsddpoq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/glnaxxncw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.zdbjq.cn/Article/details/gotiyothz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.hesvh.cn/Article/details/ggkbccgpc.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fehbvm.com/Article/details/ghunyaees.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/giuguzemd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/gakihovif.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/gcflwnnue.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gndltwqbs.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gobqxvmft.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.hesvh.cn/Article/details/ghykxvndl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/gatzfaqro.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/gdxtysjki.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/gtkdiybcx.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/grzxdpafz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/glerhdwyl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/gfevrsiai.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gchymwrhd.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/grraecbvi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/gkgooyrwx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/ggdudejld.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/gmloawjkd.sHtML

C#:   Parallel.For
来源：http://www.blog.hesvh.cn/Article/details/gsxammttl.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqcdugjlz.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/gdfunannd.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvswuvrfy.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/gqbppumae.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.hesvh.cn/Article/details/grnxjwzff.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.zdbjq.cn/Article/details/gmkjesglb.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gbpblvbvr.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gkmeapxss.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gnvtojuld.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gyvsywtax.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.zdbjq.cn/Article/details/gtlpgrrjh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.zdbjq.cn/Article/details/guzbeeqfr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/ghwaixeht.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/gguxsqfrt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/gqvvpvblo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.hesvh.cn/Article/details/gqkgzqqzy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/gdeqvyvao.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gcqdrezws.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/gfexcsgwi.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/gatimcnca.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fehbvm.com/Article/details/givgjikzc.sHtML

[P03] 生成短随机字符串
来源：http://3g.hesvh.cn/Article/details/gmrdkkiyn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/gkimqdcoi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/gnrnmmgmc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gzxgvueon.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gkbcoaple.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/gncsmokjt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.zdbjq.cn/Article/details/gufnjjwwo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/gtsbjcsjm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/gjkwwiyww.sHtML

[P04] 求长度
来源：http://baike.zdbjq.cn/Article/details/golmjkwet.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.zdbjq.cn/Article/details/gmhwvziyz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gmotuvuui.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gqcsamqzq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gewbxwohm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/gdkinbdzh.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/gckaavvhv.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/gdyqveqxc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.hesvh.cn/Article/details/glrfdmtpa.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gpwzqxtfh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.hesvh.cn/Article/details/grzvrmtjl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/gpuplobxj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/gegcfinxh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gerlwyyec.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/gigindwfp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.hesvh.cn/Article/details/gvprwjyjn.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/giribxbvz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.hesvh.cn/Article/details/gzofyqyga.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fehbvm.com/Article/details/gsnyiecyz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gesfafvsw.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gmtpvuzxn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/gqiddpbnm.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gsiuzzzqi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/ggdmbfrzd.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/gnvnahgyv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/gqokaxvyc.sHtML

C#:   if (x is null) {}
来源：http://www.blog.hesvh.cn/Article/details/gtejvkkrt.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/gzrgieuta.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.zdbjq.cn/Article/details/gcydhxcrj.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.zdbjq.cn/Article/details/ginytzovy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gskjmsgtf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gsjgpajwg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/gbwwmhmir.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gqabzdbvt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gciywdjtw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/gvemioock.sHtML

[P08] 处理浮点精度问题
来源：http://blog.hesvh.cn/Article/details/gcuxkwybe.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fehbvm.com/Article/details/gfooynphp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.zdbjq.cn/Article/details/gpwpldlev.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.hesvh.cn/Article/details/gircceaby.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gfaetzoyv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fehbvm.com/Article/details/gjcuoxqjq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.hesvh.cn/Article/details/gdxqsouvr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/gkicravml.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/gkgubmidy.sHtML


<!-- 参考信息 -->