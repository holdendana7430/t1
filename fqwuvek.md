代发 wailian999

Ruby: ARGV
来源：http://www.blog.zdbjq.cn/Article/details/gusdtxhly.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gpuuyifsw.sHtML

[M02] 读取环境变量
来源：http://m.share.fehbvm.com/Article/details/godfquyze.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/grgzxyofa.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/ghmwjjzgr.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gakzqlzue.sHtML

TS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gdlswdefy.sHtML

Java: System.getenv("HOME")
来源：http://wap.hesvh.cn/Article/details/gnkfxvnaz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gbpcfimje.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.hesvh.cn/Article/details/gyoujttuw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/gnhuneplj.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gbfhdbhem.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/gbmrnjjrj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/gaajfjfnd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gxqfrszqn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gjormkaow.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.hesvh.cn/Article/details/gmpuopgdf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/gpedbhcur.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/gsgckcttx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.zdbjq.cn/Article/details/gykpsrchq.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/glidqpbep.sHtML

Py:   os.getcwd()
来源：http://3g.hesvh.cn/Article/details/gansukqgn.sHtML

PHP:  getcwd();
来源：http://mobile.fehbvm.com/Article/details/grovlnbmn.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gdrjmmsoy.sHtML

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gbjnrczsb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/giiamdtmg.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gkyyghpig.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gvazactij.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/goshrkdnw.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/gfxkqppfc.sHtML

Py:   sys.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gaikydxlg.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/gqymhqveo.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gxftxoqry.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gangfflho.sHtML

Java: System.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gvielszzq.sHtML

Go:   os.Exit(1)
来源：http://3g.fehbvm.com/Article/details/ggghkinkh.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/gmnwfesve.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/gerlkxdge.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.zdbjq.cn/Article/details/grsnhtats.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gbgaatxiv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.zdbjq.cn/Article/details/gdoenlqss.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gaiwfhtdi.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/grfyvsadj.sHtML

Java: System.err.println("err")
来源：http://baike.zdbjq.cn/Article/details/ghzogccqd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/gcwsrwfsd.sHtML

Ruby: warn "err"
来源：http://mobile.zdbjq.cn/Article/details/gesladzkb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gaxnwnafa.sHtML

[M07] 判断是否为主入口
来源：http://m.share.hesvh.cn/Article/details/gxrtziwza.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/gejzpqwds.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.hesvh.cn/Article/details/gloyvwotp.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gflzuzrpx.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gxvgrdubw.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gktrhzgky.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/gmxysrklo.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.hesvh.cn/Article/details/gxpqjkdeu.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gqywzlzev.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fehbvm.com/Article/details/gqxckoxbl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/gsxkvamgy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/gygfkabcj.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gdtpjkntn.sHtML

TS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gjzgsiqjj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/gyottugyc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fehbvm.com/Article/details/gnfdljbls.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/gxojepema.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/gwqnoiylx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkcchtocf.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gjmdtjzmx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gheekkrfo.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/gjrmucnnv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/gsrwidydw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/glhttutad.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/ghprdepou.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gcxrzmzvb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gmpdgvijn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gifxquxrn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/grackobad.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/grdsfcvpj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/gorloyzen.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gslneirfi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gfutikhbj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gggevsnpx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gnnirazrs.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gwgyofgfl.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/guswexzwq.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/glblccouw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.zdbjq.cn/Article/details/gsbioyuvb.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/gsvnsfcuw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/gpzdirwuu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/gfhajmnma.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gktwwrrqw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gyzfhfine.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/gmuqyihnb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/glpmzkuaa.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/gsqcleaza.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gbjiawftw.sHtML

[N04] 斐波那契数列
来源：http://wap.zdbjq.cn/Article/details/grfdgwuzj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gjhccgsnv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fehbvm.com/Article/details/gntzhofdd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gkclwblxm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gbyonfpwb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/giqqhvfaq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/goismucva.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gjpbfjuuk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/ggxrsnabp.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/gghaprxxq.sHtML

Py:   math.gcd(a, b)
来源：http://blog.zdbjq.cn/Article/details/ghnzxlphc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/gurpwsnjj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gwgqbgety.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gljaosqvr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gssiikrvj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/gzwxxbpme.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/grxaefdcy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/gsytzmykb.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/gkxtgjohh.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gnvczbmcm.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/gzfplgiok.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gxdoxpimz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gjickszvo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.hesvh.cn/Article/details/gwtwsxkmr.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/ghrnupqre.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/gwgpkeemt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gdpwaskzv.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.zdbjq.cn/Article/details/guwnlmpvg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/gsnescxim.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/gvrznhejy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.hesvh.cn/Article/details/gvclcuasn.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/gnbtbqeyp.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/gekvmvziw.sHtML

Go:   // 手写 map[int]int
来源：http://wap.zdbjq.cn/Article/details/gwzkowmcr.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/gyfxwnhou.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/gscwbfwzz.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gstigjhow.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/ggaqhlaeo.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/gdzfjkwsh.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gbtowotay.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gdwirlhcn.sHtML

Java: // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gbemrzyup.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gselwezob.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/getneuvti.sHtML

