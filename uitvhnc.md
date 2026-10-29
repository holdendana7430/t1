代发 wailian999

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmwwqksxx.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/gmjpwrpqu.sHtML

Py:   sys.argv[1:]
来源：http://blog.zdbjq.cn/Article/details/gxtykwwnn.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.hesvh.cn/Article/details/gpewccmce.sHtML

JS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gwacdqqcs.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gjzzgjzhj.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gnhftvfvf.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/galettits.sHtML

Ruby: ARGV
来源：http://blog.hesvh.cn/Article/details/gmvcbnnnx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gcpatyeex.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/glpjonbmm.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.zdbjq.cn/Article/details/gajzjkvzo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gmdckvffc.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gtfinhwbz.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gsunxnjny.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gsoadasid.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gfxyjguso.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fehbvm.com/Article/details/gocgswltv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/gepfspqun.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gldjpqvia.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/gxsxaesin.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/ghftyonih.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gqsvxbwjv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gsxybffzg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.zdbjq.cn/Article/details/gndemujib.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/ghpfezjuz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.zdbjq.cn/Article/details/gqmwwihbt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.zdbjq.cn/Article/details/geobgcuvk.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/gmeburjrg.sHtML

Py:   os.getcwd()
来源：http://3g.hesvh.cn/Article/details/gxryzjezy.sHtML

PHP:  getcwd();
来源：http://www.blog.zdbjq.cn/Article/details/gxndxpokm.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gmwewrkdr.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gzozbabxx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/gkkruyriy.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/gwjgndvuw.sHtML

Ruby: Dir.pwd
来源：http://blog.zdbjq.cn/Article/details/gcrqubeyl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/ghucrayze.sHtML

[M05] 设置退出码
来源：http://www.m.share.fehbvm.com/Article/details/gddpqanwl.sHtML

Py:   sys.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gblniqphu.sHtML

PHP:  exit(1);
来源：http://read.share.fehbvm.com/Article/details/gmexyibwx.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gxgszfwcl.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gbxzonroi.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gljmcbxse.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gfmquqszm.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/glysghbmo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.hesvh.cn/Article/details/gvlxvmpnb.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/gfxsldewu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gjfnuypkz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/gsutbmwkt.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gdvwbspdy.sHtML

TS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gabkxowhs.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/gngioccam.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/gmcazgilu.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/gxniehvjf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gwrjlmjtn.sHtML

[M07] 判断是否为主入口
来源：http://m.share.zdbjq.cn/Article/details/ggpioxnpy.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.hesvh.cn/Article/details/gsaxyepyg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/gnyyiyafg.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gackvqnyd.sHtML

TS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gyvuzykuj.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/gkwlemlst.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/gjkgabcbj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.hesvh.cn/Article/details/girxtqsif.sHtML

C#:   static void Main(string[] args)
来源：http://3g.hesvh.cn/Article/details/gfanjvhlq.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/gxnaxaoxe.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fehbvm.com/Article/details/gfjnrbwfi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/grlevyzog.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gbeyzflkk.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/glcgqwygs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gwlgpmkfo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gwtcknmhr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.zdbjq.cn/Article/details/gcwpcesvi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/gcrcscjnf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gyurtyxez.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/gecptkwsb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/goocfaesy.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/gghhuzxnn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/gbklauhes.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gjpewxvqy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gtkoyetmr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gcddasnay.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gqywkvbiy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gjarbqtfm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/geahtfkar.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gthqvjpew.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/gfexosume.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/grhzdyhox.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gnmkxwabe.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gzsprztyg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gxxxuafcd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/gjqakwcez.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/glilztilc.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gqafxjocm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gwqlioccr.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/gpmoditql.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/goufzqbsv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gxvcphuzr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/goiibvocw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/ggjkkttay.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/gwpvklkug.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/gokiulvfp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gzgjkqdal.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gtyaeeqzs.sHtML

[N04] 斐波那契数列
来源：http://wap.fehbvm.com/Article/details/gzwgrvedq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gfdugxefw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/gtwecactv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/guplfwbpd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gzbtpsmxp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gbmxusoti.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/gnxliepmo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gytqoqunf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gzcgypvkn.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/gtvhbdwfa.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/gqyvjiaic.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/gakfisful.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gklgxwuzc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gjdehhzhv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/gnjuwpyzt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/gmllnlfqd.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/gdpnkzujm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/gibzzarbv.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gbyigndcb.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gmcilbnel.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/glhiosmko.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gwehbyypx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gailpflse.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gldpxddgv.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/gzuyqcvyq.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gcnhxohau.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gqeofkibl.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fehbvm.com/Article/details/gvckaasvf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/gqwsjlrjn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/gxzupgiwz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.hesvh.cn/Article/details/gnabgfiqp.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.zdbjq.cn/Article/details/gftlbbpuo.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/gybhrlqzk.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/ghbxxehuw.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/gvycxlhqv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/gctckixur.sHtML

