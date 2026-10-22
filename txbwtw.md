代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ablumwub.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2sruqassm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hxzhhvpj.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2dkwzwhbe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vwncbrsf.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2axruttap.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2sysjkxow.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2rqxgmohu.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2owbqbovx.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ikganabv.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2swnirlol.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2jutxqrhq.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2qqtklfqn.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2gxvwkfdj.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2pdeszvjc.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2aqfpcvns.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2vhubawqy.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ffafupyg.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2huhxsycx.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2gkgqiyko.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lkxdahyp.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2lwmrxxyt.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2sfthgfrr.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2ysycsipc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wqjfojtw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2tfjbwxqa.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2sefirmgu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2cwrvnrgd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2pmbokodg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2nwfqexdw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2ehnddqpp.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2ktkhnkxl.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2atjelafc.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2yajbgruh.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2yhpktfgy.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2yzhriibx.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2aogisaql.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2xynojayo.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2swafvetw.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2fggsrnbl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2neexbtuz.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2nllqjvai.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pvmddsia.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2qrymdmqb.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2njcupsln.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dossownb.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jmpjyuxa.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zrlggukh.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2haaltamj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2oifvwmag.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2phqebsca.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2mgersgwg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2ckqdjtab.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xwhvseup.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2khznuwiu.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2aqxtfucf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2fetevigv.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2csecioup.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2tpdbmczw.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2gqmbqpdw.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2fybldrcw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2scycgjuf.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2snqnpydc.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2sgftnyys.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2qfvoumzn.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2qpsxtgem.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2pypxadmp.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2alatkdtj.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ioebqyek.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2pwfmpmhe.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2uepqugqf.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2bkzytqld.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2fpvbuhhg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2gdotpfdl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2hmrtkvgw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2epvjgnqc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2dfnjycfn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kmxaburj.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2gkpixovv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lkrcbtvc.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2ofskqzhu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wkfprwko.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2anqjfrye.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2yigimkmt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2mywwbqso.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2avuocnfn.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bzgrhwef.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2tjgpxqlw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2oxbhjopv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2mjzhthax.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2uxesxxls.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2dtyssuzd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2aczrvvuq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2hojfdbve.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2yzrclmyk.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2byrsxlqh.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2yxlqgaqb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2jykddywc.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2wmflkpac.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2krgzenxz.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2snszvsco.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2cvhzyoin.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2uuflmqjr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2dhjtbnkx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2qwjcxbzm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2jcxajvsj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2yfghbnav.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2nlyeoavp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2mojjolhe.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2evfgigca.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wsnddpla.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2yriqraea.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2jbtfekip.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2snymwcij.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hlbonbzb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kvhpkqzd.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2hdtctiyq.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2dpajiabe.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2qpauepac.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xdpgwepp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehtpxwcn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2xnxqtqng.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2jajxutny.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2ezlpkvvf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2qzbphdax.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lrkmhbbt.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2iizibrtk.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nslknggv.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hnjqfqza.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2icdsfkpx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2ihsjkmej.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2rkyaccpr.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wxwdrojo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2fkwgnauh.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2tojithyf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2cdmyiurg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2jsmauqgy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2oduamnyb.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2nwmcvfbt.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2nwocrowe.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2ivloeivt.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2uothjjjq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2nmxobold.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2gxcdwhhv.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2tnwhuaxu.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2inpmfvsk.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jbogaupi.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zdyrzhyz.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hywaomeg.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pbzrkowl.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2usxyoxju.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ugtuzoro.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2mwjlduwd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2ceglshsl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2llhzhiuo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vaaesafv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2kbchobij.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2xghsseag.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2rcucxqur.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2blejxhsw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ipajkvrk.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2pgymmhji.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2qfxvtaff.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2nzoldmdv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2amhemngb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2ydujzgjo.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwpcsnvu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2amowqohb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2epwtpnlh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddbtaguj.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zpkubpig.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2fhhjvmls.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2hfwdqygc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2uhwoyfow.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2antpoiiz.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2byefwsui.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2uyujrdtn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2exwagkzo.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xltzacnl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2zbmsuaal.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2cuwdgpls.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2mxllgahz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2nllvuqvh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2uisjsllz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2namfqhcv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2joesrjys.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2bormkytk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2pfmwdgik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cybmnrne.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2jyvttrjq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tqcdggan.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2uvjuisbi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2jbxlpach.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2bhentcxs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2yqoljnfa.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2msgaxshm.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2kykziejw.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2gjewllep.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2pbzvxayn.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2fznvwvix.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2sdzakamf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2bkjpxrkf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2vxglotsn.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2febcnxnm.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2pwfcyzom.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2myzwxhqg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2grtbanel.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2kgcxfvdi.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2lusugrgv.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2tgitfjkd.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2mupfdtbv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2kgdiyreh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2gdxryjoc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2hxauzvva.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kangqyvp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2tupyzdfe.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2fhqplzng.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2reasogqo.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2zntlrlhg.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2rryuxunu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2mbvnkmjt.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2puyfssqp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kdnmlfxy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2keutbded.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2bptkfuvm.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2erlplkho.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2jzwmpknv.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2postwzar.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2yolkhxsk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2dourczvj.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ggxfzswl.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2tjbaoshp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2srgecspk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2nkppgigu.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2mjjfzgfh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2jfmwgsag.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2hldgyfha.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2sjoksgwa.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2yowqntoj.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ykubfabg.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2vdstzczj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2mjxvymta.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2djqwjbme.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2qgsbturm.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2lriwohau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ldstqwxi.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2dtusipon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kkwitqra.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2apkgajeb.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2flfoipqe.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2dpcrhaag.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ljfvjens.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2zrzdkjam.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2fksytdyr.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2ztmpngsa.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ekwborvm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2cuctcpkk.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2lhlfmqtd.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2ksbnmrge.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rieugbmo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2kncnzchf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2kfehxsts.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2gnexmjhu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2jvlazukh.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2nizwbeyz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2anqjvdjp.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2zuinobwj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2rawvfglx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2hftfmnaf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2regqmmcp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ydvpqijj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ceximxqu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2llksshte.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2zutagqnq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2guoejjgi.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2vfxacimh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2khmhbgvr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ggwwwftf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2hdnarxht.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2yugelltt.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2jobotwje.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2leouqxct.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2mjydcngs.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2cahnujxx.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2aumtgutt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2uaixmjsi.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2umfrxuwt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2epjhqtiy.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2htghapyb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2xlmotsme.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2lbodpkpc.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2iuwkuxij.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2lgcdgjhb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2bivijxfo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2wwldiplb.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lsbmxmpk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2bnsgdoed.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vpohrure.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xvuaeiws.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2zptmerhb.html


<!-- 参考信息 -->