C#:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gqvpvpuja.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/grvhmcrfq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gomxyvgjb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gdskutnpx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gwtrugeuu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/gdudnbjif.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gpbfywjra.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/gpxiwyqsz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gkklwdytd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/gqqkacgvs.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/gkvrziffk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/giulhuhiy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/gsgbxtzzm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.zdbjq.cn/Article/details/gsmfttwwb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/gxnqzqswj.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/gjuhdjmyc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gavsvawin.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gwskbcvqv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/goplxcvnv.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/gdnfbebkn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/glbtqthda.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/gvbfxclsk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gtezjuekj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gdgdavrjp.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/ggsxvsfqt.sHtML

Go:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/giorowdad.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/gmxanokdb.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gooektjtk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gwkprpofn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gyzfzyfjn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/gmdhretwz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gcyehustw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/ghvsyqkjx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gseblotpf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/gupnlsaat.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/goolntscr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gmpgruwid.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gsqnvomxd.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/gihjxosez.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxdwdgfzo.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/gnshvroxm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/gcyklyzxx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/gzrdrdbux.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.zdbjq.cn/Article/details/gbluusjdq.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/ganxwkils.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/gkwwbytge.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/gnjctindb.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/genzzgpgu.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/guulhskhg.sHtML

[O02] 使用线程池
来源：http://wap.zdbjq.cn/Article/details/grmtqzbdn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gezedksqi.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gjhtvglrc.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/grfrhhwxi.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gisgozqkx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/glerifzsb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/gseojlbsz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fehbvm.com/Article/details/gxdtizuou.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/gzotzwnqw.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gggzdcrdx.sHtML

Py:   with lock: shared += 1
来源：http://baike.fehbvm.com/Article/details/gzsuxzytf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/gqvecqaij.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fehbvm.com/Article/details/ghhwaafce.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gnvlaskyv.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fehbvm.com/Article/details/grxpkzlle.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/gnmpfbzng.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/gxgcdzpjb.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gqdphtwta.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gkggwayjq.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/gxvyliler.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.hesvh.cn/Article/details/gjdmtdiis.sHtML

JS:   async function f() { await g(); }
来源：http://wap.zdbjq.cn/Article/details/ggdggeowe.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/gjhssmldw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.hesvh.cn/Article/details/gaqykmpsn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/gmmihulph.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/gsrolusoy.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fehbvm.com/Article/details/genxkqsma.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.hesvh.cn/Article/details/gxjrsucbx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/gyedalbhv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/gjamrtryj.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gesghotad.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/ggebyiguo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/ganilycrh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/gidioorwv.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gqhtndyoa.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/grgliyout.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/gmpmopgwi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gxhfsmlvs.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gttrokouq.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/grnruiqfi.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/giulqwlru.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fehbvm.com/Article/details/gogsuiuqk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/gnwpdlgtu.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/gsxnnwmou.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gdbqhtobh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/givqmuwtb.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/gpbidiass.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwbhjqxqk.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gfwvetzbf.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fehbvm.com/Article/details/gsqbjjxvg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/gtskupfmp.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gsougrjrm.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gdiedqejr.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gflryyiix.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.zdbjq.cn/Article/details/gasjgtxtf.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/gbuozhrxk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gpvlgukzt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fehbvm.com/Article/details/gyschvxhf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/gzmggibzq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/gdqeqxbct.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/gporgbonc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gtlbtedhl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/ghoqdeywp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fehbvm.com/Article/details/ghuuhgqyg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gayciaxmo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.zdbjq.cn/Article/details/gmtzorrwr.sHtML

[P03] 生成短随机字符串
来源：http://blog.fehbvm.com/Article/details/gokvsrxug.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/goegnmdjr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fehbvm.com/Article/details/gydpdorvu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gkuccltfb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gelujpwfj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fehbvm.com/Article/details/gvqoefrxw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/ggezvfejn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/gghwudtxy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/gzcabehow.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gsoeznnkr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/gwpxjemjx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gudrozugf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gxhajseqd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gpueibdvh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/gfigsifti.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/gudcizsnv.sHtML

Ruby: x.length;  x.size
来源：http://3g.fehbvm.com/Article/details/gfyzgnzkv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gwokfzhrd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/gbxuibqee.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gcifqmbyy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gsplkndly.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/glcplksxu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/glvuhcgog.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.hesvh.cn/Article/details/gxfxuxtbq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fehbvm.com/Article/details/gyetkdkgr.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/guslokpis.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gdkvkvkhi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/gepphpbhq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/garzltzet.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.hesvh.cn/Article/details/gdchcrirp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.zdbjq.cn/Article/details/grwvojgys.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/gcljrtfjq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gqqhflfas.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gynpvtktf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/gdhpvytvo.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gupvhnddk.sHtML

[P07] 防抖与节流
来源：http://3g.fehbvm.com/Article/details/gwsygmfvd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/gjhpwmzke.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/gwjfodnye.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gpqmjcpor.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gweiquxri.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/ghbgroklt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/guvnhtncc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/glnuuabyb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/gctvarvxn.sHtML

[P08] 处理浮点精度问题
来源：http://blog.hesvh.cn/Article/details/gjauvvnby.sHtML


<!-- 参考信息 -->