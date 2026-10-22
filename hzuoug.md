代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2rizkxciq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2fevzukzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ibkhliaq.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2eubloset.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zkyttoys.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2tvonnwaz.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2txpodupk.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2xuiuxrup.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2gktwayby.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qxgboavk.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2bxifqskg.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2gdjimodu.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2hbnboihz.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2nixslmaq.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2bdsremnh.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2npubjssm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2iplckgwy.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ozqgqiyv.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ndjspydo.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wynbawep.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zyhlcktr.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2cwvbwevj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jdroiddv.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2fgwdcmtq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2mjlnvewj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2nuvbaimc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2rgzzlrxf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2zpdvnhmf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2xwewayai.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2wuowlfxw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2xpwrnrpj.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2lllcbmna.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2cgnzltsc.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2savdcbhz.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2lbqjtvip.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2vqcpfizl.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2yvdgktab.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2yovdrirs.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vmkiljto.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2jxidugpx.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2yuyllryv.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ntfagmtg.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zrytscpt.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2maxewxrp.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kxrxnvzq.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2avabvvji.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2evagttdv.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ntbzacmt.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2lzovcpga.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2npamjjar.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2uxhqbdvr.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2tqvrpjyx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2bckvnjmi.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rmlawyou.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2sgtzresy.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2rnbrlonk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2ntogwrcq.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2irtvwdxo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2xvfyprbv.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2kxhqfosa.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2wiwrcysi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2gwmnahug.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2wwoiuusi.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2wodnuiod.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2lswbvvck.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2tuzbftph.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2ftupyvgj.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2panwcqwx.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2puzuwxjv.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2xroajxdt.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2ueewhwda.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2jrsboeol.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2savudstl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2pmuzjrkk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2rcchtmwe.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2nkmzseji.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2ukpshwgd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sgzlfeqd.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2dhnnypjo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dztrltpt.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2oiibnoov.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cvrinphm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2pzfkbqcj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ddxduhvl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2kqhgvija.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qtlmbixc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jywreygl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2mrtmyvso.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wnbpcpsf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2xfnzzyyy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2barkhrex.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2wjeqqcug.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2xsaddctm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2idmknkeq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2pojqumeg.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2jjgakizh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2wdcfcapt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2exbbmbnr.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2azebznua.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2krspeclv.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2kauiafzt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2amuhbyzi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2pxgztwki.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2phnjytsz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2jvzempfm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2rljgohga.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2mekyrfll.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2pvcxqhol.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2goycbmen.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2lgttvlho.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yxnxeqvw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2idoetdzg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ycscawcy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2vpeezkmz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2biokpgic.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zlmnymvc.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2bhuywoak.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2azbimhsj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfwrigjg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztqvmhyc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ponvgoge.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2jexuqkdg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2jszrxpcb.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2zyehoagi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2puvptuvh.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xazaxjnz.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2lhpgrftt.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2shvdduqa.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tgwfiuvd.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bzscmgaw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2hjipcdvl.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2uanjavjq.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2vjbxfvad.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ragkoatm.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2jcwkvxsa.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2qaruclyf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2nunxyrdp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2rznotxlh.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2hztvenly.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2dcptqtsd.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2ufezrzxg.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2jszkcdnb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2rumqbbgs.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2aposbcvw.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2idaanwua.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2phedxibm.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jakdqjzu.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kfabcqns.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wonlrxow.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ptglfwfd.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2tdpqkddl.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2skklsgvi.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2jelzcpqi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xbvukdep.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rgqglpja.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2snezzuzr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2kzlhqgsn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2aeabtxgy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2xgemnqqo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2luucmxnz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2kskviptc.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2gvhocipu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2fgzuxvzm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2quapgsen.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2adwqqkhy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2utwdmsuh.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndjaztnq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2kypgyciw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2iiuidyyt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ieqqtgti.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tghdduse.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2rdncbqzv.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2gcermeul.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2qojlsojx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ihjqrwxv.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2oxnnikig.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2mrkcofiy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2bnkawnzh.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2txwauzmj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2ehqpxcyb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2okrgmvdr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2lmjdmjjg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2pwltijen.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2unecgzhs.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2mnzftscs.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2rlzfpyfk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2mjdyrnow.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2gzuxynix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jqryfhxr.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2iiessuyu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nktoomar.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2bepbvswl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2wudacdfe.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2wpxycokm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2gxrxqvtc.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2wcapwcwt.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2dcmjtujw.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2ucfurrlo.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2vujyofie.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2mirmqokq.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2vteqvfnd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2veacdkxe.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2szunseeb.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2lkpqjzxv.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2impoiggi.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2zeurlyfl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2fxvtnzac.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2brcaboht.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2voxgvtaf.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2thfnfecs.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2fdjnnfdb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2odoiyyio.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2adwuwlmt.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2afkrbqxw.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jypxhfcc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2maqfkyxz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2sskziqva.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2jcxvwvdp.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2oljvhfri.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2suxwsjnw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2bhapszsc.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lauqqtzp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qffieuwz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2vxbxsoun.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2qpjeviax.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2khxzcvhp.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2hjlaljge.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2zqusreyk.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2aifipknz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2btkjarfl.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2psnidbxz.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2kbchvtxv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2ekiiotqx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2lrtyqyre.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2teqnmkib.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2dovjjckq.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2njyhrdep.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2nlijmqna.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2vucyoezp.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2mddmyupd.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2jauaajtv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2zcnzssbg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2mevdfgao.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2rduwwotz.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2tbchvncs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2itaqcxuj.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2bdelkxzq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kdwcoqnt.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2sdhxsbni.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2muwupmro.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2stmcxsxi.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ikqjjspd.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2qyicwdwt.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2wdijoaau.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2kcjyvgfr.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2cqedfwxs.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2jxpmhtpn.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2mrsnijpu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2rgxuzmgd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ougpwqmi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2meiechvn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2uuacicqa.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2bgkmnjev.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2ztmyjjii.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2lblfgwzz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2ayqiapmz.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2rxluadpa.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2ffsodoke.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2zepvdwpt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2fxdxduzl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2fubvovwf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ysjpxhrx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2mydhehwv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2cbhjagga.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2rcavbzbp.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2bejrfihh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2stdragyv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hxxjtyim.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2jeovkbxh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2zlrgxcdt.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ojkiuofw.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2jhkgcbcb.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2jrvauimm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2upreutag.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2tqzosubp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2zaeiourb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2gluyjcns.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2ldhpnjrf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2friqzkci.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2rypzniaz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2bdzluytj.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2nfzkbgjz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2fwuarayc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2xzxbahon.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2splydbnu.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uqvemdmy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2fmhqahej.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2orikxumr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2smvrcqpi.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2ydoucbnh.html


<!-- 参考信息 -->