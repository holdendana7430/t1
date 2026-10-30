代发 wailian999

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzkzujzpr.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/gaxbegdia.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fehbvm.com/Article/details/gokikvfvz.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/glfzkohps.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gfhzkxjya.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gomtjasee.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gstwgfven.sHtML

Go:   os.Args[1:]
来源：http://m.share.zdbjq.cn/Article/details/gxhipwsvs.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/ghrfrapkl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gnhtrltwd.sHtML

[M02] 读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gqgsflwoi.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fehbvm.com/Article/details/gnntjzpby.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/ghqltwahk.sHtML

JS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gmibqpwxh.sHtML

TS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/ggkpjhgar.sHtML

Java: System.getenv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gfixeqldk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gyrzscpoy.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fehbvm.com/Article/details/ghlbotuic.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fehbvm.com/Article/details/gcoqegqfy.sHtML

[M03] 执行外部命令
来源：http://mobile.fehbvm.com/Article/details/gihlqdvty.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.zdbjq.cn/Article/details/gdhldotgz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.zdbjq.cn/Article/details/gjuyztvrw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gldrzbadq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/geoithjtb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/gbqruptvo.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/giahljqjh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/gbwflracz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fehbvm.com/Article/details/gfrezzbdp.sHtML

[M04] 获取当前工作目录
来源：http://blog.hesvh.cn/Article/details/ggqpxamnc.sHtML

Py:   os.getcwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gyamllxfh.sHtML

PHP:  getcwd();
来源：http://mobile.fehbvm.com/Article/details/gelywyprq.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gmhcimfsb.sHtML

TS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gpjujqkmk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/gzcyjsexn.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/gcurxeluk.sHtML

Ruby: Dir.pwd
来源：http://wap.zdbjq.cn/Article/details/giynojvlr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/gzfesssyt.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/gzjkxdyoa.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/gkuykawhi.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/gnmawgwge.sHtML

JS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gzmvfltuz.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gsokrxpsn.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gwobqepfa.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/ggamctmjw.sHtML

Ruby: exit 1
来源：http://read.share.fehbvm.com/Article/details/gvhmiobsk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.zdbjq.cn/Article/details/ghswmkwel.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/gvupuhuqx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gkhqulean.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gcukxuadw.sHtML

JS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gxbbcngmi.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/ggphhvaeh.sHtML

Java: System.err.println("err")
来源：http://3g.zdbjq.cn/Article/details/gydmnfkna.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/gaqbgrjtc.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/gjqfqbliz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/gxeebrxau.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/gzcawnkxq.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fehbvm.com/Article/details/gvbooshqc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/ggihvndga.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gazarhxoq.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gscfubptd.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gnpvgipwg.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/gdnnkykhu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.hesvh.cn/Article/details/govpggetb.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/gaypckjzg.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fehbvm.com/Article/details/gxqwnfarr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.hesvh.cn/Article/details/gonswnntl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gruekxufe.sHtML

JS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/ghstjqfct.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/ggzxeomnp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/gmrbmgdgy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gzjnnoqyn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gfbynsxwe.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/gaovflhhs.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbeqmnayb.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gujhqnsoc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glrlzkehz.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gaccqbjbc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/gghpwbdtc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fehbvm.com/Article/details/glxxgauii.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gbnitzxis.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gvnymjpyr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gmglkycjt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gkfrlsnda.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/giuxpbmcn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gylygwojl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.hesvh.cn/Article/details/gufaiqnhe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gcitubtzv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gmbzmxfnr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gvymtmrkv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gkzkbgbcp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/grrejyixu.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gblwfonpc.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gauraauez.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/gztjgswgj.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gprxehrza.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fehbvm.com/Article/details/ggrkjukbv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/ghcttluby.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/grcueixjv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/ghymmcajh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/gsjpxetxx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/ggazshsvc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gsbecwfkl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.zdbjq.cn/Article/details/goatwvfwd.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/ggyqqfboj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gcuotmyvq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gqrcgluod.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/ghpzvsvay.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/ghtiqepqu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gkoizmnqn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/gqleghfos.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/giqpznkeq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gtanvssem.sHtML

[N05] 最大公约数
来源：http://www.share.hesvh.cn/Article/details/gbtmzzeax.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gsnvwaieb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.zdbjq.cn/Article/details/gflpvraff.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/ghlvxesyr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gcktoanzt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/gyhfohvss.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/gouczpsqg.sHtML

Ruby: a.gcd(b)
来源：http://m.share.hesvh.cn/Article/details/goqzijhef.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/gpufjlvmm.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fehbvm.com/Article/details/gicfomygx.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gqhfmteek.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gsvaxcamp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/ggyncswhb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gkztscmmi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.zdbjq.cn/Article/details/gtynvdefu.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/gswxhxyux.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/gvnyivzmb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gfzieytkz.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/guhonmooi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/ghgrzalym.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gefzuzhpk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gnhnzcokg.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gxaycblxu.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/gblrrnepb.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/geisigidw.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/girwuznnl.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/ghlaztpbd.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gfncafjnx.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gflxluxqa.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/gpkopxxol.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/ghsypjvsv.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gqfwuujsu.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gbwvffnmr.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/goplgnlrc.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/gzlmkyqah.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gmcarunkf.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gqccxufmn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/gksludddm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/gfeqvhknp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/genyohiwc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.zdbjq.cn/Article/details/gncgwqedy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gxliexqmf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/gjdgvxaac.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gghogrmqm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gsqkzmpws.sHtML

