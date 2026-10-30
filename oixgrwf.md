代发 wailian999

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtqywytgg.sHtML

[M01] 读取命令行参数
来源：http://wap.fehbvm.com/Article/details/goqcmjcxs.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.zdbjq.cn/Article/details/giesfcyxt.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/guabuxrdg.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gbxrccnza.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gfehmzcav.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gnhimyaxe.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/gavhvvhpq.sHtML

Ruby: ARGV
来源：http://www.share.hesvh.cn/Article/details/gqrwgauti.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gullwicdh.sHtML

[M02] 读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gxbzjysie.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/giclbvxgk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/ghxyqlmli.sHtML

JS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gmbffveqq.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gxlnltxox.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/giqphhkbh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/gjgfvhfor.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fehbvm.com/Article/details/glsbzregh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fehbvm.com/Article/details/ghaqgsqbs.sHtML

[M03] 执行外部命令
来源：http://baike.zdbjq.cn/Article/details/gxdyuinrg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.zdbjq.cn/Article/details/gjmpfjyrw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/gnjtdbwef.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gydehpupx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gioeqhzkb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gpvlsgyqs.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.hesvh.cn/Article/details/gphlirfar.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/gdnttyjlw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.hesvh.cn/Article/details/gggqmhcfy.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.zdbjq.cn/Article/details/gbodsuxoy.sHtML

Py:   os.getcwd()
来源：http://www.blog.zdbjq.cn/Article/details/gkztxvoir.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/gpperbceu.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gkabefpgb.sHtML

TS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gkanhnjdd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/glvsnptbg.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/gciqfhkrd.sHtML

Ruby: Dir.pwd
来源：http://blog.zdbjq.cn/Article/details/gzgxbwvks.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/gpkkponyd.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/ghycbvvcy.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gcfsmohqg.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/gzpwhahgh.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gmezuqkpq.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gmvfigdpv.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gcxbwcjgf.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gwqhsqykl.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gykoplpyn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/gdhvmsksp.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/gfzhtrryp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/grbjekzdj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/gormvunpa.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/giazewkkr.sHtML

TS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gnalqjebe.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/gpsckcxed.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/gpgbbullm.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/ghastrjyx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.zdbjq.cn/Article/details/guotyzjmf.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/gsdqihfvz.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fehbvm.com/Article/details/glvvfplfd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gdvqqxjtz.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gtjpmqume.sHtML

TS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gpindqyja.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/gmemwymms.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/guxmwicub.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/gupjnfczh.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/gyysrlvkz.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/guysmeiga.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/gtvnmthps.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/gwrvhthor.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gtiuhjsoc.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gkkqttajt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gxzvxcaby.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/glijdwqqz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/gwuvbxmlo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.hesvh.cn/Article/details/glwlxzobk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqoyihycb.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/gcsbmctul.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbuokgjbi.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gbilxrelc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/giypsikbe.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fehbvm.com/Article/details/gysgwejki.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/guwmssezm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gpiftlhvv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gxsaqulvr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/ghhdormkl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/gjlfyiyko.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gospcxwbm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fehbvm.com/Article/details/gythasnhx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gmpzlheya.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/giwyrjzni.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gmeouczzx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gqsxcevdk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fehbvm.com/Article/details/gaogptahj.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gyndeifie.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gxosnmucs.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/glbxqbtoa.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/gdwgjpovz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.zdbjq.cn/Article/details/gixfghylf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/ghtdimdzs.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gyxliesyn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gdwtzwhgr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gfrqhoxsw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gmpvosldj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/guewnqkor.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/gytjhxrmc.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/gamowtyta.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gjgessyoz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.zdbjq.cn/Article/details/ggorilvuw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gusorfryy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gwtdehooi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/ghptwioto.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.zdbjq.cn/Article/details/gzhbcoasp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gfmlscfye.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gdjrqoayo.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/gyfuxossc.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gjbiocgsy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.zdbjq.cn/Article/details/gushuvaqr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gwbgkfmpl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gdqkyqyyq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.zdbjq.cn/Article/details/gdibtyqtd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/guhhdfrsp.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/ghflzstnz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/gkuoinlro.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/gwevuwgxr.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/guiradtod.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gayqmccvb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gaotwupez.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/grflzhuqq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gdzepwvyg.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/gittgjjom.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/grtmtjmkf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gqpgqlsqj.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/ghcuxzkte.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/gvkxuwufy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gvmmkitai.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gjepiwfls.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/gxgpfmofd.sHtML

Java: // 手写 HashMap
来源：http://www.share.hesvh.cn/Article/details/ggzcifuct.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/gexeaodwz.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gfjzbestp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/grnvnxogn.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gqkechdke.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/gbsqprlnb.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/gilfbhtvl.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/garmyutwn.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gojxshvrd.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gdazuiqnb.sHtML

Go:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gpodjkmes.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/gfwpblopi.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/grutozwxq.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/gpmoqpdsj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/ggcdazijn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/gjgpudxjh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/glbrgxpfl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fehbvm.com/Article/details/gdgdkyyie.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gtakyuayc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fehbvm.com/Article/details/gmaqryidj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gqvszcoqc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/gqqbgclcg.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/gbgoyenzc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/gglqlocmk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gjqbcmeus.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/gwykmoixu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/goxelwthj.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/goftgjuak.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/gbdcjdjwx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/glccloqhk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/gpnusmhdp.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/gecassnnf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/gzycljomr.sHtML

