代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gvvlqafv.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3qboksict.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3nnyhqvtv.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3gjhtyict.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ffonbfsu.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3tkekykhg.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3qhvfyukz.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3gdqvwaaz.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3izbdyyqc.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ifgamlkb.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3nmsehjuf.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ivflynpp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3yupkbpbx.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3opdofnbw.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3cjkfgumm.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kdmhsrlv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hkmjjlzg.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3agsprldw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3yaharqht.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3qaonsoxn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3juxkebwf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3envhltwp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mbpvdzrq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3oxyxohgy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ambeadkq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3paontboe.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3svcdmcne.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3nsaumvaw.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3hgqqrxxa.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3uwafucad.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3hjwtvwxi.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3udzqagcf.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rudlgwit.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3rmhuggwn.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rlzcambq.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3nefghapg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3pfywbhfg.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3cazudruq.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bpfwkfmf.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3yawmplmg.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ooxhcwhd.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xztrpqov.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eleuhsgj.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vnhmxnek.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3ztfxlmgh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3luyeuctu.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3gxcdrtsl.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3aimxymwo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3dclflssc.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3jhpzqzye.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3nltfqceh.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3lgxqrtmz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3nslthofp.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3dwerupwt.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3vsmrqhwq.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3toojnrzh.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ducjjvgz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3vduafetr.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3nvpdqwki.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3aeajavil.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3xtunxrat.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3oidkkhgd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3vtqvijcu.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3wtsafkeh.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3lxpfgftk.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3nkvtabnr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3lzrefrpx.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3xmbukvbi.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3eygdpjbq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3janjeluz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3fbsfanvw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3ikcpwjmx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3jgxtaxyr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3imetqatd.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3lphhbpwq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nwvcgngz.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3wptusclo.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ncwwldsh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3kkmbizek.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xczyszsh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jkfrwgac.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mcsauieu.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lojklwnu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3atbglzhf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nedopgqu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3rlnqgtjr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3hcbsfpry.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3rwlmhckq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3miozzmat.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3khqmnyhy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3lxdfhmed.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ngpneqmw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zowellez.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3kyuxhdix.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3lnyurbuq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3mwnnnofw.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3dmwzixhl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3llceubvg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3uxoaxlkc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3xusglrqd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3nkgsghrx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3vmuzouqo.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3fghnpnkl.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3bdxgktwn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3thadvqvk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3lznkgcnd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3afcrunsc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3olgkyjuu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3tmfrzrxn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3gqygjrxr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3chcaqeaj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fnfnctrs.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3mdfgwbpk.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3pkfrwjci.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3lgbhvyls.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3bcglmpqs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3vgwcwseu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3zqfdadgq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3kbepyzru.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3udbjyota.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3lgpvqmwy.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3bejxzemt.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3jekxtvfj.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3cdloknat.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gcrgngus.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lykafezz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3mwqlsnhc.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3aqiwhqra.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xgaqjzex.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3cbwpxtmj.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3dbalwaks.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3rkfrlcpd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3umtzuwrl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3mknsfjse.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3fhqisvwm.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3cxunvlhp.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3wtyobafc.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3blpenzus.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3ewteowez.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3ggevkqim.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3cpnofzzq.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3yiezwxjw.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tdicahot.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mrwhhqjf.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3uzgcngzc.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pmexnpui.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ixxmedbk.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3etcupneh.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3gxglsfzu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fkxihetv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3woxwgzsg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fyecjjnc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3abqjdgwt.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3hqzeakjs.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3wmuehrue.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3smqmfoae.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3xboafwaq.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3ftnpqvtr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3foughodl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3galgfhsn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tnqjzjtr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3ygqsmcdr.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqqfqurg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3zlcodxyf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3yvcfdrvh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukfwaxyw.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3qiwfamuk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3dwwrjnub.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3lljdfisz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3xhtcrqhz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3pvglqmpo.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3rpgzmvmm.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3zjsazrve.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3yqnvhuag.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3qvyktadd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3kkbouhki.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3iqfnbrpc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3wnvfnbzr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3pkjqlips.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3kpdljfdt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3osxkysdq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3zyourfkq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3wkxfnnlv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3wkxypvro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3emctuxgs.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3zkhbrqxs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ejuffvdw.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3irnmdgqa.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3xgssxwgt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3bgnlupik.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3errthdlc.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3tfthbbol.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3srtuaszn.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3uctrestt.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3pkcxwuim.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3rplwkgnd.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3bteyyrlq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3jhizfzbr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3znitbcdr.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3hnbyzymq.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3pcztsvyy.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3sfpyajjx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3nljdwktp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3dechzjwz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3jnqutxhh.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3ifjsdwlx.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3jlsifbtg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3whjslcbo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3hmrbqjxt.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ycidrjgx.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3mdmhhbkw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3lmcjyvcz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3xxhnikxk.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fownykim.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3ddptfdyc.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3prcrkoip.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3jxmojgqu.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qighgtqa.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3bdcvzhno.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3diurhldc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3lvukjhxa.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3dnsnzpry.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3nbwsslwp.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3pdsbxdow.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3xygvnuiv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3iacmpoif.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3nmpqyaeu.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ilygssru.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3nobwlycq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3yknyyfbs.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3rkfuimmu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3xjjkvikd.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ophgegjq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3htzuhxky.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3agnjgpbh.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3hzwbbrok.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3kzbjnoyq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3jlbwsfnc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3aztniatx.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3qtkuzcjk.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3frefjurc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sktdupnk.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3mmzkhqtr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jkntkora.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3vzmmdbcd.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3fzkozqwd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3fjujnjgo.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3hoiedcdf.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3fkxwhtwm.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3umvtxgxe.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3jblntlgp.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3smjocgfg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3xlxahfll.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3kxyicrdy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3ihhjkbnx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3luahevzy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3cwvvijda.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3cmlrgabi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3sclcfgiq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3kxedjigr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3egaqzrqm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3gpperdjo.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yyvnvtsi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3zqhlukps.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3kymzleqo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mlhmsirr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3wvcyzvsn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3tqpmpjkt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3msybucoe.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3iloxtwqb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3pbbtqztj.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3rgcpulna.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3bcyyauyz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3uxjlocbo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3uldyssdw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3aqcnjbbu.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3liousfxf.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3tagewplh.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3dicjnmot.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3kisexuon.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3hfgjrmtw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3nohzuctr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3mkmnjdkv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3ubfzrljf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3zwntbuxz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3gldbwwjm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3luyxtaxe.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3npdgkmfv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3whzyront.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3wrgqgclw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3qnntpzvw.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3wdccwmhx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3xpbynuxp.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3hzysqjfy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rnoqbexi.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3qlfcszrp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3agresvyu.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hclqfznq.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3jrcuncgt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3koarcdmn.html


<!-- 参考信息 -->