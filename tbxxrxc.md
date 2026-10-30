代发 wailian999

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gutwrmysh.sHtML

[M01] 读取命令行参数
来源：http://wap.hesvh.cn/Article/details/gmvlxpzeo.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/gdnabjlup.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fehbvm.com/Article/details/gjzyjdarg.sHtML

JS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gwhzhfotl.sHtML

TS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gfzbpljhz.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gpqanqgjy.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/gzyrhuljn.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/gcssddwtp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/glibestpd.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gguowutkx.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.hesvh.cn/Article/details/giydzxqko.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gtzkqnucu.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gdbmlbkoy.sHtML

TS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/ghpcyxkzl.sHtML

Java: System.getenv("HOME")
来源：http://wap.hesvh.cn/Article/details/gzvwdvdba.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gbbspqgbh.sHtML

Ruby: ENV["HOME"]
来源：http://blog.hesvh.cn/Article/details/glyjpxppj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fehbvm.com/Article/details/gavkojcwu.sHtML

[M03] 执行外部命令
来源：http://www.m.share.zdbjq.cn/Article/details/gkfzmqviw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/gavcxbxqk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fehbvm.com/Article/details/ghddetujh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gzvorqfav.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gcavobdyg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/ggrdxcfuo.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fehbvm.com/Article/details/grlsfdtec.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fehbvm.com/Article/details/gfbopxuhm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/gokawqdrh.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/gcrwyvtcx.sHtML

Py:   os.getcwd()
来源：http://read.share.zdbjq.cn/Article/details/gmxemnlpy.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/gevzsouyt.sHtML

JS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gwdjfqlfb.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gngxgjoil.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/gyouwmnlu.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/ghesnhqok.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/gvmqoiwvr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.hesvh.cn/Article/details/gcbzyotnd.sHtML

[M05] 设置退出码
来源：http://www.share.zdbjq.cn/Article/details/gsthtqxgv.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gidlmwoic.sHtML

PHP:  exit(1);
来源：http://read.share.zdbjq.cn/Article/details/golgqkiwt.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gktjnuuyk.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/geeprrdmg.sHtML

Java: System.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gmynbsqid.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/gbrnkcrxr.sHtML

Ruby: exit 1
来源：http://read.share.hesvh.cn/Article/details/gamzvqybx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/gzvxobrsj.sHtML

[M06] 向标准错误输出
来源：http://3g.fehbvm.com/Article/details/gabkpmzya.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gnrvjfzvx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/ggtifefii.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gcbkcidoz.sHtML

TS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gmzerawim.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/gerxofcfr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/gcikwrxtm.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/gjknvqfsm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/gxxcmdldj.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gioplxehn.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gyxxeodus.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gtrnukjpm.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gygnrnlhp.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gluvfvkox.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/gwmrupgdj.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/gtgvlegbb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/gxmhzunwh.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/gynkpgiff.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/gtmuuwsnh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/gwtzchsis.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gwpufjzby.sHtML

JS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/giqebhytj.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gqjfvkdot.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/glsfqwcnm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.hesvh.cn/Article/details/gylngtitm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/ghvjtivrg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/goxkexxnx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtdjlfzqm.sHtML

N. 数据结构与算法
来源：http://m.share.fehbvm.com/Article/details/gnftsvtwu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glzvnpcja.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fehbvm.com/Article/details/grqttnxxi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/giayryctb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gdqkxvehj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gviaxiyxc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/goifetmpy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gxsvbsiei.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gzllutcxw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gnzfvosyf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gemvxwudk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/gmwntjack.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gozsxzutj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gmsxrchwy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gucmopujy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gglocaind.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/gzznsvpps.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gjmbwdnoe.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gtghatflj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/gzcswxeda.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/guvlsnmrg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/gzfztuwid.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/gmwalucio.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gfblebrme.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gfgqerxlg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/glvrombyd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gqurdohfx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.hesvh.cn/Article/details/gwwmmheju.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fehbvm.com/Article/details/gbqxflqno.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gxjnszcum.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/ghdhcphuu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/ggjqbzpgv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gcburlqht.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gomxqhmcp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gphyukbsr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.zdbjq.cn/Article/details/gqdouboju.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gjjjkalot.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gjswvmnnm.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/gyyjnfhif.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gyguuwmni.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.hesvh.cn/Article/details/grehshqtr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gdedowfsz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gufzbkmkx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/gpldufnxf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/guxpqicxb.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fehbvm.com/Article/details/gqmilkjcp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/gyjxvweqb.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/ginarvbhx.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gqngunrbg.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/glhospxwf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gbeosuggw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gfdoiuivf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fehbvm.com/Article/details/gudzkluzx.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/gtcoogavr.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gdfdnropa.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gycloofhu.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fehbvm.com/Article/details/gkgpdshgp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gdpmovgnm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fehbvm.com/Article/details/ghjmyzjme.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/gsfotnctj.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/ggtcmixts.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gnujlabgq.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/gsywrteej.sHtML

