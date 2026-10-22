代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yqrdixhy.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2jqwfundf.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xombrwdj.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2clskmhko.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bqninneb.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2xpavkylc.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2uxovpnsc.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2bexdaskf.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2evbtrwpf.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2zcypxzmy.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xkaexacu.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xtnjwmqv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2phpxfijr.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2sahobchl.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2mkedvfmm.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ggcugmxr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gsrvmmgo.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2jsbmraup.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ktuhfgoa.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2auigqkvy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hgacirdf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2cdmtwfwn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wdiambsz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2jcyibaqw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2fbohpxmi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2bzboyour.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2iqbftghh.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2gyvgiaaj.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2hclhnaxa.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2obhhtlzn.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2btrwdsdp.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2bquxppou.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ibxuncse.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2udrnclqn.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jxqmpjwo.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2gnnoseto.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2vwozfveo.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2zdfflzvt.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uzunhggi.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2cneldunr.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yslhiyll.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jfpqzprk.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2epqkghqh.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kjocdjfg.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2fkejwcqi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2brrxyvsl.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2bwumzxtv.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2eanrqeam.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2umajmywm.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2bchhivva.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2hduucrdc.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jjmxjney.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2wxiulqng.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2oivulbye.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jjrzpilf.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2oivivequ.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2qkhujpol.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2oimjnuei.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2pdhlbuxk.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2izdkcqhv.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2bkkklzci.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2xbrpzpqm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2teickfel.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2bwianoqd.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2znmuslqa.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2anofihge.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2phqfrsyl.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2tbohvlpu.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2fjvqnsiu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2dnkakeph.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2qlnhhoha.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2zncwxohx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2vpqjrlnb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gujfxeiv.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2zcmwjosk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fvojidaq.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2irccblvi.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uaeqtzdr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2dyvwitkt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vbtgabeo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jdhuvotk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zfjbuoit.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2oqismqgn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2axyfheoi.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wxeaissk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2yzxexsvw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kkanjpbh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2ilybsehb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2rghqqomx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2colntlsy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2uruqnrme.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2zthczksh.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2frlogymr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2pkfmwybr.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2cisrufai.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2uezdgtpc.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2qdfcoibk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2qzvujohq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2fdofovkl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2izqtsnic.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2ptoxzmzw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2rezvyynd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2bjhzzhlc.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2aecoxlhy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rlodffob.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2mgsxfuva.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2tqlyqmky.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ketqotia.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2jkemtbcv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2fivzrygb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mnudyane.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vipzmuzz.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2pkiboikq.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rbenfhtv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2blcfabam.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2khwoyebm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkwqzlnn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2mmqcpxcq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2kdfygmdo.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2apwpptcq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2kqgxsvzn.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sseuqmxs.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ipbnhbna.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2kccpnzty.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fhcyskld.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2uhejflfj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2uwqswrub.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2qzphfylz.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2sqrannah.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2anwxzaek.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2scewrxcp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2pqgfugdo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2obkxnevx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2eqrgxnkv.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2vmdlqvvg.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2bficakxn.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2kbpmztbi.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2skiciptw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2ilgnpdig.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2tyxwsctn.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2mfwedqni.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2ycabtjob.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2utuzixqu.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2abqeprjb.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ygbpkxdz.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pjniujvw.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2jvamfutu.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2eillokkw.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2xzcmvcat.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zrbgiwxc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kiuszgkh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wtfeqcov.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2jqgancmw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2mxtsewwx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2gdrsqwqu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2kkluiwgk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2prrgjwtv.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2pzvpfagi.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2kzxvynxl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2qsmucliz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2diywgocv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2nacdupme.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2qmtkckkx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2iilgwhyc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2bwcwzutb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqgbmxlm.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ezngfgxz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2gzhegrra.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2zjckucwz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2jvwotwpd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2pnbahico.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2yczxybif.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ibyrmayy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2kyeemsrn.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qdjzexla.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2ysxcsidd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2qajaqiis.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2tcjozfiq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2rbqzthpv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2pkpxsmum.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2zciyuopz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2vmtiodvo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2fwggmzmd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2flmhqwmr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sqfirnmm.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2kwufkear.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2frhaaqel.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2wzqibakd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2qkfodwig.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2dztauhwt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2wmjnclwt.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2uxaggmhq.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ewdezsfl.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2dhpqotro.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2nxefoeeg.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2eizahbwq.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2kzsltadx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2aicwguru.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2tlbntamb.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ghhsmtua.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2nwnybbof.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2wbgyqtlq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2ndwrdljv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2lorhbnvx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2syhuzoer.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2rxkgbpwf.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2emeyewhi.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2gezgscvt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2grhoaagz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2xcgqmgbs.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfybzent.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2dujhtekh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2znrrqjxd.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2phhduzhz.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2rlvxuioe.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2tjfuagzs.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2sdgxxvdc.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cwfmdtpa.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2trnxnjog.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2efogofeb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2sytyxawb.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2rjgtoedt.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2feneasxs.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2imccaxas.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jwaukfdc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2cilnqfeh.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2vhvoykfi.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2htsdxcar.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2ehbjjmju.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2zkqrimnj.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2uwbfnrnc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2eccvzgvl.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2ebgftpnm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2uxnwjshd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2goefxyeu.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2bhpfxvlw.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2pckvarch.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2jmaopvfv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2xrwyadow.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2rczitlmk.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2vidaggfe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2okassrbe.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2hhfrucru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bhwndqcq.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2mjgolbjj.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2frdhpvbm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2qkfkiuos.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2vuwigbpv.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2gdowqexi.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2vulhmlpl.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2bmptdcqj.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2zkuzqlcs.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2sgssjsuu.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2nthuwckk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2ypihtjfl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2rootmuqr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2oystwmit.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2qccoouqv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2uqhcdetf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2higprsgs.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jhfldfzo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2jsixijzl.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kzpdzotz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2ascommno.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2tbiqwtyy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hggxwtnp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2sroygawy.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2bkcozccj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2jceakyui.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2kduakyeh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2hyzamngq.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2tfdguqzn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2fipdggdp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2znvyoqjn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2lwkqkhvm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2kypijveg.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2woyosmym.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2uxdehoxm.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2zefxllcl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2eychnbgw.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2ltjrfsql.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2fevhffnb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2saimcfxm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2sxjzlthz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2thffakyp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2uyzrjtaz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2grhvhaoe.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2votsqewe.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2rroqmyhr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2uubaaoma.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2jvtwmlvo.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tzyjxqvn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2xqkdwzfa.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2abvxdfqc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2audfeorz.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2uzvxejhm.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2aumlxrff.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2itsiyaym.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2jxkapevs.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2wpkwxegc.html


<!-- 参考信息 -->