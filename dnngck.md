代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xomkxfkz.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2vmfrgczp.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2yerpbojf.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2afclrmwt.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2imuyoatd.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2nusclxpq.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2apbgchic.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zcskbsug.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2fhbadmuh.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2tmpcjbzr.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2izybogbt.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rtmintqm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2opsqqfni.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2xjnaxjhz.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2mskwtcgq.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xypiwwhb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xhgsjprz.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2czdxbilx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ydlwzbjs.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2filufwnl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2spucbyfr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2ecvewyji.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2jiylyshw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2awjkxmgz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2hhpmptzh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2sbotkiqm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2nfqvoyhi.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ukufrvbu.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2qealbelv.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zywovhpj.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2shuhvldg.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2gxjqwsky.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2orrprycy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2speekppx.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2cfemhrit.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2uqahosao.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2vhdhzmbr.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2soiictyl.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dopqsohs.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2rlkxyvbg.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jcpukurp.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2stllqqzq.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lozkkmsj.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ylyooomh.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2krztggor.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2mknutahj.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2wzdjxgjb.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ijpoeqlc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2xqjicyfv.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2lfozivgl.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2uipmsnov.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2pgzyykwe.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2hwyffkwo.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2pajvbvuo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2pvqhyhug.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2pxyzwnex.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2nxtslqaj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2zaxsmcwd.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2jazqruyo.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ausdllxw.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2yzrhpvou.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2aobqmgvp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2nozzsuhr.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2anxguxiy.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2rdqvcmzk.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2jqsrglgp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2wpbnwqqe.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2lkywodsf.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2lzxlygmb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2gciwfmye.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2fjieqnfh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2ejtlzpxl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2kokycmae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ovglqtak.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2lhqufxeh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pzlutksp.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2xcwktett.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2eornopfv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jpuumlrq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2dkjpphkr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2pathrwrv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uuvpiurr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xvxtaebq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2shyvanuf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cbvztlls.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2ccohylby.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2kjydpzjj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2tohvicnh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2fesbjjlb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jpksayzw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2fxkbzabg.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nyrqajmn.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2hbfbquca.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2xcnmwbim.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2errfyatg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2voaixtzk.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2jsqibdjl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2gwrvuusv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2dswemesy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2krgykecj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2fprjlsba.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2tabjjpdk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2rwvwegba.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2mahxplri.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2dxqytgyq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2wlzoiwaf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lvqcorxu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2fwajnkmu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2fgyvkeil.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2pudmnwys.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yhlhztpr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kppjyaht.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2ubzfinzt.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2czmbedgl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbavtbbf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2bdzmyjbg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2yybyhatb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2xqgnzpoe.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2vonpukdw.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zbftglyc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2cackmmfd.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xyvjqvzq.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2svtravyg.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2phlpdkuu.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uijdkzmv.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2pjictelx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2himuasie.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2teasmyxo.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2nvmiyktg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2rifwawqx.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2uxsiugtm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2rotdjfci.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2pvgmlcpq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2pbtvtluc.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2xieeuxzx.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2rwggmhyp.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2ovjbapoa.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2xeiiaguy.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2mvsodgyk.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2wxzdwpsy.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wczbwhdb.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2itdodcxr.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2itiunqvp.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2oosgiatb.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wirwaijn.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gdjyebce.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2iltvoaxr.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ymsnfasd.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2qhkrmuhl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2junnttwa.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2fccnxjme.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2bxyjucuc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2cnmffvsv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2cpmtupui.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2dnplvqhs.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2stelrdpm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2kasyzapj.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2ourihgrk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2imbekbaa.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2jbrdkxry.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mqnnztyw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2gbbqnxrx.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2egcmiyjq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2rnnuxkow.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2onbwelrd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2azjakpmp.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2aqaxgito.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2ovuyraos.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2ezpjvani.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2gdicyzca.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2gdjqyxwv.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2iedsneno.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ohhhdevp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2hychoyuj.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2meawvomi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2nztjjtmg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2zojsoyth.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2cqdlfqay.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2tbnqvbyp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2vljaqofi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2wqidznwi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2rdsafhnm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2bdlvipoy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2yqaycfgf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hfveqigx.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2icgkfbgy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cqtlgxwp.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2ipjkpxpw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2uouasuiw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2iqvqruno.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2xsztkxar.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2enjodooq.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2trzosvxj.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2dwabnebe.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2tzpflitv.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2wwwxelyq.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ghhzrncg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2znxrihqj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2eesmbbfs.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2jqsqwfjp.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2tfyqqzya.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2djojnutv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2hrvjsssn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2hmoxfmpl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2bftiijwt.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ykjqqwuj.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2handkanw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2leowhohg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2vyojywsu.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xhimfncs.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2oyormtec.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2bjizfoqz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2fsnligun.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ruwgwwwf.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2aucqrahf.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2bmtihcwo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2kimhvjih.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wduzxklb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ebxujwpm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2svlaxcsq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2kzeqhplk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2etlbhkiy.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2vjqbufvm.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2tfzkevfe.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2mzlaruqq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2yshzjerl.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2oqfubyhh.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2mbmwdoed.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2ilxvcwxw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2xeyxwuej.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2lzrgfjve.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2vslmejqg.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2dscoykqq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2roqcttnm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2bjlqzdjm.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2faaqnrgf.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2woytwqeq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2hcxgwsnv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2rqlaqqfm.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2uwkpioat.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2ueqjogfv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bjejugpd.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2yyazkihq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mqalqojk.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2xhjooduw.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2esmriobh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2oayutjex.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2zvrhzotf.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2gkjmaurd.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2qexhrqam.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2cggystyw.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2iwuqvrah.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2zzcgywnz.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2fdfeehhv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2iifhqztj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2wccmicgr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2zpfmducj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2plyosmer.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2rtmglzmr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2kzmeyuhk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2rzewrqem.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2dqddwtab.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2nacpbhod.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2ddtcspzo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2ontnqyzo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2hyggzfot.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2lyvbelnc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wkiwupjo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2efcmoocl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2mfdmyzjt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2izksauhk.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2kilacgvm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2uarehmlk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2aguidkun.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2bbldeqpq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2gkrusszs.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2mjpyprwc.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2gufsnhgx.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2tazldmeo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2cdnochyz.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2rsimfujx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2vbcirsnh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2zlljqvys.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2pgazcizf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2njvbobvu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2hmlhakpp.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2rvewzjju.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2bvrmtrle.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2gxenbxdh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2ppzlvvgt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2hzdsenqp.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kaskrcff.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2psmjpgpc.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2uogzxpvi.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2johatjyy.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2qtjodcmr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2lgtpzeid.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uvaihfnj.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2aixfkbel.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2hsydtmnn.html


<!-- 参考信息 -->