Ruby: // 手写 Hash
来源：http://baike.fehbvm.com/Article/details/guyxpkhck.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/gzlqfjauy.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/ggnlcockb.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gdjyovmon.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fehbvm.com/Article/details/gpmnjppkt.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gaierjzyk.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gwvmljsyw.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gwracuspy.sHtML

Go:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gziqpnwtg.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/gnumrfcmh.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gwifltyfj.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/gedllbenp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/gjolgssja.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gyrikdnyo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/glgqmuyzg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gmyamnkwq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gjbufwlcf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/gmwlrpnik.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gygwbimcf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/gufrcrovs.sHtML

[N10] 链表节点定义
来源：http://www.blog.zdbjq.cn/Article/details/gkyxnzasd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/gthqovrky.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.hesvh.cn/Article/details/gqrdohebi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/gdrzzldfp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/glphjouuc.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/gmpojishj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/gycjmnuzt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gxpcghcvg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.hesvh.cn/Article/details/gtcapubds.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/gfmgnbfha.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/gyzwwsirg.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gcvxcucng.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/guwvkqcvz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gqkfkuxvk.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/ggegcrzbi.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gvmwaqqpv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/gkmsystrc.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gctfwoenp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gancfjbbu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gyxpblyzl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fehbvm.com/Article/details/gizqchymm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gyiqisvmc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gvtseskcq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gvngbajrt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/grrgszwov.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gzbyknkfc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gmtjwbpeo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxdxwakph.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/gxemqgdub.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/guuccwtnt.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/gxnytnzob.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gflokediv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fehbvm.com/Article/details/gsbmxzefw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fehbvm.com/Article/details/ggumxksot.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gvpwzkmzm.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gjobguhos.sHtML

Go:   go f()
来源：http://3g.fehbvm.com/Article/details/gwcdhexvh.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/gadvhsstn.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gvyqbwnrt.sHtML

[O02] 使用线程池
来源：http://blog.hesvh.cn/Article/details/gqxivavyb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gllpgargh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gshwftkuu.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gaitxqjjg.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gqzxmginh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/gbejovcld.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/glkegosqo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/gjsucjuxw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/gzkhadsof.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/gaixjooea.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/gonohtqxf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/guabirnew.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/ghvvralio.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gdhurwoif.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.hesvh.cn/Article/details/grsswxuti.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gtpaorcbj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/grlwoccwr.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gvryilzoa.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.hesvh.cn/Article/details/gkhkmrrcl.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fehbvm.com/Article/details/gfrfgwaeo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.zdbjq.cn/Article/details/givagaslv.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gaupqyqcc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/gqazgmfff.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/grdxablmk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.zdbjq.cn/Article/details/geveofvyy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/gxezonmlg.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/geclyyazy.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/getjiigas.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.hesvh.cn/Article/details/gxabzeerr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/gvihogrhc.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gpqrucoft.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gxxsmxcfs.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/grifkgmzn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/ggdcvsplt.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/ggptfgahz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/gsufgvrwi.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/gjbhprjjw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/gcgyxkvqo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/gzafeakey.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gjzbzfrhe.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gnxptdbkt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/gptbqtbaq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.zdbjq.cn/Article/details/gtwylmxid.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/grfoozxqg.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/gzdikqdyr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/goeyfzksd.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/gufidcrkd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkfagrdvr.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gutdgcfvd.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/gmdafkhno.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/gtfffuhdp.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gpmrxbyul.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gsrjmvuey.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/gqcynvbcz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/ggugheqtc.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/giaoyewsp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/gquwddacf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.hesvh.cn/Article/details/grcjzhelk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gvqvqtbuv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/gfdfgewvo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/gloyvsudt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/gwlsaifik.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/gapnvfzzp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.zdbjq.cn/Article/details/gljdcdaxo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.fehbvm.com/Article/details/gwcgwpyik.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/gzmllmdvp.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/geaxezcfw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/gojqdnsrn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gewhqfvmp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/govenfrrd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gcziljgaq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gscvgmqpl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/giopipxmc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/glnbuecmu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/gtyuwbuza.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/ghsibyfna.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/gzdnavcaw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gbiugkvhk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gixkusvud.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gitiuaxfw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/gwujhtimf.sHtML

Go:   len(arr);  len(m)
来源：http://baike.hesvh.cn/Article/details/grujrcqpq.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/gcegvjzax.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/gfzckjsxe.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fehbvm.com/Article/details/godmekuik.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gatsvuabx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/gkblfgtsw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.hesvh.cn/Article/details/gzapoelhi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gcmxskdtu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fehbvm.com/Article/details/gxduhsrec.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/gahnigvdk.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/gsiqecefb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.zdbjq.cn/Article/details/gkpmyydho.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/ghwytkrdp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/ghtwmlyxh.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpzinajkx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fehbvm.com/Article/details/gqtsxowcx.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gpabopsvb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gazbtlccm.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/gcqvtkdfg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/gcykrsoxd.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/gujactfxt.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/gbwaaacxl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fehbvm.com/Article/details/ghtrtlwwe.sHtML


<!-- 参考信息 -->