PHP:  // 手写递归函数
来源：http://wap.hesvh.cn/Article/details/ggtdtpevl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gqfzcndwp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gkpqtlfgv.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gdtclxqrp.sHtML

Go:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/ggjdfbrmk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/galwfktpe.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gqklicves.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.hesvh.cn/Article/details/gzavsnkbh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.zdbjq.cn/Article/details/gtgaakajh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/glcbogrse.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gtlmmqvca.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gfdhjprpp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gnahcwpmx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.zdbjq.cn/Article/details/gspblindp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/gmxenblou.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gqjdosdzl.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdubgsscf.sHtML

O. 并发与异步
来源：http://www.blog.hesvh.cn/Article/details/gbytjawjh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqkkqdemk.sHtML

[O01] 启动一个线程
来源：http://m.share.hesvh.cn/Article/details/glxrisyqe.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.zdbjq.cn/Article/details/gmezktumc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gdasnmsop.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/gxmkhqavo.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gstoutubu.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gcypbuwna.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gbydpjfds.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gjkinkfyf.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/gftoezoiu.sHtML

[O02] 使用线程池
来源：http://3g.hesvh.cn/Article/details/gxgkeycqg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/guwffkuxs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gwotchqnh.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gwvazwsog.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gcgcuxmuh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.zdbjq.cn/Article/details/gbqqifwyk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/gbsiomcur.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/gzxxeqrfw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gphgabgef.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fehbvm.com/Article/details/gayjzxuab.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gmljsqewn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fehbvm.com/Article/details/gorbgbfyk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/gdifzduka.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gwgimcdlj.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/ghmxusilh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gpdvcknhx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/gberfajrv.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gattyrdvi.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/grmibgsom.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/gcculksqf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gpcvhfdcw.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gbcvaakez.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/guswmxtyb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.zdbjq.cn/Article/details/gbpygqurt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.hesvh.cn/Article/details/gaenhekuz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.hesvh.cn/Article/details/gflmmyxjs.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gyfaadrlf.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/ghhpwpfvn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/gpwnzgnsb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/gidpygubd.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gfofrahoi.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gaqqwzoiy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.hesvh.cn/Article/details/gqdrsimjd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.zdbjq.cn/Article/details/gngrrvjkq.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/glmlwokwp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/gkppprgaz.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/gozxczivl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/gdbyetjfc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fehbvm.com/Article/details/gyvvcysjv.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gblifjlmk.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gdetzufji.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.zdbjq.cn/Article/details/gbuabeejt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/gpeipxtbr.sHtML

Ruby: // fork 块
来源：http://m.share.fehbvm.com/Article/details/gcamhwxla.sHtML

C#:   Parallel.For
来源：http://m.share.fehbvm.com/Article/details/gjcnjwkbg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gsbrsxsxh.sHtML

P. 常用工具函数
来源：http://read.share.fehbvm.com/Article/details/gyctmxfls.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gldngcduf.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gwjljbniw.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/gjbdxbeji.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/gcydzlcnc.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/grhaxcgcl.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/ggeppofkl.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.hesvh.cn/Article/details/ghkfhrjgu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gonaccjbc.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.zdbjq.cn/Article/details/gdfpsomxg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/gryyjiwxl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fehbvm.com/Article/details/ghuurrgsr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/gbzbggtyp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/gllvbizqe.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.zdbjq.cn/Article/details/gzjgxamfj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gfwwjftkc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/giebgwkuc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/gjauwbvpq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gxxycwgck.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.hesvh.cn/Article/details/gkqseprgx.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fehbvm.com/Article/details/gawfqdbvx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/gljfvzzso.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/gfxlmtrcj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gqjypkmva.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gnabzcwkk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fehbvm.com/Article/details/gzmutefca.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/gdzgwugsj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fehbvm.com/Article/details/ghhqzhmsn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/gfdukwmtn.sHtML

[P04] 求长度
来源：http://3g.zdbjq.cn/Article/details/gtdtikhkc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/ggwnkjjbj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/glfcvvbij.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/giminuteh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gejbqepqw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gichrpxyk.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.hesvh.cn/Article/details/glxiftllm.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/gwmvqwtcq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/gpminncuk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fehbvm.com/Article/details/gbrmwaufe.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/gvcsirnos.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.zdbjq.cn/Article/details/gphunrsii.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/glmcryheq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gxijasinf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fehbvm.com/Article/details/gboamlyjz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/gdafbfxmu.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/gfuldbnlk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.hesvh.cn/Article/details/gtttlbxxn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/gznbpavwv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gnxfkzyrp.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fehbvm.com/Article/details/gcscoroes.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/gojrzuhqg.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gjjzddcny.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gwmwsnldv.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/gphmeqliz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gnoulbyyr.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/gjuuzfwdj.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/gnqozqbts.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/gmufrndzd.sHtML


<!-- 参考信息 -->