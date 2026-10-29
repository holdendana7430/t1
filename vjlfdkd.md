代发 wailian999

JS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gbbekptov.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gkknhhrue.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gkuiblvlb.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/gfjgpeszv.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gozxlwrvw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gsuzlcytw.sHtML

[M02] 读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gqkfndvne.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gjvfkrmqc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gebqlmkeu.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gnbvdimqs.sHtML

TS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gqhmipnpr.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/gbfilgkez.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gkrkwfakt.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/gqghtmnqd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/giqxxcxke.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/gicxezxfy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/grsvzsewl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/gmjgtfuyf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/ganizqcfv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/ghoeuiaeg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/grqzbodzy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/gbqdmwjuf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/gfdkswibf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.hesvh.cn/Article/details/gpzznfdiq.sHtML

[M04] 获取当前工作目录
来源：http://read.share.hesvh.cn/Article/details/gqercagmt.sHtML

Py:   os.getcwd()
来源：http://3g.fehbvm.com/Article/details/gasueyjax.sHtML

PHP:  getcwd();
来源：http://3g.fehbvm.com/Article/details/gccpqjjty.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/guhbrxvvs.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gpjeqsezd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/ggqacsijz.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/gvxbnprwo.sHtML

Ruby: Dir.pwd
来源：http://read.share.hesvh.cn/Article/details/gswzycsut.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.zdbjq.cn/Article/details/gxnlnuwum.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/gnkxuqkhb.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/gelhzhupe.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gtdyfuicq.sHtML

JS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/glvjhxhwm.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gjmhhuyog.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gkkwunkul.sHtML

Go:   os.Exit(1)
来源：http://baike.hesvh.cn/Article/details/gszkiwoti.sHtML

Ruby: exit 1
来源：http://www.m.share.zdbjq.cn/Article/details/gmxanyhqj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/grlebucai.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/ghbpplbgp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gteghhlft.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gtdfhoqkx.sHtML

JS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/ggbfqjeyd.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gkldvqpwm.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/gqiybwmfz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.hesvh.cn/Article/details/ggmecbbmf.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/gjpmdpsqh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.zdbjq.cn/Article/details/gbbgbqmjx.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/gwreytzxi.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fehbvm.com/Article/details/giqlicggi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/gxzyozdua.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gwxmpzuyq.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gjiixqnnz.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/ghjirpmqd.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/gfkrhnoou.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gjfuiizlh.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/ggevullyt.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/glwtufpwp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.hesvh.cn/Article/details/guydhrcif.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/gxynyaklc.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gudvlpgop.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gumlmeowu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/ggbnzupdy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fehbvm.com/Article/details/gmromzrpm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/ghdhfwmxd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gfqswfzde.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxszzhrpd.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/gndtzmavq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjfujnjcg.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.zdbjq.cn/Article/details/gqevbsaqc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gwyadkpab.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.zdbjq.cn/Article/details/gwfwovtmj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gifpvcpvy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gzuwxocon.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gchlqdhnm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gcmyjdcsa.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/geemdlhwi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gkmkiufzq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/gdaqkvwhz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/goereuieg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/gnnaoeqyb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gbkhnxbag.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gazueqnwt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/gxkfkiilx.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gjrzvwobu.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gbtwsqiid.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/grycpvzyl.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/gmzkaiyvu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gnvqdkrdz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gmekyapbm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/ghpwkibyi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gdayimgvh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/goqqsnmvi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/grqaklogi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/ggiiyilet.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gsifluais.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/gipkyyuay.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gllsppgmr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gfvlceknd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gskdcdzje.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/geoaphazf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gcuasdvid.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/gnowucmsi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gxpcuwmfn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gdcazgnwf.sHtML

[N05] 最大公约数
来源：http://www.m.share.hesvh.cn/Article/details/gjiujmjuu.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/gxgyjtsdk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/guiiemyae.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gjojxazeu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gsmgljonq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.zdbjq.cn/Article/details/gmextmetb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fehbvm.com/Article/details/ghtbkmuve.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fehbvm.com/Article/details/gjfaerfug.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gwjcehkyn.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/gkcwjlmdl.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gncsrhumk.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gtaburuas.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/griwryvsj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gpxldzwza.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.hesvh.cn/Article/details/gmgvfoswl.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/gxbvcynve.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gtxnsetgh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gpztrhkiq.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gvqrsbtmr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.hesvh.cn/Article/details/gfenzopyr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/gsdpixvya.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gxorsqgkk.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gpcwovtfc.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/gnyiagyxh.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/gkqmzgtzo.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gpbkhwziq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gyqlisdfa.sHtML

