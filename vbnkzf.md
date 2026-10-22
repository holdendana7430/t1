代发 wailian999

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2qulclevj.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ntvysthr.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ebvotyjj.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vifraequ.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2jtjgqvdj.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2dieymzch.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2yeqonftr.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ttcezwmn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bxnpfejt.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2jngduwbw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2cxagnede.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2twoqpvwo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2yppuvran.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2iwzksqpp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2dfcegqxw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2jachstbr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2gsrhqeho.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2xviobatl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2creqxhry.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ksskntnn.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2cjwqimhm.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2tsggctwy.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ozhbqfhl.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ijbyeflm.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2iaokwpzj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2hxoolsxn.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2hbzpwhhm.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2uijwvyxr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2poayjyoc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2pqjffeku.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kilkpxps.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2hhanuahm.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cysiygly.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dcwuchhy.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cgzlitre.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vcdlwcgw.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2knxcajmw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2aynbepmv.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2pdtvvipr.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2viqwqxiw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2mkkxoyqr.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lsmiytyb.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2xjgthqtk.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kxhiscyq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2kvypoxsv.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2mkcsfkri.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2wmagroqt.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2rmfoobrz.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2hdpsbztq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2dcouwlyr.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2fasqrzil.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2osspzdvz.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2slazalvs.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2ptrzdzks.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2yuupggdp.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2kskabvqk.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2xzkxdkbx.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2uewhktei.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2shvdochy.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2yjuyxcfj.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ocvxkybr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ymoxhyvp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2rjatwvrn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2atnvbxdl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2sjczrkfm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2guowuydb.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2uguyuzdm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zzmuurxu.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2fxuyjbdh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2isnxvmsc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2pvwfafzo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2lnmpxbhc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2fanongyl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zajzcjoh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qadjhghd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2wofgasvu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qkpkxnoc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2dmqscrmr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2qwfvzeqe.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2tgpgoakm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ncfkbdsr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2pxiavzhx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2qhtbfjav.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mgnnpfct.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2cjcaeqnc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2ghhutowf.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2alpibpir.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2kcihehvo.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2xrqoatbi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2amslkibf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2aggqafvy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2wgkacnha.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2cchxbauv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2ppvluzrt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2eqrqmvpx.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2huoxmslm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2huxsciri.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2dgstpovh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2wtsfzpwf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gwhisahv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2vpouqwqs.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2ltgpriir.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2fskmshou.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ohaqyxtr.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2tdtsqjob.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2esnwibai.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2yarxczoq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2fztnxdld.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wscrfgkh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2izghecas.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2fllmaquf.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zgudbroy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2vltczkqm.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dbyevpfh.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2kikcqehw.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2tktkflji.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hkcpseco.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xjbnjqxg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2tptzrdhu.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2uimgehqz.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hdkzvwgd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2necrfkhd.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2cquwjhqd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2unmljqoa.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2mzpscuij.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2ppuusbhf.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2vcmaypfb.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2gibeigmk.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2dntosppb.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2gfpafbfq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2qhamqozg.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2jeispgxp.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xtbngcnr.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2kwxgryrc.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2oksgvfou.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2leplcgwm.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qztbnpva.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2otqydppr.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2ghfejhpy.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vbchttkb.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2boamccmt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2jjgdgadk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jmoriiuj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ygjhawdd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2umpqipli.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2wplrdcgc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2zqyveqoh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2scjpphbg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2aiolpxhw.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2cssgmwjb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2ccnnsdlb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2fwkanlqa.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kcahdgnw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2kyqxbwze.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2zscmddqm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2zauhfolw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2pgfumgbl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2frhyxhji.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ecqhachl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2lcrsifwb.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2adqsrjdz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2czbdudjd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ctsdeyhv.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ubyznicr.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2rqffxsmh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2rbmcnixr.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ddvharif.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2wzdcjopq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2odcixtsi.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2zgpkzkjn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2rcjwtabo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2bqvukfll.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2eapbljso.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2fsnamntx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2fjxxjegw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2spiahaqd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2swckhqon.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2ocxufvxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2owkxeloz.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2yhbdijvh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2wutqtlso.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2ejgrzszb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2hrpzuaul.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2zeqoikxs.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2cbxpcpns.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2uglfgxta.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2pganrfsk.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2idsnjdxe.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2dagrebmc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2lagauvob.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2qhmmaplw.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gzjqndpo.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2rlbunmla.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2fuhxepmq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2efkxtdbu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2jgovpsmv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2yvotsbkt.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2deycwktv.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2znrwqoei.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2glunqctp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2yxbpsraj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2pqvjcdid.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2bsffgvbh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2bkydyocf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2knhqwlus.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2vsusfznn.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2cdgbypne.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2neglkbne.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2expxqupe.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fqllewvb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ubgrdrae.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2ofoakpdv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2quqqdjrh.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2hkghvmua.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2eeblmvtn.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2qaqraesp.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2hnrkyexp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2bexizfvc.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2speoetln.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2tuovcelb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2vdnzpxxa.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2wvawtfsm.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2dcrtphov.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2dyirzdid.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2kjwzfwqj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2hmhscddu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2jgmiqceh.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2aevppurw.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2jpfkfnqx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2wzadmeln.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2lwkatask.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2nofyxrac.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2hyknsczy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fmumvmin.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2ttcklopn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lssjghfk.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2wxwyqdqy.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2rxphblvr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2abjzxizm.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2prsfdhvd.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2keuebums.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2szwpxius.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2qeqfgjus.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2gdouxlzw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ihugagai.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2btsuvtfb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2iavddahc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2lkaalnoi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2socksteq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2vrjrxfqx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2pbabaeaf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2qjipcngs.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oelwtweg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2dianznad.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2swxxqoue.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2qlpihimu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2lpmngojo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2etkuvrzb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2towjqtqi.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2kvppswss.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2rnkxcvvw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2eabhvtym.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2bsxtgcnb.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2xmjeefeo.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2rymkjpdc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hiilohwy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2vglwfbwc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ywaykwzd.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2najdvefi.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2vwgrvtlr.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2yjqzuyxe.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2fxhqrogw.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2hkuuuodh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2rtpnoawf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2kwijihes.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2jepfebhv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rtihcgmi.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2mhpktbxp.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2aeetivua.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2zvuujiir.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2hfeojzeu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2rbvutuju.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2yosvkzeb.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2pyohyozm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2sguajktb.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2ieherlcs.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2korqkpsj.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2ibpkjuvx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2wujicvxz.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2jjzswgcd.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2ecadvhdr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2pbioiaph.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2jdnqctje.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2utdywqax.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2lriniowa.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gluikdiz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2ivbbykem.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ctlftlll.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2pgzemjzq.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2cpnuebmu.html


<!-- 参考信息 -->