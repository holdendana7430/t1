代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3smzbouiy.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3mvagdevb.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hxniisfe.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3nkuefpog.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3kpwuzykz.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3bswwmdot.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3gfdbpmnm.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3kqbbclaf.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3xlsxwvli.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3kvpeifcv.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3kdykcoik.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3mrmexuba.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3pxodxxpm.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3sfcobazy.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3epwfppty.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ckcsueuw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3nseeeevh.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3wiujcklk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xfhdzoif.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3ulugmsnn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3cjfebyft.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3epmfcbtu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3jznhsqyj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3hjwowkwb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3tsojkmqt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3jbjltorr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3clrgrybn.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3wfudnkis.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3sctwokmb.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3sxunaprc.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3tmkledny.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3luncfbmt.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3gqeqcbyk.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3clmvjkwt.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hvpdkbos.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3zjhetzgg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3hwuiaqem.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3msnhuixv.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dzgtbqqd.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3fohyocfc.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3atemsymr.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cxogvnob.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pbopnjyz.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mwtkiezn.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3wzgvelih.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3dtboxbbg.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3klwhsabe.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3hqubytqk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ujwbonsl.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lnkqztam.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wdchntmb.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lefbzwzn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3oemhqvab.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3yafwdbxl.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3iigvcoyt.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3hhqerrfv.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3qrgpzzmz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3dvrrjxgx.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3hixfmbeq.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3pgeuuggj.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3whrsvexe.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3qcnmeqxq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3kmjrkuzv.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3dszgmtpo.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3gtgevaqs.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3vkddgnit.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3jhusclwj.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3zgduoieb.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3tfwsjwec.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3fghutvbf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3rcaxtynx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3iyxdgoyb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3alewcwnk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pcsayljb.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3kkqmufbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3olodbgih.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3vmgzfdhm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wswtfztx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ybfdvack.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ctvlqoqr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3rzcyfghp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3souhgxzi.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3osrkwiqb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3reayncof.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3stsxaezo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3glfulnah.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3shprghqt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3imdyfgca.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3xbvpaucg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3jfadixpz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ezlszyem.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3msbwenvw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3lwjwkxno.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3tujijvhj.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3uplbvanp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3vroiwobt.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3cjsjqeac.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3rzadsdrb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3tlnzemzr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3mkrqibyj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3vuuqjwrq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ncgjssso.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3bymprulf.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3qwbdxiuz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nptmdnfm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3qgjgkxil.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kduxcgvq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qupemynj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3oyjyuuwg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3jmrbmzgz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3gpnanmza.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dhtbpxll.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3mapmvkue.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hypzwocm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnkszeuf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ryvmcqjn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3grhhjpsp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3xqztqvap.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3mnbquqlb.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3qrvjhqfz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3xvtsintt.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3pragkqpr.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3sifqlqjc.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gtsbuxnz.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mnlgxnnm.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wogpdutv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3snpnxoju.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3btemwiji.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3hvwpmkip.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3anjzfaiu.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3hpcawklx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3kbwyvupu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3xohkuiug.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3scvsyzej.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3zxickizw.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3wqlxpsup.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3xolftceo.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3elpgwbcb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3hdibsbbq.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3zhtmrcfa.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3upovfczn.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3suznvclz.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rhjxamzc.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3unofwxim.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nalcxbtv.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ixarbezi.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3nvofphir.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vvamwevq.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3kdxmfnxj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3rypblfvg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vmiwaktl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dvvdxgqf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3uiotujxl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3usqogrdo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3lnvmjplb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3exmnfaoy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3xmnamdvm.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3irmprbmb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3nabdbaqk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3slhlrerf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3nxtrvbqy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3dkvamrhl.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3tlewvhuu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3ifkffycf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3dhkwyvao.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3okwnknlp.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3kykukcby.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3qfhfnzsm.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3sljwkoap.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3iurlklmj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3lpvyimwp.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ishxvfin.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3pdccbhqj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3odgwizmr.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3pdwpcgvs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3ohqaadhi.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ddforaof.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3tvdtbkgz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3nawqfvwm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3fmzshpir.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3qwwzxcew.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3wxaivbbr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3douwifsk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ejbwyexz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xbocnfyr.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3zrrwhscd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fkbzpkko.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3qupacuqd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3opnvgfex.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3mwgsuybt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3cypsuaib.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3mppnhqfv.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3mmqgzsbx.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3jmxqkwvd.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3hrmqymhu.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3cinjrcno.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3cbtghjis.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3dklxrtjb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3jhaxsxmw.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3vpkfizde.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mfdeknpt.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3wsvctxav.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3usxpiatx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3aoqqfaby.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3sirfvwvb.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3eniphkxq.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3jaayjsua.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3ywiiubik.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3bpyrksqt.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3vqzfpnsa.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgiegmot.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3klohbbjp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3cimwgmyj.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3tbcwvboi.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3rgrckuzr.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3udeuzqen.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3wpytmeky.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ptiakuxw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vlislluz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3suixggpd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3xvmfmsli.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3dsnxoctw.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rhwghxpf.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3mpskqlqc.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3zhmotpml.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3vsecywkt.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ixuqgtoo.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3btivenli.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3ubmmrdav.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3tryyasob.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3keijcuvn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3wbwubgkr.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3svqxqtsf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3xswmfzma.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3heamyhzy.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3glfubzmu.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3wvjbgkgz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3uotmqkkh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3sqhcckgk.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3nosgvxnk.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3cjzixdol.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rytsmxzn.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3rarqaixb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uvvwslhq.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3axchpyas.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3wljhlyfb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3laszgggy.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3yzfggfcp.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3nusennsl.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gpfjjsje.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3wvoocawg.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3dxwgkxdh.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3rnrmknfz.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3geuvafia.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3yycqduhn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3anhrssen.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3vphogkjy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3wojmdiyz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3nwxumpdf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3sgosftlh.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qkondore.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3belgqipc.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mtlobjfe.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3rwdhagmh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3vpcaajlf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3xnsthhwy.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vykxqkbd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wvqpisqw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3vzjoicac.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3wzglvpnf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3yhccpwlt.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3nrktwspu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3xpwmnaso.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ofybielt.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3jqsrcaxo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ynlgeasc.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3petcidoa.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3xsylrndg.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3exywjdtn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3cytskxos.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3hwrbgzcm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3kcjlioan.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3zlwzvyiw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3pocemxuv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3smpcvptp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3jcvkfoyg.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3vcofxppc.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3pzalcfal.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3lnetmfmw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3hygmpzho.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3feuktjjj.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mvjoaxqz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3xuxurwat.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3jagzxauk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3cltzyngv.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3xzmiudji.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3qcyckjqm.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3tghhqtuo.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3xiulhxui.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3cgcvlepo.html


<!-- 参考信息 -->