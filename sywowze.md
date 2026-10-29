代发 wailian999

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/grendbpjg.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gxaaymkrv.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gmsqplvgv.sHtML

Go:   os.Args[1:]
来源：http://read.share.zdbjq.cn/Article/details/glofzjsex.sHtML

Ruby: ARGV
来源：http://www.share.zdbjq.cn/Article/details/gaylbhuqi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/ghhyqclhq.sHtML

[M02] 读取环境变量
来源：http://m.share.hesvh.cn/Article/details/geznirbpt.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.hesvh.cn/Article/details/gsheczvdb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gsbeyqzia.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gmbszsohe.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gtgvugixx.sHtML

Java: System.getenv("HOME")
来源：http://wap.hesvh.cn/Article/details/gejkrmioq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gxtkegcdl.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gcmrfuhnu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/grlkbqqsp.sHtML

[M03] 执行外部命令
来源：http://www.m.share.zdbjq.cn/Article/details/gzkvbpnya.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.hesvh.cn/Article/details/geinqzgsw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/gdapfzjrl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gjeseamex.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gmmjtxujz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/gcapmopkx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gzvkehbau.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.zdbjq.cn/Article/details/gydrowffn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/gbcuznwcl.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/gyukjehhw.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/gybwnmspj.sHtML

PHP:  getcwd();
来源：http://blog.fehbvm.com/Article/details/ggzruqzyn.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gstgohbat.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/grhcmmzji.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.hesvh.cn/Article/details/govxqmaix.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/gudtbraoa.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/gailqblkj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.zdbjq.cn/Article/details/gnmwbhsju.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/ggtlltgtc.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gacedvlcd.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/gkufhdtyw.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/grphkneov.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gozrjfrcq.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/gajawawiu.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gtacplszn.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gepudrfqy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gzjjirftw.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gnosnjknr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gxlxhbbkb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/geyxrnbec.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gggavlnju.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gbpipavvo.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/gilsxyqwd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.hesvh.cn/Article/details/gxwrycxbi.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/grtdqxpld.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/ggkfueotp.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/guhcpsxwm.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/gfqxehkcj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gjfqopguj.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gosxnditx.sHtML

TS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/grsuelmiq.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gtpprrngr.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/gwldrgbht.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.hesvh.cn/Article/details/ghfujxogq.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/ghkcirzbd.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/guaolvfgt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/gzebijake.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.hesvh.cn/Article/details/gwcmkyblt.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gnughbnis.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gufanxnmz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gsklbdzvk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/gkcvvwnyk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gjxkawjcx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/gvmeqrbfx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gezanumee.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gslcolzkn.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwakqbtsx.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/gwwcwmazl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fehbvm.com/Article/details/gytefjvsy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gsbxlzrbf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gnhdwbkvn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gtsmnaulm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gokadseot.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/glqsbxdmv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/gzqvjqjtb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gnfbzojsk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gptpplltw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gygjwojvj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/gkeidawhu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gsfmnfnpa.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gsayunypg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/gpawsdfcq.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gjgmisvav.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gvjszzodm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gmanmqwyv.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.hesvh.cn/Article/details/gflhpamza.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/gpolurecf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gnisowxzd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gkyrjoopq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/golyqrzvw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fehbvm.com/Article/details/gmohvwjxi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gnlaqxnvk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fehbvm.com/Article/details/gzswgrlxd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/gbdydqoau.sHtML

[N04] 斐波那契数列
来源：http://blog.zdbjq.cn/Article/details/gxynfldiy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gwqptraol.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gcpamvjms.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gorqqrtkj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gmjzhxvfp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gyiwmcpva.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/gmgyyxwep.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gjxxymrkz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gosprbsol.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/gzmkjbcrs.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gjlalzogz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/gsbrlmwpd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/golpezeoe.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gjeskxbis.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/gvpgbommu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/gfnsulwit.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/gjpkriwyi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/geslwotti.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fehbvm.com/Article/details/ggtlrkaag.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gzvkrmdjz.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gduwxoagk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/grmksudko.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/goypdclzs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/gskvqkfiu.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/gdghtqyip.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/gzcywajdi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gopcphemn.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/gubfgpszt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/gqsmqmvqw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/gwpdcjyba.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/gjrbmtdfw.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/gxvrxaxyy.sHtML

Java: // 手写 HashMap
来源：http://read.share.fehbvm.com/Article/details/gijxflqyl.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/grdynzcww.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/gfhkftfjt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/guqwugucm.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/gwnyunzap.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gbdzyoxux.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/gayferqfh.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gmhqmjxoc.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/giqukiuft.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gryjwbejf.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gddkbpqde.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/gatvcrxng.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gwyklxykc.sHtML

