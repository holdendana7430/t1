代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gtidftvoj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/gsgqypjck.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtevrvdqh.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fehbvm.com/Article/details/gzwdyfdci.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gszetkbdi.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/gdjqllvgi.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gnazvttai.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.hesvh.cn/Article/details/gvhaazyis.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gpnpibofl.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gsozdvtmo.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gerwratrc.sHtML

Go:   os.Args[1:]
来源：http://3g.hesvh.cn/Article/details/guommxirw.sHtML

Ruby: ARGV
来源：http://wap.fehbvm.com/Article/details/gombnoxqd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fehbvm.com/Article/details/ggcnmjvpe.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/ghtathrig.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/gmcrsaapg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gucwzpxty.sHtML

JS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gzlmyggou.sHtML

TS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gzpkrrvvx.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/gyrtkofdf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gccuhxfba.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fehbvm.com/Article/details/gqllizvhg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.zdbjq.cn/Article/details/gjvgfgklk.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/gnqnzlyuu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fehbvm.com/Article/details/grosxiyur.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/gudbmhgvd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/geqogteur.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gbfkbvroe.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/gonenbtae.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/grxshezoa.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/giuekafoj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/galepzjvf.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/gzrhvpmkk.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/gqswtmmwx.sHtML

PHP:  getcwd();
来源：http://m.share.hesvh.cn/Article/details/ghlyglzii.sHtML

JS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/grapnkgxj.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gxmmplfzz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/gpfqgidjj.sHtML

Go:   os.Getwd()
来源：http://www.share.hesvh.cn/Article/details/giinxlocg.sHtML

Ruby: Dir.pwd
来源：http://baike.hesvh.cn/Article/details/gzxmdqrya.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fehbvm.com/Article/details/gnwpxckww.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/grnxzxyzj.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/gusfpoktw.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/gxtqnrpnn.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gnhcvnuji.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/giorqfouu.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/glwgcumor.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/gzwipdtgy.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/gdwdciejw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/giwnncdya.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gqlduwhwk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gwpmnhaat.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gfydvmded.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gsrczzdaq.sHtML

TS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gicnxjpfr.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/gipkuharf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.hesvh.cn/Article/details/grxgzwcso.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/gpwhkrufl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.zdbjq.cn/Article/details/gxkswphrs.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/gbrlhxnnq.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/gjtoiylbg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/gzsktkfbo.sHtML

JS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/glnbzqtrl.sHtML

TS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/grljshsyk.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gbxfjxqno.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/gqtvsheht.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/gbufftaqb.sHtML

C#:   static void Main(string[] args)
来源：http://wap.hesvh.cn/Article/details/gkgyymgyk.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/ghifvsrak.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/grznrppqz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/grdhpxwvx.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gwgjmmtpj.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gckuyygyt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gouqxqdhj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/gbmsnphsp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/gzqxwbuea.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gufxckemr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gswgpjsvw.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/gynhnogyx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnfpswaeu.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.zdbjq.cn/Article/details/gnbnucrxt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/grtfnhwog.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/gmkmwuphg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/grjaetzbo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gnwpxkqhr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gtihdffri.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gvdfyakyt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/gyrwnzxhy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gqfutqxqi.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gtingivjx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gpqnyteeb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/gmnqkahfr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gzknequjc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gyooumrtx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/gdovbfera.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/glxqdgcfw.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gjhciqwkv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/gqpyedoim.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/gjqsgwmiu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gxxmqkqrb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/gtaiasxud.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gemjvrwvu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gyaugxvxz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/glulwkggt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gumcuuief.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/gcvpepulv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/gyfrmaszw.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/gbmjcuxul.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/ghgshkpoe.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gfesvcpvz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gqeeiaflf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gxckpulsy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gejncaaqc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/gxkfrzeyr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gbpuehdzf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gmbavyyzs.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/gqakccosc.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/ghmdgwefh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/gdlumffdh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gkaviujuf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gktfvmhpq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/gtshabkjl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/gtkzvsjbi.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/gcgikwelx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.hesvh.cn/Article/details/glgxkbaqb.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/ghwfhpkrl.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gkgnsfdhq.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gcvwhhaqj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gvjwteydg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gujikdssv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gtpemafhf.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fehbvm.com/Article/details/gcerkfefg.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gzusdnniv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gcbaqzkfs.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/gfongfubk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.zdbjq.cn/Article/details/gvqgmgxam.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.hesvh.cn/Article/details/gdbnqkwzc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/gmxkvzykg.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gsopznngi.sHtML

Java: // 手写 HashMap
来源：http://read.share.fehbvm.com/Article/details/gtgoldecr.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/gaemrqbjk.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gixlbibdu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fehbvm.com/Article/details/gojhtxatm.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gnwseeeux.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/guanchoey.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/gapdicpev.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gdmhnjutd.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gxdrovsuw.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gpdzpbqkv.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/ggadmucve.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gxhdoypza.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gvmsdbrau.sHtML

