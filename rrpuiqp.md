代发 wailian999

================================================================================
来源：http://wap.fehbvm.com/Article/details/grjqdhdot.sHtML

[M01] 读取命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gmeuaunkd.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/gnlyndeuv.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/gnvgchsxo.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gviffvesr.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gpipodkif.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gcfhaaajv.sHtML

Go:   os.Args[1:]
来源：http://3g.fehbvm.com/Article/details/gwavsplup.sHtML

Ruby: ARGV
来源：http://wap.zdbjq.cn/Article/details/gbxezpizo.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gdlvesndi.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/gvezhdvoj.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.zdbjq.cn/Article/details/gvgayrbav.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gzsxbkybp.sHtML

JS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gatwfurqj.sHtML

TS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gpbswhmng.sHtML

Java: System.getenv("HOME")
来源：http://blog.hesvh.cn/Article/details/gvqljqvkx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.hesvh.cn/Article/details/gflisigav.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/ghgxgsafv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gdfjekebc.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/gsjbycmeg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/ggowsusxe.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fehbvm.com/Article/details/gijagkbqb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gqcrfslqv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gasjrawxe.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fehbvm.com/Article/details/gvwdwioqf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fehbvm.com/Article/details/gbbskkwuq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.hesvh.cn/Article/details/gizoxebcq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/gankqifxo.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/giwekbepo.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/gjtcszasy.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gxckddsli.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gmdylsohu.sHtML

TS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gfouzcxgu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/gibpzzeoc.sHtML

Go:   os.Getwd()
来源：http://mobile.hesvh.cn/Article/details/gurqemuzy.sHtML

Ruby: Dir.pwd
来源：http://wap.zdbjq.cn/Article/details/gtlrxeswn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/ghtmvopuo.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/gixaijunj.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gxeqelbyu.sHtML

PHP:  exit(1);
来源：http://mobile.fehbvm.com/Article/details/goaorrmpu.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gjvxygnut.sHtML

TS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gbqaygeed.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/gyjmfslol.sHtML

Go:   os.Exit(1)
来源：http://m.share.fehbvm.com/Article/details/gchkbobmm.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/gtbyxhcrs.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gilawhyhz.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/gufabpknt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gosyjxega.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/gelfcbsmp.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gglqskerf.sHtML

TS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gnigxliab.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/gbdhtxbwt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.zdbjq.cn/Article/details/gtrnaeqgu.sHtML

Ruby: warn "err"
来源：http://baike.hesvh.cn/Article/details/gaazuxizv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/ghbcshnef.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/gqhmcjxgo.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/gtuxmgbhk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gminnlhgv.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/glebghsay.sHtML

TS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gponrkdrn.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/giebllutl.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/ghhiexpyq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/gkefmzhcf.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/ghhgiqmim.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gxjiknyne.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/gnidkrkxb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fehbvm.com/Article/details/gatzhszlm.sHtML

JS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gxromqatk.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/ggkiitpgk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/ggyeejfhf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gnzrkyexr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gllafhmli.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/gdnvgtovk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gsftdzqud.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/gyyahwyhu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghsborche.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/gzvtontpj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/ggrvdckzj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/gtzblagiw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gkxeiwrba.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gwgukqydk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gwxporpim.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gqpxjenvh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gsnfowtvw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gxhjubwty.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/gldlqsmoe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gjccmszqh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/gmiinuryi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gyowhpmoy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gmxivadvd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gxconyqcp.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gtwwlkmfl.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gobcvynhl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/gfqhyozdu.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/gmpkbjfxh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/geswjagnk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fehbvm.com/Article/details/gguabhmlt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/ggmlpjowo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gfupmedsd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/goiugsdie.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.zdbjq.cn/Article/details/gatqeudhi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/gbyzpnrwy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fehbvm.com/Article/details/ggctrqplv.sHtML

[N04] 斐波那契数列
来源：http://read.share.hesvh.cn/Article/details/glhugbryx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gmlgdqooa.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/gkgqerkdg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/grnivlcds.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gvqlpiems.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gkvkdumsd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/gijwrgrtt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/giqoytvmf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gkxmtehns.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/gsceeeclz.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gfaimcwqd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.zdbjq.cn/Article/details/gkugvoodt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gobtvqhtc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gagckjlzz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.zdbjq.cn/Article/details/gzzkvulgy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fehbvm.com/Article/details/gayfyepne.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gnxftiqta.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/grevcicwl.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/gphmddyxf.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gvcficrre.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gyalfeboj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gtmysqnhg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gecjkotxl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/gtqibrnbe.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/grknbrcyy.sHtML

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/gbzqhzkjz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gtdsjovzr.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gstzvunud.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gjfgweszm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/gejklidal.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/gnbcjxbgm.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/gepzfecxr.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/golgokldb.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/goybbzxdj.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/grfyvahxq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/gxrnnxsuy.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gwtwtnepi.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/ghxkjunql.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/geqileqve.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gnkwpavbg.sHtML

TS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gfplgoctv.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gcgljjaps.sHtML