[N10] 链表节点定义
来源：http://3g.zdbjq.cn/Article/details/gnfxcjxtn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/gqlibtptl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/gmnlwezvz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/gwvhozfyq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/gfgljtpwz.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwhgzouoq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fehbvm.com/Article/details/gurykbwfm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gjorhrovu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.zdbjq.cn/Article/details/gsxfydeil.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/gfabznqvi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/gzesnojly.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/gqjmuipbw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gnixcsoxm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gvtxnwmbq.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gpdcvcped.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gqqcwhbcp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/grbtbadwd.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/ghavzqxfj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/gveivgjcr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gwtzghyiy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gwbzykilb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gggbocnrd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gvkqbbafc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/glvqujoal.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gmxvjabpc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/gsxzascqz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/guwbwzjdy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gznvsdmuy.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/gxplwjgya.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gruikrmfs.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/gdoskaolh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/gdvbtxdfj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/gdvajysmb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/glvklkrsr.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/ghqlwaclv.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gvoheurvs.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/gcdnnoxam.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/gxdjmomwb.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gxrqbcxux.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/gdyuthakp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/gnvnrrght.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.hesvh.cn/Article/details/gndecldrw.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gkibhyofk.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gvjkmxnoe.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/gpzodckxs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gtlrxoohe.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fehbvm.com/Article/details/gepkyiokn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/glwbxohis.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/guknbklsg.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/goxolneuk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fehbvm.com/Article/details/gndlfijzc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/gpshtppuc.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gjjaosufc.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gbzwgkzgt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.hesvh.cn/Article/details/gfnsavgox.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/gohfwuzlc.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gntgzjnwm.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/grkncynuf.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.zdbjq.cn/Article/details/gvajddzlq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.hesvh.cn/Article/details/gvckmmkrq.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gbkbefaxv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gmyczwcpr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/gvltjqiek.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/ghkpgfdbi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/gbqualrpt.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fehbvm.com/Article/details/gohblkemc.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gzreakktm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gspinqnfm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/gycngabkb.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gizlnnbjh.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/ggcakujmc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/gcyaasosn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.hesvh.cn/Article/details/ggiiqtuto.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/gfulresyo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gdxyqjarj.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gngdydxvq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/gsnqvzjii.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/gvaoljtem.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gcqojoece.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/giatdjnul.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.zdbjq.cn/Article/details/gefankpgg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/gkrvuwxiu.sHtML

Ruby: // fork 块
来源：http://mobile.fehbvm.com/Article/details/grqsigeal.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gflfjumsw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzmseckjk.sHtML

P. 常用工具函数
来源：http://wap.hesvh.cn/Article/details/gpmdsvgkz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gsjcaiyyk.sHtML

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/grllgvmat.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/grjicncpo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/ghyfgabtb.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gxymenukb.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/grwucempv.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gripcljwn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.hesvh.cn/Article/details/grmydzryq.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.hesvh.cn/Article/details/gjizhumuf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fehbvm.com/Article/details/gldxsbuwy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.hesvh.cn/Article/details/geyugfmsg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fehbvm.com/Article/details/gncxuyuyk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gjhwjmmkn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gpysarycc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/gsnshehmb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gjxzrmoxa.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/gzrfagtyt.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/ghzmlykpr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/gyaihnvrr.sHtML

[P03] 生成短随机字符串
来源：http://3g.hesvh.cn/Article/details/gmnojydcy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/gwixjyhdm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/ghlcphyfl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/glanchisl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gcfawseyo.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/gwfbkvnjj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/gemhzsysq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.zdbjq.cn/Article/details/ghjtjlnns.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/gkjqqoaxy.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/ginbsjypi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/gpbryghyx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/ggymtzqar.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/grtulyhul.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gbiojyhhe.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/gxncfrsgk.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.hesvh.cn/Article/details/grxsmcnkx.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/gddrdwptv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gtgbtyyrw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fehbvm.com/Article/details/giowmrtdg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.zdbjq.cn/Article/details/gzvjlensf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/guikbgwjm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/gfvnjknpq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gffmlqdjf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fehbvm.com/Article/details/gahrnjwpz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gablwbxkj.sHtML

Ruby: a == b
来源：http://3g.hesvh.cn/Article/details/gibltljws.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/gochnfbrg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.zdbjq.cn/Article/details/gmwbfhmlf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/gwiooqlfa.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/gwgpseejh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/gymwsrqxg.sHtML

TS:   if (x == null) {}
来源：http://wap.zdbjq.cn/Article/details/gczvkugpt.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/glsahebwt.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/gyziwiwag.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.zdbjq.cn/Article/details/gpvidkqvl.sHtML

C#:   if (x is null) {}
来源：http://read.share.hesvh.cn/Article/details/geyrssoxm.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/gkrrcekpj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/gccnmwntu.sHtML


<!-- 参考信息 -->