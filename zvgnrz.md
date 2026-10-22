代发 wailian999

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wvbxlkaa.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2jprjybgw.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2cqvbxqlc.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2nfootrij.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2hxnhsuyb.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ehxsnenm.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2vbbhiwxk.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kptereol.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2aqfexfxn.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ewjxkmfv.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2egokejte.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wvjqxvus.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rumvdcro.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2zxkhiyjq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2gctavidq.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2ercgwjfe.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tdjpeyxb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2yrpdlicx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2uqkoslpg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tvirhlfz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2vgirgjvn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2rllnjbga.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2mvgxrqjn.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2tsuowmxj.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2fpsdqqpk.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xmiobxki.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2sfewtphc.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ewnaajun.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ozmbseve.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2gurnaayx.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2dfmpccmj.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2glbjozlf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2mykmzhvt.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2utgfcgfk.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rsgetqjc.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2exgnsfzt.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ppktidvy.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2etnhagld.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lmtcjoiz.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wxvmbbcu.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2mnchzomp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2dqanbpzl.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2qtipwujd.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2tcdqtpdf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2smtvbeee.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2tssqkbzv.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2eyrbzwzq.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2xhutlard.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2cvypyeql.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2syrblcsh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2mxkslqvf.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2fjzcdqxl.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2ewigkcll.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2egartgux.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ewcdckqe.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ixbjjria.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2rpigbiha.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2zphyytox.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2vklfzgne.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2vmaojmxw.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2xkzuujnr.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2muemldus.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2aiijqulp.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2brvhkhvt.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2pegyvkjv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2wgfwzuqu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2codrccam.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2twrcdnlt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2ablrmdii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wvxebqrx.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2knyochan.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kbafkgbd.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2jllafsbf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2smwwqptr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2kdqbszir.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2yrypsbew.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2gpwgtofy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xhubieri.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2yznlbwud.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2syfdlohe.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zgksitce.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2nehleddw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2dqfgjnri.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2gabqhbdh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2eltvzfsm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2bcaoxjle.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2fkhfmwca.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cjhurhcv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2hjnsakeo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2bkvbxodc.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2isjusthp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2ajinpeti.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2asvqczbm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2kwgcsgkv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2rzxpkuyy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ovbzpcjt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2qqxvtayv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2ovhkakpx.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2tcddgpdd.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2jvytoptx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iqjdvviz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2gpvfsmuk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2orimeioe.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2oewoqjec.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2lpurvewc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2qhfzglgz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2vwonysxf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dbphbdxg.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2ucjwjcsl.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2nkivdgfq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2niksqpvo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2nsjywqlc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2qspffgqs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2aaaczczt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2kwdweecs.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2omiwtwfy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2qkesjyeg.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uhxetnie.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2actvdupz.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2oicfjwmz.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2majtbxnp.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2oejbpuzy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2gkspmafr.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2phifavie.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hqsgvonl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2nbquzfuf.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2vprewjzz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2icxedmkm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2adggbxfv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2oaumnnvn.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2lbijcnjw.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2mrjfegyl.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2uwiokzlk.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2bwefqzcn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2mbnvylpx.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2yzmobyvn.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2cbgukntd.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2uxssxruf.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tqjtqvab.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2porleabg.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bqtzrguy.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2roimkqlt.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2fmitwrvt.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2isaoitan.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2omvhvmkg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2gcvhqhoo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pbvceygp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vtqxlzda.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2vxtjsyts.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2qbvvdzus.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2zgoamchn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mwlozgze.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2intbpnro.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2asiykodx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2ntlemwqz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2xacxnopo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nxjxtcnx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ttrzkqrj.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2qazcnfvd.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2zqwoojlm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ryuvqtso.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2gaodluvv.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2wtohutsm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2qztevnvz.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2uwpvmxgq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2mhicrmri.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2qutxrufu.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2dnxwlmgv.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2yvxyncjp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2lnsmfcht.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2hejtwtob.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ostjkcyg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2iybnnihm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2sgapemcb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ykigytwq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2tqrogolj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2kjkljoxw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2vqzgunad.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2mmlapruo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2flvzciiv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dcwzfwuv.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2mnqbtpas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lupkjrlp.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2xqewvkdv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2jwvgqvxu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2cptkqwoa.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2usrhzznm.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2avuiokdd.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2nyeqkdhv.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2mhrlawsi.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2gzybkrfy.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2rvtrrkzn.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2jewyiuzf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2dwbxhors.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2uvqldfbs.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2dbqjbsoq.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2hpdqdrym.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2nhorfbxs.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2xdubhref.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2kjrdhrpf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2gqjyjrdc.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2docchzio.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2afkmybhi.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2shhjjjqp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2dzmejbmd.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2iwgmzckv.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkyidpos.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2hedpvcrh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2qcjcghdt.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwhfowhj.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2mxntgale.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2fgtgpife.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2vwfrnsgk.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2txeqyxec.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2taeabwuu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2egnkotrb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2cjitqhcl.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2rczqzbsv.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hiselmmn.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2ohfrfmhb.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2umlshnhp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2ufmaimxr.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2mfyudsnn.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2xyijenvf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2mhhifoap.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2qlfygsjz.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2nqjaqjpp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2nlxlfgmu.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2lzvipyzt.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2iqjyzixo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2igicrqjq.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2jkwrjlvz.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2oyvveibe.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2zhedeqab.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2gtcsipqh.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2axxqdoxf.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2hccvdair.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uzqvmbkv.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2jqtuzucw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rabiidcj.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ezehxkea.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2wkgvcapv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2qhbsfeyi.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2fillpczn.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ojihilbt.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mopzmukb.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ovgklqqf.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2lrbsvaia.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2isuvjizn.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2hehwllic.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2uaeibdse.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2skkldijy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2xopvxdue.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2hfjckwgl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2igzixmmg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2tegyhnyh.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2rmqleffk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2tnlcimgd.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2mjwksfju.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2zukhpgpa.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2tyavzffo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sxutilze.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2olpoofce.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2woupdhhx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2nbndlmuj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2rdfnlzbr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2dnkztrhr.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2cipkxtet.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2qfuenhba.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fullawcj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2erxxlosa.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2cnaufccm.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ceuqztvs.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2ldfyulbq.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2apfrnmww.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2pyspfmce.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2euntjsii.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2rfyjvyyg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2ulzsjvxl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2xtxkjsfo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kpoonyus.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2hpvbzhhs.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2pojslduj.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2mrvrttls.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2bwnwafrm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2jupxwhsb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2przcyasg.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2uqtlpmue.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2lzcdpint.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jbqvjgmx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2jrskrxzh.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2xwghupiu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2phhimkfg.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2jyifhwxb.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2yooenufd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2kkkqcahr.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2xlnwpido.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2fbwfcxsc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2vqzkypqe.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xjaopxrl.html


<!-- 参考信息 -->