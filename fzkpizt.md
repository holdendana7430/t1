代发 wailian999

================================================================================
来源：http://baike.fehbvm.com/Article/details/gejleokrs.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/garimnvsj.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.hesvh.cn/Article/details/gsndfjlpe.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fehbvm.com/Article/details/gfocwdfgk.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gndhmjkky.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gbsjhybhq.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gvkvutxaa.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/gboghlyqg.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/gxavutefs.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gnqkfkdxv.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/gqtlmebyc.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.hesvh.cn/Article/details/gwsvsfbxb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gvjespjmd.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gzqplixya.sHtML

TS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gomdyvlhr.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/ggcuynzmd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gsusihhsm.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/gvvcalocl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gdlbjmqkq.sHtML

[M03] 执行外部命令
来源：http://3g.fehbvm.com/Article/details/gnnrqdvkn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/gytckvvmy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fehbvm.com/Article/details/gagnjmevv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gixwvnocd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gysvddbkk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/gweiubbai.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/glpilbrmb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/gqlantarh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.zdbjq.cn/Article/details/gdvvrzlbv.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/gvkxadrrt.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/gcypgcifk.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/gzxfloytj.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gkacdarju.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/ggqjwpwnc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/ghuydiekg.sHtML

Go:   os.Getwd()
来源：http://mobile.hesvh.cn/Article/details/gxuikyvkr.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/gggvuaoib.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/gpsshgxtb.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/ghxotgine.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gfblhhzti.sHtML

PHP:  exit(1);
来源：http://m.share.fehbvm.com/Article/details/gexvdovrz.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gtobcnyio.sHtML

TS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/goflrzspv.sHtML

Java: System.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gbxnrhgza.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gdpldjboa.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/gfqhrgdwn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/gtzncvkzs.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/gnumhbmjg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gyiyrahcv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/gradeyeef.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gazvgvnmz.sHtML

TS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gdpwyeyhl.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/golmrwbdi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/gcwcxpftk.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/gnafmsbgl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gdrzpmwcf.sHtML

[M07] 判断是否为主入口
来源：http://blog.hesvh.cn/Article/details/gnblbwffh.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gadcrwgxw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/ghfrivalw.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gtpisjved.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gqbybaiqx.sHtML

Java: public static void main(String[] args)
来源：http://baike.fehbvm.com/Article/details/giruiwdty.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/ggiblaayp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/gbholxxcd.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gzpoyunbc.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gsvpjowrm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/gkucpywim.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gfiikmrvy.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gbaozhyof.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gknugvtfd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/gwksykaai.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/gijytdzsj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/glgsnrpsz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/gibcahopv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxbtzhcts.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/gurhspnmb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnkexuonf.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/gmkdwlxml.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/gzzrynzgp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/glltczcze.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gxolsprnn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gkyygyvay.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gwnyynyep.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gslkibrac.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/gwccdjlsy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gtysuzboj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.zdbjq.cn/Article/details/geciazqrn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gmvrszulp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/gvlbplcon.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gfntpkdux.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gciiydhwm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.hesvh.cn/Article/details/gamwezejj.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gfwgpppyl.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gybdfqpur.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/gaymojrdd.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/gjwpioimr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/glbvywztv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/gvscsyowo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gxmdbnsgg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gidxniceb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fehbvm.com/Article/details/ggkokdqdq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.hesvh.cn/Article/details/grpdrgzve.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gggwfxkyn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.zdbjq.cn/Article/details/gihhwfagh.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/gmngjhoip.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gvcnlqlvk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gmvpmyqev.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gpzyleqju.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gwvqwecay.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gxtbmdhxl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/gmpjilgyj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gdylpmcvn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gbawpvlii.sHtML

[N05] 最大公约数
来源：http://3g.fehbvm.com/Article/details/geetoqrce.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/gzhyayzam.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/giakvovkd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gnamuguqw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/groegxsxw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/gdymbwtgh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/gfbzdibrr.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/gqqjjulws.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/gmfdfzqse.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fehbvm.com/Article/details/gwmexqnff.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/gwzdcxwtv.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/gdzloqfzz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gpoyepyuz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gogzgfivs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/grjrlmgum.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gqindmozk.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gayxqketk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gvkcvkwbo.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/gcwrixmsa.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/gizbpbeaj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/grziwtlzq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gqepaiana.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/gvcommaqw.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/gzcyocksx.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/gaknygsnh.sHtML

Ruby: // 手写 Hash
来源：http://baike.zdbjq.cn/Article/details/gtfomoksk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/gmmvdnegu.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gawwexvyd.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gtsihznjq.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.hesvh.cn/Article/details/gygidjhso.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gyzdxiqrp.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gtivlzgwu.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gwzumsjie.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gvditsivw.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/gpqkqphji.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gbltthxxx.sHtML

[N09] 栈与队列
来源：http://wap.fehbvm.com/Article/details/gsglvpamh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.hesvh.cn/Article/details/gmzqvbtca.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gzuaejeik.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gvnsplder.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/grmflcznf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gaituvehg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fehbvm.com/Article/details/gbleaxspn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gfmwghnpp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/glcspcerc.sHtML