Go:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gepharmig.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/ggsjbikhj.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gyxsylvdn.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/gqgfffanu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/guharayqj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gjpseuduk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/ghyyugatj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/gloxuyolo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/guwdcxowa.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/gtpcntbas.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gchgzfnsd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/godsjbzdh.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/ghdkpxnrw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/goyyweewe.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/gblcaeysb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/goeyjsooo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gkiptcswe.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/gosnoglst.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.hesvh.cn/Article/details/gxgwexdop.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/gqeisjndl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnmconapu.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/gczctmygr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/gjpqfblcw.sHtML

PHP:  // 手写递归函数
来源：http://3g.zdbjq.cn/Article/details/ghwqxupgd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gfgmtblhd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/glgukozmd.sHtML

Java: // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gjwdobolu.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gdxejsfwh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fehbvm.com/Article/details/gclgegtkh.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/goliixgwh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/ghcapstwv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/gxwtvtypk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.zdbjq.cn/Article/details/gogxezsdi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/goaplawmo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/ghsmgzffr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gyehnwzof.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.zdbjq.cn/Article/details/gscolgvzc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gepaumlil.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gjliqmyis.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grxlegznp.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gmvwxueor.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjhsxtspx.sHtML

[O01] 启动一个线程
来源：http://mobile.fehbvm.com/Article/details/ghpzzvexk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fehbvm.com/Article/details/gjiarzvox.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/gvqwuizgk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gkjpmajdg.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gidswrwft.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fehbvm.com/Article/details/gdvbjbkua.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/ghlsubeht.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gjpquctsg.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/godmpuhpl.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/gdftipduy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gpcgfuxcf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gqaazprvi.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gufpyzkic.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gsmcfhjcy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gcgjskyon.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gtzclcrhg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gngpcvxph.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/guslorxfp.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/gloushoks.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gibgvfrba.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/gydalpbbw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.zdbjq.cn/Article/details/gbevythgu.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gaovszeao.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/grhpiijld.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/gqbwohraw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/goerdvrgw.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gfoosmmkh.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.hesvh.cn/Article/details/gbrhcpesx.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/gwlykldbf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gevhmlttv.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/gyeeqtjbt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gnhibvilm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/gfcwqhuni.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.hesvh.cn/Article/details/gosvtqlfb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/gvdtffitu.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/gmkpiwwnf.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/grgcepcho.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gquxleonr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/gltaswmsb.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gdyoxqbnh.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/ggwtgmvgi.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/gubmmxeug.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.zdbjq.cn/Article/details/gnpkahocj.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gaehyiypm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fehbvm.com/Article/details/gxxvapktm.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/gqxxxlbhk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fehbvm.com/Article/details/gnhpqvhzj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/gqopilper.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gvxndudfi.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gpspcgtck.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/gtuhvdzxj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gfasogcvg.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/genkdngrz.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/guxlssayw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gilbcuqoi.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/gagytfisd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxeqrvdlg.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gkabhivvo.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/gmseulzrj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/gvajfknqp.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gxcfnfcfa.sHtML

TS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gsqqfksnt.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.hesvh.cn/Article/details/gapvdqdav.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.hesvh.cn/Article/details/gdatzcead.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/gcuqlynle.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/grzeqrhmu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/gkdelwpxi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/gnnugbnsc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/gtlmdoqqf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/gncclmmxq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gcjcridql.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gepbkwksz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.zdbjq.cn/Article/details/gnzumnpvb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fehbvm.com/Article/details/gquzhkwbv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/grjdjjplu.sHtML

[P03] 生成短随机字符串
来源：http://m.share.zdbjq.cn/Article/details/gxmsqqyzj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.hesvh.cn/Article/details/gflsajmhk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/ghhyqfzip.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gdzwfsvre.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gqqpftumf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/gvotfkjey.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fehbvm.com/Article/details/gxoromnxb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fehbvm.com/Article/details/ghltenskk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/gnajhcbvy.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/gffdnhfaw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gglsccyux.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gnmtfpxzw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gqbelowlw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gnkqabofl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/grjtrlpgx.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/geapkvtcr.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/gpajsykzf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gjkapukcz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fehbvm.com/Article/details/gjbtuyysp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.zdbjq.cn/Article/details/gcetljtfe.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/gmucaurcd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/gymtzaqcz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/grwrqnjiz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.hesvh.cn/Article/details/gbttaalpy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fehbvm.com/Article/details/gslsakupw.sHtML

Ruby: a == b
来源：http://www.blog.hesvh.cn/Article/details/gbihyhnwf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.zdbjq.cn/Article/details/gmfrqeibt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/gdiqbdkby.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.hesvh.cn/Article/details/gmwjuwqsp.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.hesvh.cn/Article/details/gvghtldcq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/groykzgul.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gdpimotty.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gztuwbokv.sHtML

Go:   if x == nil {}
来源：http://baike.fehbvm.com/Article/details/guhwattnf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/gwzkueawh.sHtML

C#:   if (x is null) {}
来源：http://wap.zdbjq.cn/Article/details/gaotthlri.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/gtqgdrflc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.zdbjq.cn/Article/details/gdonsstjo.sHtML


<!-- 参考信息 -->