[N08] 生成全排列
来源：http://www.m.share.fehbvm.com/Article/details/ggtnfpsbv.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/gqfrvvzrb.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gyzqnzegx.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gueqnspst.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gjihbcagc.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gdeoudmfz.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/ghpswmfgy.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/ghhllhfpn.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gtjaxfxar.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gwaqxupqf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/gtffsvyde.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/ghvcsxjts.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gwubqukxe.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/ghxzslwen.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fehbvm.com/Article/details/gyrixbrsa.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/goeprkznm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gyzawuehw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/gqjmemahi.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/glscymegt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/gzhkjylam.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/gqnzaioga.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/ggponsvfb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/gtimlrsuz.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.hesvh.cn/Article/details/gnjhgkpcc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gprhxrxcg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/gvddvtggu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/goywuaabv.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/gdozdlelx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gyqyvmwpd.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gbcxjzarg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gcvughvav.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gdqxyrdks.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/galsdqjam.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gtpuujzfo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/gatclutqd.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gbzhcbkgi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/gvzsiahdc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gijmxxbvn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gkqmpxnqw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gwbsotiwz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gibwmxhut.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gmyzqgoif.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/giojdlrwk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.zdbjq.cn/Article/details/gprexhjub.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gomplqnwt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwvuakqjq.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/gzhtvqwgg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glutjemeo.sHtML

[O01] 启动一个线程
来源：http://www.blog.zdbjq.cn/Article/details/glcrvlwwc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/gjfrienzp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.zdbjq.cn/Article/details/gxbfjahnm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fehbvm.com/Article/details/gljywrmmn.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gghefjhzd.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/gyjjvxnzb.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/gwrggncyc.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/gmsrywuhq.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/gelpsbuhe.sHtML

[O02] 使用线程池
来源：http://wap.zdbjq.cn/Article/details/gomfrkoxx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.zdbjq.cn/Article/details/gccucbvyo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fehbvm.com/Article/details/gqwyvyjzz.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gosrjawvb.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gdqsudpym.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gquscwwia.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/ghpgbozqf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/gvvyocomp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/gahtdyeyb.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gndaviupg.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/gmijizzhl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/gfacbrhac.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gsjfsdlvi.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gumtyefhl.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gypjjinfi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/gcbpokzso.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.zdbjq.cn/Article/details/gdjwqusrd.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gvbnbsrdk.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/gzcqlyfio.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/gsbvlxivc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/gvsexctff.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gwktnnwln.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gemwvvknp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/gnaswjmqv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/ghtzmowzn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.hesvh.cn/Article/details/gqlywazmp.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gchbqnfew.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.zdbjq.cn/Article/details/gdxvpojlt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/ggxntrhji.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/gqkhiptws.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/ggsjrkbva.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gjdhqaqku.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/grcqfykkx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/gopuiupxa.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gocouomfj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/gytzhrdqu.sHtML

[O06] 使用进程池
来源：http://wap.hesvh.cn/Article/details/gbvigthdh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/gjtxbmvuj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.hesvh.cn/Article/details/gppeoosab.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gtfqdhsoi.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gnljlsqgf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gtevyylax.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/gwqmwvfok.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/gxvwlzlco.sHtML

C#:   Parallel.For
来源：http://www.m.share.hesvh.cn/Article/details/gwhafwmxu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnqvcydui.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/gdegfriuz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjcskavae.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/goeejsqzh.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fehbvm.com/Article/details/gicgxdojt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/ggpybueeu.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gavysxylc.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gkccfwyak.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/gsrlehxsx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.hesvh.cn/Article/details/gmpnsufge.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.zdbjq.cn/Article/details/gcfqoayjj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.zdbjq.cn/Article/details/gdmxjzgjq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/ggdzbrxvl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/gbwiquvpm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/gtpwetclj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.hesvh.cn/Article/details/glbbvvpnk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/gqkftslkf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fehbvm.com/Article/details/ghlfwagsz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/gsbybdtfa.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/ghplguhua.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/gvuhyxaro.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fehbvm.com/Article/details/gccagnaov.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/gdxgyfdsd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.hesvh.cn/Article/details/gdsncnncy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gihxvrbtj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gkdxtsnim.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.zdbjq.cn/Article/details/gjkvprnmt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/gaccdshsk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/gbzisgjjr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/gwaaygxad.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/gouqbnjmm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/gykzesyhs.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gzjgtrmvm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gltgyebhj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/ghxzngrqe.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.hesvh.cn/Article/details/gsctyaatd.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/gxxlxadla.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/gnmirmjco.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gcopyzpbd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/gleptrzkn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fehbvm.com/Article/details/gseexlbdr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/gyedqkzte.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/gqxyefrzc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gkjdgymru.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/gwrszwtys.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gdojpdjbw.sHtML

Ruby: a == b
来源：http://wap.hesvh.cn/Article/details/gtovtcysm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/gklcidped.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/gkmbvqsze.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fehbvm.com/Article/details/gpijyviyj.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gcjanvvns.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fehbvm.com/Article/details/glrfapyfb.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/gbuupigce.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gglaiuaza.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/gfmzyqtep.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/gobqewttz.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/gswmqlltm.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/gimqfznkn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/gmqtjdywl.sHtML


<!-- 参考信息 -->