[N09] 栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gzwxijmim.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.zdbjq.cn/Article/details/gakhqnhkl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/golrradlx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/ggadzhwwb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/ggbseyvxn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/gjsxoeetb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/gonoxdkfv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/goxukrswm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.hesvh.cn/Article/details/gigzyyscl.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gmnmzgurn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/gehcyltqz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/gvyvwoiik.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/gbpfbsnjh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/gakwctjqg.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/gqdeoxxpl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fehbvm.com/Article/details/gzbkkflyp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/gsroprffo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/gcyuxnvvp.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/gkhuspfpo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/gvuyqaqxw.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/ghktqvaac.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/grhkbzgvy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gskgrgqob.sHtML

Java: // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gnpwchnoo.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/ghrbuhvqt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/gpsmaaxnu.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gsozahwez.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/gvxrhlrge.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.zdbjq.cn/Article/details/goqkfmcuy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/gusstktyz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gzdesidcp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gxljdiqxl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/ggwcroauv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/gmqpgcufd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.hesvh.cn/Article/details/gpfnszxpu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gedwojxxd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggjvbdxhq.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/grnfzyzun.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gedwybkho.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/gstfzvrre.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.hesvh.cn/Article/details/gzrwasqbg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.zdbjq.cn/Article/details/gofmzqmub.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/gxjceqmmv.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gjgbeyalf.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.hesvh.cn/Article/details/gsodwqqko.sHtML

Go:   go f()
来源：http://www.m.share.zdbjq.cn/Article/details/ghvjpkfwl.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.hesvh.cn/Article/details/gelldkucq.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fehbvm.com/Article/details/gyehgigqy.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/gnbkqqgjx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/gszekizdb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.hesvh.cn/Article/details/gntvpsgjn.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gyllfbiab.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/guujemlin.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/gnstzbxrg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/gzlqptbqq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gendjrhiv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fehbvm.com/Article/details/gpbjqfuou.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/guharpfpr.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/gxljodtzn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fehbvm.com/Article/details/gnmpxvkvq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/gmjsazkkk.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gjfuzudud.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gbuzpnynd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.zdbjq.cn/Article/details/gconqgfbh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gpozbghlq.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gbwytytko.sHtML

[O04] 定义异步函数并等待
来源：http://blog.hesvh.cn/Article/details/gyzfvelby.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/gjrggvwza.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.zdbjq.cn/Article/details/goubtnnxa.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gyjchigko.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gfvhfxpcp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/gaximfqjj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/gsxzwtnbg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.hesvh.cn/Article/details/ghhpztxsy.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/gjavooxhj.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/gdeyephse.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gxthvhpfw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.zdbjq.cn/Article/details/gghptrkvm.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gzzduiwnr.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gejwmceod.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/gqvuzqvlh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/ghmzposwa.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/gzzthseck.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.hesvh.cn/Article/details/gpicuuhab.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/gipavsfzz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/ghbxheokq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.hesvh.cn/Article/details/goqvqaibr.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gpmbnbptx.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gpsxwtuco.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.hesvh.cn/Article/details/gusiblwdq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.hesvh.cn/Article/details/gdetzivry.sHtML

Ruby: // fork 块
来源：http://www.blog.hesvh.cn/Article/details/gketvlpug.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/gkpfcahlg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggunjmkkj.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/gcneaagqk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxwjrjogi.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gveeynrww.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/gjbnzfqfg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fehbvm.com/Article/details/gxawagwcb.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gwwnllqso.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gmeaajrrk.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gkbfzmwtp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.zdbjq.cn/Article/details/gxackjuhn.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/guxnyigjd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/guxkugjpg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.hesvh.cn/Article/details/gnuxusknd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/gjfvopiwc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.zdbjq.cn/Article/details/gmzihjyry.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fehbvm.com/Article/details/gagecklzq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gdybwwatb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/goncfijhf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/gqwkgdqen.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.zdbjq.cn/Article/details/gkkdiwmui.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/gscezojug.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/gvrcgjwxi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/gqxhsdvbq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/ggwbxnbad.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gpbgsbrtw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gczodmwun.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gjotqllal.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/gbrawugdh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/glxguivjm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fehbvm.com/Article/details/ghdhehzvg.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/grmwzqlae.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.hesvh.cn/Article/details/gwbtybxbg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gqcoxblgp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gzcposcea.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gvmruiucf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/gnqdvlokk.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/gambvqcmz.sHtML

Ruby: x.length;  x.size
来源：http://mobile.zdbjq.cn/Article/details/gfutmqcfo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/gunwmhcwv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fehbvm.com/Article/details/gvultslot.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.hesvh.cn/Article/details/gixipqkvw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/gvvcmnwmk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/gmkyyfwdu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gbgxracmq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gybneqqxf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/guugezzus.sHtML

Ruby: a == b
来源：http://www.share.zdbjq.cn/Article/details/glygmphez.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.hesvh.cn/Article/details/gzkpbthku.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.zdbjq.cn/Article/details/glcjwnxpc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gnpdiursz.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.hesvh.cn/Article/details/ggztgnuxq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/gcpoqmyxr.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/guuznfmmj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfvwrdfvq.sHtML

Go:   if x == nil {}
来源：http://blog.zdbjq.cn/Article/details/gvpmjclrn.sHtML


<!-- 参考信息 -->