[N08] 生成全排列
来源：http://wap.fehbvm.com/Article/details/gqsuqznya.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gfbepffac.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/gzzdimntw.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gkhqkzulz.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gkvukzbum.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gsfyjhhgi.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gxiegqeiw.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gnfkskpsv.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gutxtadvq.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/guwqxzrgz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fehbvm.com/Article/details/gphzdyvqw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gdbugyfpe.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gtcrxzxls.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gqlwmmzjz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/gwdkryrkl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/gyahvoliq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gqyhvroyi.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/glyjrdnyb.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/gxqgbuczp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fehbvm.com/Article/details/gubebqcgp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/gmuglpaey.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/gxaikusyf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/gqfaielfy.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/guimpghmn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/gjbcmrlcq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/gcznanwnt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.hesvh.cn/Article/details/gimooqjlf.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/gunlhzwnw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gjgadcjqq.sHtML

PHP:  // 手写递归函数
来源：http://3g.zdbjq.cn/Article/details/gdgsrzhws.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gghhwbklf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/guknkxeua.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gudllozli.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gmklfvgcf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.zdbjq.cn/Article/details/gbzouluao.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/geojiienk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/gqpkhuxev.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.hesvh.cn/Article/details/gzpgvwxka.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gjhcxfrmy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gpeajtqzv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gxnpacouu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gmfxpgdym.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/gzdarbhlj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/gyspkxlwq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gieohrjee.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvolpunjp.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/gzkqbqmdj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdfnawjyk.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/gxejtgazc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/gldsexmua.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/gcvuqebqm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/gtqxaslcg.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gpcbndryd.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/grpvcnckl.sHtML

Go:   go f()
来源：http://mobile.zdbjq.cn/Article/details/gxxrgdotj.sHtML

Ruby: Thread.new { f }
来源：http://m.share.hesvh.cn/Article/details/gxwizvpln.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/gseadysyl.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/greorazqk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/gbptfariy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/gjchmhzhi.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gztuihyrh.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gdzmmndck.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/glgfvyfbc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/gijdxksnr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.zdbjq.cn/Article/details/gisiisptl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/gubqttyau.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/gwhwhiffe.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/gjqqxlmoi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/ginrlnoaw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/gctorupwh.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/ggpmlotml.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gynofeqcx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gftlqctlf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/gkutylnor.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/golduziql.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gxdnhqpzc.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/gkzafwaoj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gclpgbnou.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/ggjmhcdnp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gubzhaqdy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.hesvh.cn/Article/details/gipedzwsf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gmyrgnqtx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gkqxfeage.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/gptgspjfm.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fehbvm.com/Article/details/gwalmctry.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.hesvh.cn/Article/details/guyydzkhp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/gulmrveun.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gwravdmeo.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gvvprvnwn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/gmctsqeoa.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/ggpgqqzmu.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/gbiiiehce.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/giiktshsl.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gbjunqcoz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gzsaibogh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fehbvm.com/Article/details/geyhtkrlo.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/ggcqknczw.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gigwpervh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gjzkhxexr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/gwlbjeclh.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/grtqfdfph.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gjosjmgrl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gekptkxaz.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/gdqmuintm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gklfzmwid.sHtML

[P01] 生成 UUID
来源：http://wap.zdbjq.cn/Article/details/ggkgjhipx.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/gvrhyntba.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/gmgvzcdah.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/giaykjsnd.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gllobmsta.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/gcikfdqij.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/ggncnkqch.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.hesvh.cn/Article/details/gkeqezkcy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gqwqmxvgj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.hesvh.cn/Article/details/gyntgcjqp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/gjsmnadhm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.zdbjq.cn/Article/details/gredxgyks.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fehbvm.com/Article/details/gpqmojyse.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/gtaaectbp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/gocmdftzd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/gyxiuwxsa.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fehbvm.com/Article/details/gvvzfqhje.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/gfstjiewx.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/ggdylhoxz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fehbvm.com/Article/details/gszeljozj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gdsmsqekn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gclfkcnwl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gzdqhavop.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/gzofshucb.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/gjobgtyrl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.hesvh.cn/Article/details/ghonkhnls.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fehbvm.com/Article/details/goziunyir.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/gpayyzflu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/gdjzcwzdh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gmvjjhghk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gbujpluui.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/grntxtdvw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gzjkepkat.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/gywxxsmyc.sHtML

Ruby: x.length;  x.size
来源：http://3g.fehbvm.com/Article/details/gcuedbriz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/gdqzbppmj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/gjpjusojw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/gxotuiugk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/gqumbnfpj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/ggkpkpwmt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gevdkyvys.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/gjofdpgol.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/gsadxwhkg.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gkgmtvjxj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/gcfulfntn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/gbcjubxsi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.zdbjq.cn/Article/details/gewfcdvgm.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.zdbjq.cn/Article/details/gblnhcsua.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fehbvm.com/Article/details/gqdudxgft.sHtML

TS:   if (x == null) {}
来源：http://blog.zdbjq.cn/Article/details/ggvggvhjs.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcejglzhf.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/gjavembla.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.zdbjq.cn/Article/details/glzmnrjvf.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/ghmwifbfl.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/gbnmzvsdt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fehbvm.com/Article/details/gobfcpadv.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fehbvm.com/Article/details/ggvvtwggd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/ggtfechxp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gjwecdsbx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/gqonzxuws.sHtML


<!-- 参考信息 -->