[N10] 链表节点定义
来源：http://www.m.share.zdbjq.cn/Article/details/gvcmltvpd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/gojjhwgrx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.zdbjq.cn/Article/details/gwhjhchvw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/gxonaxdrx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gcetcmpon.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/gzjtfgdns.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fehbvm.com/Article/details/gbgsqlbuy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/gmvgjmkfl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/gtzrzdgoz.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gooriryii.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fehbvm.com/Article/details/ghfmflnay.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/gfegzslut.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gpsdpbgwf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gtnehbgnj.sHtML

Java: // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gdoipfshn.sHtML

Go:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gmatlkbfn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fehbvm.com/Article/details/gnrvvizcx.sHtML

C#:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gerzpfhoj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/ghodlkohc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/gbyhiatcw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fehbvm.com/Article/details/gwnvpnmbx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/guoiztteg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/ghwdppthu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gcxqisraz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gdcfhjovd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gzgivqbbm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gvfqyptwz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggeiwnhef.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/gtjsqlavw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjejhxhks.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/gvlwqyvyu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.hesvh.cn/Article/details/giduoohmk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/gtwjixdfx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/glyglxlno.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gnwvsdylq.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/glwabjpuz.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/gbattqvmd.sHtML

Ruby: Thread.new { f }
来源：http://blog.fehbvm.com/Article/details/giodzmilr.sHtML

C#:   Task.Run(() => F());
来源：http://3g.hesvh.cn/Article/details/garjdvcjt.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/gxplicplr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.zdbjq.cn/Article/details/gkzrwiaku.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/gqebtzumg.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gwvqifbjj.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/grflkhmyc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/gmaciogpx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/gbjerwrup.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/gmprvxzws.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/geojrpvmy.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.zdbjq.cn/Article/details/gmuxpztau.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/grdldbydj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/guazmtncj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/gvhynwnnq.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gdmcjvbgk.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gpojgexry.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.hesvh.cn/Article/details/gpjctuume.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.zdbjq.cn/Article/details/gtqepflsx.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gvhturhre.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.zdbjq.cn/Article/details/gljwvgwlk.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/gcdaivaob.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gcmwyzfgt.sHtML

JS:   async function f() { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gtsfqyyvw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/glgsoqbtx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.hesvh.cn/Article/details/gxtkhkqvg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/gdwgctpxz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gdevqorca.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.hesvh.cn/Article/details/gpyvjlojc.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.hesvh.cn/Article/details/gzxcwafhv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/gmfofuvlh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.hesvh.cn/Article/details/gmyowgkcd.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gtcxgdosv.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gwrodegxm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.hesvh.cn/Article/details/gyuzkdabq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/grczgsmyx.sHtML

Ruby: threads.map(&:join)
来源：http://wap.zdbjq.cn/Article/details/gyzxugkqa.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/gwzcutdmk.sHtML

[O06] 使用进程池
来源：http://3g.zdbjq.cn/Article/details/gwtjxrref.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/gnslizick.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gfxptglda.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gvsbdzwaj.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gldprdliv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gbpvllpad.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/gjoosljgg.sHtML

Ruby: // fork 块
来源：http://mobile.hesvh.cn/Article/details/ggjdbloup.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/gzhhpznvo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggwtumfkq.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/gtiyykrdc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gutspavro.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gyqmyuogq.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.hesvh.cn/Article/details/gczzcgcqb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fehbvm.com/Article/details/giencvncf.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gswosuxeq.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gtejpgdlt.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gamaycrou.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/gpyoxyqyj.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/gzhdtyccf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.hesvh.cn/Article/details/gtkhbfppf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/gwxeaetsf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.hesvh.cn/Article/details/ggbqrigzl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/gqvazsmxc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/glmohnokg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/giixqtbbm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gsoslirxm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.hesvh.cn/Article/details/gazenmtbc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gjgovsjxo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/gxrxrtzmj.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gmrvkoxwj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gjbixrjov.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/gmpprinfl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gxgdiuhzh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/goczrnzhz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/gulwiezuu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/gjpiaolhr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/gqjccdabv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gbvuvbcrr.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/gvdmirfei.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fehbvm.com/Article/details/gcqhtyrjr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gserzgirg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gshedflsy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gthdxifjr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gwzkkkufq.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gndynfxij.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/gwnbbihwd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/gpgftwzol.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/gqwjmlwbo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.zdbjq.cn/Article/details/gpvpagoqp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/gpcihbcxt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.zdbjq.cn/Article/details/gnddnwjnn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gfaouhkoe.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gdqewkibz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.hesvh.cn/Article/details/gykgrwbki.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/gukbuffdm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/gahhbalgh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/gqpmqtert.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fehbvm.com/Article/details/gufssuhhw.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/gwaontxpw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fehbvm.com/Article/details/gsdpjtgel.sHtML

TS:   if (x == null) {}
来源：http://blog.fehbvm.com/Article/details/gfzthaedx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gkphbbwdz.sHtML

Go:   if x == nil {}
来源：http://baike.fehbvm.com/Article/details/gtnfseaud.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.zdbjq.cn/Article/details/glcdzoxgn.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/ghbnbuona.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/gwjeasivb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/gdouptzyz.sHtML


<!-- 参考信息 -->