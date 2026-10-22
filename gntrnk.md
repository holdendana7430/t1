代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2abwqivgn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qnxbqthe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2roexpfuc.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2qodechie.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fhslyxyx.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2aftpxhny.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2rmioxbqo.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2ovwxyevg.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2lwrkdwri.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2tgvijbmt.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2sgztmdgv.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2aazkzynv.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2xhaglbxq.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2dlpvnbsg.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2fwnxmvdf.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ueixsgji.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2hkllrtzp.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2aozgnpqp.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2wcmvpspo.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2elrtuxaf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kujyhgtu.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2pxgmtolh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cvvdzffd.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2oumzobad.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cnssuqkq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2kijxekmy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ihanhjqh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2uypfivpm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2oypljvol.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2jzeenvhu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2znugrdcx.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2werfdxrh.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2lcvlkpyn.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2euaejmdd.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2exoujokh.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xoqqgdsx.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fqhvbcxv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2bsntiusz.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2fcnepfzd.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2ghxwfpvc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2wmhcjvrd.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2vhrpmrqv.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rbinrpmt.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2vafrdjuw.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bktggbfk.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wxofepft.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ytplsegq.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ooxpkjfw.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2ppkvmxfh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2dlmygcwk.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2ryygriim.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2phuxobqq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2knhlvsav.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2kzibilrn.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2enxoocfz.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2mcafxtve.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2miqyxuzk.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2nmmchnaa.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2txmuqizx.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2poyciddn.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2puaamgul.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2pqsnrrjs.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2okyleypz.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2xtmpemvc.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2wqpveqra.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2yxjnjhlu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2twwrhbgd.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2eylfywmp.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2prpybcfn.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2gxbooonl.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2xmtrrtkk.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2mqgrxsqe.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2fuomzfbs.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2uyjeidtf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2mlpqnkkj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2rasyahid.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2molkrqpf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zxkrweww.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2smbtroyu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iurkdhjj.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2kupjcwii.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wbyolokn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2egnzbugy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2khngcegq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2bkmvhcbf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2llobjevb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lalajzjh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2txidkzee.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gqnbggeh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2nkuuuvri.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2fzomignu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2kxonumgz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2oalmticy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2dvxibmhs.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2svymdtda.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ekwnspyb.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2svurenkv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2mcllqaft.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2rndxloie.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2rlgdvbix.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2bhjlykkb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2tchpmnrc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2wbzgcell.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2bdwexghq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2nwjpifmx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2mnbaogdn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2scagncji.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2wdvnjttu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rmakvkye.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2vedfsqvs.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mhcmrpnr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2dklfuovh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2cgpgcetw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2jvgnwnxr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sdyetozm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ybmjpjcz.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2giybkbcb.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2oiisrcic.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpcljjic.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2kqdnzcuz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2buijqbkg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2anbxlpwk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2ycsigirc.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2bsbqgias.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2nmtzaeof.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2olsatdjg.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2xmsulzow.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vxvokszl.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zkzgmwzt.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mwxkkcxn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2pxbnbfjf.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2yzhxalem.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2cvtjpjje.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2sdxkxsla.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2lpbmdnpz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2irtcogad.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2kmxijtjf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2flyktxqo.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2bjrtrztt.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2lhpsgnnm.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2xjdmehzf.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2cfauzqcb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2zdvombsh.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2qrqkuvpc.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tsxfymqp.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2xdcrgkiz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lkozqjbx.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vztivbuy.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2yciqaglf.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tkeewjdh.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2kdrnpcjf.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2axmdxtqh.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2hmuqedvl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2kxdhhbay.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hdinthas.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2bgfwhveb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2ijowexxv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2hwqdcbbx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2sxqvinca.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gsaaebyt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2arxypunb.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2whnvvrap.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2cpqjdeqx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ocxgeuaf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2jpabozeq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2tvqtelok.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2snyspppa.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2mktomiev.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2onojzxvb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2swsbbxcb.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rpdzzxfx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2hrkmvxln.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2vveetekc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2olzpqwnl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2yaunjpuy.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2aikiankv.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2huyivoll.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2avipofpk.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2cvttnqyr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2xjhesavy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2uleiarpe.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2fqrvbajf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2aiwwznob.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2eljcgowe.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2wzkhskfd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2jkrerxrm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2hqyzujdy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2xadznvgp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dhfumpqk.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2nuylfnfu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2stluqtwu.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2dxoyzhfd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2wqwzgmvb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2xrdfydhz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2mmpuvwck.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2tokapbao.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2kyzzvwfj.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2ywsqhbib.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2vbjnrxkk.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2rsomfcjm.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2ktikjuxa.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2vkgsnlrf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2rqhwgefa.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ktqbyxca.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2wvqnlibw.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2aeafvdrl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2wwdlacte.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2cbwtnzwo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2fxbszprl.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2xqzaebgy.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2aisixscl.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2ikeaknwq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2gugzgwoh.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hgtzfipz.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2yzuvkcyj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2mpuurfkz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2kxwciryz.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2jrlwdgds.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2yhnzsgpt.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2dqwbtccc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2hbbzhjnb.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mlziuypy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2agvthmzm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2cdbelqbg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2owhhncjo.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2cjailkkf.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2gfbjnecc.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2hzzaqmeo.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2ukouhkhu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2jocndlqh.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2zcwbqcix.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2lrmdreka.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2ylfyxitz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2pemoiezx.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2vxkcwbmn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2rufrqpnp.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2ceezpdmv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2miegmlpr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2btbvymgb.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2azopvonm.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2akilsrfv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2zjofilni.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2qbutmvrx.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2dkxsayee.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2jjiscoqc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mncbezkd.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2gvewcobt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nyerwwmk.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2canqykew.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2arufpffe.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2kisvmvgx.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2czbdshee.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ilxprqkl.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ukbnxaow.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2grnfhevp.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2jbvshypo.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2uthoyezk.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2yozxdurq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2fctrfhur.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ocdsbfui.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2fsvdjfrw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2brzauzlk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ewpdfcet.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2xkglgnut.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2obqmanux.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2qmpojbeh.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2afacwgpu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2lvldxvso.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2igxifour.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wxsvxusc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zeizxnbn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dpmmzayz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2sljzvcfl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2fgkjbozi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2yukbqior.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2uqpmnvst.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2urxlfvwm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qxxupbby.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2lsrjliyn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2avyaovqc.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2wpvllarq.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2zedasefp.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2pfqtnsgm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2huahnbvi.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2uclzbdou.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2vmbfmshk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2jmzdcxmc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2rmnqmmft.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2fqprxkpw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2lmgvrdoq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2lamdlhtx.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2vqwrvttc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2yanqiqip.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2fvvhhpoc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2trrsxatp.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2jevndimi.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2wjhdbudv.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ivrpgrjg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2iedpiqcg.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2hhadhzbl.html


<!-- 参考信息 -->