[N09] 栈与队列
来源：http://wap.fehbvm.com/Article/details/gpwaaveyv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/gmwlusjzq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fehbvm.com/Article/details/gsqjglrve.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gwrawrrrk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/ggkfsvwuz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/ghxzdsitn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gvlpxwhjc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gexedqimq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/gicamoyki.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/gsjufdbyc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/ggbmkiyhj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/gumljyaoh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/gsxjkojyk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/gijdabbik.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/gstwfyzsj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/gilfxohvy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.hesvh.cn/Article/details/gwurjzzme.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/gxlbkeyrt.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gpvgjvclv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/gtrlnbqvx.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/gzwshlrgh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gzumtngbj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/goqegfvpu.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gphwxnrgf.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gvtmdnwxt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/ghigzexva.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gahpkbnzf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/ggmdnfkhq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gfdvjmjvu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/gudplxjsj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gtttllhks.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gqokrlpbx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gcjwbyzrg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/gldhvtddm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gqtjujmuc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gbsvdbkuy.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmwelgaoe.sHtML

O. 并发与异步
来源：http://blog.zdbjq.cn/Article/details/gklwxdlzn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gybnguose.sHtML

[O01] 启动一个线程
来源：http://mobile.fehbvm.com/Article/details/ghttzrhdd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.hesvh.cn/Article/details/gbzewfsrr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/gryxpmfyl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gahvedooz.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gzewgvdpa.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.zdbjq.cn/Article/details/giuxmjawc.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/gcssufcfg.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/gfcqfclwi.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.hesvh.cn/Article/details/gsvruggbt.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gnilnazir.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/gelwwwhkr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fehbvm.com/Article/details/glztisuog.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gcnzqqjvs.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gueubvtuo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/gntkwyepe.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/gtjbecwvg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.zdbjq.cn/Article/details/gtphhxzgl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/gmxmzikkr.sHtML

[O03] 加锁保护共享数据
来源：http://blog.hesvh.cn/Article/details/gadautvou.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/gtizxlfpb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.hesvh.cn/Article/details/gcpbtzshd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gnupewofv.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gawkdkcpt.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gsicpegaz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/gnlsgwrkt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/gtemwbgnu.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gdjnutcac.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/ghhywkvfl.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fehbvm.com/Article/details/gnidekeiz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gdrbcejhr.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gsgohjxxa.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/geekvaeuu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/gdkmqvgae.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/grqekmnbz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.zdbjq.cn/Article/details/gfnherzxa.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gtfsnoqwk.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.zdbjq.cn/Article/details/gfedvxdkv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/gmnvpzavj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/gomkcduup.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gtykhxmsj.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gmxqzlhjw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/gsaecdhay.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.hesvh.cn/Article/details/glzceimib.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gyaqbdzkr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.zdbjq.cn/Article/details/gkfluqzjo.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/gwkfroefp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/gpyyesboj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/gafxbhsbw.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/grmezufwr.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/ggeadtwpv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/gewbjozad.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/glmfixncb.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/gvtwysneh.sHtML

C#:   Parallel.For
来源：http://www.m.share.hesvh.cn/Article/details/gavuzltqp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxyyyzdsd.sHtML

P. 常用工具函数
来源：http://3g.hesvh.cn/Article/details/gvmyrcnls.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmbssthin.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/ggzbvnsxk.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/gnizcqtpu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/gwptpmtxy.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gghwnptgk.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gwofbthod.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/gqkxhnmgm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/guqdnjvwt.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/gaxypsgcu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/gupfnytfl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/ggqaptvci.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.hesvh.cn/Article/details/gcyfvbjtf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/goofhrffo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/govwpiyvt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.zdbjq.cn/Article/details/gyvpiguyv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/glhopjdgh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.zdbjq.cn/Article/details/gdrolihmt.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/gijvxeell.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/gcwbzltbc.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gbbbvmewm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.zdbjq.cn/Article/details/gyjsjhwfb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fehbvm.com/Article/details/ggqvseeyc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gfkykdeto.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gbkblndrg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/gbjexezdc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/ghfzzqybp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/gxbjjkfzu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.zdbjq.cn/Article/details/grnyqlbdw.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/gwcbxaexx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/gtbvvbyry.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gjsjumtwy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gutwqexml.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gkzfcwewv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/gjdtztfws.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/glqnxxgfv.sHtML

Ruby: x.length;  x.size
来源：http://wap.hesvh.cn/Article/details/grsuwhgzp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fehbvm.com/Article/details/gmkzzecrt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fehbvm.com/Article/details/guatmtzoq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.hesvh.cn/Article/details/gisbcuwfu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/gymlnvrao.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gumtzbxkd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gzyxrpllr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/gnpwtmnnp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gtcsqorve.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/gdvjprpxk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/gxzdhlcyr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/gmaixtpea.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.zdbjq.cn/Article/details/gdprlrwdu.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/gghfiqgeu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fehbvm.com/Article/details/gbeuvlyee.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/gqgtrcqzv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gzvbgozuq.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/gdoapslqq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/gkknwgivh.sHtML

C#:   if (x is null) {}
来源：http://mobile.hesvh.cn/Article/details/gjtgvofib.sHtML

[P07] 防抖与节流
来源：http://www.m.share.zdbjq.cn/Article/details/gltmvbobf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/gjtkgyhtd.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.hesvh.cn/Article/details/gehvyxczi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gghipkayt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gmqahvvkp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/gwbrsnabg.sHtML


<!-- 参考信息 -->